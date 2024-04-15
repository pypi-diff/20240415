# Comparing `tmp/dbt-fabric-1.8.1.tar.gz` & `tmp/dbt-fabric-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.8.1.tar", last modified: Thu Apr 11 23:57:28 2024, max compression
+gzip compressed data, was "dbt-fabric-1.8.2.tar", last modified: Mon Apr 15 18:44:23 2024, max compression
```

## Comparing `dbt-fabric-1.8.1.tar` & `dbt-fabric-1.8.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.879519 dbt-fabric-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-11 23:57:28.879519 dbt-fabric-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.871519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.875519 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.879519 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:57:28.879519 dbt-fabric-1.8.1/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-11 23:57:28.000000 dbt-fabric-1.8.1/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-11 23:57:28.000000 dbt-fabric-1.8.1/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:57:28.000000 dbt-fabric-1.8.1/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 23:57:28.000000 dbt-fabric-1.8.1/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 23:57:28.000000 dbt-fabric-1.8.1/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:57:28.879519 dbt-fabric-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-11 23:56:46.000000 dbt-fabric-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/setup.py
```

### Comparing `dbt-fabric-1.8.1/LICENSE` & `dbt-fabric-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/PKG-INFO` & `dbt-fabric-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.1/README.md` & `dbt-fabric-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.8.2/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from dbt_common.events.functions import fire_event
 from dbt_common.utils.casting import cast_to_str
 
 from dbt.adapters.fabric import __version__
 from dbt.adapters.fabric.fabric_credentials import FabricCredentials
 
 AZURE_CREDENTIAL_SCOPE = "https://database.windows.net//.default"
+SYNAPSE_SPARK_CREDENTIAL_SCOPE = "DW"
 _TOKEN: Optional[AccessToken] = None
 AZURE_AUTH_FUNCTION_TYPE = Callable[[FabricCredentials], AccessToken]
 
 logger = AdapterLogger("fabric")
 
 # https://github.com/mkleehammer/pyodbc/wiki/Data-Types
 datatypes = {
@@ -83,14 +84,37 @@
     out : bytes
         The Microsoft byte string.
     """
     value = bytes(token.token, "UTF-8")
     return convert_bytes_to_mswindows_byte_string(value)
 
 
+def get_synapse_spark_access_token(credentials: FabricCredentials) -> AccessToken:
+    """
+    Get an Azure access token by using mspsarkutils
+    Parameters
+    -----------
+    credentials: FabricCredentials
+        Credentials.
+    Returns
+    -------
+    out : AccessToken
+        The access token.
+    """
+    from notebookutils import mssparkutils
+
+    aad_token = mssparkutils.credentials.getToken(SYNAPSE_SPARK_CREDENTIAL_SCOPE)
+    expires_on = int(time.time() + 4500.0)
+    token = AccessToken(
+        token=aad_token,
+        expires_on=expires_on,
+    )
+    return token
+
+
 def get_cli_access_token(credentials: FabricCredentials) -> AccessToken:
     """
     Get an Azure access token using the CLI credentials
 
     First login with:
 
     ```bash
@@ -148,14 +172,15 @@
     return token
 
 
 AZURE_AUTH_FUNCTIONS: Mapping[str, AZURE_AUTH_FUNCTION_TYPE] = {
     "cli": get_cli_access_token,
     "auto": get_auto_access_token,
     "environment": get_environment_access_token,
+    "synapsespark": get_synapse_spark_access_token,
 }
 
 
 def get_pyodbc_attrs_before(credentials: FabricCredentials) -> Dict:
     """
     Get the pyodbc attrs before.
```

### Comparing `dbt-fabric-1.8.1/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/catalog.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/clone.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/table/table.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/models/view/view.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/helpers.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt/include/fabric/macros/materializations/tests/helpers.sql` & `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.8.2/dbt_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.1/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.8.2/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.1/setup.py` & `dbt-fabric-1.8.2/setup.py`

 * *Files identical despite different names*

