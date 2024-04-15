# Comparing `tmp/dbt-athena-community-1.7.2.tar.gz` & `tmp/dbt_athena_community-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.7.2.tar", last modified: Tue Feb  6 09:32:33 2024, max compression
+gzip compressed data, was "dbt_athena_community-1.8.0.tar", last modified: Mon Apr 15 15:25:59 2024, max compression
```

## Comparing `dbt-athena-community-1.7.2.tar` & `dbt_athena_community-1.8.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.025803 dbt-athena-community-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-02-06 09:32:33.025803 dbt-athena-community-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39354 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.017803 dbt-athena-community-1.7.2/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.017803 dbt-athena-community-1.7.2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.017803 dbt-athena-community-1.7.2/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58350 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/lakeformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.013803 dbt-athena-community-1.7.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.017803 dbt-athena-community-1.7.2/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.013803 dbt-athena-community-1.7.2/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/python_submissions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.013803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.021803 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.025803 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:32:33.025803 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-02-06 09:32:33.000000 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-06 09:32:33.000000 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 09:32:33.000000 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-06 09:32:33.000000 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-06 09:32:33.000000 dbt-athena-community-1.7.2/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 09:32:33.025803 dbt-athena-community-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-06 09:32:23.000000 dbt-athena-community-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.440155 dbt_athena_community-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33193 2024-04-15 15:25:59.440155 dbt_athena_community-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32051 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.432155 dbt_athena_community-1.8.0/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.432155 dbt_athena_community-1.8.0/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.432155 dbt_athena_community-1.8.0/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57359 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/lakeformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.428156 dbt_athena_community-1.8.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.432155 dbt_athena_community-1.8.0/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.428156 dbt_athena_community-1.8.0/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/python_submissions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.428156 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.436155 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.440155 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:25:59.440155 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33193 2024-04-15 15:25:59.000000 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-15 15:25:59.000000 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:25:59.000000 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 15:25:59.000000 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 15:25:59.000000 dbt_athena_community-1.8.0/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:25:59.440155 dbt_athena_community-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 15:25:53.000000 dbt_athena_community-1.8.0/setup.py
```

### Comparing `dbt-athena-community-1.7.2/LICENSE.txt` & `dbt_athena_community-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/PKG-INFO` & `dbt_athena_community-1.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.7.2
+Version: 1.8.0
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: boto3~=1.34
-Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]~=1.34
-Requires-Dist: dbt-core~=1.7.0
-Requires-Dist: mmh3<4.2.0,>=4.0.1
+Requires-Dist: dbt-common<2.0,>=1.0.0b2
+Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: boto3>=1.28
+Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]>=1.28
 Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: mmh3<4.2.0,>=4.0.1
 Requires-Dist: pydantic<3.0,>=1.10
 Requires-Dist: tenacity~=8.2
 
 <!-- markdownlint-disable-next-line MD041 -->
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/">
@@ -528,16 +529,14 @@
 #### HA Known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
