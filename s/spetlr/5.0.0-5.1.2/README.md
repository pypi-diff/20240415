# Comparing `tmp/spetlr-5.0.0.tar.gz` & `tmp/spetlr-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-5.0.0.tar", last modified: Thu Mar 21 13:13:21 2024, max compression
+gzip compressed data, was "spetlr-5.1.2.tar", last modified: Mon Apr 15 07:53:35 2024, max compression
```

## Comparing `spetlr-5.0.0.tar` & `spetlr-5.1.2.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.147560 spetlr-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-21 13:12:56.000000 spetlr-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-21 13:12:56.000000 spetlr-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-03-21 13:13:21.147560 spetlr-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-03-21 13:12:56.000000 spetlr-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-21 13:12:56.000000 spetlr-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-21 13:13:21.147560 spetlr-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 13:12:56.000000 spetlr-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.107560 spetlr-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/azure_log_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/_cli/ConfiguratorCli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.119560 spetlr-5.0.0/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/parse_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/configurator/sql/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.119560 spetlr-5.0.0/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.119560 spetlr-5.0.0/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.119560 spetlr-5.0.0/src/spetlr/deltaspec/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/DeltaDatabaseSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpecBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpecDifference.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/deltaspec/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/check_schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/lazy_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/lazy_simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/extractors/stream_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/load_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/scd2_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/loaders/upsert_loader_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.123560 spetlr-5.0.0/src/spetlr/etl/log/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/log_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/log_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/etl/log/log_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/log_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/log_transformers/count_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/log/log_transformers/null_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/etl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/SimpleSqlTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/clean_column_names_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/data_change_capture_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/dropColumnsTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/generate_md5_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/selectColumnsTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/timezone_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/transformers/validfromto_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/filehandle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/filehandle/file_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.127560 spetlr-5.0.0/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/power_bi/
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/power_bi/PowerBi.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/power_bi/PowerBiClient.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/power_bi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.131560 spetlr-5.0.0/src/spetlr/sqlrepr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sqlrepr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/sqlrepr/sql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/src/spetlr/testutils/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/testutils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/testutils/stop_test_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/DeleteMismatchedSchemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/Md5HashColumn.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-21 13:12:56.000000 spetlr-5.0.0/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.115560 spetlr-5.0.0/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-03-21 13:13:21.000000 spetlr-5.0.0/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 13:13:20.000000 spetlr-5.0.0/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.111560 spetlr-5.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.111560 spetlr-5.0.0/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/delta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/delta/deltaspec/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/deltaspec/test_dbspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/deltaspec/test_tblspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/test_delta_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/test_delta_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/test_filehandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/delta/test_sparkexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.135560 spetlr-5.0.0/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_checkschemaextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_simpleloader_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_upsertloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/etl/test_upsertloader_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/filehandle/test_filehandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/loaders/test_scd2_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_sql_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/transformations/test_simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/cluster/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/utils/test_delete_schema_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/utils/test_spark_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/cluster/utils/test_stop_test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.139560 spetlr-5.0.0/tests/local/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/delta/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/delta/test_DeltaDatabaseSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/delta/test_DeltaTableSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/delta/test_table_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/entry_points/test_generalized_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/etl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/etl/log/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/etl/log/log_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/log/log_transformers/test_count_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/log/log_transformers/test_null_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/log/test_log_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/log/test_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/test_lazy_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/test_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/test_simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/etl/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/filehandle/test_filehandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/power_bi/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/power_bi/test_power_bi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/repr/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/repr/test_repr_sql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/sql/test_SqlExecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.143560 spetlr-5.0.0/tests/local/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/streaming/test_deltahandle_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/streaming/test_stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.147560 spetlr-5.0.0/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_clean_column_names_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_data_change_capture_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_generate_md5_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_select_and_cast_columns_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_timezone_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:13:21.147560 spetlr-5.0.0/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_md5_hashcolumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_selectandcastcolumns.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-21 13:12:56.000000 spetlr-5.0.0/tests/local/utils/test_stop_test_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.782350 spetlr-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 07:53:23.000000 spetlr-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 07:53:23.000000 spetlr-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-15 07:53:35.782350 spetlr-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-15 07:53:23.000000 spetlr-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-15 07:53:23.000000 spetlr-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 07:53:35.782350 spetlr-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:53:23.000000 spetlr-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.738350 spetlr-5.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/azure_log_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/_cli/ConfiguratorCli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.750350 spetlr-5.1.2/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/configurator/sql/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.750350 spetlr-5.1.2/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.750350 spetlr-5.1.2/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.750350 spetlr-5.1.2/src/spetlr/deltaspec/
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/DeltaDatabaseSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpecBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpecDifference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/deltaspec/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.750350 spetlr-5.1.2/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/check_schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/lazy_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/lazy_simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/extractors/stream_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/load_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/scd2_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/loaders/upsert_loader_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/etl/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/log_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/log_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.754350 spetlr-5.1.2/src/spetlr/etl/log/log_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/log_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/log_transformers/count_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/log/log_transformers/null_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/etl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/SimpleSqlTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/clean_column_names_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/data_change_capture_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/dropColumnsTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/generate_md5_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/selectColumnsTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/timezone_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/transformers/validfromto_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/filehandle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/filehandle/file_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.758350 spetlr-5.1.2/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/power_bi/
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/power_bi/PowerBi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/power_bi/PowerBiClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/power_bi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.762350 spetlr-5.1.2/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/src/spetlr/sqlrepr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sqlrepr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/sqlrepr/sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/src/spetlr/testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/testutils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/testutils/stop_test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/DeleteMismatchedSchemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/Md5HashColumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 07:53:23.000000 spetlr-5.1.2/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.746350 spetlr-5.1.2/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:53:35.000000 spetlr-5.1.2/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.742350 spetlr-5.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.742350 spetlr-5.1.2/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/tests/cluster/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.766350 spetlr-5.1.2/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/delta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/delta/deltaspec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/deltaspec/test_dbspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/deltaspec/test_tblspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/test_delta_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/test_filehandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_checkschemaextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_simpleloader_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_upsertloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/etl/test_upsertloader_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/filehandle/test_filehandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/loaders/test_scd2_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.770350 spetlr-5.1.2/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_sql_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/transformations/test_simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/cluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/utils/test_delete_schema_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/utils/test_spark_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/cluster/utils/test_stop_test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/delta/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/delta/test_DeltaDatabaseSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/delta/test_DeltaTableSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/delta/test_table_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.774350 spetlr-5.1.2/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/entry_points/test_generalized_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/etl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/etl/log/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/etl/log/log_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/log/log_transformers/test_count_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/log/log_transformers/test_null_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/log/test_log_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/log/test_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/test_lazy_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/test_simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/etl/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/filehandle/test_filehandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/power_bi/
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/power_bi/test_power_bi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/repr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/repr/test_repr_sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/sql/test_SqlExecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.778350 spetlr-5.1.2/tests/local/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/streaming/test_deltahandle_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/streaming/test_stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.782350 spetlr-5.1.2/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_clean_column_names_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_data_change_capture_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_generate_md5_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_select_and_cast_columns_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_timezone_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:53:35.782350 spetlr-5.1.2/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_md5_hashcolumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_selectandcastcolumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-15 07:53:23.000000 spetlr-5.1.2/tests/local/utils/test_stop_test_streams.py
```

### Comparing `spetlr-5.0.0/LICENSE` & `spetlr-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/PKG-INFO` & `spetlr-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 5.0.0
+Version: 5.1.2
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-5.0.0/README.md` & `spetlr-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/setup.cfg` & `spetlr-5.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py` & `spetlr-5.1.2/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/cache/CachedLoader.py` & `spetlr-5.1.2/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-5.1.2/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/_cli/ConfiguratorCli.py` & `spetlr-5.1.2/src/spetlr/configurator/_cli/ConfiguratorCli.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-5.1.2/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/configurator.py` & `spetlr-5.1.2/src/spetlr/configurator/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,17 @@
         """
         if not kwargs:
             raise ValueError("No value passed.")
 
         key = json_hash(kwargs)
         return self.register(key, kwargs)
 
+    @deprecated(
+        reason="Use .get(table_id,property_name) instead.",
+    )
     def table_property(
         self, table_id: str, property_name: str, default_value: str = None
     ):
         """
         Return the table property (e.g. name, path, format, etc.)
             for the specified table id.
         :param table_id: Table id in the .json or .yaml files.
