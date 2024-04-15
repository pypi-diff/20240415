# Comparing `tmp/b2sdk-2.0.0.tar.gz` & `tmp/b2sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sdk-2.0.0.tar", last modified: Tue Apr  2 12:02:25 2024, max compression
+gzip compressed data, was "b2sdk-2.1.0.tar", last modified: Mon Apr 15 13:35:21 2024, max compression
```

## Comparing `b2sdk-2.0.0.tar` & `b2sdk-2.1.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11963 2024-04-02 12:02:17.615899 b2sdk-2.0.0/LICENSE
--rw-r--r--   0        0        0     2219 2024-04-02 12:02:17.615899 b2sdk-2.0.0/README.md
-lrwxr-xr-x   0        0        0        0 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0      422 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/__init__.py
--rw-r--r--   0        0        0      319 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/__main__.py
--rw-r--r--   0        0        0      443 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/__init__.py
--rw-r--r--   0        0        0      414 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/__init__.py
--rw-r--r--   0        0        0    12688 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/abstract.py
--rw-r--r--   0        0        0     1381 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/exception.py
--rw-r--r--   0        0        0     4400 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/in_memory.py
--rw-r--r--   0        0        0    24095 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/sqlite_account_info.py
--rw-r--r--   0        0        0     4349 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/stub.py
--rw-r--r--   0        0        0     3534 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/upload_url_pool.py
--rw-r--r--   0        0        0    26244 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/api.py
--rw-r--r--   0        0        0     1748 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/api_config.py
--rw-r--r--   0        0        0     5835 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/application_key.py
--rw-r--r--   0        0        0    21710 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/b2http.py
--rw-r--r--   0        0        0     2316 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/bounded_queue_executor.py
--rw-r--r--   0        0        0    80069 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/bucket.py
--rw-r--r--   0        0        0     3746 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/cache.py
--rw-r--r--   0        0        0      340 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/__init__.py
--rw-r--r--   0        0        0    12661 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/setting.py
--rw-r--r--   0        0        0     1433 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/types.py
--rw-r--r--   0        0        0    19632 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/exception.py
--rw-r--r--   0        0        0    13765 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/file_lock.py
--rw-r--r--   0        0        0    23877 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/file_version.py
--rw-r--r--   0        0        0     1997 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/filter.py
--rw-r--r--   0        0        0     1555 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/http_constants.py
--rw-r--r--   0        0        0      863 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/included_sources.py
--rw-r--r--   0        0        0      340 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/__init__.py
--rw-r--r--   0        0        0     1496 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/part.py
--rw-r--r--   0        0        0     4777 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/services.py
--rw-r--r--   0        0        0     2923 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/unfinished_large_file.py
--rw-r--r--   0        0        0     7131 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/progress.py
--rw-r--r--   0        0        0    36052 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/raw_api.py
--rw-r--r--   0        0        0    76908 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/raw_simulator.py
--rw-r--r--   0        0        0      341 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/__init__.py
--rw-r--r--   0        0        0     8707 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/monitoring.py
--rw-r--r--   0        0        0     7331 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/setting.py
--rw-r--r--   0        0        0    13198 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/setup.py
--rw-r--r--   0        0        0      710 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/types.py
--rw-r--r--   0        0        0    10141 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/LICENSE
--rw-r--r--   0        0        0      289 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/NOTICE
--rw-r--r--   0        0        0      232 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/README.md
--rw-r--r--   0        0        0     3275 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/__init__.py
--rw-r--r--   0        0        0      868 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/included_source_meta.py
--rw-r--r--   0        0        0      334 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/scan/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/scan/exception.py
--rw-r--r--   0        0        0    15863 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/folder.py
--rw-r--r--   0        0        0     2021 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/folder_parser.py
--rw-r--r--   0        0        0     2724 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/path.py
--rw-r--r--   0        0        0     9060 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/policies.py
--rw-r--r--   0        0        0     6071 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/report.py
--rw-r--r--   0        0        0     3935 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/scan.py
--rw-r--r--   0        0        0    20904 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/session.py
--rw-r--r--   0        0        0      615 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/__init__.py
--rw-r--r--   0        0        0      531 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/base.py
--rw-r--r--   0        0        0     5273 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/chained.py
--rw-r--r--   0        0        0     2389 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/hashing.py
--rw-r--r--   0        0        0     3100 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/progress.py
--rw-r--r--   0        0        0     2597 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/range.py
--rw-r--r--   0        0        0     2278 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/wrapper.py
--rw-r--r--   0        0        0      334 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/__init__.py
--rw-r--r--   0        0        0    18071 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/action.py
--rw-r--r--   0        0        0     3901 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/encryption_provider.py
--rw-r--r--   0        0        0      422 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/exception.py
--rw-r--r--   0        0        0    18364 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/policy.py
--rw-r--r--   0        0        0     4378 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/policy_manager.py
--rw-r--r--   0        0        0     6351 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/report.py
--rw-r--r--   0        0        0    14535 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/sync.py
--rw-r--r--   0        0        0      620 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/__init__.py
--rw-r--r--   0        0        0      345 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/__init__.py
--rw-r--r--   0        0        0    14793 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/emerger.py
--rw-r--r--   0        0        0      556 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/exception.py
--rw-r--r--   0        0        0    29077 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/executor.py
--rw-r--r--   0        0        0      353 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
--rw-r--r--   0        0        0     5456 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
--rw-r--r--   0        0        0    32575 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/planner.py
--rw-r--r--   0        0        0     3582 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
--rw-r--r--   0        0        0     8394 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
--rw-r--r--   0        0        0     3229 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/write_intent.py
--rw-r--r--   0        0        0      346 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/__init__.py
--rw-r--r--   0        0        0     4399 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/download_manager.py
--rw-r--r--   0        0        0     9663 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
--rw-r--r--   0        0        0      357 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
--rw-r--r--   0        0        0    18395 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
--rw-r--r--   0        0        0     3518 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
--rw-r--r--   0        0        0     3114 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
--rw-r--r--   0        0        0      347 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/__init__.py
--rw-r--r--   0        0        0    10338 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_manager.py
--rw-r--r--   0        0        0     3118 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_source.py
--rw-r--r--   0        0        0     2114 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
--rw-r--r--   0        0        0     1804 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/outbound_source.py
--rw-r--r--   0        0        0     1625 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
--rw-r--r--   0        0        0     9583 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_manager.py
--rw-r--r--   0        0        0    13100 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_source.py
--rw-r--r--   0        0        0      560 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/transfer_manager.py
--rw-r--r--   0        0        0    14788 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1561 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/docs.py
--rw-r--r--   0        0        0     1643 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/escape.py
--rw-r--r--   0        0        0      948 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/filesystem.py
--rw-r--r--   0        0        0     1186 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/http_date.py
--rw-r--r--   0        0        0     1660 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/range_.py
--rw-r--r--   0        0        0     3546 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/thread_pool.py
--rw-r--r--   0        0        0      561 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/typing.py
--rw-r--r--   0        0        0     6873 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/version_utils.py
--rw-r--r--   0        0        0      551 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_pyinstaller/__init__.py
--rw-r--r--   0        0        0      417 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_pyinstaller/hook-b2sdk.py
--rw-r--r--   0        0        0    12389 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_v3/__init__.py
--rw-r--r--   0        0        0     7083 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_v3/exception.py
--rw-r--r--   0        0        0      705 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/__init__.py
--rw-r--r--   0        0        0     2035 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/account_info.py
--rw-r--r--   0        0        0      999 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/api.py
--rw-r--r--   0        0        0     1078 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/bucket.py
--rw-r--r--   0        0        0      969 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/exception.py
--rw-r--r--   0        0        0     7245 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/sync.py
--rw-r--r--   0        0        0     1351 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/__init__.py
--rw-r--r--   0        0        0     5908 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/account_info.py
--rw-r--r--   0        0        0     8348 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/api.py
--rw-r--r--   0        0        0     1927 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/b2http.py
--rw-r--r--   0        0        0    13668 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/bucket.py
--rw-r--r--   0        0        0      530 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/cache.py
--rw-r--r--   0        0        0     6787 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/download_dest.py
--rw-r--r--   0        0        0     1580 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/exception.py
--rw-r--r--   0        0        0     2218 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/file_metadata.py
--rw-r--r--   0        0        0     7019 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/file_version.py
--rw-r--r--   0        0        0      334 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/replication/__init__.py
--rw-r--r--   0        0        0     1148 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/replication/monitoring.py
--rw-r--r--   0        0        0     2596 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/session.py
--rw-r--r--   0        0        0      505 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/__init__.py
--rw-r--r--   0        0        0     3869 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/encryption_provider.py
--rw-r--r--   0        0        0     3849 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/file.py
--rw-r--r--   0        0        0     2816 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/file_to_path_translator.py
--rw-r--r--   0        0        0     2318 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/folder.py
--rw-r--r--   0        0        0      738 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/folder_parser.py
--rw-r--r--   0        0        0      846 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/report.py
--rw-r--r--   0        0        0     6929 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/scan_policies.py
--rw-r--r--   0        0        0     5387 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/sync.py
--rw-r--r--   0        0        0     1356 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/__init__.py
--rw-r--r--   0        0        0      454 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/_compat.py
--rw-r--r--   0        0        0      494 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/account_info.py
--rw-r--r--   0        0        0     2235 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/api.py
--rw-r--r--   0        0        0      803 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/b2http.py
--rw-r--r--   0        0        0     3086 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/bucket.py
--rw-r--r--   0        0        0      812 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/exception.py
--rw-r--r--   0        0        0     2902 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/file_version.py
--rw-r--r--   0        0        0     1339 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/large_file.py
--rw-r--r--   0        0        0     2751 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/raw_api.py
--rw-r--r--   0        0        0     3704 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/raw_simulator.py
--rw-r--r--   0        0        0     1523 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/session.py
--rw-r--r--   0        0        0      369 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/sync.py
--rw-r--r--   0        0        0      584 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/transfer.py
--rw-r--r--   0        0        0     1033 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/utils.py
--rw-r--r--   0        0        0     1612 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/version_utils.py
--rw-r--r--   0        0        0      767 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/version.py
--rw-r--r--   0        0        0     4285 2024-04-02 12:02:25.727878 b2sdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11963 2024-04-15 13:35:12.516558 b2sdk-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2219 2024-04-15 13:35:12.516558 b2sdk-2.1.0/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      422 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/__init__.py
+-rw-r--r--   0        0        0      319 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/__main__.py
+-rw-r--r--   0        0        0      443 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/__init__.py
+-rw-r--r--   0        0        0    12688 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/abstract.py
+-rw-r--r--   0        0        0     1381 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/exception.py
+-rw-r--r--   0        0        0     4400 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/in_memory.py
+-rw-r--r--   0        0        0    24095 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/sqlite_account_info.py
+-rw-r--r--   0        0        0     4349 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/stub.py
+-rw-r--r--   0        0        0     3534 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/upload_url_pool.py
+-rw-r--r--   0        0        0    26244 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/api.py
+-rw-r--r--   0        0        0     1748 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/api_config.py
+-rw-r--r--   0        0        0     5835 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/application_key.py
+-rw-r--r--   0        0        0    21710 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/b2http.py
+-rw-r--r--   0        0        0     2316 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/bounded_queue_executor.py
+-rw-r--r--   0        0        0    80634 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/bucket.py
+-rw-r--r--   0        0        0     3746 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/cache.py
+-rw-r--r--   0        0        0      340 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/__init__.py
+-rw-r--r--   0        0        0    12661 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/setting.py
+-rw-r--r--   0        0        0     1433 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/types.py
+-rw-r--r--   0        0        0    20991 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/exception.py
+-rw-r--r--   0        0        0    13765 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/file_lock.py
+-rw-r--r--   0        0        0    23877 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/file_version.py
+-rw-r--r--   0        0        0     1997 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/filter.py
+-rw-r--r--   0        0        0     1555 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/http_constants.py
+-rw-r--r--   0        0        0      863 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/included_sources.py
+-rw-r--r--   0        0        0      340 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/part.py
+-rw-r--r--   0        0        0     4777 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/services.py
+-rw-r--r--   0        0        0     2923 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/unfinished_large_file.py
+-rw-r--r--   0        0        0     7131 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/progress.py
+-rw-r--r--   0        0        0    39876 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/raw_api.py
+-rw-r--r--   0        0        0    80006 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/raw_simulator.py
+-rw-r--r--   0        0        0      341 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/__init__.py
+-rw-r--r--   0        0        0     8707 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/monitoring.py
+-rw-r--r--   0        0        0     7331 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/setting.py
+-rw-r--r--   0        0        0    13198 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/setup.py
+-rw-r--r--   0        0        0      710 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/types.py
+-rw-r--r--   0        0        0    10141 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/LICENSE
+-rw-r--r--   0        0        0      289 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/NOTICE
+-rw-r--r--   0        0        0      232 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/README.md
+-rw-r--r--   0        0        0     3275 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/included_source_meta.py
+-rw-r--r--   0        0        0      334 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/exception.py
+-rw-r--r--   0        0        0    15863 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/folder.py
+-rw-r--r--   0        0        0     2021 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/folder_parser.py
+-rw-r--r--   0        0        0     2724 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/path.py
+-rw-r--r--   0        0        0     9060 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/policies.py
+-rw-r--r--   0        0        0     6071 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/report.py
+-rw-r--r--   0        0        0     3935 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/scan.py
+-rw-r--r--   0        0        0    21244 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/session.py
+-rw-r--r--   0        0        0      615 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/base.py
+-rw-r--r--   0        0        0     5273 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/chained.py
+-rw-r--r--   0        0        0     2389 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/hashing.py
+-rw-r--r--   0        0        0     3100 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/progress.py
+-rw-r--r--   0        0        0     2597 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/range.py
+-rw-r--r--   0        0        0     2278 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/wrapper.py
+-rw-r--r--   0        0        0      334 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/__init__.py
+-rw-r--r--   0        0        0    18071 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/action.py
+-rw-r--r--   0        0        0     3901 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/encryption_provider.py
+-rw-r--r--   0        0        0      422 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/exception.py
+-rw-r--r--   0        0        0    18364 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/policy.py
+-rw-r--r--   0        0        0     4378 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/policy_manager.py
+-rw-r--r--   0        0        0     6351 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/report.py
+-rw-r--r--   0        0        0    14535 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/sync.py
+-rw-r--r--   0        0        0      620 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/__init__.py
+-rw-r--r--   0        0        0      345 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/__init__.py
+-rw-r--r--   0        0        0    14793 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/emerger.py
+-rw-r--r--   0        0        0      556 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/exception.py
+-rw-r--r--   0        0        0    29077 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/executor.py
+-rw-r--r--   0        0        0      353 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
+-rw-r--r--   0        0        0     5456 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
+-rw-r--r--   0        0        0    32575 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/planner.py
+-rw-r--r--   0        0        0     3582 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
+-rw-r--r--   0        0        0     8394 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
+-rw-r--r--   0        0        0     3229 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/write_intent.py
+-rw-r--r--   0        0        0      346 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/__init__.py
+-rw-r--r--   0        0        0     4399 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/download_manager.py
+-rw-r--r--   0        0        0    10032 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
+-rw-r--r--   0        0        0      357 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
+-rw-r--r--   0        0        0    18422 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
+-rw-r--r--   0        0        0     3702 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
+-rw-r--r--   0        0        0     3114 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
+-rw-r--r--   0        0        0      347 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/__init__.py
+-rw-r--r--   0        0        0    10338 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_manager.py
+-rw-r--r--   0        0        0     3118 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_source.py
+-rw-r--r--   0        0        0     2114 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
+-rw-r--r--   0        0        0     1804 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/outbound_source.py
+-rw-r--r--   0        0        0     1625 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
+-rw-r--r--   0        0        0     9583 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_manager.py
+-rw-r--r--   0        0        0    13100 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_source.py
+-rw-r--r--   0        0        0      560 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/transfer_manager.py
+-rw-r--r--   0        0        0    14788 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1561 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/docs.py
+-rw-r--r--   0        0        0     1643 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/escape.py
+-rw-r--r--   0        0        0      948 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0     1186 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/http_date.py
+-rw-r--r--   0        0        0     1660 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/range_.py
+-rw-r--r--   0        0        0     3546 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/thread_pool.py
+-rw-r--r--   0        0        0      561 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/typing.py
+-rw-r--r--   0        0        0     7160 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/version_utils.py
+-rw-r--r--   0        0        0      551 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_pyinstaller/hook-b2sdk.py
+-rw-r--r--   0        0        0    12542 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_v3/__init__.py
+-rw-r--r--   0        0        0     7083 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_v3/exception.py
+-rw-r--r--   0        0        0      705 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/__init__.py
+-rw-r--r--   0        0        0     2035 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/account_info.py
+-rw-r--r--   0        0        0      999 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/api.py
+-rw-r--r--   0        0        0     1078 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/bucket.py
+-rw-r--r--   0        0        0      969 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/exception.py
+-rw-r--r--   0        0        0     7245 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/sync.py
+-rw-r--r--   0        0        0     1351 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/__init__.py
+-rw-r--r--   0        0        0     5908 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/account_info.py
+-rw-r--r--   0        0        0     8348 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/api.py
+-rw-r--r--   0        0        0     1927 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/b2http.py
+-rw-r--r--   0        0        0    13668 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/bucket.py
+-rw-r--r--   0        0        0      530 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/cache.py
+-rw-r--r--   0        0        0     6787 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/download_dest.py
+-rw-r--r--   0        0        0     1580 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/exception.py
+-rw-r--r--   0        0        0     2218 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/file_metadata.py
+-rw-r--r--   0        0        0     7019 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/file_version.py
+-rw-r--r--   0        0        0      334 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/replication/__init__.py
+-rw-r--r--   0        0        0     1148 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/replication/monitoring.py
+-rw-r--r--   0        0        0     2596 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/session.py
+-rw-r--r--   0        0        0      505 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/encryption_provider.py
+-rw-r--r--   0        0        0     3849 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/file.py
+-rw-r--r--   0        0        0     2816 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/file_to_path_translator.py
+-rw-r--r--   0        0        0     2318 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/folder.py
+-rw-r--r--   0        0        0      738 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/folder_parser.py
+-rw-r--r--   0        0        0      846 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/report.py
+-rw-r--r--   0        0        0     6929 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/scan_policies.py
+-rw-r--r--   0        0        0     5387 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/sync.py
+-rw-r--r--   0        0        0     1356 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v2/__init__.py
+-rw-r--r--   0        0        0      454 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v2/_compat.py
+-rw-r--r--   0        0        0      494 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/account_info.py
+-rw-r--r--   0        0        0     2235 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/api.py
+-rw-r--r--   0        0        0      803 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/b2http.py
+-rw-r--r--   0        0        0     3086 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/bucket.py
+-rw-r--r--   0        0        0      812 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/exception.py
+-rw-r--r--   0        0        0     2902 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/file_version.py
+-rw-r--r--   0        0        0     1339 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/large_file.py
+-rw-r--r--   0        0        0     2751 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/raw_api.py
+-rw-r--r--   0        0        0     3704 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/raw_simulator.py
+-rw-r--r--   0        0        0     1523 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/session.py
+-rw-r--r--   0        0        0      369 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/sync.py
+-rw-r--r--   0        0        0      584 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/transfer.py
+-rw-r--r--   0        0        0     1033 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/utils.py
+-rw-r--r--   0        0        0     1612 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/version_utils.py
+-rw-r--r--   0        0        0      767 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/version.py
+-rw-r--r--   0        0        0     4436 2024-04-15 13:35:21.780540 b2sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.1.0/PKG-INFO
```

### Comparing `b2sdk-2.0.0/LICENSE` & `b2sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/README.md` & `b2sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/abstract.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/exception.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/in_memory.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/in_memory.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/sqlite_account_info.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/sqlite_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/stub.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/stub.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/account_info/upload_url_pool.py` & `b2sdk-2.1.0/b2sdk/_internal/account_info/upload_url_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/api.py` & `b2sdk-2.1.0/b2sdk/_internal/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/api_config.py` & `b2sdk-2.1.0/b2sdk/_internal/api_config.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/application_key.py` & `b2sdk-2.1.0/b2sdk/_internal/application_key.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/b2http.py` & `b2sdk-2.1.0/b2sdk/_internal/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/bounded_queue_executor.py` & `b2sdk-2.1.0/b2sdk/_internal/bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/bucket.py` & `b2sdk-2.1.0/b2sdk/_internal/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from __future__ import annotations
 
 import datetime as dt
 import fnmatch
 import logging
 import pathlib
 from contextlib import suppress