-- The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a
-  precision parameter for timestamps
 
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
@@ -842,45 +841,12 @@
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sanromeo"><img src="https://avatars.githubusercontent.com/u/44975602?v=4?s=100" width="100px;" alt="Roman Korsun"/><br /><sub><b>Roman Korsun</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=sanromeo" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asanromeo" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Danya-Fpnk"><img src="https://avatars.githubusercontent.com/u/122433975?v=4?s=100" width="100px;" alt="DanyaF"/><br /><sub><b>DanyaF</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Danya-Fpnk" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ADanya-Fpnk" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/octiva"><img src="https://avatars.githubusercontent.com/u/53303191?v=4?s=100" width="100px;" alt="Spencer"/><br /><sub><b>Spencer</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=octiva" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Avinash-1394"><img src="https://avatars.githubusercontent.com/u/43074786?v=4?s=100" width="100px;" alt="Avinash Santhanagopalan"/><br /><sub><b>Avinash Santhanagopalan</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Avinash-1394" title="Code">💻</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+<a href="https://github.com/dbt-athena/dbt-athena/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=dbt-athena/dbt-athena" />
+</a>
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.7.2 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-boto3~=1.34 Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]~=1.34
-Requires-Dist: dbt-core~=1.7.0 Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist:
-pyathena<4.0,>=2.25 Requires-Dist: pydantic<3.0,>=1.10 Requires-Dist:
-tenacity~=8.2
+Programming Language :: Python :: 3.12 Requires-Python: >=3.8,<3.13
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: dbt-common<2.0,>=1.0.0b2 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: boto3>=1.28 Requires-Dist: boto3-stubs
+[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist: pydantic<3.0,>=1.10 Requires-
+Dist: tenacity~=8.2
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
@@ -261,17 +262,15 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed - The macro `athena__end_of_time` needs to be
-overwritten by the user if using Athena engine v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
+older location removed ## Snapshots The adapter supports snapshot
 materialization. It supports both timestamp and check strategy. To create a
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
@@ -386,28 +385,9 @@
 entirely (for instance `array`) even though they won't be checked. Indeed, as
 dbt recommends, we only compare the broader type (array, map, int, varchar).
 The complete definition is used in order to check that the data types defined
 in athena are ok (pre-flight check). - the adapter does not support the
 constraints since no constraints don't exist in Athena. ## Contributing See
 [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
 this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-     _[_n_i_c_o_r_8_8_]      _[_J_e_s_s_e         _[_L_e_m_i_f_f_e_]   _[_J_Ã_©_r_Ã_©_m_y   _[_T_o_m_]        _[_M_a_t_t_i_a_]   _[_G_a_t_s_b_y
-      _nn_ii_cc_oo_rr_88_88     _D_o_b_b_e_l_a_e_r_e_]       _LL_ee_mm_ii_ff_ff_ee    _G_u_i_s_e_l_i_n_]    _TT_oo_mm          _MM_aa_tt_tt_ii_aa     _L_e_e_]
-  _ð___» _ð___§ _ð___     _JJ_ee_ss_ss_ee            _ð___¨     _JJ_?Ã_?©_rr_?Ã_?©_mm_yy  _ð___§ _ð___»        _ð___§     _GG_aa_tt_ss_bb_yy
-                  _DD_oo_bb_bb_ee_ll_aa_ee_rr_ee                   _GG_uu_ii_ss_ee_ll_ii_nn                              _LL_ee_ee
-                   _ð___ _ð___§                   _ð___§ _ð___»                            _ð___
-                                                 _ð___
-_[_B_r_e_c_h_t_D_e_V_l_i_e_g_e_r_]    _[_A_n_d_r_e_a      _[_M_a_i_a_r_a       _[_H_e_n_r_i    _[_S_e_r_h_i_i   _[_c_h_r_i_s_c_h_i_n_4_7_8_] _[_R_o_m_a_n
- _BB_rr_ee_cc_hh_tt_DD_ee_VV_ll_ii_ee_gg_ee_rr    _A_r_t_a_r_i_a_]     _R_e_i_n_a_l_d_o_]     _B_l_a_n_c_k_e_]  _D_i_m_c_h_e_n_k_o_]  _cc_hh_rr_ii_ss_cc_hh_ii_nn_44_77_88  _K_o_r_s_u_n_]
-      _ð___           _AA_nn_dd_rr_ee_aa   _MM_aa_ii_aa_rr_aa_ _RR_ee_ii_nn_aa_ll_dd_oo    _HH_ee_nn_rr_ii     _SS_ee_rr_hh_ii_ii     _ð___» _ð___     _RR_oo_mm_aa_nn
-                     _AA_rr_tt_aa_rr_ii_aa        _ð___        _BB_ll_aa_nn_cc_kk_ee  _DD_ii_mm_cc_hh_ee_nn_kk_oo                 _KK_oo_rr_ss_uu_nn
-                      _ð___                     _ð___» _ð___ _ð___» _ð___                  _ð___»
-                                                                                    _ð___
-      _[_D_a_n_y_a_F_]     _[_S_p_e_n_c_e_r_]      _[_A_v_i_n_a_s_h
-       _DD_aa_nn_yy_aa_FF       _SS_pp_ee_nn_cc_ee_rr   _S_a_n_t_h_a_n_a_g_o_p_a_l_a_n_]
-      _ð___» _ð___      _ð___»         _AA_vv_ii_nn_aa_ss_hh
-                              _SS_aa_nn_tt_hh_aa_nn_aa_gg_oo_pp_aa_ll_aa_nn
-                                    _ð___»
-This project follows the [all-contributors](https://github.com/all-
-contributors/all-contributors) specification. Contributions of any kind
-welcome!
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt-athena-community-1.7.2/README.md` & `dbt_athena_community-1.8.0/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: dbt-athena-community
+Version: 1.8.0
+Summary: The athena adapter plugin for dbt (data build tool)
+Home-page: https://github.com/dbt-athena/dbt-athena
+License: Apache License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8,<3.13
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: dbt-common<2.0,>=1.0.0b2
+Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: boto3>=1.28
+Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]>=1.28
+Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: mmh3<4.2.0,>=4.0.1
+Requires-Dist: pydantic<3.0,>=1.10
+Requires-Dist: tenacity~=8.2
+
 <!-- markdownlint-disable-next-line MD041 -->
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/">
       <img src="https://badge.fury.io/py/dbt-athena-community.svg" />
     </a>
     <a target="_blank" href="https://pypi.org/project/dbt-athena-community/" style="background:none">
@@ -500,16 +529,14 @@
 #### HA Known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
-- The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a
-  precision parameter for timestamps
 
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
@@ -814,45 +841,12 @@
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sanromeo"><img src="https://avatars.githubusercontent.com/u/44975602?v=4?s=100" width="100px;" alt="Roman Korsun"/><br /><sub><b>Roman Korsun</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=sanromeo" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asanromeo" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Danya-Fpnk"><img src="https://avatars.githubusercontent.com/u/122433975?v=4?s=100" width="100px;" alt="DanyaF"/><br /><sub><b>DanyaF</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Danya-Fpnk" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ADanya-Fpnk" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/octiva"><img src="https://avatars.githubusercontent.com/u/53303191?v=4?s=100" width="100px;" alt="Spencer"/><br /><sub><b>Spencer</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=octiva" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Avinash-1394"><img src="https://avatars.githubusercontent.com/u/43074786?v=4?s=100" width="100px;" alt="Avinash Santhanagopalan"/><br /><sub><b>Avinash Santhanagopalan</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Avinash-1394" title="Code">💻</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+<a href="https://github.com/dbt-athena/dbt-athena/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=dbt-athena/dbt-athena" />
+</a>
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0 Summary: The
+athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
+dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Python: >=3.8,<3.13
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: dbt-common<2.0,>=1.0.0b2 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: boto3>=1.28 Requires-Dist: boto3-stubs
+[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist: pydantic<3.0,>=1.10 Requires-
+Dist: tenacity~=8.2
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
@@ -246,17 +262,15 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed - The macro `athena__end_of_time` needs to be
-overwritten by the user if using Athena engine v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
+older location removed ## Snapshots The adapter supports snapshot
 materialization. It supports both timestamp and check strategy. To create a
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
@@ -371,28 +385,9 @@
 entirely (for instance `array`) even though they won't be checked. Indeed, as
 dbt recommends, we only compare the broader type (array, map, int, varchar).
 The complete definition is used in order to check that the data types defined
 in athena are ok (pre-flight check). - the adapter does not support the
 constraints since no constraints don't exist in Athena. ## Contributing See
 [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
 this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-     _[_n_i_c_o_r_8_8_]      _[_J_e_s_s_e         _[_L_e_m_i_f_f_e_]   _[_J_Ã_©_r_Ã_©_m_y   _[_T_o_m_]        _[_M_a_t_t_i_a_]   _[_G_a_t_s_b_y
-      _nn_ii_cc_oo_rr_88_88     _D_o_b_b_e_l_a_e_r_e_]       _LL_ee_mm_ii_ff_ff_ee    _G_u_i_s_e_l_i_n_]    _TT_oo_mm          _MM_aa_tt_tt_ii_aa     _L_e_e_]
-  _ð___» _ð___§ _ð___     _JJ_ee_ss_ss_ee            _ð___¨     _JJ_?Ã_?©_rr_?Ã_?©_mm_yy  _ð___§ _ð___»        _ð___§     _GG_aa_tt_ss_bb_yy
-                  _DD_oo_bb_bb_ee_ll_aa_ee_rr_ee                   _GG_uu_ii_ss_ee_ll_ii_nn                              _LL_ee_ee
-                   _ð___ _ð___§                   _ð___§ _ð___»                            _ð___
-                                                 _ð___
-_[_B_r_e_c_h_t_D_e_V_l_i_e_g_e_r_]    _[_A_n_d_r_e_a      _[_M_a_i_a_r_a       _[_H_e_n_r_i    _[_S_e_r_h_i_i   _[_c_h_r_i_s_c_h_i_n_4_7_8_] _[_R_o_m_a_n
- _BB_rr_ee_cc_hh_tt_DD_ee_VV_ll_ii_ee_gg_ee_rr    _A_r_t_a_r_i_a_]     _R_e_i_n_a_l_d_o_]     _B_l_a_n_c_k_e_]  _D_i_m_c_h_e_n_k_o_]  _cc_hh_rr_ii_ss_cc_hh_ii_nn_44_77_88  _K_o_r_s_u_n_]
-      _ð___           _AA_nn_dd_rr_ee_aa   _MM_aa_ii_aa_rr_aa_ _RR_ee_ii_nn_aa_ll_dd_oo    _HH_ee_nn_rr_ii     _SS_ee_rr_hh_ii_ii     _ð___» _ð___     _RR_oo_mm_aa_nn
-                     _AA_rr_tt_aa_rr_ii_aa        _ð___        _BB_ll_aa_nn_cc_kk_ee  _DD_ii_mm_cc_hh_ee_nn_kk_oo                 _KK_oo_rr_ss_uu_nn
-                      _ð___                     _ð___» _ð___ _ð___» _ð___                  _ð___»
-                                                                                    _ð___
-      _[_D_a_n_y_a_F_]     _[_S_p_e_n_c_e_r_]      _[_A_v_i_n_a_s_h
-       _DD_aa_nn_yy_aa_FF       _SS_pp_ee_nn_cc_ee_rr   _S_a_n_t_h_a_n_a_g_o_p_a_l_a_n_]
-      _ð___» _ð___      _ð___»         _AA_vv_ii_nn_aa_ss_hh
-                              _SS_aa_nn_tt_hh_aa_nn_aa_gg_oo_pp_aa_ll_aa_nn
-                                    _ð___»
-This project follows the [all-contributors](https://github.com/all-
-contributors/all-contributors) specification. Contributions of any kind
-welcome!
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/column.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from typing import ClassVar, Dict
 
+from dbt_common.exceptions import DbtRuntimeError
+
 from dbt.adapters.athena.relation import TableType
 from dbt.adapters.base.column import Column
-from dbt.exceptions import DbtRuntimeError
 
 
 @dataclass
 class AthenaColumn(Column):
     table_type: TableType = TableType.TABLE
 
     TYPE_LABELS: ClassVar[Dict[str, str]] = {
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/config.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/config.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/connections.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import hashlib
 import json
 import re
 import time
 from concurrent.futures.thread import ThreadPoolExecutor
 from contextlib import contextmanager
 from copy import deepcopy
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Any, ContextManager, Dict, List, Optional, Tuple
 
 import tenacity
+from dbt_common.exceptions import ConnectionError, DbtRuntimeError
+from dbt_common.utils import md5
 from pyathena.connection import Connection as AthenaConnection
 from pyathena.cursor import Cursor
 from pyathena.error import OperationalError, ProgrammingError
 
 # noinspection PyProtectedMember
 from pyathena.formatter import (
     _DEFAULT_FORMATTERS,
@@ -26,19 +27,23 @@
 from pyathena.util import RetryConfig
 from tenacity.retry import retry_if_exception
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_exponential
 
 from dbt.adapters.athena.config import get_boto3_config
 from dbt.adapters.athena.constants import LOGGER
+from dbt.adapters.athena.query_headers import AthenaMacroQueryStringSetter
 from dbt.adapters.athena.session import get_boto3_session
-from dbt.adapters.base import Credentials
+from dbt.adapters.contracts.connection import (
+    AdapterResponse,
+    Connection,
+    ConnectionState,
+    Credentials,
+)
 from dbt.adapters.sql import SQLConnectionManager
-from dbt.contracts.connection import AdapterResponse, Connection, ConnectionState
-from dbt.exceptions import ConnectionError, DbtRuntimeError
 
 
 @dataclass
 class AthenaAdapterResponse(AdapterResponse):
     data_scanned_in_bytes: Optional[int] = None
 
 
@@ -68,15 +73,15 @@
 
     @property
     def type(self) -> str:
         return "athena"
 
     @property
     def unique_field(self) -> str:
-        return f"athena-{hashlib.md5(self.s3_staging_dir.encode()).hexdigest()}"
+        return f"athena-{md5(self.s3_staging_dir)}"
 
     @property
     def effective_num_retries(self) -> int:
         return self.num_boto3_retries or self.num_retries
 
     def _connection_keys(self) -> Tuple[str, ...]:
         return (
@@ -197,14 +202,17 @@
         )
         return retry(inner)
 
 
 class AthenaConnectionManager(SQLConnectionManager):
     TYPE = "athena"
 
+    def set_query_header(self, query_header_context: Dict[str, Any]) -> None:
+        self.query_header = AthenaMacroQueryStringSetter(self.profile, query_header_context)
+
     @classmethod
     def data_type_code_to_name(cls, type_code: str) -> str:
         """
         Get the string representation of the data type from the Athena metadata. Dbt performs a
         query to retrieve the types of the columns in the SQL query. Then these types are compared
         to the types in the contract config, simplified because they need to match what is returned
         by Athena metadata (we are only interested in the broader type, without subtypes nor granularity).
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/constants.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dbt.events import AdapterLogger
+from dbt.adapters.events.logging import AdapterLogger
 
 DEFAULT_THREAD_COUNT = 4
 DEFAULT_RETRY_ATTEMPTS = 3
 DEFAULT_POLLING_INTERVAL = 5
 DEFAULT_SPARK_COORDINATOR_DPU_SIZE = 1
 DEFAULT_SPARK_MAX_CONCURRENT_DPUS = 2
 DEFAULT_SPARK_EXECUTOR_DPU_SIZE = 1
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/impl.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 import os
 import posixpath as path
 import re
 import struct
 import tempfile
 from dataclasses import dataclass
 from datetime import date, datetime
-from itertools import chain
+from functools import lru_cache
 from textwrap import dedent
 from threading import Lock
-from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Type
+from typing import Any, Dict, FrozenSet, Iterable, List, Optional, Set, Tuple, Type
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import agate
 import mmh3
 from botocore.exceptions import ClientError
-from mypy_boto3_athena.type_defs import DataCatalogTypeDef
+from dbt_common.clients.agate_helper import table_from_rows
+from dbt_common.contracts.constraints import ConstraintType
+from dbt_common.exceptions import DbtRuntimeError
+from mypy_boto3_athena import AthenaClient
+from mypy_boto3_athena.type_defs import DataCatalogTypeDef, GetWorkGroupOutputTypeDef
 from mypy_boto3_glue.type_defs import (
     ColumnTypeDef,
     GetTableResponseTypeDef,
     TableInputTypeDef,
     TableTypeDef,
     TableVersionTypeDef,
 )
@@ -59,21 +63,17 @@
     get_chunks,
     is_valid_table_parameter_key,
     stringify_table_parameter_value,
 )
 from dbt.adapters.base import ConstraintSupport, PythonJobHelper, available
 from dbt.adapters.base.impl import AdapterConfig
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.sql import SQLAdapter
-from dbt.clients.agate_helper import table_from_rows
-from dbt.config.runtime import RuntimeConfig
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.graph.nodes import CompiledNode, ConstraintType
-from dbt.exceptions import DbtRuntimeError
 
 boto3_client_lock = Lock()
 
 
 @dataclass
 class AthenaConfig(AdapterConfig):
     """
@@ -210,29 +210,36 @@
                 )
             catalog = self._get_data_catalog(relation.database)
             catalog_id = get_catalog_id(catalog)
             lf_permissions = LfPermissions(catalog_id, relation, lf)  # type: ignore
             lf_permissions.process_filters(lf_config)
             lf_permissions.process_permissions(lf_config)
 
+    @lru_cache()
+    def _get_work_group(self, client: AthenaClient, work_group: str) -> GetWorkGroupOutputTypeDef:
+        """
+        helper function to cache the result of the get_work_group to avoid APIs throttling
+        """
+        return client.get_work_group(WorkGroup=work_group)
+
     @available
     def is_work_group_output_location_enforced(self) -> bool:
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
 
         with boto3_client_lock:
             athena_client = client.session.client(
                 "athena",
                 region_name=client.region_name,
                 config=get_boto3_config(num_retries=creds.effective_num_retries),
             )
 
         if creds.work_group:
-            work_group = athena_client.get_work_group(WorkGroup=creds.work_group)
+            work_group = self._get_work_group(athena_client, creds.work_group)
             output_location = (
                 work_group.get("WorkGroup", {})
                 .get("Configuration", {})
                 .get("ResultConfiguration", {})
                 .get("OutputLocation", None)
             )
 
@@ -394,14 +401,20 @@
             "Expression": where_condition,
             "ExcludeColumnSchema": True,
         }
         partition_pg = paginator.paginate(**partition_params)
         partitions = partition_pg.build_full_result().get("Partitions")
         for partition in partitions:
             self.delete_from_s3(partition["StorageDescriptor"]["Location"])
+            glue_client.delete_partition(
+                CatalogId=catalog_id,
+                DatabaseName=relation.schema,
+                TableName=relation.identifier,
+                PartitionValues=partition["Values"],
+            )
 
     @available
     def clean_up_table(self, relation: AthenaRelation) -> None:
         # this check avoids issues for when the table location is an empty string
         # or when the table does not exist and table location is None
         if table_location := self.get_glue_table_location(relation):
             self.delete_from_s3(table_location)
@@ -519,37 +532,14 @@
                 "s3",
                 region_name=client.region_name,
                 config=get_boto3_config(num_retries=creds.effective_num_retries),
             )
         response = s3_client.list_objects_v2(Bucket=s3_bucket, Prefix=s3_prefix)
         return True if "Contents" in response else False
 
-    def _join_catalog_table_owners(self, table: agate.Table, manifest: Manifest) -> agate.Table:
-        owners = []
-        # Get the owner for each model from the manifest
-        for node in manifest.nodes.values():
-            if node.resource_type == "model":
-                owners.append(
-                    {
-                        "table_database": node.database,
-                        "table_schema": node.schema,
-                        "table_name": node.alias,
-                        "table_owner": node.config.meta.get("owner"),
-                    }
-                )
-        owners_table = agate.Table.from_object(owners)
-
-        # Join owners with the results from catalog
-        join_keys = ["table_database", "table_schema", "table_name"]
-        return table.join(
-            right_table=owners_table,
-            left_key=join_keys,
-            right_key=join_keys,
-        )
-
     def _get_one_table_for_catalog(self, table: TableTypeDef, database: str) -> List[Dict[str, Any]]:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
             "table_type": RELATION_TYPE_MAP[table.get("TableType", "EXTERNAL_TABLE")].value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
@@ -589,21 +579,21 @@
             }
             for idx, col in enumerate(table["Columns"] + table.get("PartitionKeys", []))
         ]
 
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
-        schemas: Dict[str, Optional[Set[str]]],
-        manifest: Manifest,
+        schemas: Set[str],
+        used_schemas: FrozenSet[Tuple[str, str]],
     ) -> agate.Table:
         """
         This function is invoked by Adapter.get_catalog for each schema.
         """