@@ -391,15 +394,15 @@
 
     def table_name(self, table_id: str):
         """
         Return the table name for the specified table id.
         :param table_id: Table id in the .json or .yaml files.
         :return: str: table name
         """
-        return self.table_property(table_id, "name")
+        return self.get(table_id, "name")
 
     @deprecated(
         reason='Use .get(table_id,"path") instead.',
     )
     def table_path(self, table_id: str):
         """
         Return the table path for the specified table id.
```

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/comments.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/create.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/db.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/substructures.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/table.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/configurator/sql/view.py` & `spetlr-5.1.2/src/spetlr/configurator/sql/view.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/cosmos/cosmos.py` & `spetlr-5.1.2/src/spetlr/cosmos/cosmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             default_ttl=container.get("defaultTtl", None),
             indexing_policy=container.get("indexingPolicy", None),
         )
 
     def from_tc(self, table_id: str) -> CosmosHandle:
         tc = Configurator()
         name = tc.table_name(table_id)
-        rows_per_partition = tc.table_property(table_id, "rows_per_partition", "")
+        rows_per_partition = tc.get(table_id, "rows_per_partition", "")
         rows_per_partition = int(rows_per_partition) if rows_per_partition else None
 
         try:
             schema = SchemaManager().get_schema(table_id)
         except NoSuchSchemaException:
             schema = None
```

### Comparing `spetlr-5.0.0/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-5.1.2/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-5.1.2/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/db_auto.py` & `spetlr-5.1.2/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/delta/db_handle.py` & `spetlr-5.1.2/src/spetlr/delta/db_handle.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         self._validate()
 
     @classmethod
     def from_tc(cls, id: str):
         tc = Configurator()
         return cls(
             name=tc.table_name(id),
-            location=tc.table_property(id, "path", ""),
-            data_format=tc.table_property(id, "format", "db"),
+            location=tc.get(id, "path", ""),
+            data_format=tc.get(id, "format", "db"),
         )
 
     def _validate(self):
         # name is either `db`.`table` or just `table`
         if "." in self._name:
             raise DbHandleInvalidName(f"Invalid DB name {self._name}")
```

### Comparing `spetlr-5.0.0/src/spetlr/delta/delta_handle.py` & `spetlr-5.1.2/src/spetlr/delta/delta_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,21 @@
         if max_bytes_per_trigger and max_bytes_per_trigger != "":
             self._options_dict["maxBytesPerTrigger"] = str(max_bytes_per_trigger)
 
     @classmethod
     def from_tc(cls, id: str) -> "DeltaHandle":
         tc = Configurator()
         return cls(
-            name=tc.table_property(id, "name", ""),
-            location=tc.table_property(id, "path", ""),
+            name=tc.get(id, "name", ""),
+            location=tc.get(id, "path", ""),
             schema=SchemaManager().get_schema(id, None),
-            data_format=tc.table_property(id, "format", "delta"),
-            ignore_changes=tc.table_property(id, "ignore_changes", "True"),
-            stream_start=tc.table_property(id, "stream_start", ""),
-            max_bytes_per_trigger=tc.table_property(id, "max_bytes_per_trigger", ""),
+            data_format=tc.get(id, "format", "delta"),
+            ignore_changes=tc.get(id, "ignore_changes", "True"),
+            stream_start=tc.get(id, "stream_start", ""),
+            max_bytes_per_trigger=tc.get(id, "max_bytes_per_trigger", ""),
         )
 
     def _validate(self):
         """Validates that the name is either db.table or just table."""
         if not self._name:
             if not self._location:
                 raise DeltaHandleInvalidName(
```

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/DeltaDatabaseSpec.py` & `spetlr-5.1.2/src/spetlr/deltaspec/DeltaDatabaseSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpec.py` & `spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpecBase.py` & `spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpecBase.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/DeltaTableSpecDifference.py` & `spetlr-5.1.2/src/spetlr/deltaspec/DeltaTableSpecDifference.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/__init__.py` & `spetlr-5.1.2/src/spetlr/deltaspec/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/exceptions.py` & `spetlr-5.1.2/src/spetlr/deltaspec/exceptions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/deltaspec/helpers.py` & `spetlr-5.1.2/src/spetlr/deltaspec/helpers.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/eh/EventHubCapture.py` & `spetlr-5.1.2/src/spetlr/eh/EventHubCapture.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     partitioning: str
     auto_create: bool
 
     @classmethod
     def from_tc(cls, id: str):
         tc = Configurator()
         return cls(
-            name=tc.table_property(id, "name"),
-            path=tc.table_property(id, "path"),
-            format=tc.table_property(id, "format"),
-            partitioning=tc.table_property(id, "partitioning"),
+            name=tc.get(id, "name"),
+            path=tc.get(id, "path"),
+            format=tc.get(id, "format"),
+            partitioning=tc.get(id, "partitioning"),
         )
 
     def __init__(
         self,
         name: str,
         path: str,
         format: str,
```

### Comparing `spetlr-5.0.0/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-5.1.2/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
     path: str
     partitioning: str
 
     @classmethod
     def from_tc(cls, tbl_id: str):
         tc = Configurator()
-        assert tc.table_property(tbl_id, "format") == "avro"
+        assert tc.get(tbl_id, "format") == "avro"
         return cls(
-            path=tc.table_property(tbl_id, "path"),
-            partitioning=tc.table_property(tbl_id, "partitioning"),
+            path=tc.get(tbl_id, "path"),
+            partitioning=tc.get(tbl_id, "partitioning"),
         )
 
     def __init__(self, path: str, partitioning: str):
         self.path = path
         self.partitioning = partitioning.lower()
         assert self.partitioning in ["ymd", "ymdh"]
```

### Comparing `spetlr-5.0.0/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-5.1.2/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/eh/EventHubStream.py` & `spetlr-5.1.2/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/eh/PartitionSpec.py` & `spetlr-5.1.2/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-5.1.2/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/entry_points/task_entry_point.py` & `spetlr-5.1.2/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/__init__.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/check_schema_extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/check_schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/lazy_extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/lazy_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/lazy_simple_extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/lazy_simple_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-5.1.2/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loader.py` & `spetlr-5.1.2/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/scd2_loader.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/scd2_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/stream_loader.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/loaders/upsert_loader_streaming.py` & `spetlr-5.1.2/src/spetlr/etl/loaders/upsert_loader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/log/log_orchestrator.py` & `spetlr-5.1.2/src/spetlr/etl/log/log_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/log/log_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/log/log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/log/log_transformers/count_log_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/log/log_transformers/count_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/log/log_transformers/null_log_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/log/log_transformers/null_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/orchestrator.py` & `spetlr-5.1.2/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/SimpleSqlTransformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/SimpleSqlTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/__init__.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/clean_column_names_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/clean_column_names_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/country_to_alphacode_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/data_change_capture_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/data_change_capture_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/dropColumnsTransformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/dropColumnsTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/fuzzy_select.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/generate_md5_column_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/generate_md5_column_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/join_dataframes_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/selectColumnsTransformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/selectColumnsTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/simple_sql_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/timezone_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/timezone_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/union_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/etl/transformers/validfromto_transformer.py` & `spetlr-5.1.2/src/spetlr/etl/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/exceptions/__init__.py` & `spetlr-5.1.2/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-5.1.2/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/filehandle/file_handle.py` & `spetlr-5.1.2/src/spetlr/filehandle/file_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/formatting/git_hooks.py` & `spetlr-5.1.2/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/functions.py` & `spetlr-5.1.2/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/mount/main.py` & `spetlr-5.1.2/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-5.1.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-5.1.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-5.1.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/power_bi/PowerBi.py` & `spetlr-5.1.2/src/spetlr/power_bi/PowerBi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import time
 from datetime import datetime, timedelta
+from typing import Dict, List, Union
 
 import msal
 import pandas as pd
 import requests
 from dateutil import parser
 from pytz import timezone, utc
 
 from spetlr.exceptions import SpetlrException
-
-from .PowerBiClient import PowerBiClient
+from spetlr.power_bi.PowerBiClient import PowerBiClient
 
 
 class PowerBi:
     def __init__(
         self,
         client: PowerBiClient,
         *,
         workspace_id: str = None,
         workspace_name: str = None,
         dataset_id: str = None,
         dataset_name: str = None,
+        table_names: List[str] = None,
         max_minutes_after_last_refresh: int = 12 * 60,
         timeout_in_seconds: int = 15 * 60,
         number_of_retries: int = 0,
         local_timezone_name: str = "UTC",
         ignore_errors: bool = False,
     ):
         """