-from typing import Sequence
+from typing import Iterable, Sequence
 
 from .encryption.setting import EncryptionSetting, EncryptionSettingFactory
 from .encryption.types import EncryptionMode
 from .exception import (
     BucketIdNotFound,
     CopySourceTooBig,
     FileNotPresent,
@@ -33,15 +33,15 @@
     FileRetentionSetting,
     LegalHold,
 )
 from .file_version import DownloadVersion, FileVersion
 from .filter import Filter, FilterMatcher
 from .http_constants import LIST_FILE_NAMES_MAX_LIMIT
 from .progress import AbstractProgressListener, DoNothingProgressListener
-from .raw_api import LifecycleRule
+from .raw_api import LifecycleRule, NotificationRule, NotificationRuleResponse
 from .replication.setting import ReplicationConfiguration, ReplicationConfigurationFactory
 from .transfer.emerge.executor import AUTO_CONTENT_TYPE
 from .transfer.emerge.unbound_write_intent import UnboundWriteIntentGenerator
 from .transfer.emerge.write_intent import WriteIntent
 from .transfer.inbound.downloaded_file import DownloadedFile
 from .transfer.outbound.copy_source import CopySource
 from .transfer.outbound.upload_source import UploadMode, UploadSourceBytes, UploadSourceLocalFile