-        data_catalog = self._get_data_catalog(information_schema.path.database)
+        data_catalog = self._get_data_catalog(information_schema.database)
         data_catalog_type = get_catalog_type(data_catalog)
 
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
         if data_catalog_type == AthenaCatalogType.GLUE:
             with boto3_client_lock:
@@ -611,70 +601,61 @@
                     "glue",
                     region_name=client.region_name,
                     config=get_boto3_config(num_retries=creds.effective_num_retries),
                 )
 
             catalog = []
             paginator = glue_client.get_paginator("get_tables")
-            for schema, relations in schemas.items():
+            for schema in schemas:
                 kwargs = {
                     "DatabaseName": schema,
                     "MaxResults": 100,
                 }
                 # If the catalog is `awsdatacatalog` we don't need to pass CatalogId as boto3
                 # infers it from the account Id.
                 catalog_id = get_catalog_id(data_catalog)
                 if catalog_id:
                     kwargs["CatalogId"] = catalog_id
 
                 for page in paginator.paginate(**kwargs):
                     for table in page["TableList"]:
-                        if relations and table["Name"] in relations:
-                            catalog.extend(self._get_one_table_for_catalog(table, information_schema.path.database))
+                        catalog.extend(self._get_one_table_for_catalog(table, information_schema.database))
             table = agate.Table.from_object(catalog)
         else:
             with boto3_client_lock:
                 athena_client = client.session.client(
                     "athena",
                     region_name=client.region_name,
                     config=get_boto3_config(num_retries=creds.effective_num_retries),
                 )
 
             catalog = []
             paginator = athena_client.get_paginator("list_table_metadata")