@@ -38,14 +39,16 @@
 
         :param str workspace_id: The GUID of the workspace.
         :param str workspace_name: The name of the workspace
             (specified instead of the workspace_id).
         :param str dataset_id: The GUID of the dataset.
         :param str dataset_name: The name of the dataset
             (specified instead of the dataset_id).
+        :param List[str] table_names: Optional list of table names to be
+            refreshed. By default all tables are refreshed.
         :param int max_minutes_after_last_refresh: The number of minutes
             for which the last succeeded refresh is considered valid,
             or 0 to disable time checking. Default is 12 hours.
         :param bool timeout_in_seconds: The number of seconds after which
             the refresh() method times out. Default is 15 minutes.
         :param int number_of_retries: The number of retries on transient
             errors when calling refresh(). Default is 0 (no retries).
@@ -77,14 +80,15 @@
                 "must be greater than or equal zero!"
             )
 
         self.workspace_id = workspace_id
         self.workspace_name = workspace_name
         self.dataset_id = dataset_id
         self.dataset_name = dataset_name
+        self.table_names = table_names
 
         # Set access parameters
         self.client = client
 
         self.max_minutes_after_last_refresh = max_minutes_after_last_refresh
         self.timeout_in_seconds = timeout_in_seconds
         self.number_of_retries = number_of_retries