@@ -1488,14 +1488,27 @@
         result['replication'] = self.replication and self.replication.as_dict()
 
         return result
 
     def __repr__(self):
         return f'Bucket<{self.id_},{self.name},{self.type_}>'
 
+    def get_notification_rules(self) -> list[NotificationRuleResponse]:
+        """
+        Get all notification rules for this bucket.
+        """
+        return self.api.session.get_bucket_notification_rules(self.id_)
+
+    def set_notification_rules(self,
+                               rules: Iterable[NotificationRule]) -> list[NotificationRuleResponse]:
+        """
+        Set notification rules for this bucket.
+        """
+        return self.api.session.set_bucket_notification_rules(self.id_, rules)
+
 
 class BucketFactory:
     """
     This is a factory for creating bucket objects from different kind of objects.
     """
     BUCKET_CLASS = staticmethod(Bucket)
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/cache.py` & `b2sdk-2.1.0/b2sdk/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/encryption/setting.py` & `b2sdk-2.1.0/b2sdk/_internal/encryption/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/encryption/types.py` & `b2sdk-2.1.0/b2sdk/_internal/encryption/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/exception.py` & `b2sdk-2.1.0/b2sdk/_internal/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 from __future__ import annotations
 
 import logging
 import re
+import typing
 import warnings
 from abc import ABCMeta
 from typing import Any
 
 from .utils import camelcase_to_underscore, trace_call
 
 UPLOAD_TOKEN_USED_CONCURRENTLY_ERROR_MESSAGE_RE = re.compile(
@@ -570,23 +571,77 @@
     pass
 
 
 class DestinationDirectoryDoesntAllowOperation(DestinationDirectoryError):
     pass
 
 
+class EventTypeError(BadRequest):
+    pass
+
+
+class EventTypeCategoriesError(EventTypeError):
+    pass
+
+
+class EventTypeOverlapError(EventTypeError):
+    pass
+
+
+class EventTypesEmptyError(EventTypeError):
+    pass
+
+
+class EventTypeInvalidError(EventTypeError):
+    pass
+
+
+def _event_type_invalid_error(code: str, message: str, **_) -> B2Error:
+    from b2sdk._internal.raw_api import EVENT_TYPE
+
+    valid_types = sorted(typing.get_args(EVENT_TYPE))
+    return EventTypeInvalidError(
+        f"Event Type error: {message!r}. Valid types: {sorted(valid_types)!r}", code
+    )
+
+
+_error_handlers: dict[tuple[int, str | None], typing.Callable] = {
+    (400, "event_type_categories"):
+        lambda code, message, **_: EventTypeCategoriesError(message, code),
+    (400, "event_type_overlap"):
+        lambda code, message, **_: EventTypeOverlapError(message, code),
+    (400, "event_types_empty"):
+        lambda code, message, **_: EventTypesEmptyError(message, code),
+    (400, "event_type_invalid"):
+        _event_type_invalid_error,
+}
+
+
 @trace_call(logger)
 def interpret_b2_error(
     status: int,
     code: str | None,
     message: str | None,
     response_headers: dict[str, Any],
     post_params: dict[str, Any] | None = None
 ) -> B2Error:
     post_params = post_params or {}
+
+    handler = _error_handlers.get((status, code))
+    if handler:
+        error = handler(
+            status=status,
+            code=code,
+            message=message,
+            response_headers=response_headers,
+            post_params=post_params
+        )
+        if error:
+            return error
+
     if status == 400 and code == "already_hidden":
         return FileAlreadyHidden(post_params.get('fileName'))
     elif status == 400 and code == 'bad_json':
         return BadJson(message)
     elif (
         (status == 400 and code in ("no_such_file", "file_not_present")) or
         (status == 404 and code == "not_found")
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/file_lock.py` & `b2sdk-2.1.0/b2sdk/_internal/file_lock.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/file_version.py` & `b2sdk-2.1.0/b2sdk/_internal/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/filter.py` & `b2sdk-2.1.0/b2sdk/_internal/filter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/http_constants.py` & `b2sdk-2.1.0/b2sdk/_internal/http_constants.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/included_sources.py` & `b2sdk-2.1.0/b2sdk/_internal/included_sources.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/large_file/part.py` & `b2sdk-2.1.0/b2sdk/_internal/large_file/part.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/large_file/services.py` & `b2sdk-2.1.0/b2sdk/_internal/large_file/services.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/large_file/unfinished_large_file.py` & `b2sdk-2.1.0/b2sdk/_internal/large_file/unfinished_large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/progress.py` & `b2sdk-2.1.0/b2sdk/_internal/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/raw_api.py` & `b2sdk-2.1.0/b2sdk/_internal/raw_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 from __future__ import annotations
 
 import base64
+import functools
+import warnings
 from abc import ABCMeta, abstractmethod
 from enum import Enum, unique
 from logging import getLogger
-from typing import Any
+from typing import Any, Iterable
 
 from .utils.escape import unprintable_to_hex
 from .utils.typing import JSON
+from .version_utils import FeaturePreviewWarning
 
 try:
-    from typing_extensions import NotRequired, TypedDict
+    from typing_extensions import Literal, NotRequired, TypedDict
 except ImportError:
-    from typing import NotRequired, TypedDict
+    from typing import Literal, NotRequired, TypedDict
 
 from .encryption.setting import EncryptionMode, EncryptionSetting
 from .exception import (
     AccessDenied,
     FileOrBucketNotFound,
     InvalidMetadataDirective,
     ResourceNotFound,
@@ -69,14 +72,16 @@
     'writeBucketReplications',
     'bypassGovernance',
     'listFiles',
     'readFiles',
     'shareFiles',
     'writeFiles',
     'deleteFiles',
+    'readBucketNotifications',
+    'writeBucketNotifications',
 ]
 
 # API version number to use when calling the service
 API_VERSION = 'v2'
 
 logger = getLogger(__name__)
 
@@ -98,14 +103,90 @@
     .. _B2 Cloud Storage Lifecycle Rules: https://www.backblaze.com/docs/cloud-storage-lifecycle-rules
     """
     fileNamePrefix: str
     daysFromHidingToDeleting: NotRequired[int | None]
     daysFromUploadingToHiding: NotRequired[int | None]
 
 
+class NameValueDict(TypedDict):
+    name: str
+    value: str
+
+
+class NotificationTargetConfiguration(TypedDict):
+    """
+    Notification Target Configuration.
+
+    `hmacSha256SigningSecret`, if present, has to be a string of 32 alphanumeric characters.
+    """
+    # TODO: add URL to the documentation
+
+    targetType: Literal['webhook']
+    url: str
+    customHeaders: NotRequired[list[NameValueDict] | None]
+    hmacSha256SigningSecret: NotRequired[str]
+
+
+EVENT_TYPE = Literal[
+    'b2:ObjectCreated:*', 'b2:ObjectCreated:Upload', 'b2:ObjectCreated:MultipartUpload',
+    'b2:ObjectCreated:Copy', 'b2:ObjectCreated:Replica', 'b2:ObjectCreated:MultipartReplica',
+    'b2:ObjectDeleted:*', 'b2:ObjectDeleted:Delete', 'b2:ObjectDeleted:LifecycleRule',
+    'b2:HideMarkerCreated:*', 'b2:HideMarkerCreated:Hide', 'b2:HideMarkerCreated:LifecycleRule',]
+
+
+class _NotificationRule(TypedDict):
+    """
+    Notification Rule.
+    """
+    eventTypes: list[EVENT_TYPE]
+    isEnabled: bool
+    name: str
+    objectNamePrefix: str
+    targetConfiguration: NotificationTargetConfiguration
+    suspensionReason: NotRequired[str]
+
+
+class NotificationRule(_NotificationRule):
+    """
+    Notification Rule.
+
+    When creating or modifying a notification rule, `isSuspended` and `suspensionReason` are ignored.
+    """
+    isSuspended: NotRequired[bool]
+
+
+class NotificationRuleResponse(_NotificationRule):
+    isSuspended: bool
+
+
+def _bucket_notification_rule_feature_preview_warning(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        warnings.warn(
+            "Event Notifications feature is in \"Private Preview\" state and may change without notice. "
+            "See https://www.backblaze.com/blog/announcing-event-notifications/ for details.",
+            FeaturePreviewWarning,
+            stacklevel=2,
+        )
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+@_bucket_notification_rule_feature_preview_warning
+def notification_rule_response_to_request(rule: NotificationRuleResponse) -> NotificationRule:
+    """
+    Convert NotificationRuleResponse to NotificationRule.
+    """
+    rule = rule.copy()
+    for key in ('isSuspended', 'suspensionReason'):
+        rule.pop(key, None)
+    return rule
+
+
 class AbstractRawApi(metaclass=ABCMeta):
     """
     Direct access to the B2 web apis.
     """
 
     @abstractmethod
     def authorize_account(self, realm_url, application_key_id, application_key):
@@ -411,14 +492,26 @@
 
     def get_download_url_by_id(self, download_url, file_id):
         return f'{download_url}/b2api/{API_VERSION}/b2_download_file_by_id?fileId={file_id}'
 
     def get_download_url_by_name(self, download_url, bucket_name, file_name):
         return download_url + '/file/' + bucket_name + '/' + b2_url_encode(file_name)
 
+    @abstractmethod
+    def set_bucket_notification_rules(
+        self, api_url: str, account_auth_token: str, bucket_id: str,
+        rules: Iterable[NotificationRule]
+    ) -> list[NotificationRuleResponse]:
+        pass
+
+    @abstractmethod
+    def get_bucket_notification_rules(self, api_url: str, account_auth_token: str,
+                                      bucket_id: str) -> list[NotificationRuleResponse]:
+        pass
+
 
 class B2RawHTTPApi(AbstractRawApi):
     """
     Provide access to the B2 web APIs, exactly as they are provided by b2.
 
     Requires that you provide all necessary URLs and auth tokens for each call.
 
@@ -1084,14 +1177,40 @@
                 largeFileId=large_file_id,
                 partNumber=part_number,
                 **kwargs
             )
         except AccessDenied:
             raise SSECKeyError()
 
+    @_bucket_notification_rule_feature_preview_warning
+    def set_bucket_notification_rules(
+        self, api_url: str, account_auth_token: str, bucket_id: str, rules: list[NotificationRule]
+    ) -> list[NotificationRuleResponse]:
+        return self._post_json(
+            api_url,
+            'b2_set_bucket_notification_rules',
+            account_auth_token,
+            **{
+                'bucketId': bucket_id,
+                'eventNotificationRules': rules,
+            },
+        )["eventNotificationRules"]
+
+    @_bucket_notification_rule_feature_preview_warning
+    def get_bucket_notification_rules(self, api_url: str, account_auth_token: str,
+                                      bucket_id: str) -> list[NotificationRuleResponse]:
+        return self._get_json(
+            api_url,
+            'b2_get_bucket_notification_rules',
+            account_auth_token,
+            **{
+                'bucketId': bucket_id,
+            },
+        )["eventNotificationRules"]
+
 
 def _add_range_header(headers, range_):
     if range_ is not None:
         assert len(range_) == 2, range_
         assert (range_[0] + 0) <= (range_[1] + 0), range_  # not strings
         assert range_[0] >= 0, range_
         headers['Range'] = "bytes=%d-%d" % range_
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/raw_simulator.py` & `b2sdk-2.1.0/b2sdk/_internal/raw_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 from __future__ import annotations
 
 import collections
+import dataclasses
 import io
 import logging
 import random
 import re
 import threading
 import time
 from contextlib import contextmanager, suppress
+from typing import Iterable
 
 from requests.structures import CaseInsensitiveDict
 
 from .b2http import ResponseContextManager
 from .encryption.setting import EncryptionMode, EncryptionSetting
 from .exception import (
     AccessDenied,
@@ -35,29 +37,37 @@
     FileNotPresent,
     FileSha1Mismatch,
     InvalidAuthToken,
     InvalidMetadataDirective,
     MissingPart,
     NonExistentBucket,
     PartSha1Mismatch,
+    ResourceNotFound,
     SourceReplicationConflict,
     SSECKeyError,
     Unauthorized,
     UnsatisfiableRange,
 )
 from .file_lock import (
     NO_RETENTION_BUCKET_SETTING,
     BucketRetentionSetting,
     FileRetentionSetting,
     LegalHold,
     RetentionMode,
 )
 from .file_version import UNVERIFIED_CHECKSUM_PREFIX
 from .http_constants import FILE_INFO_HEADER_PREFIX, HEX_DIGITS_AT_END
-from .raw_api import ALL_CAPABILITIES, AbstractRawApi, LifecycleRule, MetadataDirectiveMode
+from .raw_api import (
+    ALL_CAPABILITIES,
+    AbstractRawApi,
+    LifecycleRule,
+    MetadataDirectiveMode,
+    NotificationRule,
+    NotificationRuleResponse,
+)
 from .replication.setting import ReplicationConfiguration
 from .replication.types import ReplicationStatus
 from .stream.hashing import StreamWithHash
 from .utils import ConcurrentUsedAuthTokenGuard, b2_url_decode, b2_url_encode, hex_sha1_of_bytes
 
 logger = logging.getLogger(__name__)
 
@@ -443,33 +453,60 @@
         if encryption.key is None:
             secret = None
         else:
             secret = encryption.key.secret
         return mode, secret
 
 
-FakeRequest = collections.namedtuple('FakeRequest', 'url headers')
+@dataclasses.dataclass
+class FakeRequest:
+    url: str
+    headers: CaseInsensitiveDict
+
+
+@dataclasses.dataclass
+class FakeRaw:
+    data_bytes: bytes
+    _position: int = 0
+
+    def tell(self):
+        return self._position
+
+    def read(self, size):
+        data = self.data_bytes[self._position:self._position + size]
+        self._position += len(data)
+        return data
 
 
 class FakeResponse:
     def __init__(self, account_auth_token_or_none, file_sim, url, range_=None):
-        self.data_bytes = file_sim.data_bytes
+        self.raw = FakeRaw(file_sim.data_bytes)
         self.headers = file_sim.as_download_headers(account_auth_token_or_none, range_)
         self.url = url
         self.range_ = range_
         if range_ is not None:
             self.data_bytes = self.data_bytes[range_[0]:range_[1] + 1]
 
+    @property
+    def data_bytes(self):
+        return self.raw.data_bytes
+
+    @data_bytes.setter
+    def data_bytes(self, value):
+        self.raw = FakeRaw(value)
+
     def iter_content(self, chunk_size=1):
-        start = 0
         rnd = random.Random(self.url)
-        while start <= len(self.data_bytes):
-            time.sleep(rnd.random() * 0.01)
-            yield self.data_bytes[start:start + chunk_size]
-            start += chunk_size
+        while True:
+            chunk = self.raw.read(chunk_size)
+            if chunk:
+                time.sleep(rnd.random() * 0.01)
+                yield chunk
+            else:
+                break
 
     @property
     def request(self):
         headers = CaseInsensitiveDict()
         if self.range_ is not None:
             headers['Range'] = '{}-{}'.format(*self.range_)
         return FakeRequest(self.url, headers)
@@ -510,14 +547,15 @@
         self.account_id = account_id
         self.bucket_name = bucket_name
         self.bucket_id = bucket_id
         self.bucket_type = bucket_type
         self.bucket_info = bucket_info or {}
         self.cors_rules = cors_rules or []
         self.lifecycle_rules = lifecycle_rules or []
+        self._notification_rules = []
         self.options_set = options_set or set()
         self.revision = 1
         self.upload_url_counter = iter(range(200))
         # File IDs count down, so that the most recent will come first when they are sorted.
         self.file_id_counter = iter(range(self.FIRST_FILE_NUMBER, 0, -1))
         self.upload_timestamp_counter = iter(range(5000, 9999))
         self.file_id_to_file: dict[str, FileSimulator] = dict()
@@ -1128,14 +1166,52 @@
         if content_length % chunk_size > 0:
             chunks_number = chunks_number + 1
         return chunks_number
 
     def _next_file_id(self):
         return str(next(self.file_id_counter))
 
+    def get_notification_rules(self) -> list[NotificationRule]:
+        return self._notification_rules
+
+    def set_notification_rules(self,
+                               rules: Iterable[NotificationRule]) -> list[NotificationRuleResponse]:
+        old_rules_by_name = {rule["name"]: rule for rule in self._notification_rules}
+        new_rules: list[NotificationRuleResponse] = []
+        for rule in rules:
+            for field in ("isSuspended", "suspensionReason"):
+                rule.pop(field, None)
+            old_rule = old_rules_by_name.get(rule["name"], {"targetConfiguration": {}})
+            new_rule = {
+                **{
+                    "isSuspended": False,
+                    "suspensionReason": "",
+                },
+                **old_rule,
+                **rule,
+                "targetConfiguration":
+                    {
+                        **old_rule.get("targetConfiguration", {}),
+                        **rule.get("targetConfiguration", {}),
+                    },
+            }
+            new_rules.append(new_rule)
+        self._notification_rules = new_rules
+        return self._notification_rules
+
+    def simulate_notification_rule_suspension(
+        self, rule_name: str, reason: str, is_suspended: bool | None = None
+    ) -> None:
+        for rule in self._notification_rules:
+            if rule["name"] == rule_name:
+                rule["isSuspended"] = bool(reason) if is_suspended is None else is_suspended
+                rule["suspensionReason"] = reason
+                return
+        raise ResourceNotFound(f"Rule {rule_name} not found")
+
 
 class RawSimulator(AbstractRawApi):
     """
     Implement the same interface as B2RawHTTPApi by simulating all of the
     calls and keeping state in memory.
 
     The intended use for this class is for unit tests that test things
@@ -1203,14 +1279,16 @@
         auth_token_expired error.
         """
         assert auth_token in self.auth_token_to_key
         self.expired_auth_tokens.add(auth_token)
 
     def create_account(self):
         """
+        Simulate creating an account.
+
         Return (accountId, masterApplicationKey) for a newly created account.
         """
         # Pick the IDs for the account and the key
         account_id = 'account-%d' % (self.account_counter,)
         master_key = 'masterKey-%d' % (self.account_counter,)
         self.account_counter += 1
 
@@ -1941,7 +2019,25 @@
             raise NonExistentBucket(bucket_id)
         return self.bucket_id_to_bucket[bucket_id]
 
     def _get_bucket_by_name(self, bucket_name):
         if bucket_name not in self.bucket_name_to_bucket:
             raise NonExistentBucket(bucket_name)
         return self.bucket_name_to_bucket[bucket_name]
+
+    def set_bucket_notification_rules(
+        self, api_url: str, account_auth_token: str, bucket_id: str,
+        rules: Iterable[NotificationRule]
+    ):
+        bucket = self._get_bucket_by_id(bucket_id)
+        self._assert_account_auth(
+            api_url, account_auth_token, bucket.account_id, 'writeBucketNotifications'
+        )
+        return bucket.set_notification_rules(rules)
+
+    def get_bucket_notification_rules(self, api_url: str, account_auth_token: str,
+                                      bucket_id: str) -> list[NotificationRule]:
+        bucket = self._get_bucket_by_id(bucket_id)
+        self._assert_account_auth(
+            api_url, account_auth_token, bucket.account_id, 'readBucketNotifications'
+        )
+        return bucket.get_notification_rules()
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/replication/monitoring.py` & `b2sdk-2.1.0/b2sdk/_internal/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/replication/setting.py` & `b2sdk-2.1.0/b2sdk/_internal/replication/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/replication/setup.py` & `b2sdk-2.1.0/b2sdk/_internal/replication/setup.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/replication/types.py` & `b2sdk-2.1.0/b2sdk/_internal/replication/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/requests/LICENSE` & `b2sdk-2.1.0/b2sdk/_internal/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/requests/__init__.py` & `b2sdk-2.1.0/b2sdk/_internal/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/requests/included_source_meta.py` & `b2sdk-2.1.0/b2sdk/_internal/requests/included_source_meta.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/exception.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/folder.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/folder.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/folder_parser.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/path.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/path.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/policies.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/report.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/scan/scan.py` & `b2sdk-2.1.0/b2sdk/_internal/scan/scan.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/session.py` & `b2sdk-2.1.0/b2sdk/_internal/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,7 +568,15 @@
     ):
         return self._wrap_default_token(
             self.raw_api.update_file_legal_hold,
             file_id,
             file_name,
             legal_hold,
         )