-            for schema, relations in schemas.items():
+            for schema in schemas:
                 for page in paginator.paginate(
-                    CatalogName=information_schema.path.database,
+                    CatalogName=information_schema.database,
                     DatabaseName=schema,
                     MaxResults=50,  # Limit supported by this operation
                 ):
                     for table in page["TableMetadataList"]:
-                        if relations and table["Name"].lower() in relations:
-                            catalog.extend(
-                                self._get_one_table_for_non_glue_catalog(
-                                    table, schema, information_schema.path.database
-                                )
-                            )
+                        catalog.extend(
+                            self._get_one_table_for_non_glue_catalog(table, schema, information_schema.database)
+                        )
             table = agate.Table.from_object(catalog)
 
-        filtered_table = self._catalog_filter_table(table, manifest)
-        return self._join_catalog_table_owners(filtered_table, manifest)
+        return self._catalog_filter_table(table, used_schemas)
 
-    def _get_catalog_schemas(self, manifest: Manifest) -> AthenaSchemaSearchMap:
+    def _get_catalog_schemas(self, relation_configs: Iterable[RelationConfig]) -> AthenaSchemaSearchMap:
         """
         Get the schemas from the catalog.
         It's called by the `get_catalog` method.
         """
         info_schema_name_map = AthenaSchemaSearchMap()