@@ -306,15 +310,17 @@
                 end_time = df.endTime[0]
                 if (
                     self.last_status == "Completed"
                     and end_time is not None
                     and len(end_time) > 0
                 ):
                     self.last_refresh_utc = parser.parse(end_time).replace(tzinfo=utc)
-                    if start_time is not None and len(start_time) > 0:
+                    if self.table_names:
+                        self.last_duration_in_seconds = 0
+                    elif start_time is not None and len(start_time) > 0:
                         self.last_duration_in_seconds = int(
                             (
                                 parser.parse(end_time) - parser.parse(start_time)
                             ).total_seconds()
                         )
             return True
         elif api_call.status_code == 404:
@@ -372,14 +378,30 @@
             self._raise_error(f"Last refresh failed! {self.last_exception}")
         else:
             self._raise_error(
                 f"Unknown refresh status: {self.last_status}! {self.last_exception}"
             )
         return False
 
+    def _get_table_names_json(self) -> Union[Dict[str, object], None]:
+        """
+        Returns the HTTP body of the PowerBI refresh API call
+        containing table names to refresh.
+
+        :rtype: JSON object or None
+        """
+        if self.table_names:
+            return {
+                "type": "full",
+                "commitMode": "transactional",
+                "objects": [{"table": table} for table in self.table_names],
+                "applyRefreshPolicy": "false",
+            }
+        return None
+
     def _trigger_new_refresh(self) -> bool:
         """
         Starts a refresh of the PowerBI dataset.
 
         :return: True if succeeded or False if failed (when ignore_errors==True)
         :rtype: bool
         :raises SpetlrException: if failed and ignore_errors==False
@@ -390,15 +412,17 @@
                 print(f"Warning: Last refresh failed! {self.last_exception}")
                 print()
 
             api_url = (
                 f"{self.powerbi_url}groups/{self.workspace_id}"
                 f"/datasets/{self.dataset_id}/refreshes"
             )
-            api_call = requests.post(url=api_url, headers=self.api_header)
+            api_call = requests.post(
+                url=api_url, headers=self.api_header, json=self._get_table_names_json()
+            )
             if api_call.status_code == 202:
                 print("A new refresh has been successfully triggered.")
                 return True
             else:
                 self._raise_api_error("Failed to trigger a refresh!", api_call)
         elif self.last_status == "Unknown":
             print("Refresh is already in progress!")
```

### Comparing `spetlr-5.0.0/src/spetlr/reporting/JobReflection.py` & `spetlr-5.1.2/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/reporting/SlackNotifier.py` & `spetlr-5.1.2/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/schema_manager/schema_manager.py` & `spetlr-5.1.2/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/schema_manager/spark_schema.py` & `spetlr-5.1.2/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/spark.py` & `spetlr-5.1.2/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sql/CommonBaseServer.py` & `spetlr-5.1.2/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sql/SqlBaseServer.py` & `spetlr-5.1.2/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sql/SqlExecutor.py` & `spetlr-5.1.2/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sql/SqlServer.py` & `spetlr-5.1.2/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sql/sql_handle.py` & `spetlr-5.1.2/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/sqlrepr/sql_types.py` & `spetlr-5.1.2/src/spetlr/sqlrepr/sql_types.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/tables/TableHandle.py` & `spetlr-5.1.2/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/testutils/CleanupTestDatabases.py` & `spetlr-5.1.2/src/spetlr/testutils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/testutils/stop_test_streams.py` & `spetlr-5.1.2/src/spetlr/testutils/stop_test_streams.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/transformations.py` & `spetlr-5.1.2/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/transformers/__init__.py` & `spetlr-5.1.2/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/CheckDfMerge.py` & `spetlr-5.1.2/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/DataframeCreator.py` & `spetlr-5.1.2/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/DeleteMismatchedSchemas.py` & `spetlr-5.1.2/src/spetlr/utils/DeleteMismatchedSchemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def get_table_ids_to_check():
     print("Remember to initialize the configurator first!")
     c = Configurator()
     table_ids_to_check = []
     for key in c._raw_resource_details.keys():
-        if c.table_property(key, "delete_on_delta_schema_mismatch", False):
+        if c.get(key, "delete_on_delta_schema_mismatch", False):
             table_ids_to_check.append(key)
     return table_ids_to_check
 
 
 def DeleteMismatchedSchemas(
     table_ids_to_check: List[str] = None,
     spark_executor: SqlExecutor = None,
```

### Comparing `spetlr-5.0.0/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-5.1.2/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/GetMergeStatement.py` & `spetlr-5.1.2/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/Md5HashColumn.py` & `spetlr-5.1.2/src/spetlr/utils/Md5HashColumn.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/MockLoader.py` & `spetlr-5.1.2/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-5.1.2/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr/utils/__init__.py` & `spetlr-5.1.2/src/spetlr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr.egg-info/PKG-INFO` & `spetlr-5.1.2/src/spetlr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 5.0.0
+Version: 5.1.2
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-5.0.0/src/spetlr.egg-info/SOURCES.txt` & `spetlr-5.1.2/src/spetlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/src/spetlr.egg-info/requires.txt` & `spetlr-5.1.2/src/spetlr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py` & `spetlr-5.1.2/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/cache/test_cache.py` & `spetlr-5.1.2/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/cosmos/test_cosmos.py` & `spetlr-5.1.2/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/deltaspec/test_dbspec.py` & `spetlr-5.1.2/tests/cluster/delta/deltaspec/test_dbspec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/deltaspec/test_tblspec.py` & `spetlr-5.1.2/tests/cluster/delta/deltaspec/test_tblspec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-5.1.2/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/test_delta_class.py` & `spetlr-5.1.2/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/test_delta_stream.py` & `spetlr-5.1.2/tests/cluster/delta/test_delta_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/test_filehandle.py` & `spetlr-5.1.2/tests/cluster/delta/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/delta/test_sparkexecutor.py` & `spetlr-5.1.2/tests/cluster/delta/test_sparkexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-5.1.2/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-5.1.2/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/eh/test_eh_saving.py` & `spetlr-5.1.2/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_checkschemaextractor.py` & `spetlr-5.1.2/tests/cluster/etl/test_checkschemaextractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-5.1.2/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_deltaupsert.py` & `spetlr-5.1.2/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_extractor.py` & `spetlr-5.1.2/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-5.1.2/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_loader.py` & `spetlr-5.1.2/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-5.1.2/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_simpleloader_upsert.py` & `spetlr-5.1.2/tests/cluster/etl/test_simpleloader_upsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_upsertloader.py` & `spetlr-5.1.2/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/etl/test_upsertloader_streaming.py` & `spetlr-5.1.2/tests/cluster/etl/test_upsertloader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/filehandle/test_filehandle.py` & `spetlr-5.1.2/tests/cluster/filehandle/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/loaders/test_scd2_loader.py` & `spetlr-5.1.2/tests/cluster/loaders/test_scd2_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-5.1.2/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-5.1.2/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-5.1.2/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/sql/test_deliverysql.py` & `spetlr-5.1.2/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-5.1.2/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/sql/test_sql_streaming.py` & `spetlr-5.1.2/tests/cluster/sql/test_sql_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/sql/test_sqlhandle.py` & `spetlr-5.1.2/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-5.1.2/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/transformations/test_simple_sql_transformer.py` & `spetlr-5.1.2/tests/cluster/transformations/test_simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/transformations/test_union_transformer.py` & `spetlr-5.1.2/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/utils/test_delete_schema_mismatch.py` & `spetlr-5.1.2/tests/cluster/utils/test_delete_schema_mismatch.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/utils/test_spark_version.py` & `spetlr-5.1.2/tests/cluster/utils/test_spark_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/cluster/utils/test_stop_test_stream.py` & `spetlr-5.1.2/tests/cluster/utils/test_stop_test_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py` & `spetlr-5.1.2/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/configurator/test_configurator.py` & `spetlr-5.1.2/tests/local/configurator/test_configurator.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def test_06_freestyle(self):
         tc = Configurator()
         tc.set_prod()
         tc.add_resource_path(tables4)
         details = tc.get_all_details()
         self.assertTrue("MyFreeTable_eggs", details)
-        self.assertEqual(tc.table_property("MyFreeTable", "bacon"), "")
+        self.assertEqual(tc.get("MyFreeTable", "bacon"), "")
 
     def test_07_bare_strings_and_structures(self):
         tc = Configurator()
         tc.set_prod()
         tc.add_resource_path(tables5)
         self.assertEqual(tc.get("MyPlainLiteral"), "Bar")
         self.assertEqual(tc.get_all_details()["MyCompositeLiteral"], "FooBar")
```

### Comparing `spetlr-5.0.0/tests/local/configurator/test_configurator_cli.py` & `spetlr-5.1.2/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/delta/test_DeltaDatabaseSpec.py` & `spetlr-5.1.2/tests/local/delta/test_DeltaDatabaseSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/delta/test_DeltaTableSpec.py` & `spetlr-5.1.2/tests/local/delta/test_DeltaTableSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/delta/test_table_name.py` & `spetlr-5.1.2/tests/local/delta/test_table_name.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-5.1.2/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-5.1.2/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-5.1.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-5.1.2/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-5.1.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/entry_points/test_generalized_entry_points.py` & `spetlr-5.1.2/tests/local/entry_points/test_generalized_entry_points.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/log/log_transformers/test_count_log_transformer.py` & `spetlr-5.1.2/tests/local/etl/log/log_transformers/test_count_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/log/log_transformers/test_null_log_transformer.py` & `spetlr-5.1.2/tests/local/etl/log/log_transformers/test_null_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/log/test_log_orchestrator.py` & `spetlr-5.1.2/tests/local/etl/log/test_log_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/log/test_log_transformer.py` & `spetlr-5.1.2/tests/local/etl/log/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/test_lazy_extractor.py` & `spetlr-5.1.2/tests/local/etl/test_lazy_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/etl/test_transformer.py` & `spetlr-5.1.2/tests/local/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-5.1.2/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/filehandle/test_filehandle.py` & `spetlr-5.1.2/tests/local/filehandle/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/power_bi/test_power_bi.py` & `spetlr-5.1.2/tests/local/power_bi/test_power_bi.py`

 * *Files 5% similar despite different names*

```diff
@@ -188,14 +188,46 @@
         # Act
         with self.assertRaises(SpetlrException) as context:
             sut._verify_last_refresh()
 
         # Assert
         self.assertIn("Last refresh finished more than", str(context.exception))
 
+    def test_get_table_names_json_default(self):
+        # Arrange
+        sut = PowerBi(
+            PowerBiClient(),
+            workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
+            dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
+        )
+
+        # Act
+        result = sut._get_table_names_json()
+
+        # Assert
+        self.assertIsNone(result)
+
+    def test_get_table_names_json_explicit(self):
+        # Arrange
+        sut = PowerBi(
+            PowerBiClient(),
+            workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
+            dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
+            table_names=["Invoices", "Customers"],
+        )
+        expected_result = [{"table": "Invoices"}, {"table": "Customers"}]
+
+        # Act
+        result = sut._get_table_names_json()
+
+        # Assert
+        self.assertIsNotNone(result)
+        self.assertTrue("objects" in result)
+        self.assertEqual(result["objects"], expected_result)
+
     @patch("requests.post")
     def test_trigger_new_refresh_success(self, mock_get):
         # Arrange
         mock_response = Mock()
         mock_response.status_code = 202
         mock_get.return_value = mock_response
```

### Comparing `spetlr-5.0.0/tests/local/reporting/test_slack_reporting.py` & `spetlr-5.1.2/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/repr/test_repr_sql_types.py` & `spetlr-5.1.2/tests/local/repr/test_repr_sql_types.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/schema_manager/test_schema_manager.py` & `spetlr-5.1.2/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/sql/test_SqlExecutor.py` & `spetlr-5.1.2/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/streaming/test_stream_loader.py` & `spetlr-5.1.2/tests/local/streaming/test_stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/test_functions.py` & `spetlr-5.1.2/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/test_get_schema.py` & `spetlr-5.1.2/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/test_sqlServer.py` & `spetlr-5.1.2/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/test_transformations.py` & `spetlr-5.1.2/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_clean_column_names_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_clean_column_names_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_concat_df.py` & `spetlr-5.1.2/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_country_to_alphacode_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_data_change_capture_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_data_change_capture_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_drop_columns.py` & `spetlr-5.1.2/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-5.1.2/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_fuzzy_select.py` & `spetlr-5.1.2/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_generate_md5_column_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_generate_md5_column_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_select_and_cast_columns_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_select_and_cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_select_columns.py` & `spetlr-5.1.2/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_timezone_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_timezone_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_union_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-5.1.2/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_dataframe_creation.py` & `spetlr-5.1.2/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-5.1.2/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_getmergestatement.py` & `spetlr-5.1.2/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_md5_hashcolumn.py` & `spetlr-5.1.2/tests/local/utils/test_md5_hashcolumn.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_mock_etl.py` & `spetlr-5.1.2/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.0.0/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-5.1.2/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