+
+    def get_bucket_notification_rules(self, bucket_id):
+        return self._wrap_default_token(self.raw_api.get_bucket_notification_rules, bucket_id)
+
+    def set_bucket_notification_rules(self, bucket_id, rules):
+        return self._wrap_default_token(
+            self.raw_api.set_bucket_notification_rules, bucket_id, rules
+        )
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/__init__.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/base.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/base.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/chained.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/chained.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/hashing.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/hashing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/progress.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/range.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/range.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/stream/wrapper.py` & `b2sdk-2.1.0/b2sdk/_internal/stream/wrapper.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/action.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/action.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/encryption_provider.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/policy.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/policy.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/policy_manager.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/policy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/report.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/sync/sync.py` & `b2sdk-2.1.0/b2sdk/_internal/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/__init__.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/emerger.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/emerger.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/exception.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/executor.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/planner.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/planner.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/write_intent.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/download_manager.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/download_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloaded_file.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloaded_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,23 @@
         """
         if allow_seeking is None:
             allow_seeking = file.seekable()
         elif allow_seeking and not file.seekable():
             logger.warning('File is not seekable, disabling strategies that require seeking')
             allow_seeking = False
 
+        if allow_seeking:  # check if file allows reading from arbitrary position
+            try:
+                file.read(0)
+            except io.UnsupportedOperation:
+                logger.warning(
+                    'File is seekable, but does not allow reads, disabling strategies that require seeking'
+                )
+                allow_seeking = False
+
         if self.progress_listener:
             file = WritingStreamWithProgress(file, self.progress_listener)
             if self.range_ is not None:
                 total_bytes = self.range_[1] - self.range_[0] + 1
             else:
                 total_bytes = self.download_version.content_length
             self.progress_listener.set_total_bytes(total_bytes)
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,95 @@
 ######################################################################
 #
-# File: b2sdk/_internal/transfer/inbound/downloader/abstract.py
+# File: b2sdk/_internal/transfer/inbound/downloader/simple.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 from __future__ import annotations
 
-import hashlib
-from abc import abstractmethod
-from concurrent.futures import ThreadPoolExecutor
+import logging
 from io import IOBase
 
 from requests.models import Response
 
 from b2sdk._internal.encryption.setting import EncryptionSetting
 from b2sdk._internal.file_version import DownloadVersion
 from b2sdk._internal.session import B2Session
-from b2sdk._internal.utils import B2TraceMetaAbstract
-from b2sdk._internal.utils.range_ import Range
 
+from .abstract import AbstractDownloader
 
-class EmptyHasher:
-    def __init__(self, *args, **kwargs):
-        pass
+logger = logging.getLogger(__name__)
 
-    def update(self, data):
-        pass
 
-    def digest(self):
-        return b''
+class SimpleDownloader(AbstractDownloader):
 
-    def hexdigest(self):
-        return ''
+    REQUIRES_SEEKING = False
+    SUPPORTS_DECODE_CONTENT = True
 
-    def copy(self):
-        return self
-
-
-class AbstractDownloader(metaclass=B2TraceMetaAbstract):
-
-    REQUIRES_SEEKING = True
-    DEFAULT_THREAD_POOL_CLASS = staticmethod(ThreadPoolExecutor)
-    DEFAULT_ALIGN_FACTOR = 4096
-
-    def __init__(
+    def _download(
         self,
-        thread_pool: ThreadPoolExecutor | None = None,
-        force_chunk_size: int | None = None,
-        min_chunk_size: int | None = None,
-        max_chunk_size: int | None = None,
-        align_factor: int | None = None,
-        check_hash: bool = True,
-        **kwargs
+        file: IOBase,
+        response: Response,
+        download_version: DownloadVersion,
+        session: B2Session,
+        encryption: EncryptionSetting | None = None,
     ):
-        align_factor = align_factor or self.DEFAULT_ALIGN_FACTOR
-        assert force_chunk_size is not None or (
-            min_chunk_size is not None and max_chunk_size is not None and
-            0 < min_chunk_size <= max_chunk_size and max_chunk_size >= align_factor
-        )
-        self._min_chunk_size = min_chunk_size
-        self._max_chunk_size = max_chunk_size
-        self._forced_chunk_size = force_chunk_size
-        self._align_factor = align_factor
-        self._check_hash = check_hash
-        self._thread_pool = thread_pool if thread_pool is not None \
-            else self.DEFAULT_THREAD_POOL_CLASS()
-        super().__init__(**kwargs)
-
-    def _get_hasher(self):
-        if self._check_hash:
-            return hashlib.sha1()
-        return EmptyHasher()
-
-    def _get_chunk_size(self, content_length: int | None):
-        if self._forced_chunk_size is not None:
-            return self._forced_chunk_size
-        ideal = max(content_length // 1000, self._align_factor)
-        non_aligned = min(max(ideal, self._min_chunk_size), self._max_chunk_size)
-        aligned = non_aligned // self._align_factor * self._align_factor
-        return aligned
-
-    @classmethod
-    def _get_remote_range(cls, response: Response, download_version: DownloadVersion):
-        """
-        Get a range from response or original request (as appropriate).
-
-        :param response: requests.Response of initial request
-        :param download_version: b2sdk.v2.DownloadVersion
-        :return: a range object
-        """
-        if 'Range' in response.request.headers:
-            return Range.from_header(response.request.headers['Range'])
-        return download_version.range_
-
-    def is_suitable(self, download_version: DownloadVersion, allow_seeking: bool):
-        """
-        Analyze download_version (possibly against options passed earlier to constructor
-        to find out whether the given download request should be handled by this downloader).
-        """
-        if self.REQUIRES_SEEKING and not allow_seeking:
-            return False
-        return True
+        actual_size = self._get_remote_range(response, download_version).size()
+        chunk_size = self._get_chunk_size(actual_size)
+
+        digest = self._get_hasher()
+        decoded_bytes_read = 0
+        for data in response.iter_content(chunk_size=chunk_size):
+            file.write(data)
+            digest.update(data)
+            decoded_bytes_read += len(data)
+        bytes_read = response.raw.tell()
+
+        assert actual_size >= 1  # code below does `actual_size - 1`, but it should never reach that part with an empty file
+
+        # now, normally bytes_read == download_version.content_length, but sometimes there is a timeout
+        # or something and the server closes connection, while neither tcp or http have a problem
+        # with the truncated output, so we detect it here and try to continue
+
+        num_tries = 5  # this is hardcoded because we are going to replace the entire retry interface soon, so we'll avoid deprecation here and keep it private
+        retries_left = num_tries - 1
+        while retries_left and bytes_read < download_version.content_length:
+            new_range = self._get_remote_range(
+                response,
+                download_version,
+            ).subrange(bytes_read, actual_size - 1)
+            # original response is not closed at this point yet, as another layer is responsible for closing it, so a new socket might be allocated,
+            # but this is a very rare case and so it is not worth the optimization
+            logger.debug(
+                're-download attempts remaining: %i, bytes read: %i (decoded: %i). Getting range %s now.',
+                retries_left, bytes_read, decoded_bytes_read, new_range
+            )
+            with session.download_file_from_url(
+                response.request.url,
+                new_range.as_tuple(),
+                encryption=encryption,
+            ) as followup_response:
+                for data in followup_response.iter_content(
+                    chunk_size=self._get_chunk_size(actual_size)
+                ):
+                    file.write(data)
+                    digest.update(data)
+                    decoded_bytes_read += len(data)
+                bytes_read += followup_response.raw.tell()
+            retries_left -= 1
+        return bytes_read, digest.hexdigest()
 
-    @abstractmethod
     def download(
         self,
         file: IOBase,
         response: Response,
         download_version: DownloadVersion,
         session: B2Session,
         encryption: EncryptionSetting | None = None,
     ):
-        """
-        @returns (bytes_read, actual_sha1)
-        """
-        pass
+        future = self._thread_pool.submit(
+            self._download, file, response, download_version, session, encryption
+        )
+        return future.result()
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 from .abstract import AbstractDownloader
 from .stats_collector import StatsCollector
 
 logger = logging.getLogger(__name__)
 
 
 class ParallelDownloader(AbstractDownloader):
+    """
+    Downloader using threads to download&write multiple parts of an object in parallel.
+
+    Each part is downloaded by its own thread, while all writes are done by additional dedicated thread.
+    This can increase performance even for a small file, as fetching & writing can be done in parallel.
+    """
     # situations to consider:
     #
     # local file start                                         local file end
     # |                                                                     |
     # |                                                                     |
     # |      write range start                        write range end       |
     # |      |                                                      |       |
@@ -46,40 +52,34 @@
     #        |          |          |          |          |          |
     #      #######################################################################
     #      ^                                                                     ^
     #      |                                                                     |
     #      cloud file start                                         cloud file end
     #
     FINISH_HASHING_BUFFER_SIZE = 1024**2
+    SUPPORTS_DECODE_CONTENT = False
 
     def __init__(self, min_part_size: int, max_streams: int | None = None, **kwargs):
         """
         :param max_streams: maximum number of simultaneous streams
         :param min_part_size: minimum amount of data a single stream will retrieve, in bytes
         """
         super().__init__(**kwargs)
         self.max_streams = max_streams
         self.min_part_size = min_part_size
 
-    def is_suitable(self, download_version: DownloadVersion, allow_seeking: bool):
-        if not super().is_suitable(download_version, allow_seeking):
-            return False
-        return self._get_number_of_streams(
-            download_version.content_length
-        ) >= 2 and download_version.content_length >= 2 * self.min_part_size
-
-    def _get_number_of_streams(self, content_length):
+    def _get_number_of_streams(self, content_length: int) -> int:
         num_streams = content_length // self.min_part_size
         if self.max_streams is not None:
             num_streams = min(num_streams, self.max_streams)
         else:
             max_threadpool_workers = getattr(self._thread_pool, '_max_workers', None)
             if max_threadpool_workers is not None:
                 num_streams = min(num_streams, max_threadpool_workers)
-        return num_streams
+        return max(num_streams, 1)
 
     def download(
         self,
         file: IOBase,
         response: Response,
         download_version: DownloadVersion,
         session: B2Session,
```

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_manager.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_source.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/outbound_source.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/outbound_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/progress_reporter.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_manager.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_source.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/transfer/transfer_manager.py` & `b2sdk-2.1.0/b2sdk/_internal/transfer/transfer_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/__init__.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/docs.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/docs.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/escape.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/escape.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/filesystem.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/http_date.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/http_date.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/range_.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/range_.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/thread_pool.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/utils/typing.py` & `b2sdk-2.1.0/b2sdk/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_internal/version_utils.py` & `b2sdk-2.1.0/b2sdk/_internal/version_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,7 +190,17 @@
 
         return wrapper
 
 
 class rename_method(rename_function):
     WHAT = 'method'
     ALTERNATIVE_DECORATOR = 'discourage_method'
+
+
+class FeaturePreviewWarning(FutureWarning):
+    """
+    Feature Preview Warning
+
+    Marks a feature, that is in "Feature Preview" state.
+    Such features are not yet fully stable and are subject to change or even outright removal.
+    Do not rely on them in production code.
+    """
```

### Comparing `b2sdk-2.0.0/b2sdk/_pyinstaller/__init__.py` & `b2sdk-2.1.0/b2sdk/_pyinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/_v3/__init__.py` & `b2sdk-2.1.0/b2sdk/_v3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # core
 
 from b2sdk._internal.api import B2Api
 from b2sdk._internal.api import Services
 from b2sdk._internal.bucket import Bucket
 from b2sdk._internal.bucket import BucketFactory
-from b2sdk._internal.raw_api import ALL_CAPABILITIES, REALM_URLS
+from b2sdk._internal.raw_api import ALL_CAPABILITIES, REALM_URLS, EVENT_TYPE
 
 # encryption
 
 from b2sdk._internal.encryption.setting import EncryptionSetting
 from b2sdk._internal.encryption.setting import EncryptionSettingFactory
 from b2sdk._internal.encryption.setting import EncryptionKey
 from b2sdk._internal.encryption.setting import SSE_NONE, SSE_B2_AES, UNKNOWN_KEY_ID
@@ -55,15 +55,15 @@
 from b2sdk._internal.account_info.stub import StubAccountInfo
 from b2sdk._internal.account_info.upload_url_pool import UploadUrlPool
 from b2sdk._internal.account_info.upload_url_pool import UrlPoolAccountInfo
 
 # version & version utils
 
 from b2sdk.version import VERSION, USER_AGENT
-from b2sdk._internal.version_utils import rename_argument, rename_function
+from b2sdk._internal.version_utils import rename_argument, rename_function, FeaturePreviewWarning
 
 # utils
 
 from b2sdk._internal.utils import (
     b2_url_encode,
     b2_url_decode,
     choose_part_ranges,
@@ -134,14 +134,15 @@
 
 # raw_api
 
 from b2sdk._internal.raw_api import AbstractRawApi
 from b2sdk._internal.raw_api import B2RawHTTPApi
 from b2sdk._internal.raw_api import MetadataDirectiveMode
 from b2sdk._internal.raw_api import LifecycleRule
+from b2sdk._internal.raw_api import NotificationRule, NotificationRuleResponse, notification_rule_response_to_request
 
 # stream
 
 from b2sdk._internal.stream.chained import StreamOpener
 from b2sdk._internal.stream.progress import AbstractStreamWithProgress
 from b2sdk._internal.stream import RangeOfInputStream
 from b2sdk._internal.stream import ReadingStreamWithProgress
```

### Comparing `b2sdk-2.0.0/b2sdk/_v3/exception.py` & `b2sdk-2.1.0/b2sdk/_v3/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/__init__.py` & `b2sdk-2.1.0/b2sdk/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/account_info.py` & `b2sdk-2.1.0/b2sdk/v0/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/api.py` & `b2sdk-2.1.0/b2sdk/v0/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/bucket.py` & `b2sdk-2.1.0/b2sdk/v0/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/exception.py` & `b2sdk-2.1.0/b2sdk/v0/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v0/sync.py` & `b2sdk-2.1.0/b2sdk/v0/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/__init__.py` & `b2sdk-2.1.0/b2sdk/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/account_info.py` & `b2sdk-2.1.0/b2sdk/v1/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/api.py` & `b2sdk-2.1.0/b2sdk/v1/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/b2http.py` & `b2sdk-2.1.0/b2sdk/v1/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/bucket.py` & `b2sdk-2.1.0/b2sdk/v1/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/cache.py` & `b2sdk-2.1.0/b2sdk/v1/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/download_dest.py` & `b2sdk-2.1.0/b2sdk/v1/download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/exception.py` & `b2sdk-2.1.0/b2sdk/v1/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/file_metadata.py` & `b2sdk-2.1.0/b2sdk/v1/file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/file_version.py` & `b2sdk-2.1.0/b2sdk/v1/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/replication/monitoring.py` & `b2sdk-2.1.0/b2sdk/v1/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/session.py` & `b2sdk-2.1.0/b2sdk/v1/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/encryption_provider.py` & `b2sdk-2.1.0/b2sdk/v1/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/file.py` & `b2sdk-2.1.0/b2sdk/v1/sync/file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/file_to_path_translator.py` & `b2sdk-2.1.0/b2sdk/v1/sync/file_to_path_translator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/folder.py` & `b2sdk-2.1.0/b2sdk/v1/sync/folder.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/folder_parser.py` & `b2sdk-2.1.0/b2sdk/v1/sync/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/report.py` & `b2sdk-2.1.0/b2sdk/v1/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/scan_policies.py` & `b2sdk-2.1.0/b2sdk/v1/sync/scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v1/sync/sync.py` & `b2sdk-2.1.0/b2sdk/v1/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/__init__.py` & `b2sdk-2.1.0/b2sdk/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/api.py` & `b2sdk-2.1.0/b2sdk/v2/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/b2http.py` & `b2sdk-2.1.0/b2sdk/v2/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/bucket.py` & `b2sdk-2.1.0/b2sdk/v2/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/exception.py` & `b2sdk-2.1.0/b2sdk/v2/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/file_version.py` & `b2sdk-2.1.0/b2sdk/v2/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/large_file.py` & `b2sdk-2.1.0/b2sdk/v2/large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/raw_api.py` & `b2sdk-2.1.0/b2sdk/v2/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/raw_simulator.py` & `b2sdk-2.1.0/b2sdk/v2/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/session.py` & `b2sdk-2.1.0/b2sdk/v2/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/transfer.py` & `b2sdk-2.1.0/b2sdk/v2/transfer.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/utils.py` & `b2sdk-2.1.0/b2sdk/v2/utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/v2/version_utils.py` & `b2sdk-2.1.0/b2sdk/v2/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/b2sdk/version.py` & `b2sdk-2.1.0/b2sdk/version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.0.0/pyproject.toml` & `b2sdk-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "2.0.0"
+version = "2.1.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Backblaze/b2-sdk-python"
 
@@ -181,14 +181,16 @@
     "ruff==0.1.15",
     "pytest==6.2.5",
     "liccheck==0.9.2",
     "setuptools",
 ]
 test = [
     "coverage==7.2.7",
+    "eval_type_backport>=0.1.3,<1; python_version<'3.10'",
+    "pydantic>=2.0.1,<3; python_version>='3.8' and platform_python_implementation!='PyPy'",
     "pytest==6.2.5",
     "pytest-cov==3.0.0",
     "pytest-mock==3.6.1",
     "pytest-lazy-fixture==0.6.3",
     "pytest-xdist==2.5.0",
     "pytest-timeout==2.1.0",
     "tqdm<5.0.0,>=4.5.0",
```

### Comparing `b2sdk-2.0.0/PKG-INFO` & `b2sdk-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: Backblaze B2 SDK
-Keywords: backblaze b2 cloud storage
+Keywords: backblaze,b2,cloud,storage
 Author-Email: Backblaze Inc <support@backblaze.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