-        nodes: Iterator[CompiledNode] = chain(
-            [node for node in manifest.nodes.values() if (node.is_relational and not node.is_ephemeral_model)],
-            manifest.sources.values(),
-        )
-        for node in nodes:
-            relation = self.Relation.create_from(self.config, node)
+        for relation_config in relation_configs:
+            relation = self.Relation.create_from(quoting=self.config, relation_config=relation_config)
             info_schema_name_map.add(relation)
         return info_schema_name_map
 
     def _get_data_catalog(self, database: str) -> Optional[DataCatalogTypeDef]:
         if database:
             conn = self.connections.get_thread_connection()
             creds = conn.credentials
@@ -730,15 +711,15 @@
             for page in page_iterator:
                 tables = page["TableList"]
                 for table in tables:
                     if "TableType" not in table:
                         LOGGER.debug(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
                         continue
                     _type = table["TableType"]
-                    _detailed_table_type = table["Parameters"].get("table_type", "")
+                    _detailed_table_type = table.get("Parameters", {}).get("table_type", "")
                     if _type == "VIRTUAL_VIEW":
                         _type = self.Relation.View
                     else:
                         _type = self.Relation.Table
 
                     relations.append(
                         self.Relation.create(
@@ -756,35 +737,34 @@
             LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
 
         return relations
 
     def _get_one_catalog_by_relations(
         self,
         information_schema: InformationSchema,
-        relations: List[BaseRelation],
-        manifest: Manifest,
-    ) -> agate.Table:
+        relations: List[AthenaRelation],
+        used_schemas: FrozenSet[Tuple[str, str]],
+    ) -> "agate.Table":
         """
         Overwrite of _get_one_catalog_by_relations for Athena, in order to use glue apis.
         This function is invoked by Adapter.get_catalog_by_relations.
         """
         _table_definitions = []
         for _rel in relations:
             glue_table_definition = self.get_glue_table(_rel)
             if glue_table_definition:
                 _table_definition = self._get_one_table_for_catalog(glue_table_definition["Table"], _rel.database)
                 _table_definitions.extend(_table_definition)
         table = agate.Table.from_object(_table_definitions)
         # picked from _catalog_filter_table, force database + schema to be strings
-        table_casted = table_from_rows(
+        return table_from_rows(
             table.rows,
             table.column_names,
             text_only_columns=["table_database", "table_schema", "table_name"],
         )
-        return self._join_catalog_table_owners(table_casted, manifest)
 
     @available
     def swap_table(self, src_relation: AthenaRelation, target_relation: AthenaRelation) -> None:
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
 
@@ -993,19 +973,17 @@
             table_parameters["comment"] = clean_table_description
 
             # Get dbt model meta if available
             meta: Dict[str, Any] = model.get("config", {}).get("meta", {})
             # Add some of dbt model config fields as table meta
             meta["unique_id"] = model.get("unique_id")
             meta["materialized"] = model.get("config", {}).get("materialized")
-            # Get dbt runtime config to be able to get dbt project metadata
-            runtime_config: RuntimeConfig = self.config
             # Add dbt project metadata to table meta
-            meta["dbt_project_name"] = runtime_config.project_name
-            meta["dbt_project_version"] = runtime_config.version
+            meta["dbt_project_name"] = self.config.project_name
+            meta["dbt_project_version"] = self.config.version
             # Prepare meta values for table properties and check if update is required
             for meta_key, meta_value_raw in meta.items():
                 if is_valid_table_parameter_key(meta_key):
                     meta_value = stringify_table_parameter_value(meta_value_raw)
                     if meta_value is not None:
                         # Check that meta value is already attached to Glue table
                         current_meta_value: Optional[str] = table_parameters.get(meta_key)
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/lakeformation.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/lakeformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """AWS Lakeformation permissions management helper utilities."""
 
 from typing import Dict, List, Optional, Sequence, Set, Union
 
+from dbt_common.exceptions import DbtRuntimeError
 from mypy_boto3_lakeformation import LakeFormationClient
 from mypy_boto3_lakeformation.type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     ColumnLFTagTypeDef,
     DataCellsFilterTypeDef,
     GetResourceLFTagsResponseTypeDef,
     LFTagPairTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
     ResourceTypeDef,
 )
 from pydantic import BaseModel
 
 from dbt.adapters.athena.relation import AthenaRelation
-from dbt.events import AdapterLogger
-from dbt.exceptions import DbtRuntimeError
+from dbt.adapters.events.logging import AdapterLogger
 
 logger = AdapterLogger("AthenaLakeFormation")
 
 
 class LfTagsConfig(BaseModel):
     enabled: bool = False
     tags: Optional[Dict[str, str]] = None
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/python_submissions.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/python_submissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 from functools import cached_property
 from typing import Any, Dict
 
 import botocore
+from dbt_common.exceptions import DbtRuntimeError
 
 from dbt.adapters.athena.config import AthenaSparkSessionConfig
 from dbt.adapters.athena.connections import AthenaCredentials
 from dbt.adapters.athena.constants import LOGGER
 from dbt.adapters.athena.session import AthenaSparkSessionManager
 from dbt.adapters.base import PythonJobHelper
-from dbt.exceptions import DbtRuntimeError
 
 SUBMISSION_LANGUAGE = "python"
 
 
 class AthenaPythonJobHelper(PythonJobHelper):
     """
     Default helper to execute python models with Athena Spark.
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/query_headers.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/query_headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-import dbt.adapters.base.query_headers
+from typing import Any, Dict
 
+from dbt.adapters.base.query_headers import MacroQueryStringSetter, _QueryComment
+from dbt.adapters.contracts.connection import AdapterRequiredConfig
 
-class _QueryComment(dbt.adapters.base.query_headers._QueryComment):
+
+class AthenaMacroQueryStringSetter(MacroQueryStringSetter):
+    def __init__(self, config: AdapterRequiredConfig, query_header_context: Dict[str, Any]):
+        super().__init__(config, query_header_context)
+        self.comment = _AthenaQueryComment(None)
+
+
+class _AthenaQueryComment(_QueryComment):
     """
     Athena DDL does not always respect /* ... */ block quotations.
     This function is the same as _QueryComment.add except that
     a leading "-- " is prepended to the query_comment and any newlines
     in the query_comment are replaced with " ". This allows the default
     query_comment to be added to `create external table` statements.
     """
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/relation.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/session.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from functools import cached_property
 from hashlib import md5
 from typing import Any, Dict
 from uuid import UUID
 
 import boto3
 import boto3.session
+from dbt_common.exceptions import DbtRuntimeError
+from dbt_common.invocation import get_invocation_id
 
 from dbt.adapters.athena.config import get_boto3_config
 from dbt.adapters.athena.constants import (
     DEFAULT_THREAD_COUNT,
     LOGGER,
     SESSION_IDLE_TIMEOUT_MIN,
 )
-from dbt.contracts.connection import Connection
-from dbt.events.functions import get_invocation_id
-from dbt.exceptions import DbtRuntimeError
+from dbt.adapters.contracts.connection import Connection
 
 invocation_id = get_invocation_id()
 spark_session_list: Dict[UUID, str] = {}
 spark_session_load: Dict[UUID, int] = {}
 
 
 def get_boto3_session(connection: Connection) -> boto3.session.Session:
```

### Comparing `dbt-athena-community-1.7.2/dbt/adapters/athena/utils.py` & `dbt_athena_community-1.8.0/dbt/adapters/athena/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/columns.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/metadata.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/python_submissions.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/python_submissions.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/adapters/relation.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/hooks.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/hooks.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% macro run_hooks(hooks, inside_transaction=True) %}
   {% set re = modules.re %}
   {% for hook in hooks | selectattr('transaction', 'equalto', inside_transaction) %}
     {% set rendered = render(hook.get('sql')) | trim %}
     {% if (rendered | length) > 0 %}
-      {%- if re.match("optimize\W+\w+\W+rewrite data using bin_pack", rendered.lower(), re.MULTILINE) -%}
+      {%- if re.match("optimize\W+\S+\W+rewrite data using bin_pack", rendered.lower(), re.MULTILINE) -%}
         {%- do adapter.run_optimize_with_partition_limit_catching(rendered) -%}
       {%- else -%}
         {% call statement(auto_begin=inside_transaction) %}
           {{ rendered }}
         {% endcall %}
       {%- endif -%}
     {% endif %}
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-{% macro alter_relation_add_columns(relation, add_columns = none) -%}
+{% macro alter_relation_add_columns(relation, add_columns = none, table_type = 'hive') -%}
   {% if add_columns is none %}
     {% set add_columns = [] %}
   {% endif %}
 
   {% set sql -%}
       alter {{ relation.type }} {{ relation.render_hive() }}
           add columns (
             {%- for column in add_columns -%}
-                {{ column.name }} {{ ddl_data_type(column.data_type) }}{{ ', ' if not loop.last }}
+                {{ column.name }} {{ ddl_data_type(column.data_type, table_type) }}{{ ', ' if not loop.last }}
             {%- endfor -%}
           )
   {%- endset -%}
 
   {% if (add_columns | length) > 0 %}
     {{ return(run_query(sql)) }}
   {% endif %}
@@ -26,33 +26,33 @@
     {% set sql -%}
       alter {{ relation.type }} {{ relation.render_hive() }} drop column {{ column.name }}
     {% endset %}
     {% do run_query(sql) %}
   {%- endfor -%}
 {% endmacro %}
 
-{% macro alter_relation_replace_columns(relation, replace_columns = none) -%}
+{% macro alter_relation_replace_columns(relation, replace_columns = none, table_type = 'hive') -%}
   {% if replace_columns is none %}
     {% set replace_columns = [] %}
   {% endif %}
 
   {% set sql -%}
       alter {{ relation.type }} {{ relation.render_hive() }}
           replace columns (
             {%- for column in replace_columns -%}
-                {{ column.name }} {{ ddl_data_type(column.data_type) }}{{ ', ' if not loop.last }}
+                {{ column.name }} {{ ddl_data_type(column.data_type, table_type) }}{{ ', ' if not loop.last }}
             {%- endfor -%}
           )
   {%- endset -%}
 
   {% if (replace_columns | length) > 0 %}
     {{ return(run_query(sql)) }}
   {% endif %}
 {% endmacro %}
 
-{% macro alter_relation_rename_column(relation, source_column, target_column, target_column_type) -%}
+{% macro alter_relation_rename_column(relation, source_column, target_column, target_column_type, table_type = 'hive') -%}
   {% set sql -%}
       alter {{ relation.type }} {{ relation.render_pure() }}
-          change column {{ source_column }} {{ target_column }} {{ ddl_data_type(target_column_type) }}
+          change column {{ source_column }} {{ target_column }} {{ ddl_data_type(target_column_type, table_type) }}
   {%- endset -%}
   {{ return(run_query(sql)) }}
 {% endmacro %}
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files 16% similar despite different names*

```diff
@@ -3,50 +3,50 @@
   {% set table_type = config.get('table_type', default='hive') | lower %}
   {%- if partitioned_by is none -%}
       {%- set partitioned_by = [] -%}
   {%- endif %}
   {%- set add_to_target_arr = schema_changes_dict['source_not_in_target'] -%}
   {%- if on_schema_change == 'append_new_columns'-%}
      {%- if add_to_target_arr | length > 0 -%}
-       {%- do alter_relation_add_columns(target_relation, add_to_target_arr) -%}
+       {%- do alter_relation_add_columns(target_relation, add_to_target_arr, table_type) -%}
      {%- endif -%}
   {% elif on_schema_change == 'sync_all_columns' %}
      {%- set remove_from_target_arr = schema_changes_dict['target_not_in_source'] -%}
      {%- set new_target_types = schema_changes_dict['new_target_types'] -%}
      {% if table_type == 'iceberg' %}
        {#
           If last run of alter_column_type was failed on rename tmp column to origin.
           Do rename to protect origin column from deletion and losing data.
        #}
        {% for remove_col in remove_from_target_arr if remove_col.column.endswith('__dbt_alter') %}
          {%- set origin_col_name = remove_col.column | replace('__dbt_alter', '') -%}
          {% for add_col in add_to_target_arr if add_col.column == origin_col_name %}
-             {%- do alter_relation_rename_column(target_relation, remove_col.name, add_col.name, add_col.data_type) -%}
+             {%- do alter_relation_rename_column(target_relation, remove_col.name, add_col.name, add_col.data_type, table_type) -%}
              {%- do remove_from_target_arr.remove(remove_col) -%}
              {%- do add_to_target_arr.remove(add_col) -%}
          {% endfor %}
        {% endfor %}
 
        {% if add_to_target_arr | length > 0 %}
-         {%- do alter_relation_add_columns(target_relation, add_to_target_arr) -%}
+         {%- do alter_relation_add_columns(target_relation, add_to_target_arr, table_type) -%}
        {% endif %}
        {% if remove_from_target_arr | length > 0 %}
          {%- do alter_relation_drop_columns(target_relation, remove_from_target_arr) -%}
        {% endif %}
        {% if new_target_types != [] %}
          {% for ntt in new_target_types %}
            {% set column_name = ntt['column_name'] %}
            {% set new_type = ntt['new_type'] %}
            {% do alter_column_type(target_relation, column_name, new_type) %}
          {% endfor %}
        {% endif %}
      {% else %}
        {%- set replace_with_target_arr = remove_partitions_from_columns(schema_changes_dict['source_columns'], partitioned_by) -%}
        {% if add_to_target_arr | length > 0 or remove_from_target_arr | length > 0 or new_target_types | length > 0 %}
-         {%- do alter_relation_replace_columns(target_relation, replace_with_target_arr) -%}
+         {%- do alter_relation_replace_columns(target_relation, replace_with_target_arr, table_type) -%}
        {% endif %}
      {% endif %}
   {% endif %}
   {% set schema_change_message %}
     In {{ target_relation }}:
         Schema change approach: {{ on_schema_change }}
         Columns added: {{ add_to_target_arr }}
@@ -59,18 +59,19 @@
 {% macro athena__alter_column_type(relation, column_name, new_column_type) -%}
   {#
     1. Create a new column (w/ temp name and correct type)
     2. Copy data over to it
     3. Drop the existing column
     4. Rename the new column to existing column
   #}
+  {%- set table_type = config.get('table_type', 'hive') -%}
   {%- set tmp_column = column_name + '__dbt_alter' -%}
-  {%- set new_ddl_data_type = ddl_data_type(new_column_type) -%}
+  {%- set new_ddl_data_type = ddl_data_type(new_column_type, table_type) -%}
 
-  {#- do alter_relation_add_columns(relation, [ tmp_column ]) -#}
+  {#- do alter_relation_add_columns(relation, [ tmp_column ], table_type) -#}
   {%- set add_column_query -%}
     alter {{ relation.type }} {{ relation.render_pure() }} add columns({{ tmp_column }} {{ new_ddl_data_type }});
   {%- endset -%}
   {%- do run_query(add_column_query) -%}
 
   {%- set update_query -%}
     update {{ relation.render_pure() }} set {{ tmp_column }} = cast({{ column_name }} as {{ new_column_type }});
@@ -79,10 +80,10 @@
 
   {#- do alter_relation_drop_columns(relation, [ column_name ]) -#}
   {%- set drop_column_query -%}
     alter {{ relation.type }} {{ relation.render_pure() }} drop column {{ column_name }};
   {%- endset -%}
   {%- do run_query(drop_column_query) -%}
 
-  {%- do alter_relation_rename_column(relation, tmp_column, column_name, new_column_type) -%}
+  {%- do alter_relation_rename_column(relation, tmp_column, column_name, new_column_type, table_type) -%}
 
 {% endmacro %}
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         bucketed_by or bucket_count cannot be used with Iceberg tables. You have to use the bucket function
         when partitioning. Will be ignored
         {%- endset -%}
         {%- set bucketed_by = none -%}
         {%- set bucket_count = none -%}
         {% do log(ignored_bucket_iceberg) %}
       {%- endif -%}
-      {%- if materialization == 'table' and ( 'unique' not in s3_data_naming or external_location is not none) -%}
+      {%- if materialized == 'table' and ( 'unique' not in s3_data_naming or external_location is not none) -%}
         {%- set error_unique_location_iceberg -%}
           You need to have an unique table location when creating Iceberg table since we use the RENAME feature
           to have near-zero downtime.
         {%- endset -%}
         {% do exceptions.raise_compiler_error(error_unique_location_iceberg) %}
       {%- endif -%}
     {%- endif %}
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/models/view/view.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
 
 
       {% if missing_columns %}
-        {% do alter_relation_add_columns(target_relation, missing_columns) %}
+        {% do alter_relation_add_columns(target_relation, missing_columns, table_type) %}
       {% endif %}
 
 
       {% set source_columns = adapter.get_columns_in_relation(staging_table)
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/datediff.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/ddl_dml_data_type.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/ddl_dml_data_type.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 {# Athena has different types between DML and DDL #}
 {# ref: https://docs.aws.amazon.com/athena/latest/ug/data-types.html #}
-{% macro ddl_data_type(col_type) -%}
-  {%- set table_type = config.get('table_type', 'hive') -%}
-
+{% macro ddl_data_type(col_type, table_type = 'hive') -%}
   -- transform varchar
   {% set re = modules.re %}
   {% set data_type = re.sub('(?:varchar|character varying)(?:\(\d+\))?', 'string', col_type) %}
 
   -- transform array and map
   {%- if 'array' in data_type or 'map' in data_type -%}
     {% set data_type = data_type.replace('(', '<').replace(')', '>') -%}
```

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/macros/utils/timestamps.sql` & `dbt_athena_community-1.8.0/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt/include/athena/profile_template.yml` & `dbt_athena_community-1.8.0/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/dbt_athena_community.egg-info/PKG-INFO` & `dbt_athena_community-1.8.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-athena-community
-Version: 1.7.2
-Summary: The athena adapter plugin for dbt (data build tool)
-Home-page: https://github.com/dbt-athena/dbt-athena
-License: Apache License 2.0
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: boto3~=1.34
-Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]~=1.34
-Requires-Dist: dbt-core~=1.7.0
-Requires-Dist: mmh3<4.2.0,>=4.0.1
-Requires-Dist: pyathena<4.0,>=2.25
-Requires-Dist: pydantic<3.0,>=1.10
-Requires-Dist: tenacity~=8.2
-
 <!-- markdownlint-disable-next-line MD041 -->
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/">
       <img src="https://badge.fury.io/py/dbt-athena-community.svg" />
     </a>
     <a target="_blank" href="https://pypi.org/project/dbt-athena-community/" style="background:none">
@@ -528,16 +500,14 @@
 #### HA Known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
-- The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a
-  precision parameter for timestamps
 
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
@@ -842,45 +812,12 @@
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sanromeo"><img src="https://avatars.githubusercontent.com/u/44975602?v=4?s=100" width="100px;" alt="Roman Korsun"/><br /><sub><b>Roman Korsun</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=sanromeo" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asanromeo" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Danya-Fpnk"><img src="https://avatars.githubusercontent.com/u/122433975?v=4?s=100" width="100px;" alt="DanyaF"/><br /><sub><b>DanyaF</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Danya-Fpnk" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ADanya-Fpnk" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/octiva"><img src="https://avatars.githubusercontent.com/u/53303191?v=4?s=100" width="100px;" alt="Spencer"/><br /><sub><b>Spencer</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=octiva" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Avinash-1394"><img src="https://avatars.githubusercontent.com/u/43074786?v=4?s=100" width="100px;" alt="Avinash Santhanagopalan"/><br /><sub><b>Avinash Santhanagopalan</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=Avinash-1394" title="Code">💻</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+<a href="https://github.com/dbt-athena/dbt-athena/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=dbt-athena/dbt-athena" />
+</a>
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.7.2 Summary: The
-athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-boto3~=1.34 Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]~=1.34
-Requires-Dist: dbt-core~=1.7.0 Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist:
-pyathena<4.0,>=2.25 Requires-Dist: pydantic<3.0,>=1.10 Requires-Dist:
-tenacity~=8.2
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
@@ -261,17 +246,15 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed - The macro `athena__end_of_time` needs to be
-overwritten by the user if using Athena engine v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
+older location removed ## Snapshots The adapter supports snapshot
 materialization. It supports both timestamp and check strategy. To create a
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
@@ -386,28 +369,9 @@
 entirely (for instance `array`) even though they won't be checked. Indeed, as
 dbt recommends, we only compare the broader type (array, map, int, varchar).
 The complete definition is used in order to check that the data types defined
 in athena are ok (pre-flight check). - the adapter does not support the
 constraints since no constraints don't exist in Athena. ## Contributing See
 [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
 this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-     _[_n_i_c_o_r_8_8_]      _[_J_e_s_s_e         _[_L_e_m_i_f_f_e_]   _[_J_Ã_©_r_Ã_©_m_y   _[_T_o_m_]        _[_M_a_t_t_i_a_]   _[_G_a_t_s_b_y
-      _nn_ii_cc_oo_rr_88_88     _D_o_b_b_e_l_a_e_r_e_]       _LL_ee_mm_ii_ff_ff_ee    _G_u_i_s_e_l_i_n_]    _TT_oo_mm          _MM_aa_tt_tt_ii_aa     _L_e_e_]
-  _ð___» _ð___§ _ð___     _JJ_ee_ss_ss_ee            _ð___¨     _JJ_?Ã_?©_rr_?Ã_?©_mm_yy  _ð___§ _ð___»        _ð___§     _GG_aa_tt_ss_bb_yy
-                  _DD_oo_bb_bb_ee_ll_aa_ee_rr_ee                   _GG_uu_ii_ss_ee_ll_ii_nn                              _LL_ee_ee
-                   _ð___ _ð___§                   _ð___§ _ð___»                            _ð___
-                                                 _ð___
-_[_B_r_e_c_h_t_D_e_V_l_i_e_g_e_r_]    _[_A_n_d_r_e_a      _[_M_a_i_a_r_a       _[_H_e_n_r_i    _[_S_e_r_h_i_i   _[_c_h_r_i_s_c_h_i_n_4_7_8_] _[_R_o_m_a_n
- _BB_rr_ee_cc_hh_tt_DD_ee_VV_ll_ii_ee_gg_ee_rr    _A_r_t_a_r_i_a_]     _R_e_i_n_a_l_d_o_]     _B_l_a_n_c_k_e_]  _D_i_m_c_h_e_n_k_o_]  _cc_hh_rr_ii_ss_cc_hh_ii_nn_44_77_88  _K_o_r_s_u_n_]
-      _ð___           _AA_nn_dd_rr_ee_aa   _MM_aa_ii_aa_rr_aa_ _RR_ee_ii_nn_aa_ll_dd_oo    _HH_ee_nn_rr_ii     _SS_ee_rr_hh_ii_ii     _ð___» _ð___     _RR_oo_mm_aa_nn
-                     _AA_rr_tt_aa_rr_ii_aa        _ð___        _BB_ll_aa_nn_cc_kk_ee  _DD_ii_mm_cc_hh_ee_nn_kk_oo                 _KK_oo_rr_ss_uu_nn
-                      _ð___                     _ð___» _ð___ _ð___» _ð___                  _ð___»
-                                                                                    _ð___
-      _[_D_a_n_y_a_F_]     _[_S_p_e_n_c_e_r_]      _[_A_v_i_n_a_s_h
-       _DD_aa_nn_yy_aa_FF       _SS_pp_ee_nn_cc_ee_rr   _S_a_n_t_h_a_n_a_g_o_p_a_l_a_n_]
-      _ð___» _ð___      _ð___»         _AA_vv_ii_nn_aa_ss_hh
-                              _SS_aa_nn_tt_hh_aa_nn_aa_gg_oo_pp_aa_ll_aa_nn
-                                    _ð___»
-This project follows the [all-contributors](https://github.com/all-
-contributors/all-contributors) specification. Contributions of any kind
-welcome!
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt-athena-community-1.7.2/dbt_athena_community.egg-info/SOURCES.txt` & `dbt_athena_community-1.8.0/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/pyproject.toml` & `dbt_athena_community-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.7.2/setup.py` & `dbt_athena_community-1.8.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,41 +27,36 @@
 
 
 def _get_package_version() -> str:
     parts = _get_plugin_version_dict()
     return f'{parts["major"]}.{parts["minor"]}.{parts["patch"]}'
 
 
-dbt_version = "1.7"
-package_version = _get_package_version()
 description = "The athena adapter plugin for dbt (data build tool)"
 
-if not package_version.startswith(dbt_version):
-    raise ValueError(f"Invalid setup.py: package_version={package_version} must start with dbt_version={dbt_version}")
-
 
 setup(
     name=package_name,
-    version=package_version,
+    version=_get_package_version(),
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms="any",
     license="Apache License 2.0",
     license_files=("LICENSE.txt",),
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        # In order to control dbt-core version and package version
-        "boto3~=1.34",
-        "boto3-stubs[athena,glue,lakeformation,sts]~=1.34",
-        "dbt-core~=1.7.0",
-        "mmh3>=4.0.1,<4.2.0",
+        "dbt-common>=1.0.0b2,<2.0",
+        "dbt-adapters>=1.0.0b2,<2.0",
+        "boto3>=1.28",
+        "boto3-stubs[athena,glue,lakeformation,sts]>=1.28",
         "pyathena>=2.25,<4.0",
+        "mmh3>=4.0.1,<4.2.0",
         "pydantic>=1.10,<3.0",
         "tenacity~=8.2",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
@@ -69,9 +64,9 @@
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.8,<3.13",
 )
```

