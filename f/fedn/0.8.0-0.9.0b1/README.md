# Comparing `tmp/fedn-0.8.0.tar.gz` & `tmp/fedn-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedn-0.8.0.tar", last modified: Fri Feb  9 14:41:26 2024, max compression
+gzip compressed data, was "fedn-0.9.0b1.tar", last modified: Mon Apr 15 08:31:46 2024, max compression
```

## Comparing `fedn-0.8.0.tar` & `fedn-0.9.0b1.tar`

### file list

```diff
@@ -1,111 +1,138 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      495 2024-02-09 14:41:26.395066 fedn-0.8.0/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-01-29 16:01:38.000000 fedn-0.8.0/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.391066 fedn-0.8.0/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       80 2024-01-29 16:01:38.000000 fedn-0.8.0/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-01-29 16:01:38.000000 fedn-0.8.0/cli/main.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6956 2024-02-09 14:41:02.000000 fedn-0.8.0/cli/run_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.391066 fedn-0.8.0/cli/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/cli/tests/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2024-01-29 16:01:38.000000 fedn-0.8.0/cli/tests/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.391066 fedn-0.8.0/fedn/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3085 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2755 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1522 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/common/net/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11354 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    37997 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5070 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13868 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    28680 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4332 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6058 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      633 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5323 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/aggregators/aggregator.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6518 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4128 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5899 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/aggregators/fedopt.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    26146 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4433 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10314 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7239 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15160 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14293 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11278 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10858 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2186 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      591 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1343 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      421 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1153 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1634 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3209 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3983 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3943 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    30442 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/tests/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      329 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1435 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/utils/dispatcher.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1132 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3328 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4640 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/helpers/plugins/numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15762 2024-02-09 14:41:02.000000 fedn-0.8.0/fedn/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      801 2024-01-29 16:01:38.000000 fedn-0.8.0/fedn/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:26.395066 fedn-0.8.0/fedn.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      495 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2747 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       35 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/entry_points.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-01-29 16:02:31.000000 fedn-0.8.0/fedn.egg-info/not-zip-safe
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      258 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2024-02-09 14:41:26.000000 fedn-0.8.0/fedn.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-02-09 14:41:26.395066 fedn-0.8.0/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1290 2024-02-09 14:41:02.000000 fedn-0.8.0/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 08:31:46.397624 fedn-0.9.0b1/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-01-29 16:01:38.000000 fedn-0.9.0b1/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/cli/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       80 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/main.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     8980 2024-04-15 08:28:35.000000 fedn-0.9.0b1/cli/run_cmd.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/cli/tests/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/tests/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/tests/tests.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/certificate/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/certificate/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3140 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/certificate/certificate.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/certificate/certificatemanager.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3499 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/config.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/exceptions.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3421 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/log_config.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/net/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/net/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/api/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/api/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2338 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/auth.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    24093 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/client.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    38027 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/interface.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5115 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/network.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    20111 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/server.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/api/tests.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/api/v1/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    11190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/client_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10343 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/combiner_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    18235 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/model_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13598 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/package_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9335 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/round_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9284 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/session_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/shared.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    12614 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/status_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13391 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/validation_routes.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/clients/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    32914 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/client.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5827 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/connect.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5967 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/package.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      633 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/state.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/test_client.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/combiner/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/combiner/aggregators/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5323 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregator.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6744 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregatorbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4353 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/fedavg.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5905 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/fedopt.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    26190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/combiner.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/combiner_tests.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4694 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/connect.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10314 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/interfaces.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     7239 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/modelservice.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14861 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/roundhandler.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/config.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/controller/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/controller/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14347 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/controller/control.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    11363 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/controller/controlbase.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/grpc/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/grpc/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3564 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/auth.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/fedn_pb2.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/fedn_pb2_grpc.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/server.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/loadbalancer/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      591 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/firstavailable.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1343 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/leastpacked.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      421 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/loadbalancerbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1153 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/state.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/models/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/memorymodelstorage.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1634 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/modelstorage.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3220 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/models/tempmodelstorage.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/s3/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/s3/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/s3/base.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3897 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/s3/miniorepository.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3943 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/s3/repository.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/statestore/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/statestore/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    30398 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/mongostatestore.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/statestore/statestorebase.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/network/storage/statestore/stores/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/client_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/combiner_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/model_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/package_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/round_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/session_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/shared.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/status_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/validation_store.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/utils/checksum.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9331 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/dispatcher.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4067 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/environment.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/flowercompat/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/flowercompat/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4767 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/flowercompat/client_app_adapter.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/helpers/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/helperbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1132 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/helpers.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/helpers/plugins/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3377 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/androidhelper.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4640 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/numpyhelper.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    15799 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/plots.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6033 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/process.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3841 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       35 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/entry_points.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-01-29 16:02:31.000000 fedn-0.9.0b1/fedn.egg-info/not-zip-safe
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      235 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/top_level.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-04-15 08:31:46.397624 fedn-0.9.0b1/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1294 2024-04-15 08:31:26.000000 fedn-0.9.0b1/setup.py
```

### Comparing `fedn-0.8.0/cli/run_cmd.py` & `fedn-0.9.0b1/cli/run_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import os
+import shutil
+import tarfile
 import uuid
 
 import click
 import yaml
 
 from fedn.common.exceptions import InvalidClientConfig
 from fedn.common.log_config import logger
 from fedn.network.clients.client import Client
 from fedn.network.combiner.combiner import Combiner
+from fedn.utils.dispatcher import Dispatcher, _read_yaml_file
 
 from .main import main
 
 
 def get_statestore_config_from_file(init):
     """
 
@@ -175,7 +179,72 @@
               'init': init}
 
     if config['init']:
         apply_config(config)
 
     combiner = Combiner(config)
     combiner.run()
+
+
+@run_cmd.command('build')
+@click.option('-p', '--path', required=True, help='Path to package directory containing fedn.yaml')
+@click.pass_context
+def build_cmd(ctx, path):
+    """ Execute 'build' entrypoint in fedn.yaml.
+
+    :param ctx:
+    :param path: Path to folder containing fedn.yaml
+    :type path: str
+    """
+    path = os.path.abspath(path)
+    yaml_file = os.path.join(path, 'fedn.yaml')
+    if not os.path.exists(yaml_file):
+        logger.error(f"Could not find fedn.yaml in {path}")
+        exit(-1)
+
+    config = _read_yaml_file(yaml_file)
+    # Check that build is defined in fedn.yaml under entry_points
+    if 'build' not in config['entry_points']:
+        logger.error("No build command defined in fedn.yaml")
+        exit(-1)
+
+    dispatcher = Dispatcher(config, path)
+    _ = dispatcher._get_or_create_python_env()
+    dispatcher.run_cmd("build")
+
+    # delete the virtualenv
+    if dispatcher.python_env_path:
+        logger.info(f"Removing virtualenv {dispatcher.python_env_path}")
+        shutil.rmtree(dispatcher.python_env_path)
+
+
+@main.group('package')
+@click.pass_context
+def package_cmd(ctx):
+    """
+
+    :param ctx:
+    """
+    pass
+
+
+@package_cmd.command('create')
+@click.option('-p', '--path', required=True, help='Path to package directory containing fedn.yaml')
+@click.option('-n', '--name', required=False, default='package.tgz', help='Name of package tarball')
+@click.pass_context
+def create_cmd(ctx, path, name):
+    """ Create compute package.
+
+    Make a tar.gz archive of folder given by --path
+
+    :param ctx:
+    :param path:
+    """
+    path = os.path.abspath(path)
+    yaml_file = os.path.join(path, 'fedn.yaml')
+    if not os.path.exists(yaml_file):
+        logger.error(f"Could not find fedn.yaml in {path}")
+        exit(-1)
+
+    with tarfile.open(name, "w:gz") as tar:
+        tar.add(path, arcname=os.path.basename(path))
+        logger.info(f"Created package {name}")
```

### Comparing `fedn-0.8.0/cli/tests/tests.py` & `fedn-0.9.0b1/cli/tests/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/common/certificate/certificate.py` & `fedn-0.9.0b1/fedn/common/certificate/certificate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import os
 import random
 import uuid
 
 from OpenSSL import crypto
 
+from fedn.common.log_config import logger
+
 
 class Certificate:
     """
     Utility to generate unsigned certificates.
 
     """
     CERT_NAME = "cert.pem"
@@ -16,17 +18,17 @@
     BITS = 2048
 
     def __init__(self, cwd, name=None, key_name="key.pem", cert_name="cert.pem", create_dirs=True):
 
         try:
             os.makedirs(cwd)
         except OSError:
-            print("Directory exists, will store all cert and keys here.")
+            logger.info("Directory exists, will store all cert and keys here.")
         else:
-            print(
+            logger.info(
                 "Successfully created the directory to store cert and keys in {}".format(cwd))
 
         self.key_path = os.path.join(cwd, key_name)
         self.cert_path = os.path.join(cwd, cert_name)
 
         if name:
             self.name = name
```

### Comparing `fedn-0.8.0/fedn/common/certificate/certificatemanager.py` & `fedn-0.9.0b1/fedn/common/certificate/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/api/client.py` & `fedn-0.9.0b1/fedn/network/combiner/interfaces.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,322 +1,326 @@
+import base64
+import copy
 import json
+import time
+from io import BytesIO
 
-import requests
+import grpc
 
-__all__ = ['APIClient']
+import fedn.network.grpc.fedn_pb2 as fedn
+import fedn.network.grpc.fedn_pb2_grpc as rpc
 
 
-class APIClient:
-    """ An API client for interacting with the statestore and controller.
+class CombinerUnavailableError(Exception):
+    pass
 
-    :param host: The host of the api server.
-    :type host: str
-    :param port: The port of the api server.
+
+class Channel:
+    """ Wrapper for a gRPC channel.
+
+    :param address: The address for the gRPC server.
+    :type address: str
+    :param port: The port for connecting to the gRPC server.
     :type port: int
-    :param secure: Whether to use https.
-    :type secure: bool
-    :param verify: Whether to verify the server certificate.
-    :type verify: bool
+    :param certificate: The certificate for connecting to the gRPC server (optional)
+    :type certificate: str
     """
 
-    def __init__(self, host, port, secure=False, verify=False):
-        self.host = host
-        self.port = port
-        self.secure = secure
-        self.verify = verify
-
-    def _get_url(self, endpoint):
-        if self.secure:
-            protocol = 'https'
-        else:
-            protocol = 'http'
-        return f'{protocol}://{self.host}:{self.port}/{endpoint}'
+    def __init__(self, address, port, certificate=None):
+        """ Create a channel.
 
-    def get_model_trail(self):
-        """ Get the model trail.
+        If a valid certificate is given, a secure channel is created, else insecure.
 
-        :return: The model trail as dict including commit timestamp.
-        :rtype: dict
+        :parameter address: The address for the gRPC server.
+        :type address: str
+        :parameter port: The port for connecting to the gRPC server.
+        :type port: int
+        :parameter certificate: The certificate for connecting to the gRPC server (optional)
+        :type certificate: str
         """
-        response = requests.get(self._get_url('get_model_trail'), verify=self.verify)
-        return response.json()
-
-    def list_models(self, session_id=None):
-        """ Get all models from the statestore.
+        self.address = address
+        self.port = port
+        self.certificate = certificate
 
-        :return: All models.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('list_models'), params={'session_id': session_id}, verify=self.verify)
-        return response.json()
+        if self.certificate:
+            credentials = grpc.ssl_channel_credentials(
+                root_certificates=copy.deepcopy(certificate))
+            self.channel = grpc.secure_channel('{}:{}'.format(
+                self.address, str(self.port)), credentials)
+        else:
+            self.channel = grpc.insecure_channel(
+                '{}:{}'.format(self.address, str(self.port)))
 
-    def list_clients(self):
-        """ Get all clients from the statestore.
+    def get_channel(self):
+        """ Get a channel.
 
-        return: All clients.
-        rtype: dict
+        :return: An instance of a gRPC channel
+        :rtype: :class:`grpc.Channel`
         """
-        response = requests.get(self._get_url('list_clients'))
-        return response.json()
+        return copy.copy(self.channel)
+
+
+class CombinerInterface:
+    """ Interface for the Combiner (aggregation server).
+        Abstraction on top of the gRPC server servicer.
+
+    :param parent: The parent combiner (controller)
+    :type parent: :class:`fedn.network.api.interfaces.API`
+    :param name: The name of the combiner.
+    :type name: str
+    :param address: The address of the combiner.
+    :type address: str
+    :param fqdn: The fully qualified domain name of the combiner.
+    :type fqdn: str
+    :param port: The port of the combiner.
+    :type port: int
+    :param certificate: The certificate of the combiner (optional).
+    :type certificate: str
+    :param key: The key of the combiner (optional).
+    :type key: str
+    :param ip: The ip of the combiner (optional).
+    :type ip: str
+    :param config: The configuration of the combiner (optional).
+    :type config: dict
+    """
 
-    def get_active_clients(self, combiner_id):
-        """ Get all active clients from the statestore.
+    def __init__(self, parent, name, address, fqdn, port, certificate=None, key=None, ip=None, config=None):
+        """ Initialize the combiner interface."""
+        self.parent = parent
+        self.name = name
+        self.address = address
+        self.fqdn = fqdn
+        self.port = port
+        self.certificate = certificate
+        self.key = key
+        self.ip = ip
+
+        if not config:
+            self.config = {
+                'max_clients': 8
+            }
+        else:
+            self.config = config
 
-        :param combiner_id: The combiner id to get active clients for.
-        :type combiner_id: str
-        :return: All active clients.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_active_clients'), params={'combiner': combiner_id}, verify=self.verify)
-        return response.json()
+    @classmethod
+    def from_json(combiner_config):
+        """ Initialize the combiner config from a json document.
 
-    def get_client_config(self, checksum=True):
-        """ Get the controller configuration. Optionally include the checksum.
-        The config is used for clients to connect to the controller and ask for combiner assignment.
-
-        :param checksum: Whether to include the checksum of the package.
-        :type checksum: bool
-        :return: The client configuration.
-        :rtype: dict
+        :parameter combiner_config: The combiner configuration.
+        :type combiner_config: dict
+        :return: An instance of the combiner interface.
+        :rtype: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         """
-        response = requests.get(self._get_url('get_client_config'), params={'checksum': checksum}, verify=self.verify)
-        return response.json()
+        return CombinerInterface(**combiner_config)
 
-    def list_combiners(self):
-        """ Get all combiners in the network.
+    def to_dict(self):
+        """ Export combiner configuration to a dictionary.
 
-        :return: All combiners with info.
+        :return: A dictionary with the combiner configuration.
         :rtype: dict
         """
-        response = requests.get(self._get_url('list_combiners'))
-        return response.json()
 
-    def get_combiner(self, combiner_id):
-        """ Get a combiner from the statestore.
+        data = {
+            'parent': self.parent,
+            'name': self.name,
+            'address': self.address,
+            'fqdn': self.fqdn,
+            'port': self.port,
+            'ip': self.ip,
+            'certificate': None,
+            'key': None,
+            'config': self.config
+        }
 
-        :param combiner_id: The combiner id to get.
-        :type combiner_id: str
-        :return: The combiner info.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url(f'get_combiner?combiner={combiner_id}'), verify=self.verify)
-        return response.json()
+        if self.certificate:
+            cert_b64 = base64.b64encode(self.certificate)
+            key_b64 = base64.b64encode(self.key)
+            data['certificate'] = str(cert_b64).split('\'')[1]
+            data['key'] = str(key_b64).split('\'')[1]
 
-    def list_rounds(self):
-        """ Get all rounds from the statestore.
+        return data
 
-        :return: All rounds with config and metrics.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('list_rounds'))
-        return response.json()
+    def to_json(self):
+        """ Export combiner configuration to json.
 
-    def get_round(self, round_id):
-        """ Get a round from the statestore.
-
-        :param round_id: The round id to get.
-        :type round_id: str
-        :return: The round config and metrics.
-        :rtype: dict
+        :return: A json document with the combiner configuration.
+        :rtype: str
         """
-        response = requests.get(self._get_url(f'get_round?round_id={round_id}'), verify=self.verify)
-        return response.json()
+        return json.dumps(self.to_dict())
 
-    def start_session(self, session_id=None, aggregator='fedavg', model_id=None, round_timeout=180, rounds=5, round_buffer_size=-1, delete_models=True,
-                      validate=True, helper='numpyhelper', min_clients=1, requested_clients=8):
-        """ Start a new session.
-
-        :param session_id: The session id to start.
-        :type session_id: str
-        :param aggregator: The aggregator plugin to use.
-        :type aggregator: str
-        :param model_id: The id of the initial model.
-        :type model_id: str
-        :param round_timeout: The round timeout to use in seconds.
-        :type round_timeout: int
-        :param rounds: The number of rounds to perform.
-        :type rounds: int
-        :param round_buffer_size: The round buffer size to use.
-        :type round_buffer_size: int
-        :param delete_models: Whether to delete models after each round at combiner (save storage).
-        :type delete_models: bool
-        :param validate: Whether to validate the model after each round.
-        :type validate: bool
-        :param helper: The helper type to use.
-        :type helper: str
-        :param min_clients: The minimum number of clients required.
-        :type min_clients: int
-        :param requested_clients: The requested number of clients.
-        :type requested_clients: int
-        :return: A dict with success or failure message and session config.
-        :rtype: dict
+    def get_certificate(self):
+        """ Get combiner certificate.
+
+        :return: The combiner certificate.
+        :rtype: str, None if no certificate is set.
         """
-        response = requests.post(self._get_url('start_session'), json={
-            'session_id': session_id,
-            'aggregator': aggregator,
-            'model_id': model_id,
-            'round_timeout': round_timeout,
-            'rounds': rounds,
-            'round_buffer_size': round_buffer_size,
-            'delete_models': delete_models,
-            'validate': validate,
-            'helper': helper,
-            'min_clients': min_clients,
-            'requested_clients': requested_clients
-        }, verify=self.verify
-        )
-        return response.json()
+        if self.certificate:
+            cert_b64 = base64.b64encode(self.certificate)
+            return str(cert_b64).split('\'')[1]
+        else:
+            return None
 
-    def list_sessions(self):
-        """ Get all sessions from the statestore.
+    def get_key(self):
+        """ Get combiner key.
 
-        :return: All sessions in dict.
-        :rtype: dict
+        :return: The combiner key.
+        :rtype: str, None if no key is set.
         """
-        response = requests.get(self._get_url('list_sessions'), verify=self.verify)
-        return response.json()
+        if self.key:
+            key_b64 = base64.b64encode(self.key)
+            return str(key_b64).split('\'')[1]
+        else:
+            return None
 
-    def get_session(self, session_id):
-        """ Get a session from the statestore.
+    def flush_model_update_queue(self):
+        """ Reset the model update queue on the combiner. """
 
-        :param session_id: The session id to get.
-        :type session_id: str
-        :return: The session as a json object.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url(f'get_session?session_id={session_id}'), self.verify)
-        return response.json()
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        control = rpc.ControlStub(channel)
 
-    def session_is_finished(self, session_id):
-        """ Check if a session with id session_id has finished.
+        request = fedn.ControlRequest()
 
-        :param session_id: The session id to get.
-        :type session_id: str
-        :return: The session as a json object.
-        :rtype: dict
-        """
         try:
-            status = self.get_session(session_id)['status']
-            if status == 'Finished':
-                return True
+            control.FlushAggregationQueue(request)
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.UNAVAILABLE:
+                raise CombinerUnavailableError
             else:
-                return False
-        except json.JSONDecodeError:
-            # Could happen if the session has not been written to db yet
-            return False
-        except Exception:
-            raise
+                raise
 
-    def set_package(self, path: str, helper: str, name: str = None, description: str = None):
-        """ Set the compute package in the statestore.
+    def set_aggregator(self, aggregator):
+        """ Set the active aggregator module.
 
-        :param path: The file path of the compute package to set.
-        :type path: str
-        :param helper: The helper type to use.
-        :type helper: str
-        :return: A dict with success or failure message.
-        :rtype: dict
+        :param aggregator: The name of the aggregator module.
+        :type config: str
         """
-        with open(path, 'rb') as file:
-            response = requests.post(self._get_url('set_package'), files={'file': file}, data={
-                                     'helper': helper, 'name': name, 'description': description}, verify=self.verify)
-        return response.json()
 
-    def get_package(self):
-        """ Get the compute package from the statestore.
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        control = rpc.ControlStub(channel)
 
-        :return: The compute package with info.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_package'), verify=self.verify)
-        return response.json()
+        request = fedn.ControlRequest()
+        p = request.parameter.add()
+        p.key = "aggregator"
+        p.value = aggregator
 
-    def list_compute_packages(self):
-        """ Get all compute packages from the statestore.
-
-        :return: All compute packages with info.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('list_compute_packages'), verify=self.verify)
-        return response.json()
-
-    def download_package(self, path):
-        """ Download the compute package.
-
-        :param path: The path to download the compute package to.
-        :type path: str
-        :return: Message with success or failure.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('download_package'), verify=self.verify)
-        if response.status_code == 200:
-            with open(path, 'wb') as file:
-                file.write(response.content)
-            return {'success': True, 'message': 'Package downloaded successfully.'}
-        else:
-            return {'success': False, 'message': 'Failed to download package.'}
-
-    def get_package_checksum(self):
-        """ Get the checksum of the compute package.
-
-        :return: The checksum.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_package_checksum'), verify=self.verify)
-        return response.json()
-
-    def get_latest_model(self):
-        """ Get the latest model from the statestore.
-
-        :return: The latest model id.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_latest_model'), verify=self.verify)
-        return response.json()
+        try:
+            control.SetAggregator(request)
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.UNAVAILABLE:
+                raise CombinerUnavailableError
+            else:
+                raise
 
-    def get_initial_model(self):
-        """ Get the initial model from the statestore.
+    def submit(self, config):
+        """ Submit a compute plan to the combiner.
 
-        :return: The initial model id.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_initial_model'), verify=self.verify)
-        return response.json()
+        :param config: The job configuration.
+        :type config: dict
+        :return: Server ControlResponse object.
+        :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
+        """
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        control = rpc.ControlStub(channel)
+        request = fedn.ControlRequest()
+        request.command = fedn.Command.START
+        for k, v in config.items():
+            p = request.parameter.add()
+            p.key = str(k)
+            p.value = str(v)
 
-    def set_initial_model(self, path):
-        """ Set the initial model in the statestore and upload to model repository.
+        try:
+            response = control.Start(request)
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.UNAVAILABLE:
+                raise CombinerUnavailableError
+            else:
+                raise
 
-        :param path: The file path of the initial model to set.
-        :type path: str
-        :return: A dict with success or failure message.
-        :rtype: dict
-        """
-        with open(path, 'rb') as file:
-            response = requests.post(self._get_url('set_initial_model'), files={'file': file}, verify=self.verify)
-        return response.json()
+        return response
 
-    def get_controller_status(self):
-        """ Get the status of the controller.
+    def get_model(self, id, timeout=10):
+        """ Download a model from the combiner server.
 
-        :return: The status of the controller.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_controller_status'), verify=self.verify)
-        return response.json()
+        :param id: The model id.
+        :type id: str
+        :return: A file-like object containing the model.
+        :rtype: :class:`io.BytesIO`, None if the model is not available.
+        """
+
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        modelservice = rpc.ModelServiceStub(channel)
+
+        data = BytesIO()
+        data.seek(0, 0)
+
+        time_start = time.time()
+
+        request = fedn.ModelRequest(id=id)
+        request.sender.name = self.name
+        request.sender.role = fedn.WORKER
+
+        parts = modelservice.Download(request)
+        for part in parts:
+            if part.status == fedn.ModelStatus.IN_PROGRESS:
+                data.write(part.data)
+            if part.status == fedn.ModelStatus.OK:
+                return data
+            if part.status == fedn.ModelStatus.FAILED:
+                return None
+            if part.status == fedn.ModelStatus.UNKNOWN:
+                if time.time() - time_start > timeout:
+                    return None
+                continue
+
+    def allowing_clients(self):
+        """ Check if the combiner is allowing additional client connections.
+
+        :return: True if accepting, else False.
+        :rtype: bool
+        """
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        connector = rpc.ConnectorStub(channel)
+        request = fedn.ConnectionRequest()
 
-    def get_events(self, **kwargs):
-        """ Get the events from the statestore. Pass kwargs to filter events.
+        try:
+            response = connector.AcceptingClients(request)
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.UNAVAILABLE:
+                raise CombinerUnavailableError
+            else:
+                raise
+        if response.status == fedn.ConnectionStatus.NOT_ACCEPTING:
+            return False
+        if response.status == fedn.ConnectionStatus.ACCEPTING:
+            return True
+        if response.status == fedn.ConnectionStatus.TRY_AGAIN_LATER:
+            return False
 
-        :return: The events in dict
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('get_events'), params=kwargs, verify=self.verify)
-        return response.json()
+        return False
 
-    def list_validations(self, **kwargs):
-        """ Get all validations from the statestore. Pass kwargs to filter validations.
+    def list_active_clients(self, queue=1):
+        """ List active clients.
 
-        :return: All validations in dict.
-        :rtype: dict
-        """
-        response = requests.get(self._get_url('list_validations'), params=kwargs, verify=self.verify)
-        return response.json()
+        :param queue: The channel (queue) to use (optional). Default is 1 = MODEL_UPDATE_REQUESTS channel.
+            see :class:`fedn.network.grpc.fedn_pb2.Channel`
+        :type channel: int
+        :return: A list of active clients.
+        :rtype: json
+        """
+        channel = Channel(self.address, self.port,
+                          self.certificate).get_channel()
+        control = rpc.ConnectorStub(channel)
+        request = fedn.ListClientsRequest()
+        request.channel = queue
+        try:
+            response = control.ListActiveClients(request)
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.UNAVAILABLE:
+                raise CombinerUnavailableError
+            else:
+                raise
+        return response.client
```

### Comparing `fedn-0.8.0/fedn/network/api/interface.py` & `fedn-0.9.0b1/fedn/network/api/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import uuid
 from io import BytesIO
 
 from flask import jsonify, send_from_directory
 from werkzeug.utils import secure_filename
 
 from fedn.common.config import get_controller_config, get_network_config
+from fedn.common.log_config import logger
 from fedn.network.combiner.interfaces import (CombinerInterface,
                                               CombinerUnavailableError)
 from fedn.network.state import ReducerState, ReducerStateToString
 from fedn.utils.checksum import sha
 from fedn.utils.plots import Plot
 
 __all__ = ("API",)
@@ -270,15 +271,15 @@
             message = "No compute package found."
             return None, message
         else:
             try:
                 name = package_objects["storage_file_name"]
             except KeyError as e:
                 message = "No compute package found. Key error."
-                print(e)
+                logger.debug(e)
                 return None, message
             return name, "success"
 
     def get_compute_package(self):
         """Get the compute package from the statestore.
 
         :return: The compute package as a json response.
@@ -651,15 +652,15 @@
             "fqdn": combiner.fqdn,
             "package": "remote",  # TODO: Make this configurable
             "ip": combiner.ip,
             "port": combiner.port,
             "certificate": cert,
             "helper_type": self.control.statestore.get_helper(),
         }
-        print("Seding payload: ", payload, flush=True)
+        logger.info(f"Sending payload: {payload}")
 
         return jsonify(payload)
 
     def get_initial_model(self):
         """Get the initial model from the statestore.
 
         :return: The initial model as a json response.
@@ -683,15 +684,15 @@
             file.seek(0)
             object.write(file.read())
             helper = self.control.get_helper()
             object.seek(0)
             model = helper.load(object)
             self.control.commit(file.filename, model)
         except Exception as e:
-            print(e, flush=True)
+            logger.debug(e)
             return jsonify({"success": False, "message": e})
 
         return jsonify(
             {"success": True, "message": "Initial model added successfully."}
         )
 
     def get_latest_model(self):
@@ -963,15 +964,15 @@
         try:
             valid_metrics = plot.fetch_valid_metrics()
             feature = feature or valid_metrics[0]
             box_plot = plot.create_box_plot(feature)
         except Exception as e:
             valid_metrics = None
             box_plot = None
-            print(e, flush=True)
+            logger.debug(e)
 
         result = {
             "valid_metrics": valid_metrics,
             "box_plot": box_plot,
         }
 
         return jsonify(result)
@@ -1077,15 +1078,15 @@
         clients_available = 0
         for combiner in self.control.network.get_combiners():
             try:
                 nr_active_clients = len(combiner.list_active_clients())
                 clients_available = clients_available + int(nr_active_clients)
             except CombinerUnavailableError as e:
                 # TODO: Handle unavailable combiner, stop session or continue?
-                print("COMBINER UNAVAILABLE: {}".format(e), flush=True)
+                logger.error("COMBINER UNAVAILABLE: {}".format(e))
                 continue
 
         if clients_available < min_clients:
             return jsonify(
                 {
                     "success": False,
                     "message": "Not enough clients available to start session.",
```

### Comparing `fedn-0.8.0/fedn/network/api/network.py` & `fedn-0.9.0b1/fedn/network/api/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 
+from fedn.common.log_config import logger
 from fedn.network.combiner.interfaces import CombinerInterface
 from fedn.network.loadbalancer.leastpacked import LeastPacked
 
 __all__ = 'Network',
 
 
 class Network:
@@ -63,32 +64,32 @@
         """ Add a new combiner to the network.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         if not self.control.idle():
-            print("Reducer is not idle, cannot add additional combiner.")
+            logger.warning("Reducer is not idle, cannot add additional combiner.")
             return
 
         if self.get_combiner(combiner.name):
             return
 
-        print("adding combiner {}".format(combiner.name), flush=True)
+        logger.info("adding combiner {}".format(combiner.name))
         self.statestore.set_combiner(combiner.to_dict())
 
     def remove_combiner(self, combiner):
         """ Remove a combiner from the network.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         if not self.control.idle():
-            print("Reducer is not idle, cannot remove combiner.")
+            logger.warning("Reducer is not idle, cannot remove combiner.")
             return
         self.statestore.delete_combiner(combiner.name)
 
     def find_available_combiner(self):
         """ Find an available combiner in the network.
 
         :return: The combiner instance object
@@ -101,29 +102,29 @@
         """ This callback is triggered if a combiner is found to be unresponsive.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         # TODO: Implement strategy to handle an unavailable combiner.
-        print("REDUCER CONTROL: Combiner {} unavailable.".format(
-            combiner.name), flush=True)
+        logger.warning("REDUCER CONTROL: Combiner {} unavailable.".format(
+            combiner.name))
 
     def add_client(self, client):
         """ Add a new client to the network.
 
         :param client: The client instance object
         :type client: dict
         :return: None
         """
 
         if self.get_client(client['name']):
             return
 
-        print("adding client {}".format(client['name']), flush=True)
+        logger.info("adding client {}".format(client['name']))
         self.statestore.set_client(client)
 
     def get_client(self, name):
         """ Get client by name.
 
         :param name: name of client
         :type name: str
```

### Comparing `fedn-0.8.0/fedn/network/api/tests.py` & `fedn-0.9.0b1/fedn/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/clients/client.py` & `fedn-0.9.0b1/fedn/network/clients/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 import io
 import json
 import os
 import queue
 import re
 import socket
 import sys
-import tempfile
 import threading
 import time
 import uuid
 from datetime import datetime
 from distutils.dir_util import copy_tree
 from io import BytesIO
 
 import grpc
 from cryptography.hazmat.primitives.serialization import Encoding
 from google.protobuf.json_format import MessageToJson
 from OpenSSL import SSL
+from tenacity import retry, stop_after_attempt
 
 import fedn.network.grpc.fedn_pb2 as fedn
 import fedn.network.grpc.fedn_pb2_grpc as rpc
+from fedn.common.config import FEDN_AUTH_SCHEME, FEDN_PACKAGE_EXTRACT_DIR
 from fedn.common.log_config import (logger, set_log_level_from_string,
                                     set_log_stream)
 from fedn.network.clients.connect import ConnectorClient, Status
 from fedn.network.clients.package import PackageRuntime
 from fedn.network.clients.state import ClientState, ClientStateToString
-from fedn.network.combiner.modelservice import upload_request_generator
+from fedn.network.combiner.modelservice import (get_tmp_path,
+                                                upload_request_generator)
 from fedn.utils.dispatcher import Dispatcher
 from fedn.utils.helpers.helpers import get_helper
 
 CHUNK_SIZE = 1024 * 1024
 VALID_NAME_REGEX = '^[a-zA-Z0-9_-]*$'
 
 
 class GrpcAuth(grpc.AuthMetadataPlugin):
     def __init__(self, key):
         self._key = key
 
     def __call__(self, context, callback):
-        callback((('authorization', f'Token {self._key}'),), None)
+        callback((('authorization', f'{FEDN_AUTH_SCHEME} {self._key}'),), None)
 
 
 class Client:
     """FEDn Client. Service running on client/datanodes in a federation,
     recieving and handling model update and model validation requests.
 
     :param config: A configuration dictionary containing connection information for the discovery service (controller)
@@ -51,18 +53,18 @@
     :type config: dict
     """
 
     def __init__(self, config):
         """Initialize the client."""
         self.state = None
         self.error_state = False
-        self._attached = False
+        self._connected = False
         self._missed_heartbeat = 0
         self.config = config
-
+        self.trace_attribs = False
         set_log_level_from_string(config.get('verbosity', "INFO"))
         set_log_stream(config.get('logfile', None))
 
         self.connector = ConnectorClient(host=config['discover_host'],
                                          port=config['discover_port'],
                                          token=config['token'],
                                          name=config['name'],
@@ -73,66 +75,72 @@
                                          id=config['client_id'])
 
         # Validate client name
         match = re.search(VALID_NAME_REGEX, config['name'])
         if not match:
             raise ValueError('Unallowed character in client name. Allowed characters: a-z, A-Z, 0-9, _, -.')
 
+        # Folder where the client will store downloaded compute package and logs
         self.name = config['name']
-        dirname = time.strftime("%Y%m%d-%H%M%S")
-        self.run_path = os.path.join(os.getcwd(), dirname)
-        os.mkdir(self.run_path)
+        if FEDN_PACKAGE_EXTRACT_DIR:
+            self.run_path = os.path.join(os.getcwd(), FEDN_PACKAGE_EXTRACT_DIR)
+        else:
+            dirname = self.name+"-"+time.strftime("%Y%m%d-%H%M%S")
+            self.run_path = os.path.join(os.getcwd(), dirname)
+        if not os.path.exists(self.run_path):
+            os.mkdir(self.run_path)
 
         self.started_at = datetime.now()
         self.logs = []
 
         self.inbox = queue.Queue()
 
         # Attach to the FEDn network (get combiner)
-        client_config = self._attach()
+        combiner_config = self.assign()
+        self.connect(combiner_config)
 
         self._initialize_dispatcher(config)
 
-        self._initialize_helper(client_config)
+        self._initialize_helper(combiner_config)
         if not self.helper:
             logger.warning("Failed to retrieve helper class settings: {}".format(
-                client_config))
+                combiner_config))
 
         self._subscribe_to_combiner(config)
 
         self.state = ClientState.idle
 
-    def _assign(self):
+    def assign(self):
         """Contacts the controller and asks for combiner assignment.
 
         :return: A configuration dictionary containing connection information for combiner.
         :rtype: dict
         """
 
         logger.info("Initiating assignment request.")
         while True:
             status, response = self.connector.assign()
             if status == Status.TryAgain:
-                logger.info(response)
+                logger.warning(response)
+                logger.info("Assignment request failed. Retrying in 5 seconds.")
                 time.sleep(5)
                 continue
             if status == Status.Assigned:
-                client_config = response
+                combiner_config = response
                 break
             if status == Status.UnAuthorized:
                 logger.critical(response)
                 sys.exit("Exiting: Unauthorized")
             if status == Status.UnMatchedConfig:
                 logger.critical(response)
                 sys.exit("Exiting: UnMatchedConfig")
             time.sleep(5)
-
         logger.info("Assignment successfully received.")
-        logger.info("Received combiner configuration: {}".format(client_config))
-        return client_config
+        logger.info("Received combiner configuration: {}".format(combiner_config))
+        return combiner_config
 
     def _add_grpc_metadata(self, key, value):
         """Add metadata for gRPC calls.
 
         :param key: The key of the metadata.
         :type key: str
         :param value: The value of the metadata.
@@ -162,40 +170,43 @@
         ssl_sock.do_handshake()
         cert = ssl_sock.get_peer_certificate()
         ssl_sock.close()
         sock.close()
         cert = cert.to_cryptography().public_bytes(Encoding.PEM).decode()
         return cert
 
-    def _connect(self, client_config):
-        """Connect to assigned combiner.
+    def connect(self, combiner_config):
+        """Connect to combiner.
 
-        :param client_config: A configuration dictionary containing connection information for
-        the combiner.
-        :type client_config: dict
+        :param combiner_config: connection information for the combiner.
+        :type combiner_config: dict
         """
 
-        # TODO use the client_config['certificate'] for setting up secure comms'
-        host = client_config['host']
+        if self._connected:
+            logger.info("Client is already attached. ")
+            return None
+
+        # TODO use the combiner_config['certificate'] for setting up secure comms'
+        host = combiner_config['host']
         # Add host to gRPC metadata
         self._add_grpc_metadata('grpc-server', host)
-        logger.info("Client using metadata: {}.".format(self.metadata))
-        port = client_config['port']
+        logger.debug("Client using metadata: {}.".format(self.metadata))
+        port = combiner_config['port']
         secure = False
-        if client_config['fqdn'] is not None:
-            host = client_config['fqdn']
+        if combiner_config['fqdn'] is not None:
+            host = combiner_config['fqdn']
             # assuming https if fqdn is used
             port = 443
         logger.info(f"Initiating connection to combiner host at: {host}:{port}")
 
-        if client_config['certificate']:
+        if combiner_config['certificate']:
             logger.info("Utilizing CA certificate for GRPC channel authentication.")
             secure = True
             cert = base64.b64decode(
-                client_config['certificate'])  # .decode('utf-8')
+                combiner_config['certificate'])  # .decode('utf-8')
             credentials = grpc.ssl_channel_credentials(root_certificates=cert)
             channel = grpc.secure_channel("{}:{}".format(host, str(port)), credentials)
         elif os.getenv("FEDN_GRPC_ROOT_CERT_PATH"):
             secure = True
             logger.info("Using root certificate from environment variable for GRPC channel.")
             with open(os.environ["FEDN_GRPC_ROOT_CERT_PATH"], 'rb') as f:
                 credentials = grpc.ssl_channel_credentials(f.read())
@@ -227,56 +238,39 @@
         self.modelStub = rpc.ModelServiceStub(channel)
 
         logger.info("Successfully established {} connection to {}:{}".format("secure" if secure else "insecure",
                                                                              host,
                                                                              port))
 
         logger.info("Using {} compute package.".format(
-            client_config["package"]))
-
-    def _disconnect(self):
-        """Disconnect from the combiner."""
-        self.channel.close()
+            combiner_config["package"]))
 
-    def detach(self):
-        """Detach from the FEDn network (disconnect from combiner)"""
-        # Setting _attached to False will make all processing threads return
-        if not self._attached:
-            logger.info("Client is not attached.")
-
-        self._attached = False
-        # Close gRPC connection to combiner
-        self._disconnect()
-
-    def _attach(self):
-        """Attach to the FEDn network (connect to combiner)"""
-        # Ask controller for a combiner and connect to that combiner.
-        if self._attached:
-            logger.info("Client is already attached. ")
-            return None
+        self._connected = True
 
-        client_config = self._assign()
-        self._connect(client_config)
+    def disconnect(self):
+        """Disconnect from the combiner."""
+        if not self._connected:
+            logger.info("Client is not connected.")
 
-        if client_config:
-            self._attached = True
-        return client_config
+        self.channel.close()
+        self._connected = False
+        logger.info("Client {} disconnected.".format(self.name))
 
-    def _initialize_helper(self, client_config):
+    def _initialize_helper(self, combiner_config):
         """Initialize the helper class for the client.
 
-        :param client_config: A configuration dictionary containing connection information for
+        :param combiner_config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
-        :type client_config: dict
+        :type combiner_config: dict
         :return:
         """
 
-        if 'helper_type' in client_config.keys():
-            self.helper = get_helper(client_config['helper_type'])
+        if 'helper_type' in combiner_config.keys():
+            self.helper = get_helper(combiner_config['helper_type'])
 
     def _subscribe_to_combiner(self, config):
         """Listen to combiner message stream and start all processing threads.
 
         :param config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
@@ -285,19 +279,23 @@
         # Start sending heartbeats to the combiner.
         threading.Thread(target=self._send_heartbeat, kwargs={
             'update_frequency': config['heartbeat_interval']}, daemon=True).start()
 
         # Start listening for combiner training and validation messages
         threading.Thread(
             target=self._listen_to_task_stream, daemon=True).start()
-        self._attached = True
+        self._connected = True
 
         # Start processing the client message inbox
         threading.Thread(target=self.process_request, daemon=True).start()
 
+    @retry(stop=stop_after_attempt(3))
+    def untar_package(self, package_runtime):
+        package_runtime.unpack()
+
     def _initialize_dispatcher(self, config):
         """ Initialize the dispatcher for the client.
 
         :param config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         :type config: dict
@@ -330,34 +328,41 @@
                     checks_out = pr.validate(config['checksum'])
                     if not checks_out:
                         logger.critical("Validation of local package failed. Client terminating.")
                         self.error_state = True
                         return
 
             if retval:
-                pr.unpack()
+                self.untar_package(pr)
 
             self.dispatcher = pr.dispatcher(self.run_path)
             try:
                 logger.info("Initiating Dispatcher with entrypoint set to: startup")
+                activate_cmd = self.dispatcher._get_or_create_python_env()
                 self.dispatcher.run_cmd("startup")
             except KeyError:
+                logger.info("No startup command found in package. Continuing.")
                 pass
             except Exception as e:
                 logger.error(f"Caught exception: {type(e).__name__}")
+
         else:
             # TODO: Deprecate
             dispatch_config = {'entry_points':
                                {'predict': {'command': 'python3 predict.py'},
                                 'train': {'command': 'python3 train.py'},
                                 'validate': {'command': 'python3 validate.py'}}}
             from_path = os.path.join(os.getcwd(), 'client')
 
             copy_tree(from_path, self.run_path)
             self.dispatcher = Dispatcher(dispatch_config, self.run_path)
+        # Get or create python environment
+        activate_cmd = self.dispatcher._get_or_create_python_env()
+        if activate_cmd:
+            logger.info("To activate the virtual environment, run: {}".format(activate_cmd))
 
     def get_model_from_combiner(self, id, timeout=20):
         """Fetch a model from the assigned combiner.
         Downloads the model update object via a gRPC streaming channel.
 
         :param id: The id of the model update object.
         :type id: str
@@ -366,29 +371,32 @@
         """
         data = BytesIO()
         time_start = time.time()
         request = fedn.ModelRequest(id=id)
         request.sender.name = self.name
         request.sender.role = fedn.WORKER
 
-        for part in self.modelStub.Download(request, metadata=self.metadata):
-
-            if part.status == fedn.ModelStatus.IN_PROGRESS:
-                data.write(part.data)
+        try:
+            for part in self.modelStub.Download(request, metadata=self.metadata):
 
-            if part.status == fedn.ModelStatus.OK:
-                return data
+                if part.status == fedn.ModelStatus.IN_PROGRESS:
+                    data.write(part.data)
 
-            if part.status == fedn.ModelStatus.FAILED:
-                return None
+                if part.status == fedn.ModelStatus.OK:
+                    return data
 
-            if part.status == fedn.ModelStatus.UNKNOWN:
-                if time.time() - time_start >= timeout:
+                if part.status == fedn.ModelStatus.FAILED:
                     return None
-                continue
+
+                if part.status == fedn.ModelStatus.UNKNOWN:
+                    if time.time() - time_start >= timeout:
+                        return None
+                    continue
+        except grpc.RpcError as e:
+            logger.critical(f"GRPC: An error occurred during model download: {e}")
 
         return data
 
     def send_model_to_combiner(self, model, id):
         """Send a model update to the assigned combiner.
         Uploads the model updated object via a gRPC streaming channel, Upload.
 
@@ -405,15 +413,18 @@
             for d in model.stream(32 * 1024):
                 bt.write(d)
         else:
             bt = model
 
         bt.seek(0, 0)
 
-        result = self.modelStub.Upload(upload_request_generator(bt, id), metadata=self.metadata)
+        try:
+            result = self.modelStub.Upload(upload_request_generator(bt, id), metadata=self.metadata)
+        except grpc.RpcError as e:
+            logger.critical(f"GRPC: An error occurred during model upload: {e}")
 
         return result
 
     def _listen_to_task_stream(self):
         """Subscribe to the model update request stream.
 
         :return: None
@@ -422,62 +433,74 @@
 
         r = fedn.ClientAvailableMessage()
         r.sender.name = self.name
         r.sender.role = fedn.WORKER
         # Add client to metadata
         self._add_grpc_metadata('client', self.name)
 
-        while self._attached:
+        while self._connected:
             try:
                 for request in self.combinerStub.TaskStream(r, metadata=self.metadata):
                     if request:
                         logger.debug("Received model update request from combiner: {}.".format(request))
                     if request.sender.role == fedn.COMBINER:
                         # Process training request
-                        self._send_status("Received model update request.", log_level=fedn.Status.AUDIT,
-                                          type=fedn.StatusType.MODEL_UPDATE_REQUEST, request=request)
+                        self.send_status("Received model update request.", log_level=fedn.Status.AUDIT,
+                                         type=fedn.StatusType.MODEL_UPDATE_REQUEST, request=request, sesssion_id=request.session_id)
                         logger.info("Received model update request of type {} for model_id {}".format(request.type, request.model_id))
 
                         if request.type == fedn.StatusType.MODEL_UPDATE and self.config['trainer']:
                             self.inbox.put(('train', request))
                         elif request.type == fedn.StatusType.MODEL_VALIDATION and self.config['validator']:
                             self.inbox.put(('validate', request))
                         else:
                             logger.error("Unknown request type: {}".format(request.type))
 
             except grpc.RpcError as e:
                 # Handle gRPC errors
                 status_code = e.code()
                 if status_code == grpc.StatusCode.UNAVAILABLE:
-                    logger.warning("GRPC server unavailable during model update request stream. Retrying.")
+                    logger.warning("GRPC TaskStream: server unavailable during model update request stream. Retrying.")
                     # Retry after a delay
                     time.sleep(5)
+                if status_code == grpc.StatusCode.UNAUTHENTICATED:
+                    details = e.details()
+                    if details == 'Token expired':
+                        logger.warning("GRPC TaskStream: Token expired. Reconnecting.")
+                        self.detach()
+
+                if status_code == grpc.StatusCode.CANCELLED:
+                    # Expected if the client is detached
+                    logger.critical("GRPC TaskStream: Client detached from combiner. Atempting to reconnect.")
+
                 else:
                     # Log the error and continue
-                    logger.error(f"An error occurred during model update request stream: {e}")
+                    logger.error(f"GRPC TaskStream: An error occurred during model update request stream: {e}")
 
             except Exception as ex:
                 # Handle other exceptions
-                logger.error(f"An error occurred during model update request stream: {ex}")
+                logger.error(f"GRPC TaskStream: An error occurred during model update request stream: {ex}")
 
         # Detach if not attached
-        if not self._attached:
+        if not self._connected:
             return
 
-    def _process_training_request(self, model_id):
+    def _process_training_request(self, model_id: str, session_id: str = None):
         """Process a training (model update) request.
 
         :param model_id: The model id of the model to be updated.
         :type model_id: str
+        :param session_id: The id of the current session
+        :type session_id: str
         :return: The model id of the updated model, or None if the update failed. And a dict with metadata.
         :rtype: tuple
         """
 
-        self._send_status(
-            "\t Starting processing of training request for model_id {}".format(model_id))
+        self.send_status(
+            "\t Starting processing of training request for model_id {}".format(model_id), sesssion_id=session_id)
         self.state = ClientState.training
 
         try:
             meta = {}
             tic = time.time()
             mdl = self.get_model_from_combiner(str(model_id))
             if mdl is None:
@@ -522,44 +545,46 @@
             updated_model_id = None
             meta = {'status': 'failed', 'error': str(e)}
 
         self.state = ClientState.idle
 
         return updated_model_id, meta
 
-    def _process_validation_request(self, model_id, is_inference):
+    def _process_validation_request(self, model_id: str, is_inference: bool, session_id: str = None):
         """Process a validation request.
 
         :param model_id: The model id of the model to be validated.
         :type model_id: str
         :param is_inference: True if the validation is an inference request, False if it is a validation request.
         :type is_inference: bool
+        :param session_id: The id of the current session.
+        :type session_id: str
         :return: The validation metrics, or None if validation failed.
         :rtype: dict
         """
         # Figure out cmd
         if is_inference:
             cmd = 'infer'
         else:
             cmd = 'validate'
 
-        self._send_status(
-            f"Processing {cmd} request for model_id {model_id}")
+        self.send_status(
+            f"Processing {cmd} request for model_id {model_id}", sesssion_id=session_id)
         self.state = ClientState.validating
         try:
             model = self.get_model_from_combiner(str(model_id))
             if model is None:
                 logger.error("Could not retrieve model from combiner. Aborting validation request.")
                 return None
             inpath = self.helper.get_tmp_path()
 
             with open(inpath, "wb") as fh:
                 fh.write(model.getbuffer())
 
-            _, outpath = tempfile.mkstemp()
+            outpath = get_tmp_path()
             self.dispatcher.run_cmd(f"{cmd} {inpath} {outpath}")
 
             with open(outpath, "r") as fh:
                 validation = json.loads(fh.read())
 
             os.unlink(inpath)
             os.unlink(outpath)
@@ -572,91 +597,113 @@
         self.state = ClientState.idle
         return validation
 
     def process_request(self):
         """Process training and validation tasks. """
         while True:
 
-            if not self._attached:
+            if not self._connected:
                 return
 
             try:
                 (task_type, request) = self.inbox.get(timeout=1.0)
                 if task_type == 'train':
 
                     tic = time.time()
                     self.state = ClientState.training
                     model_id, meta = self._process_training_request(
-                        request.model_id)
-                    processing_time = time.time()-tic
-                    meta['processing_time'] = processing_time
-                    meta['config'] = request.data
+                        request.model_id, session_id=request.session_id)
+
+                    if meta is not None:
+                        processing_time = time.time()-tic
+                        meta['processing_time'] = processing_time
+                        meta['config'] = request.data
 
                     if model_id is not None:
                         # Send model update to combiner
                         update = fedn.ModelUpdate()
                         update.sender.name = self.name
                         update.sender.role = fedn.WORKER
                         update.receiver.name = request.sender.name
                         update.receiver.role = request.sender.role
                         update.model_id = request.model_id
                         update.model_update_id = str(model_id)
                         update.timestamp = str(datetime.now())
                         update.correlation_id = request.correlation_id
                         update.meta = json.dumps(meta)
-                        # TODO: Check responses
-                        _ = self.combinerStub.SendModelUpdate(update, metadata=self.metadata)
-                        self._send_status("Model update completed.", log_level=fedn.Status.AUDIT,
-                                          type=fedn.StatusType.MODEL_UPDATE, request=update)
 
+                        try:
+                            _ = self.combinerStub.SendModelUpdate(update, metadata=self.metadata)
+                            self.send_status("Model update completed.", log_level=fedn.Status.AUDIT,
+                                             type=fedn.StatusType.MODEL_UPDATE, request=update, sesssion_id=request.session_id)
+                        except grpc.RpcError as e:
+                            status_code = e.code()
+                            logger.error("GRPC error, {}.".format(
+                                status_code.name))
+                            logger.debug(e)
+                        except ValueError as e:
+                            logger.error("GRPC error, RPC channel closed. {}".format(e))
+                            logger.debug(e)
                     else:
-                        self._send_status("Client {} failed to complete model update.",
-                                          log_level=fedn.Status.WARNING,
-                                          request=request)
+                        self.send_status("Client {} failed to complete model update.",
+                                         log_level=fedn.Status.WARNING,
+                                         request=request, sesssion_id=request.session_id)
+
                     self.state = ClientState.idle
                     self.inbox.task_done()
 
                 elif task_type == 'validate':
                     self.state = ClientState.validating
                     metrics = self._process_validation_request(
-                        request.model_id, False)
+                        request.model_id, False, request.session_id)
 
                     if metrics is not None:
                         # Send validation
                         validation = fedn.ModelValidation()
                         validation.sender.name = self.name
                         validation.sender.role = fedn.WORKER
                         validation.receiver.name = request.sender.name
                         validation.receiver.role = request.sender.role
                         validation.model_id = str(request.model_id)
                         validation.data = json.dumps(metrics)
                         validation.timestamp.GetCurrentTime()
                         validation.correlation_id = request.correlation_id
+                        validation.session_id = request.session_id
 
-                        _ = self.combinerStub.SendModelValidation(
-                            validation, metadata=self.metadata)
-
-                        status_type = fedn.StatusType.MODEL_VALIDATION
-
-                        self._send_status("Model validation completed.", log_level=fedn.Status.AUDIT,
-                                          type=status_type, request=validation)
+                        try:
+                            _ = self.combinerStub.SendModelValidation(
+                                validation, metadata=self.metadata)
+
+                            status_type = fedn.StatusType.MODEL_VALIDATION
+                            self.send_status("Model validation completed.", log_level=fedn.Status.AUDIT,
+                                             type=status_type, request=validation, sesssion_id=request.session_id)
+                        except grpc.RpcError as e:
+                            status_code = e.code()
+                            logger.error("GRPC error, {}.".format(
+                                status_code.name))
+                            logger.debug(e)
+                        except ValueError as e:
+                            logger.error("GRPC error, RPC channel closed. {}".format(e))
+                            logger.debug(e)
                     else:
-                        self._send_status("Client {} failed to complete model validation.".format(self.name),
-                                          log_level=fedn.Status.WARNING, request=request)
+                        self.send_status("Client {} failed to complete model validation.".format(self.name),
+                                         log_level=fedn.Status.WARNING, request=request, sesssion_id=request.session_id)
 
                     self.state = ClientState.idle
                     self.inbox.task_done()
             except queue.Empty:
                 pass
+            except grpc.RpcError as e:
+                logger.critical(f"GRPC process_request: An error occurred during process request: {e}")
 
     def _handle_combiner_failure(self):
         """ Register failed combiner connection."""
         self._missed_heartbeat += 1
         if self._missed_heartbeat > self.config['reconnect_after_missed_heartbeat']:
-            self.detach()()
+            self.disconnect()
 
     def _send_heartbeat(self, update_frequency=2.0):
         """Send a heartbeat to the combiner.
 
         :param update_frequency: The frequency of the heartbeat in seconds.
         :type update_frequency: float
         :return: None if the client is detached.
@@ -666,66 +713,87 @@
             heartbeat = fedn.Heartbeat(sender=fedn.Client(
                 name=self.name, role=fedn.WORKER))
             try:
                 self.connectorStub.SendHeartbeat(heartbeat, metadata=self.metadata)
                 self._missed_heartbeat = 0
             except grpc.RpcError as e:
                 status_code = e.code()
-                logger.warning("Client heartbeat: GRPC error, {}. Retrying.".format(
-                    status_code.name))
+                if status_code == grpc.StatusCode.UNAVAILABLE:
+                    logger.warning("GRPC hearbeat: server unavailable during send heartbeat. Retrying.")
+                if status_code == grpc.StatusCode.UNAUTHENTICATED:
+                    details = e.details()
+                    if details == 'Token expired':
+                        logger.warning("GRPC hearbeat: Token expired. Reconnecting.")
+                        self.detach()
                 logger.debug(e)
                 self._handle_combiner_failure()
 
             time.sleep(update_frequency)
-            if not self._attached:
+            if not self._connected:
+                logger.info("SendStatus: Client disconnected.")
                 return
 
-    def _send_status(self, msg, log_level=fedn.Status.INFO, type=None, request=None):
+    def send_status(self, msg, log_level=fedn.Status.INFO, type=None, request=None, sesssion_id: str = None):
         """Send status message.
 
         :param msg: The message to send.
         :type msg: str
         :param log_level: The log level of the message.
         :type log_level: fedn.Status.INFO, fedn.Status.WARNING, fedn.Status.ERROR
         :param type: The type of the message.
         :type type: str
         :param request: The request message.
         :type request: fedn.Request
         """
+
+        if not self._connected:
+            logger.info("SendStatus: Client disconnected.")
+            return
+
         status = fedn.Status()
         status.timestamp.GetCurrentTime()
         status.sender.name = self.name
         status.sender.role = fedn.WORKER
         status.log_level = log_level
         status.status = str(msg)
+        status.session_id = sesssion_id
         if type is not None:
             status.type = type
 
         if request is not None:
             status.data = MessageToJson(request)
 
         self.logs.append(
             "{} {} LOG LEVEL {} MESSAGE {}".format(str(datetime.now()), status.sender.name, status.log_level,
                                                    status.status))
-        _ = self.connectorStub.SendStatus(status, metadata=self.metadata)
+        try:
+            _ = self.connectorStub.SendStatus(status, metadata=self.metadata)
+        except grpc.RpcError as e:
+            status_code = e.code()
+            if status_code == grpc.StatusCode.UNAVAILABLE:
+                logger.warning("GRPC SendStatus: server unavailable during send status.")
+            if status_code == grpc.StatusCode.UNAUTHENTICATED:
+                details = e.details()
+                if details == 'Token expired':
+                    logger.warning("GRPC SendStatus: Token expired.")
 
     def run(self):
         """ Run the client. """
         try:
             cnt = 0
             old_state = self.state
             while True:
                 time.sleep(1)
                 if cnt == 0:
                     logger.info("Client is active, waiting for model update requests.")
                     cnt = 1
                 if self.state != old_state:
                     logger.info("Client in {} state.".format(ClientStateToString(self.state)))
-                if not self._attached:
+                if not self._connected:
                     logger.info("Detached from combiner.")
                     # TODO: Implement a check/condition to ulitmately close down if too many reattachment attepts have failed. s
-                    self._attach()
+                    self.attach()
                     self._subscribe_to_combiner(self.config)
                 if self.error_state:
                     return
         except KeyboardInterrupt:
             logger.info("Shutting down.")
```

### Comparing `fedn-0.8.0/fedn/network/clients/connect.py` & `fedn-0.9.0b1/fedn/network/combiner/connect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,132 @@
-# This file contains the Connector class for assigning client to the FEDn network via the discovery service (REST-API).
-# The Connector class is used by the Client class in fedn/network/clients/client.py.
-# Once assigned, the client will retrieve combiner assignment from the discovery service.
-# The discovery service will also add the client to the statestore.
+# This file contains the Connector class for announcing combiner to the FEDn network via the discovery service (REST-API).
+# The Connector class is used by the Combiner class in fedn/network/combiner/server.py.
+# Once announced, the combiner will be able to receive controller requests from the controllerStub via gRPC.
+# The discovery service will also add the combiner to the statestore.
 #
 #
 import enum
+import os
 
 import requests
 
 from fedn.common.log_config import logger
 
 
 class Status(enum.Enum):
-    """ Enum for representing the status of a client assignment."""
+    """ Enum for representing the status of a combiner announcement."""
     Unassigned = 0
     Assigned = 1
     TryAgain = 2
     UnAuthorized = 3
     UnMatchedConfig = 4
 
 
-class ConnectorClient:
-    """ Connector for assigning client to a combiner in the FEDn network.
+class ConnectorCombiner:
+    """ Connector for annnouncing combiner to the FEDn network.
 
     :param host: host of discovery service
     :type host: str
     :param port: port of discovery service
     :type port: int
+    :param myhost: host of combiner
+    :type myhost: str
+    :param fqdn: fully qualified domain name of combiner
+    :type fqdn: str
+    :param myport: port of combiner
+    :type myport: int
     :param token: token for authentication
     :type token: str
-    :param name: name of client
+    :param name: name of combiner
     :type name: str
-    :param remote_package: True if remote package is used, False if local
-    :type remote_package: bool
-    :param force_ssl: True if https is used, False if http
-    :type force_ssl: bool
+    :param secure: True if https is used, False if http
+    :type secure: bool
     :param verify: True if certificate is verified, False if not
     :type verify: bool
-    :param combiner: name of preferred combiner
-    :type combiner: str
-    :param id: id of client
     """
 
-    def __init__(self, host, port, token, name, remote_package, force_ssl=False, verify=False, combiner=None, id=None):
+    def __init__(self, host, port, myhost, fqdn, myport, token, name, secure=False, verify=False):
+        """ Initialize the ConnectorCombiner.
+
+        :param host: The host of the discovery service.
+        :type host: str
+        :param port: The port of the discovery service.
+        :type port: int
+        :param myhost: The host of the combiner.
+        :type myhost: str
+        :param fqdn: The fully qualified domain name of the combiner.
+        :type fqdn: str
+        :param myport: The port of the combiner.
+        :type myport: int
+        :param token: The token for the discovery service.
+        :type token: str
+        :param name: The name of the combiner.
+        :type name: str
+        :param secure: Use https for the connection to the discovery service.
+        :type secure: bool
+        :param verify: Verify the connection to the discovery service.
+        :type verify: bool
+        """
 
         self.host = host
+        self.fqdn = fqdn
         self.port = port
+        self.myhost = myhost
+        self.myport = myport
         self.token = token
+        self.token_scheme = os.environ.get('FEDN_AUTH_SCHEME', 'Bearer')
         self.name = name
+        self.secure = secure
         self.verify = verify
-        self.preferred_combiner = combiner
-        self.id = id
-        self.package = 'remote' if remote_package else 'local'
+
+        if not self.token:
+            self.token = os.environ.get('FEDN_AUTH_TOKEN', None)
 
         # for https we assume a an ingress handles permanent redirect (308)
-        if force_ssl:
-            self.prefix = "https://"
-        else:
-            self.prefix = "http://"
-        if self.port:
+        self.prefix = "http://"
+        if port:
             self.connect_string = "{}{}:{}".format(
                 self.prefix, self.host, self.port)
         else:
             self.connect_string = "{}{}".format(
                 self.prefix, self.host)
 
-        logger.info("Setting connection string to {}.".format(self.connect_string))
+        logger.info("Setting connection string to {}".format(self.connect_string))
 
-    def assign(self):
+    def announce(self):
         """
-        Connect client to FEDn network discovery service, ask for combiner assignment.
+        Announce combiner to FEDn network via discovery service (REST-API).
 
-        :return: Tuple with assingment status, combiner connection information if sucessful, else None.
-        :rtype: tuple(:class:`fedn.network.clients.connect.Status`, str)
+        :return: Tuple with announcement Status, FEDn network configuration if sucessful, else None.
+        :rtype: :class:`fedn.network.combiner.connect.Status`, str
         """
+        payload = {
+            "combiner_id": self.name,
+            "address": self.myhost,
+            "fqdn": self.fqdn,
+            "port": self.myport,
+            "secure_grpc": self.secure
+        }
+        url_prefix = os.environ.get('FEDN_CUSTOM_URL_PREFIX', '')
         try:
-            retval = None
-            payload = {'client_id': self.name, 'preferred_combiner': self.preferred_combiner}
-
-            retval = requests.post(self.connect_string + '/add_client',
-                                   json=payload,
+            retval = requests.post(self.connect_string + url_prefix + '/add_combiner', json=payload,
                                    verify=self.verify,
-                                   allow_redirects=True,
-                                   headers={'Authorization': 'Token {}'.format(self.token)})
-        except Exception as e:
-            print('***** {}'.format(e), flush=True)
+                                   headers={'Authorization': f'{self.token_scheme} {self.token}'})
+        except Exception:
             return Status.Unassigned, {}
 
         if retval.status_code == 400:
             # Get error messange from response
             reason = retval.json()['message']
             return Status.UnMatchedConfig, reason
 
         if retval.status_code == 401:
             reason = "Unauthorized connection to reducer, make sure the correct token is set"
             return Status.UnAuthorized, reason
 
         if retval.status_code >= 200 and retval.status_code < 204:
             if retval.json()['status'] == 'retry':
-                if 'message' in retval.json():
-                    reason = retval.json()['message']
-                else:
-                    reason = "Reducer was not ready. Try again later."
-
+                reason = retval.json()['message']
                 return Status.TryAgain, reason
-
-            reducer_package = retval.json()['package']
-            if reducer_package != self.package:
-                reason = "Unmatched config of compute package between client and reducer.\n" +\
-                    "Reducer uses {} package and client uses {}.".format(
-                        reducer_package, self.package)
-                return Status.UnMatchedConfig, reason
-
             return Status.Assigned, retval.json()
 
         return Status.Unassigned, None
```

### Comparing `fedn-0.8.0/fedn/network/clients/package.py` & `fedn-0.9.0b1/fedn/network/clients/package.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 #
 import cgi
 import os
 import tarfile
 from distutils.dir_util import copy_tree
 
 import requests
-import yaml
 
+from fedn.common.config import FEDN_AUTH_SCHEME, FEDN_CUSTOM_URL_PREFIX
 from fedn.common.log_config import logger
 from fedn.utils.checksum import sha
-from fedn.utils.dispatcher import Dispatcher
+from fedn.utils.dispatcher import Dispatcher, _read_yaml_file
 
 
 class PackageRuntime:
     """ PackageRuntime is used to download, validate and unpack compute packages.
 
     :param package_path: path to compute package
     :type package_path: str
@@ -48,42 +48,42 @@
         """
         # for https we assume a an ingress handles permanent redirect (308)
         if force_ssl:
             scheme = "https"
         else:
             scheme = "http"
         if port:
-            path = f"{scheme}://{host}:{port}/download_package"
+            path = f"{scheme}://{host}:{port}{FEDN_CUSTOM_URL_PREFIX}/download_package"
         else:
-            path = f"{scheme}://{host}/download_package"
+            path = f"{scheme}://{host}{FEDN_CUSTOM_URL_PREFIX}/download_package"
         if name:
             path = path + "?name={}".format(name)
 
-        with requests.get(path, stream=True, verify=False, headers={'Authorization': 'Token {}'.format(token)}) as r:
+        with requests.get(path, stream=True, verify=False, headers={'Authorization': f'{FEDN_AUTH_SCHEME} {token}'}) as r:
             if 200 <= r.status_code < 204:
 
                 params = cgi.parse_header(
                     r.headers.get('Content-Disposition', ''))[-1]
                 try:
                     self.pkg_name = params['filename']
                 except KeyError:
                     logger.error("No package returned.")
                     return None
                 r.raise_for_status()
                 with open(os.path.join(self.pkg_path, self.pkg_name), 'wb') as f:
                     for chunk in r.iter_content(chunk_size=8192):
                         f.write(chunk)
         if port:
-            path = f"{scheme}://{host}:{port}/get_package_checksum"
+            path = f"{scheme}://{host}:{port}{FEDN_CUSTOM_URL_PREFIX}/get_package_checksum"
         else:
-            path = f"{scheme}://{host}/get_package_checksum"
+            path = f"{scheme}://{host}{FEDN_CUSTOM_URL_PREFIX}/get_package_checksum"
 
         if name:
             path = path + "?name={}".format(name)
-        with requests.get(path, verify=False, headers={'Authorization': 'Token {}'.format(token)}) as r:
+        with requests.get(path, verify=False, headers={'Authorization': f'{FEDN_AUTH_SCHEME} {token}'}) as r:
             if 200 <= r.status_code < 204:
 
                 data = r.json()
                 try:
                     self.checksum = data['checksum']
                 except Exception:
                     logger.error("Could not extract checksum.")
@@ -153,21 +153,11 @@
         :rtype: :class:`fedn.utils.dispatcher.Dispatcher`
         """
         from_path = os.path.join(os.getcwd(), 'client')
 
         # preserve_times=False ensures compatibility with Gramine LibOS
         copy_tree(from_path, run_path, preserve_times=False)
 
-        try:
-            cfg = None
-            with open(os.path.join(run_path, 'fedn.yaml'), 'rb') as config_file:
-
-                cfg = yaml.safe_load(config_file.read())
-                self.dispatch_config = cfg
-
-        except Exception:
-            logger.error(
-                "Error trying to load and unpack dispatcher config - trying default")
-
+        self.dispatch_config = _read_yaml_file(os.path.join(run_path, 'fedn.yaml'))
         dispatcher = Dispatcher(self.dispatch_config, run_path)
 
         return dispatcher
```

### Comparing `fedn-0.8.0/fedn/network/clients/state.py` & `fedn-0.9.0b1/fedn/network/clients/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/clients/test_client.py` & `fedn-0.9.0b1/fedn/network/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/combiner/aggregators/aggregator.py` & `fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/combiner/aggregators/aggregatorbase.py` & `fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregatorbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,19 +112,25 @@
         :type helper: fedn.utils.helpers.helperbase.Helper
         :return: A tuple of (parameters, metadata)
         :rtype: tuple
         """
         model_id = model_update.model_update_id
         model = self.round_handler.load_model_update(helper, model_id)
         # Get relevant metadata
-        data = json.loads(model_update.meta)['training_metadata']
-        config = json.loads(json.loads(model_update.meta)['config'])
-        data['round_id'] = config['round_id']
+        metadata = json.loads(model_update.meta)
+        if 'config' in metadata.keys():
+            # Used in Python client
+            config = json.loads(metadata['config'])
+        else:
+            # Used in C++ client
+            config = json.loads(model_update.config)
+        training_metadata = metadata['training_metadata']
+        training_metadata['round_id'] = config['round_id']
 
-        return model, data
+        return model, training_metadata
 
     def get_state(self):
         """ Get the state of the aggregator's queue, including the number of model updates."""
         state = {
             'queue_len': self.model_updates.qsize()
         }
         return state
```

### Comparing `fedn-0.8.0/fedn/network/combiner/aggregators/fedavg.py` & `fedn-0.9.0b1/fedn/network/combiner/aggregators/fedavg.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,19 @@
 
         logger.info(
             "AGGREGATOR({}): Aggregating model updates... ".format(self.name))
 
         while not self.model_updates.empty():
             try:
                 # Get next model from queue
+                logger.info("AGGREGATOR({}): Getting next model update from queue.".format(self.name))
                 model_update = self.next_model_update()
 
                 # Load model parameters and metadata
+                logger.info("AGGREGATOR({}): Loading model metadata {}.".format(self.name, model_update.model_update_id))
                 model_next, metadata = self.load_model_update(model_update, helper)
 
                 logger.info(
                     "AGGREGATOR({}): Processing model update {}, metadata: {}  ".format(self.name, model_update.model_update_id, metadata))
 
                 # Increment total number of examples
                 total_examples += metadata['num_examples']
```

### Comparing `fedn-0.8.0/fedn/network/combiner/aggregators/fedopt.py` & `fedn-0.9.0b1/fedn/network/combiner/aggregators/fedopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,21 @@
         super().__init__(storage, server, modelservice, round_handler)
 
         self.name = "fedopt"
         self.v = None
         self.m = None
 
         # Server side hyperparameters. Note that these may need extensive fine tuning.
-        self.eta = 0.1
+        self.eta = 1e-2
         self.beta1 = 0.9
         self.beta2 = 0.99
         self.tau = 1e-4
 
     def combine_models(self, helper=None, delete_models=True):
-        """Compute pseudo gradients usigng model updates in the queue.
+        """Compute pseudo gradients using model updates in the queue.
 
         :param helper: An instance of :class: `fedn.utils.helpers.helpers.HelperBase`, ML framework specific helper, defaults to None
         :type helper: class: `fedn.utils.helpers.helpers.HelperBase`, optional
         :param time_window: The time window for model aggregation, defaults to 180
         :type time_window: int, optional
         :param max_nr_models: The maximum number of updates aggregated, defaults to 100
         :type max_nr_models: int, optional
@@ -71,28 +71,28 @@
                 model_update = self.next_model_update()
 
                 # Load model paratmeters and metadata
                 model_next, metadata = self.load_model_update(model_update, helper)
 
                 logger.info(
                     "AGGREGATOR({}): Processing model update {}, metadata: {}  ".format(self.name, model_update.model_update_id, metadata))
-                print("***** ", model_update, flush=True)
+                logger.info("***** {}".format(model_update))
 
                 # Increment total number of examples
                 total_examples += metadata['num_examples']
 
                 if nr_aggregated_models == 0:
                     model_old = self.round_handler.load_model_update(helper, model_update.model_id)
                     pseudo_gradient = helper.subtract(model_next, model_old)
                 else:
                     pseudo_gradient_next = helper.subtract(model_next, model_old)
                     pseudo_gradient = helper.increment_average(
                         pseudo_gradient, pseudo_gradient_next, metadata['num_examples'], total_examples)
 
-                print("NORM PSEUDOGRADIENT: ", helper.norm(pseudo_gradient), flush=True)
+                logger.info("NORM PSEUDOGRADIENT: {}".format(helper.norm(pseudo_gradient)))
 
                 nr_aggregated_models += 1
                 # Delete model from storage
                 if delete_models:
                     self.modelservice.temp_model_storage.delete(model_update.model_update_id)
                     logger.info(
                         "AGGREGATOR({}): Deleted model update {} from storage.".format(self.name, model_update.model_update_id))
```

### Comparing `fedn-0.8.0/fedn/network/combiner/combiner.py` & `fedn-0.9.0b1/fedn/network/combiner/combiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,14 @@
 
         # Set up gRPC server configuration
         grpc_config = {'port': config['port'],
                        'secure': config['secure'],
                        'certificate': cert,
                        'key': key}
 
-        print(announce_config, flush=True)
-
         # Set up model repository
         self.repository = Repository(
             announce_config['storage']['storage_config'])
 
         self.statestore = MongoStateStore(
             announce_config['statestore']['network_id'],
             announce_config['statestore']['mongo_config']
@@ -171,14 +169,15 @@
         # The request to be added to the client queue
         request = fedn.TaskRequest()
         request.model_id = config['model_id']
         request.correlation_id = str(uuid.uuid4())
         request.timestamp = str(datetime.now())
         request.data = json.dumps(config)
         request.type = fedn.StatusType.MODEL_UPDATE
+        request.session_id = config['session_id']
 
         request.sender.name = self.id
         request.sender.role = fedn.COMBINER
 
         if len(clients) == 0:
             clients = self.get_active_trainers()
 
@@ -211,14 +210,15 @@
         request.correlation_id = str(uuid.uuid4())
         request.timestamp = str(datetime.now())
         # request.is_inference = (config['task'] == 'inference')
         request.type = fedn.StatusType.MODEL_VALIDATION
 
         request.sender.name = self.id
         request.sender.role = fedn.COMBINER
+        request.session_id = config["session_id"]
 
         if len(clients) == 0:
             clients = self.get_active_validators()
 
         for client in clients:
             request.receiver.name = client
             request.receiver.role = fedn.WORKER
@@ -558,15 +558,15 @@
                 response.status = fedn.ConnectionStatus.NOT_ACCEPTING
                 return response
             if len(active_clients) < requested:
                 response.status = fedn.ConnectionStatus.ACCEPTING
                 return response
 
         except Exception as e:
-            logger.error("Combiner not properly configured! {}".format(e), flush=True)
+            logger.error("Combiner not properly configured! {}".format(e))
             raise
 
         response.status = fedn.ConnectionStatus.TRY_AGAIN_LATER
         return response
 
     def SendHeartbeat(self, heartbeat: fedn.Heartbeat, context):
         """ RPC that lets clients send a hearbeat, notifying the server that
```

### Comparing `fedn-0.8.0/fedn/network/combiner/modelservice.py` & `fedn-0.9.0b1/fedn/network/combiner/modelservice.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/combiner/roundhandler.py` & `fedn-0.9.0b1/fedn/network/combiner/roundhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,46 +250,33 @@
             n = len(clients)
 
         # If not, we pick a random subsample of all available clients.
         clients = random.sample(clients, n)
 
         return clients
 
-    def _check_nr_round_clients(self, config, timeout=0.0):
+    def _check_nr_round_clients(self, config):
         """Check that the minimal number of clients required to start a round are available.
 
         :param config: The round config object.
         :type config: dict
         :param timeout: Timeout in seconds, defaults to 0.0
         :type timeout: float, optional
         :return: True if the required number of clients are available, False otherwise.
         :rtype: bool
         """
 
-        ready = False
-        t = 0.0
-        while not ready:
-            active = self.server.nr_active_trainers()
-
-            if active >= int(config['clients_requested']):
-                return True
-            else:
-                logger.info("waiting for {} clients to get started, currently: {}".format(
-                    int(config['clients_requested']) - active,
-                    active))
-            if t >= timeout:
-                if active >= int(config['clients_required']):
-                    return True
-                else:
-                    return False
-
-            time.sleep(1.0)
-            t += 1.0
-
-        return ready
+        active = self.server.nr_active_trainers()
+        if active >= int(config['clients_required']):
+            logger.info("Number of clients required ({0}) to start round met {1}.".format(
+                config['clients_required'], active))
+            return True
+        else:
+            logger.info("Too few clients to start round.")
+            return False
 
     def execute_validation_round(self, round_config):
         """ Coordinate validation rounds as specified in config.
 
         :param round_config: The round config object.
         :type round_config: dict
         """
```

### Comparing `fedn-0.8.0/fedn/network/controller/control.py` & `fedn-0.9.0b1/fedn/network/controller/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,23 +141,24 @@
         : type round_id: str
 
         """
 
         self.create_round({'round_id': round_id, 'status': "Pending"})
 
         if len(self.network.get_combiners()) < 1:
-            logger.warning("Round cannot start, no combiners connected!", flush=True)
+            logger.warning("Round cannot start, no combiners connected!")
             self.set_round_status(round_id, 'Failed')
             return None, self.statestore.get_round(round_id)
 
         # Assemble round config for this global round
         round_config = copy.deepcopy(session_config)
         round_config["rounds"] = 1
         round_config["round_id"] = round_id
         round_config["task"] = "training"
+        round_config["session_id"] = session_config["session_id"]
 
         self.set_round_config(round_id, round_config)
 
         # Get combiners that are able to participate in the round, given round_config
         participating_combiners = self.get_participating_combiners(round_config)
 
         # Check if the policy to start the round is met
```

### Comparing `fedn-0.8.0/fedn/network/controller/controlbase.py` & `fedn-0.9.0b1/fedn/network/controller/controlbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,25 +173,26 @@
         if compute_package == "":
             compute_package = self.get_compute_package_name()
         if compute_package:
             return self.model_repository.get_compute_package(compute_package)
         else:
             return None
 
-    def create_session(self, config):
+    def create_session(self, config, status='Initialized'):
         """ Initialize a new session in backend db. """
 
         if "session_id" not in config.keys():
             session_id = uuid.uuid4()
             config["session_id"] = str(session_id)
         else:
             session_id = config["session_id"]
 
         self.statestore.create_session(id=session_id)
         self.statestore.set_session_config(session_id, config)
+        self.statestore.set_session_status(session_id, status)
 
     def set_session_status(self, session_id, status):
         """ Set the round round stats.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param status: The status
```

### Comparing `fedn-0.8.0/fedn/network/grpc/fedn_pb2.py` & `fedn-0.9.0b1/fedn/network/grpc/fedn_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,82 +10,82 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66\x65\x64n/network/grpc/fedn.proto\x12\x04grpc\x1a\x1fgoogle/protobuf/timestamp.proto\":\n\x08Response\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x10\n\x08response\x18\x02 \x01(\t\"\xa8\x02\n\x06Status\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x0e\n\x06status\x18\x02 \x01(\t\x12(\n\tlog_level\x18\x03 \x01(\x0e\x32\x15.grpc.Status.LogLevel\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x04type\x18\x07 \x01(\x0e\x32\x10.grpc.StatusType\x12\r\n\x05\x65xtra\x18\x08 \x01(\t\"B\n\x08LogLevel\x12\x08\n\x04INFO\x10\x00\x12\t\n\x05\x44\x45\x42UG\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\t\n\x05\x41UDIT\x10\x04\"\xd8\x01\n\x0bTaskRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04meta\x18\x07 \x01(\t\x12\x12\n\nsession_id\x18\x08 \x01(\t\x12\x1e\n\x04type\x18\t \x01(\x0e\x32\x10.grpc.StatusType\"\xaf\x01\n\x0bModelUpdate\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x17\n\x0fmodel_update_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04meta\x18\x07 \x01(\t\"\xc4\x01\n\x0fModelValidation\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04meta\x18\x07 \x01(\t\"\x89\x01\n\x0cModelRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\n\n\x02id\x18\x04 \x01(\t\x12!\n\x06status\x18\x05 \x01(\x0e\x32\x11.grpc.ModelStatus\"]\n\rModelResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x06status\x18\x03 \x01(\x0e\x32\x11.grpc.ModelStatus\x12\x0f\n\x07message\x18\x04 \x01(\t\"U\n\x15GetGlobalModelRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\"h\n\x16GetGlobalModelResponse\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\")\n\tHeartbeat\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\"W\n\x16\x43lientAvailableMessage\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\ttimestamp\x18\x03 \x01(\t\"P\n\x12ListClientsRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1c\n\x07\x63hannel\x18\x02 \x01(\x0e\x32\x0b.grpc.Queue\"*\n\nClientList\x12\x1c\n\x06\x63lient\x18\x01 \x03(\x0b\x32\x0c.grpc.Client\"0\n\x06\x43lient\x12\x18\n\x04role\x18\x01 \x01(\x0e\x32\n.grpc.Role\x12\x0c\n\x04name\x18\x02 \x01(\t\"m\n\x0fReassignRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x0e\n\x06server\x18\x03 \x01(\t\x12\x0c\n\x04port\x18\x04 \x01(\r\"c\n\x10ReconnectRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.grpc.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.grpc.Client\x12\x11\n\treconnect\x18\x03 \x01(\r\"\'\n\tParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"T\n\x0e\x43ontrolRequest\x12\x1e\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\r.grpc.Command\x12\"\n\tparameter\x18\x02 \x03(\x0b\x32\x0f.grpc.Parameter\"F\n\x0f\x43ontrolResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\"\n\tparameter\x18\x02 \x03(\x0b\x32\x0f.grpc.Parameter\"\x13\n\x11\x43onnectionRequest\"<\n\x12\x43onnectionResponse\x12&\n\x06status\x18\x01 \x01(\x0e\x32\x16.grpc.ConnectionStatus*\x84\x01\n\nStatusType\x12\x07\n\x03LOG\x10\x00\x12\x18\n\x14MODEL_UPDATE_REQUEST\x10\x01\x12\x10\n\x0cMODEL_UPDATE\x10\x02\x12\x1c\n\x18MODEL_VALIDATION_REQUEST\x10\x03\x12\x14\n\x10MODEL_VALIDATION\x10\x04\x12\r\n\tINFERENCE\x10\x05*$\n\x05Queue\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0e\n\nTASK_QUEUE\x10\x01*S\n\x0bModelStatus\x12\x06\n\x02OK\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x12\n\x0eIN_PROGRESS_OK\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x0b\n\x07UNKNOWN\x10\x04*8\n\x04Role\x12\n\n\x06WORKER\x10\x00\x12\x0c\n\x08\x43OMBINER\x10\x01\x12\x0b\n\x07REDUCER\x10\x02\x12\t\n\x05OTHER\x10\x03*J\n\x07\x43ommand\x12\x08\n\x04IDLE\x10\x00\x12\t\n\x05START\x10\x01\x12\t\n\x05PAUSE\x10\x02\x12\x08\n\x04STOP\x10\x03\x12\t\n\x05RESET\x10\x04\x12\n\n\x06REPORT\x10\x05*I\n\x10\x43onnectionStatus\x12\x11\n\rNOT_ACCEPTING\x10\x00\x12\r\n\tACCEPTING\x10\x01\x12\x13\n\x0fTRY_AGAIN_LATER\x10\x02\x32z\n\x0cModelService\x12\x33\n\x06Upload\x12\x12.grpc.ModelRequest\x1a\x13.grpc.ModelResponse(\x01\x12\x35\n\x08\x44ownload\x12\x12.grpc.ModelRequest\x1a\x13.grpc.ModelResponse0\x01\x32\xf8\x01\n\x07\x43ontrol\x12\x34\n\x05Start\x12\x14.grpc.ControlRequest\x1a\x15.grpc.ControlResponse\x12\x33\n\x04Stop\x12\x14.grpc.ControlRequest\x1a\x15.grpc.ControlResponse\x12\x44\n\x15\x46lushAggregationQueue\x12\x14.grpc.ControlRequest\x1a\x15.grpc.ControlResponse\x12<\n\rSetAggregator\x12\x14.grpc.ControlRequest\x1a\x15.grpc.ControlResponse2V\n\x07Reducer\x12K\n\x0eGetGlobalModel\x12\x1b.grpc.GetGlobalModelRequest\x1a\x1c.grpc.GetGlobalModelResponse2\xab\x03\n\tConnector\x12\x44\n\x14\x41llianceStatusStream\x12\x1c.grpc.ClientAvailableMessage\x1a\x0c.grpc.Status0\x01\x12*\n\nSendStatus\x12\x0c.grpc.Status\x1a\x0e.grpc.Response\x12?\n\x11ListActiveClients\x12\x18.grpc.ListClientsRequest\x1a\x10.grpc.ClientList\x12\x45\n\x10\x41\x63\x63\x65ptingClients\x12\x17.grpc.ConnectionRequest\x1a\x18.grpc.ConnectionResponse\x12\x30\n\rSendHeartbeat\x12\x0f.grpc.Heartbeat\x1a\x0e.grpc.Response\x12\x37\n\x0eReassignClient\x12\x15.grpc.ReassignRequest\x1a\x0e.grpc.Response\x12\x39\n\x0fReconnectClient\x12\x16.grpc.ReconnectRequest\x1a\x0e.grpc.Response2\xbf\x01\n\x08\x43ombiner\x12?\n\nTaskStream\x12\x1c.grpc.ClientAvailableMessage\x1a\x11.grpc.TaskRequest0\x01\x12\x34\n\x0fSendModelUpdate\x12\x11.grpc.ModelUpdate\x1a\x0e.grpc.Response\x12<\n\x13SendModelValidation\x12\x15.grpc.ModelValidation\x1a\x0e.grpc.Responseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66\x65\x64n/network/grpc/fedn.proto\x12\x04\x66\x65\x64n\x1a\x1fgoogle/protobuf/timestamp.proto\":\n\x08Response\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x10\n\x08response\x18\x02 \x01(\t\"\xbc\x02\n\x06Status\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x0e\n\x06status\x18\x02 \x01(\t\x12(\n\tlog_level\x18\x03 \x01(\x0e\x32\x15.fedn.Status.LogLevel\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x04type\x18\x07 \x01(\x0e\x32\x10.fedn.StatusType\x12\r\n\x05\x65xtra\x18\x08 \x01(\t\x12\x12\n\nsession_id\x18\t \x01(\t\"B\n\x08LogLevel\x12\x08\n\x04INFO\x10\x00\x12\t\n\x05\x44\x45\x42UG\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\t\n\x05\x41UDIT\x10\x04\"\xd8\x01\n\x0bTaskRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04meta\x18\x07 \x01(\t\x12\x12\n\nsession_id\x18\x08 \x01(\t\x12\x1e\n\x04type\x18\t \x01(\x0e\x32\x10.fedn.StatusType\"\xbf\x01\n\x0bModelUpdate\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x17\n\x0fmodel_update_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\t\x12\x0c\n\x04meta\x18\x07 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x08 \x01(\t\"\xd8\x01\n\x0fModelValidation\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04meta\x18\x07 \x01(\t\x12\x12\n\nsession_id\x18\x08 \x01(\t\"\x89\x01\n\x0cModelRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\n\n\x02id\x18\x04 \x01(\t\x12!\n\x06status\x18\x05 \x01(\x0e\x32\x11.fedn.ModelStatus\"]\n\rModelResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x06status\x18\x03 \x01(\x0e\x32\x11.fedn.ModelStatus\x12\x0f\n\x07message\x18\x04 \x01(\t\"U\n\x15GetGlobalModelRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\"h\n\x16GetGlobalModelResponse\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x10\n\x08model_id\x18\x03 \x01(\t\")\n\tHeartbeat\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\"W\n\x16\x43lientAvailableMessage\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\ttimestamp\x18\x03 \x01(\t\"P\n\x12ListClientsRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1c\n\x07\x63hannel\x18\x02 \x01(\x0e\x32\x0b.fedn.Queue\"*\n\nClientList\x12\x1c\n\x06\x63lient\x18\x01 \x03(\x0b\x32\x0c.fedn.Client\"0\n\x06\x43lient\x12\x18\n\x04role\x18\x01 \x01(\x0e\x32\n.fedn.Role\x12\x0c\n\x04name\x18\x02 \x01(\t\"m\n\x0fReassignRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x0e\n\x06server\x18\x03 \x01(\t\x12\x0c\n\x04port\x18\x04 \x01(\r\"c\n\x10ReconnectRequest\x12\x1c\n\x06sender\x18\x01 \x01(\x0b\x32\x0c.fedn.Client\x12\x1e\n\x08receiver\x18\x02 \x01(\x0b\x32\x0c.fedn.Client\x12\x11\n\treconnect\x18\x03 \x01(\r\"\'\n\tParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"T\n\x0e\x43ontrolRequest\x12\x1e\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\r.fedn.Command\x12\"\n\tparameter\x18\x02 \x03(\x0b\x32\x0f.fedn.Parameter\"F\n\x0f\x43ontrolResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\"\n\tparameter\x18\x02 \x03(\x0b\x32\x0f.fedn.Parameter\"\x13\n\x11\x43onnectionRequest\"<\n\x12\x43onnectionResponse\x12&\n\x06status\x18\x01 \x01(\x0e\x32\x16.fedn.ConnectionStatus*\x84\x01\n\nStatusType\x12\x07\n\x03LOG\x10\x00\x12\x18\n\x14MODEL_UPDATE_REQUEST\x10\x01\x12\x10\n\x0cMODEL_UPDATE\x10\x02\x12\x1c\n\x18MODEL_VALIDATION_REQUEST\x10\x03\x12\x14\n\x10MODEL_VALIDATION\x10\x04\x12\r\n\tINFERENCE\x10\x05*$\n\x05Queue\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0e\n\nTASK_QUEUE\x10\x01*S\n\x0bModelStatus\x12\x06\n\x02OK\x10\x00\x12\x0f\n\x0bIN_PROGRESS\x10\x01\x12\x12\n\x0eIN_PROGRESS_OK\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x0b\n\x07UNKNOWN\x10\x04*8\n\x04Role\x12\n\n\x06WORKER\x10\x00\x12\x0c\n\x08\x43OMBINER\x10\x01\x12\x0b\n\x07REDUCER\x10\x02\x12\t\n\x05OTHER\x10\x03*J\n\x07\x43ommand\x12\x08\n\x04IDLE\x10\x00\x12\t\n\x05START\x10\x01\x12\t\n\x05PAUSE\x10\x02\x12\x08\n\x04STOP\x10\x03\x12\t\n\x05RESET\x10\x04\x12\n\n\x06REPORT\x10\x05*I\n\x10\x43onnectionStatus\x12\x11\n\rNOT_ACCEPTING\x10\x00\x12\r\n\tACCEPTING\x10\x01\x12\x13\n\x0fTRY_AGAIN_LATER\x10\x02\x32z\n\x0cModelService\x12\x33\n\x06Upload\x12\x12.fedn.ModelRequest\x1a\x13.fedn.ModelResponse(\x01\x12\x35\n\x08\x44ownload\x12\x12.fedn.ModelRequest\x1a\x13.fedn.ModelResponse0\x01\x32\xf8\x01\n\x07\x43ontrol\x12\x34\n\x05Start\x12\x14.fedn.ControlRequest\x1a\x15.fedn.ControlResponse\x12\x33\n\x04Stop\x12\x14.fedn.ControlRequest\x1a\x15.fedn.ControlResponse\x12\x44\n\x15\x46lushAggregationQueue\x12\x14.fedn.ControlRequest\x1a\x15.fedn.ControlResponse\x12<\n\rSetAggregator\x12\x14.fedn.ControlRequest\x1a\x15.fedn.ControlResponse2V\n\x07Reducer\x12K\n\x0eGetGlobalModel\x12\x1b.fedn.GetGlobalModelRequest\x1a\x1c.fedn.GetGlobalModelResponse2\xab\x03\n\tConnector\x12\x44\n\x14\x41llianceStatusStream\x12\x1c.fedn.ClientAvailableMessage\x1a\x0c.fedn.Status0\x01\x12*\n\nSendStatus\x12\x0c.fedn.Status\x1a\x0e.fedn.Response\x12?\n\x11ListActiveClients\x12\x18.fedn.ListClientsRequest\x1a\x10.fedn.ClientList\x12\x45\n\x10\x41\x63\x63\x65ptingClients\x12\x17.fedn.ConnectionRequest\x1a\x18.fedn.ConnectionResponse\x12\x30\n\rSendHeartbeat\x12\x0f.fedn.Heartbeat\x1a\x0e.fedn.Response\x12\x37\n\x0eReassignClient\x12\x15.fedn.ReassignRequest\x1a\x0e.fedn.Response\x12\x39\n\x0fReconnectClient\x12\x16.fedn.ReconnectRequest\x1a\x0e.fedn.Response2\xbf\x01\n\x08\x43ombiner\x12?\n\nTaskStream\x12\x1c.fedn.ClientAvailableMessage\x1a\x11.fedn.TaskRequest0\x01\x12\x34\n\x0fSendModelUpdate\x12\x11.fedn.ModelUpdate\x1a\x0e.fedn.Response\x12<\n\x13SendModelValidation\x12\x15.fedn.ModelValidation\x1a\x0e.fedn.Responseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fedn.network.grpc.fedn_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_STATUSTYPE']._serialized_start=2257
-  _globals['_STATUSTYPE']._serialized_end=2389
-  _globals['_QUEUE']._serialized_start=2391
-  _globals['_QUEUE']._serialized_end=2427
-  _globals['_MODELSTATUS']._serialized_start=2429
-  _globals['_MODELSTATUS']._serialized_end=2512
-  _globals['_ROLE']._serialized_start=2514
-  _globals['_ROLE']._serialized_end=2570
-  _globals['_COMMAND']._serialized_start=2572
-  _globals['_COMMAND']._serialized_end=2646
-  _globals['_CONNECTIONSTATUS']._serialized_start=2648
-  _globals['_CONNECTIONSTATUS']._serialized_end=2721
+  _globals['_STATUSTYPE']._serialized_start=2313
+  _globals['_STATUSTYPE']._serialized_end=2445
+  _globals['_QUEUE']._serialized_start=2447
+  _globals['_QUEUE']._serialized_end=2483
+  _globals['_MODELSTATUS']._serialized_start=2485
+  _globals['_MODELSTATUS']._serialized_end=2568
+  _globals['_ROLE']._serialized_start=2570
+  _globals['_ROLE']._serialized_end=2626
+  _globals['_COMMAND']._serialized_start=2628
+  _globals['_COMMAND']._serialized_end=2702
+  _globals['_CONNECTIONSTATUS']._serialized_start=2704
+  _globals['_CONNECTIONSTATUS']._serialized_end=2777
   _globals['_RESPONSE']._serialized_start=71
   _globals['_RESPONSE']._serialized_end=129
   _globals['_STATUS']._serialized_start=132
-  _globals['_STATUS']._serialized_end=428
-  _globals['_STATUS_LOGLEVEL']._serialized_start=362
-  _globals['_STATUS_LOGLEVEL']._serialized_end=428
-  _globals['_TASKREQUEST']._serialized_start=431
-  _globals['_TASKREQUEST']._serialized_end=647
-  _globals['_MODELUPDATE']._serialized_start=650
-  _globals['_MODELUPDATE']._serialized_end=825
-  _globals['_MODELVALIDATION']._serialized_start=828
-  _globals['_MODELVALIDATION']._serialized_end=1024
-  _globals['_MODELREQUEST']._serialized_start=1027
-  _globals['_MODELREQUEST']._serialized_end=1164
-  _globals['_MODELRESPONSE']._serialized_start=1166
-  _globals['_MODELRESPONSE']._serialized_end=1259
-  _globals['_GETGLOBALMODELREQUEST']._serialized_start=1261
-  _globals['_GETGLOBALMODELREQUEST']._serialized_end=1346
-  _globals['_GETGLOBALMODELRESPONSE']._serialized_start=1348
-  _globals['_GETGLOBALMODELRESPONSE']._serialized_end=1452
-  _globals['_HEARTBEAT']._serialized_start=1454
-  _globals['_HEARTBEAT']._serialized_end=1495
-  _globals['_CLIENTAVAILABLEMESSAGE']._serialized_start=1497
-  _globals['_CLIENTAVAILABLEMESSAGE']._serialized_end=1584
-  _globals['_LISTCLIENTSREQUEST']._serialized_start=1586
-  _globals['_LISTCLIENTSREQUEST']._serialized_end=1666
-  _globals['_CLIENTLIST']._serialized_start=1668
-  _globals['_CLIENTLIST']._serialized_end=1710
-  _globals['_CLIENT']._serialized_start=1712
-  _globals['_CLIENT']._serialized_end=1760
-  _globals['_REASSIGNREQUEST']._serialized_start=1762
-  _globals['_REASSIGNREQUEST']._serialized_end=1871
-  _globals['_RECONNECTREQUEST']._serialized_start=1873
-  _globals['_RECONNECTREQUEST']._serialized_end=1972
-  _globals['_PARAMETER']._serialized_start=1974
-  _globals['_PARAMETER']._serialized_end=2013
-  _globals['_CONTROLREQUEST']._serialized_start=2015
-  _globals['_CONTROLREQUEST']._serialized_end=2099
-  _globals['_CONTROLRESPONSE']._serialized_start=2101
-  _globals['_CONTROLRESPONSE']._serialized_end=2171
-  _globals['_CONNECTIONREQUEST']._serialized_start=2173
-  _globals['_CONNECTIONREQUEST']._serialized_end=2192
-  _globals['_CONNECTIONRESPONSE']._serialized_start=2194
-  _globals['_CONNECTIONRESPONSE']._serialized_end=2254
-  _globals['_MODELSERVICE']._serialized_start=2723
-  _globals['_MODELSERVICE']._serialized_end=2845
-  _globals['_CONTROL']._serialized_start=2848
-  _globals['_CONTROL']._serialized_end=3096
-  _globals['_REDUCER']._serialized_start=3098
-  _globals['_REDUCER']._serialized_end=3184
-  _globals['_CONNECTOR']._serialized_start=3187
-  _globals['_CONNECTOR']._serialized_end=3614
-  _globals['_COMBINER']._serialized_start=3617
-  _globals['_COMBINER']._serialized_end=3808
+  _globals['_STATUS']._serialized_end=448
+  _globals['_STATUS_LOGLEVEL']._serialized_start=382
+  _globals['_STATUS_LOGLEVEL']._serialized_end=448
+  _globals['_TASKREQUEST']._serialized_start=451
+  _globals['_TASKREQUEST']._serialized_end=667
+  _globals['_MODELUPDATE']._serialized_start=670
+  _globals['_MODELUPDATE']._serialized_end=861
+  _globals['_MODELVALIDATION']._serialized_start=864
+  _globals['_MODELVALIDATION']._serialized_end=1080
+  _globals['_MODELREQUEST']._serialized_start=1083
+  _globals['_MODELREQUEST']._serialized_end=1220
+  _globals['_MODELRESPONSE']._serialized_start=1222
+  _globals['_MODELRESPONSE']._serialized_end=1315
+  _globals['_GETGLOBALMODELREQUEST']._serialized_start=1317
+  _globals['_GETGLOBALMODELREQUEST']._serialized_end=1402
+  _globals['_GETGLOBALMODELRESPONSE']._serialized_start=1404
+  _globals['_GETGLOBALMODELRESPONSE']._serialized_end=1508
+  _globals['_HEARTBEAT']._serialized_start=1510
+  _globals['_HEARTBEAT']._serialized_end=1551
+  _globals['_CLIENTAVAILABLEMESSAGE']._serialized_start=1553
+  _globals['_CLIENTAVAILABLEMESSAGE']._serialized_end=1640
+  _globals['_LISTCLIENTSREQUEST']._serialized_start=1642
+  _globals['_LISTCLIENTSREQUEST']._serialized_end=1722
+  _globals['_CLIENTLIST']._serialized_start=1724
+  _globals['_CLIENTLIST']._serialized_end=1766
+  _globals['_CLIENT']._serialized_start=1768
+  _globals['_CLIENT']._serialized_end=1816
+  _globals['_REASSIGNREQUEST']._serialized_start=1818
+  _globals['_REASSIGNREQUEST']._serialized_end=1927
+  _globals['_RECONNECTREQUEST']._serialized_start=1929
+  _globals['_RECONNECTREQUEST']._serialized_end=2028
+  _globals['_PARAMETER']._serialized_start=2030
+  _globals['_PARAMETER']._serialized_end=2069
+  _globals['_CONTROLREQUEST']._serialized_start=2071
+  _globals['_CONTROLREQUEST']._serialized_end=2155
+  _globals['_CONTROLRESPONSE']._serialized_start=2157
+  _globals['_CONTROLRESPONSE']._serialized_end=2227
+  _globals['_CONNECTIONREQUEST']._serialized_start=2229
+  _globals['_CONNECTIONREQUEST']._serialized_end=2248
+  _globals['_CONNECTIONRESPONSE']._serialized_start=2250
+  _globals['_CONNECTIONRESPONSE']._serialized_end=2310
+  _globals['_MODELSERVICE']._serialized_start=2779
+  _globals['_MODELSERVICE']._serialized_end=2901
+  _globals['_CONTROL']._serialized_start=2904
+  _globals['_CONTROL']._serialized_end=3152
+  _globals['_REDUCER']._serialized_start=3154
+  _globals['_REDUCER']._serialized_end=3240
+  _globals['_CONNECTOR']._serialized_start=3243
+  _globals['_CONNECTOR']._serialized_end=3670
+  _globals['_COMBINER']._serialized_start=3673
+  _globals['_COMBINER']._serialized_end=3864
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fedn-0.8.0/fedn/network/grpc/fedn_pb2_grpc.py` & `fedn-0.9.0b1/fedn/network/grpc/fedn_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Upload = channel.stream_unary(
-                '/grpc.ModelService/Upload',
+                '/fedn.ModelService/Upload',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelResponse.FromString,
                 )
         self.Download = channel.unary_stream(
-                '/grpc.ModelService/Download',
+                '/fedn.ModelService/Download',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelResponse.FromString,
                 )
 
 
 class ModelServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -52,15 +52,15 @@
             'Download': grpc.unary_stream_rpc_method_handler(
                     servicer.Download,
                     request_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelRequest.FromString,
                     response_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'grpc.ModelService', rpc_method_handlers)
+            'fedn.ModelService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ModelService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -71,15 +71,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/grpc.ModelService/Upload',
+        return grpc.experimental.stream_unary(request_iterator, target, '/fedn.ModelService/Upload',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Download(request,
@@ -88,15 +88,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/grpc.ModelService/Download',
+        return grpc.experimental.unary_stream(request, target, '/fedn.ModelService/Download',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class ControlStub(object):
@@ -105,30 +105,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Start = channel.unary_unary(
-                '/grpc.Control/Start',
+                '/fedn.Control/Start',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
                 )
         self.Stop = channel.unary_unary(
-                '/grpc.Control/Stop',
+                '/fedn.Control/Stop',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
                 )
         self.FlushAggregationQueue = channel.unary_unary(
-                '/grpc.Control/FlushAggregationQueue',
+                '/fedn.Control/FlushAggregationQueue',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
                 )
         self.SetAggregator = channel.unary_unary(
-                '/grpc.Control/SetAggregator',
+                '/fedn.Control/SetAggregator',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
                 )
 
 
 class ControlServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -178,15 +178,15 @@
             'SetAggregator': grpc.unary_unary_rpc_method_handler(
                     servicer.SetAggregator,
                     request_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.FromString,
                     response_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'grpc.Control', rpc_method_handlers)
+            'fedn.Control', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Control(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -197,15 +197,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Control/Start',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Control/Start',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Stop(request,
@@ -214,15 +214,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Control/Stop',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Control/Stop',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def FlushAggregationQueue(request,
@@ -231,15 +231,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Control/FlushAggregationQueue',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Control/FlushAggregationQueue',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SetAggregator(request,
@@ -248,15 +248,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Control/SetAggregator',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Control/SetAggregator',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ControlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class ReducerStub(object):
@@ -265,15 +265,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetGlobalModel = channel.unary_unary(
-                '/grpc.Reducer/GetGlobalModel',
+                '/fedn.Reducer/GetGlobalModel',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelResponse.FromString,
                 )
 
 
 class ReducerServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -290,15 +290,15 @@
             'GetGlobalModel': grpc.unary_unary_rpc_method_handler(
                     servicer.GetGlobalModel,
                     request_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelRequest.FromString,
                     response_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'grpc.Reducer', rpc_method_handlers)
+            'fedn.Reducer', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Reducer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -309,15 +309,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Reducer/GetGlobalModel',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Reducer/GetGlobalModel',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.GetGlobalModelResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class ConnectorStub(object):
@@ -326,45 +326,45 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.AllianceStatusStream = channel.unary_stream(
-                '/grpc.Connector/AllianceStatusStream',
+                '/fedn.Connector/AllianceStatusStream',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientAvailableMessage.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Status.FromString,
                 )
         self.SendStatus = channel.unary_unary(
-                '/grpc.Connector/SendStatus',
+                '/fedn.Connector/SendStatus',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Status.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
         self.ListActiveClients = channel.unary_unary(
-                '/grpc.Connector/ListActiveClients',
+                '/fedn.Connector/ListActiveClients',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ListClientsRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientList.FromString,
                 )
         self.AcceptingClients = channel.unary_unary(
-                '/grpc.Connector/AcceptingClients',
+                '/fedn.Connector/AcceptingClients',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ConnectionRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ConnectionResponse.FromString,
                 )
         self.SendHeartbeat = channel.unary_unary(
-                '/grpc.Connector/SendHeartbeat',
+                '/fedn.Connector/SendHeartbeat',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Heartbeat.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
         self.ReassignClient = channel.unary_unary(
-                '/grpc.Connector/ReassignClient',
+                '/fedn.Connector/ReassignClient',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ReassignRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
         self.ReconnectClient = channel.unary_unary(
-                '/grpc.Connector/ReconnectClient',
+                '/fedn.Connector/ReconnectClient',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ReconnectRequest.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
 
 
 class ConnectorServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -452,15 +452,15 @@
             'ReconnectClient': grpc.unary_unary_rpc_method_handler(
                     servicer.ReconnectClient,
                     request_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ReconnectRequest.FromString,
                     response_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'grpc.Connector', rpc_method_handlers)
+            'fedn.Connector', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Connector(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -471,15 +471,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/grpc.Connector/AllianceStatusStream',
+        return grpc.experimental.unary_stream(request, target, '/fedn.Connector/AllianceStatusStream',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientAvailableMessage.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendStatus(request,
@@ -488,15 +488,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/SendStatus',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/SendStatus',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Status.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListActiveClients(request,
@@ -505,15 +505,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/ListActiveClients',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/ListActiveClients',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ListClientsRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AcceptingClients(request,
@@ -522,15 +522,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/AcceptingClients',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/AcceptingClients',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ConnectionRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ConnectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendHeartbeat(request,
@@ -539,15 +539,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/SendHeartbeat',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/SendHeartbeat',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Heartbeat.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ReassignClient(request,
@@ -556,15 +556,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/ReassignClient',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/ReassignClient',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ReassignRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ReconnectClient(request,
@@ -573,15 +573,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Connector/ReconnectClient',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Connector/ReconnectClient',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ReconnectRequest.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class CombinerStub(object):
@@ -590,25 +590,25 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.TaskStream = channel.unary_stream(
-                '/grpc.Combiner/TaskStream',
+                '/fedn.Combiner/TaskStream',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientAvailableMessage.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.TaskRequest.FromString,
                 )
         self.SendModelUpdate = channel.unary_unary(
-                '/grpc.Combiner/SendModelUpdate',
+                '/fedn.Combiner/SendModelUpdate',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelUpdate.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
         self.SendModelValidation = channel.unary_unary(
-                '/grpc.Combiner/SendModelValidation',
+                '/fedn.Combiner/SendModelValidation',
                 request_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelValidation.SerializeToString,
                 response_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
                 )
 
 
 class CombinerServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -648,15 +648,15 @@
             'SendModelValidation': grpc.unary_unary_rpc_method_handler(
                     servicer.SendModelValidation,
                     request_deserializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelValidation.FromString,
                     response_serializer=fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'grpc.Combiner', rpc_method_handlers)
+            'fedn.Combiner', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Combiner(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -667,15 +667,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/grpc.Combiner/TaskStream',
+        return grpc.experimental.unary_stream(request, target, '/fedn.Combiner/TaskStream',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ClientAvailableMessage.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.TaskRequest.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendModelUpdate(request,
@@ -684,15 +684,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Combiner/SendModelUpdate',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Combiner/SendModelUpdate',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelUpdate.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendModelValidation(request,
@@ -701,12 +701,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/grpc.Combiner/SendModelValidation',
+        return grpc.experimental.unary_unary(request, target, '/fedn.Combiner/SendModelValidation',
             fedn_dot_network_dot_grpc_dot_fedn__pb2.ModelValidation.SerializeToString,
             fedn_dot_network_dot_grpc_dot_fedn__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `fedn-0.8.0/fedn/network/grpc/server.py` & `fedn-0.9.0b1/fedn/network/grpc/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import grpc
 from grpc_health.v1 import health, health_pb2_grpc
 
 import fedn.network.grpc.fedn_pb2_grpc as rpc
 from fedn.common.log_config import (logger, set_log_level_from_string,
                                     set_log_stream)
+from fedn.network.grpc.auth import JWTInterceptor
 
 
 class Server:
     """ Class for configuring and launching the gRPC server."""
 
     def __init__(self, servicer, modelservicer, config):
 
         set_log_level_from_string(config.get('verbosity', "INFO"))
         set_log_stream(config.get('logfile', None))
 
-        self.server = grpc.server(futures.ThreadPoolExecutor(max_workers=350))
+        self.server = grpc.server(futures.ThreadPoolExecutor(max_workers=350), interceptors=[JWTInterceptor()])
         self.certificate = None
         self.health_servicer = health.HealthServicer()
 
         if isinstance(servicer, rpc.CombinerServicer):
             rpc.add_CombinerServicer_to_server(servicer, self.server)
         if isinstance(servicer, rpc.ConnectorServicer):
             rpc.add_ConnectorServicer_to_server(servicer, self.server)
@@ -36,15 +37,15 @@
         if config['secure']:
             logger.info(f'Creating secure gRPCS server using certificate: {config["certificate"]}')
             server_credentials = grpc.ssl_server_credentials(
                 ((config['key'], config['certificate'],),))
             self.server.add_secure_port(
                 '[::]:' + str(config['port']), server_credentials)
         else:
-            logger.info("Creating insecure gRPC server")
+            logger.info("Creating gRPC server")
             self.server.add_insecure_port('[::]:' + str(config['port']))
 
     def start(self):
         """ Start the gRPC server."""
         logger.info("gRPC Server started")
         self.server.start()
```

### Comparing `fedn-0.8.0/fedn/network/loadbalancer/firstavailable.py` & `fedn-0.9.0b1/fedn/network/loadbalancer/firstavailable.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/loadbalancer/leastpacked.py` & `fedn-0.9.0b1/fedn/network/loadbalancer/leastpacked.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/state.py` & `fedn-0.9.0b1/fedn/network/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/storage/models/memorymodelstorage.py` & `fedn-0.9.0b1/fedn/network/storage/models/memorymodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/storage/models/modelstorage.py` & `fedn-0.9.0b1/fedn/network/storage/models/modelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/storage/models/tempmodelstorage.py` & `fedn-0.9.0b1/fedn/network/storage/models/tempmodelstorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from io import BytesIO
 
 import fedn.network.grpc.fedn_pb2 as fedn
+from fedn.common.log_config import logger
 from fedn.network.storage.models.modelstorage import ModelStorage
 
 CHUNK_SIZE = 1024 * 1024
 
 
 class TempModelStorage(ModelStorage):
     """ Class for managing local temporary models on file on combiners."""
@@ -26,18 +27,18 @@
             return True
         return False
 
     def get(self, model_id):
 
         try:
             if self.models_metadata[model_id] != fedn.ModelStatus.OK:
-                print("File not ready! Try again", flush=True)
+                logger.warning("File not ready! Try again")
                 return None
         except KeyError:
-            print("No such model have been made available yet!", flush=True)
+            logger.error("No such model has been made available yet!")
             return None
 
         obj = BytesIO()
         with open(os.path.join(self.default_dir, str(model_id)), 'rb') as f:
             obj.write(f.read())
 
         obj.seek(0, 0)
@@ -70,33 +71,33 @@
         self.models_metadata.update({model_id: model_metadata})
 
     # Delete model from disk
     def delete(self, model_id):
 
         try:
             os.remove(os.path.join(self.default_dir, str(model_id)))
-            print("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id), flush=True)
+            logger.info("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id))
             # Delete id from metadata and models dict
             del self.models_metadata[model_id]
             del self.models[model_id]
         except FileNotFoundError:
-            print("Could not delete model from disk. File not found!", flush=True)
+            logger.error("Could not delete model from disk. File not found!")
             return False
         return True
 
     # Delete all models from disk
     def delete_all(self):
 
         ids_pop = []
         for model_id in self.models.keys():
             try:
                 os.remove(os.path.join(self.default_dir, str(model_id)))
-                print("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id), flush=True)
+                logger.info("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id))
                 # Add id to list of ids to pop/delete from metadata and models dict
                 ids_pop.append(model_id)
             except FileNotFoundError:
-                print("TEMPMODELSTORAGE: Could not delete model {} from disk. File not found!".format(model_id), flush=True)
+                logger.error("TEMPMODELSTORAGE: Could not delete model {} from disk. File not found!".format(model_id))
         # Remove id from metadata and models dict
         for model_id in ids_pop:
             del self.models_metadata[model_id]
             del self.models[model_id]
         return True
```

### Comparing `fedn-0.8.0/fedn/network/storage/s3/base.py` & `fedn-0.9.0b1/fedn/network/storage/s3/base.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/storage/s3/miniorepository.py` & `fedn-0.9.0b1/fedn/network/storage/s3/miniorepository.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
                                 secret_key=config['storage_secret_key'],
                                 secure=config['storage_secure_mode'], http_client=manager)
         else:
             self.client = Minio("{0}:{1}".format(config['storage_hostname'], config['storage_port']),
                                 access_key=config['storage_access_key'],
                                 secret_key=config['storage_secret_key'],
                                 secure=config['storage_secure_mode'])
-            logger.warning(
-                "S3/MINIO RUNNING IN **INSECURE** MODE!")
 
     def set_artifact(self, instance_name, instance, bucket, is_file=False):
 
         if is_file:
             self.client.fput_object(bucket, instance_name, instance)
         else:
             try:
```

### Comparing `fedn-0.8.0/fedn/network/storage/s3/repository.py` & `fedn-0.9.0b1/fedn/network/storage/s3/repository.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/network/storage/statestore/mongostatestore.py` & `fedn-0.9.0b1/fedn/network/storage/statestore/mongostatestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import uuid
 from datetime import datetime
 
 import pymongo
 from google.protobuf.json_format import MessageToDict
 
+from fedn.common.log_config import logger
 from fedn.network.state import ReducerStateToString, StringToReducerState
 
 
 class MongoStateStore:
     """Statestore implementation using MongoDB.
 
     :param network_id: The network id.
@@ -44,15 +45,15 @@
             self.validations = self.control["validations"]
 
             # Logging
             self.status = self.control["status"]
 
             self.__inited = True
         except Exception as e:
-            print("FAILED TO CONNECT TO MONGODB, {}".format(e), flush=True)
+            logger.error("FAILED TO CONNECT TO MONGODB, {}".format(e))
             self.state = None
             self.model = None
             self.control = None
             self.network = None
             self.combiners = None
             self.clients = None
             raise
@@ -120,15 +121,15 @@
         if old_state != state:
             return self.state.update_one(
                 {"state": "current_state"},
                 {"$set": {"state": ReducerStateToString(state)}},
                 True,
             )
         else:
-            print(
+            logger.info(
                 "Not updating state, already in {}".format(
                     ReducerStateToString(state)
                 )
             )
 
     def get_sessions(self, limit=None, skip=None, sort_key="_id", sort_order=pymongo.DESCENDING):
         """Get all sessions.
@@ -274,15 +275,15 @@
 
                 self.model.update_one(
                     {"key": "current_model"}, {"$set": {"model": model_id, "committed_at": committed_at, "session_id": None}}, True
                 )
 
                 return True
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error("ERROR: {}".format(e))
 
         return False
 
     def get_latest_round(self):
         """Get the id of the most recent round.
 
         :return: The id of the most recent round.
@@ -345,15 +346,15 @@
             doc["key"] = "active"
 
             self.control.package.replace_one(
                 {"key": "active"}, doc
             )
 
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error("ERROR: {}".format(e))
             return False
 
         return True
 
     def set_compute_package(self, file_name: str, storage_file_name: str, helper_type: str, name: str = None, description: str = None):
         """Set the active compute package in statestore.
 
@@ -396,15 +397,15 @@
         try:
 
             find = {"key": "active"}
             projection = {"key": False, "_id": False}
             ret = self.control.package.find_one(find, projection)
             return ret
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error("ERROR: {}".format(e))
             return None
 
     def list_compute_packages(self, limit: int = None, skip: int = None, sort_key="committed_at", sort_order=pymongo.DESCENDING):
         """List compute packages in the statestore (paginated).
 
         :param limit: The maximum number of compute packages to return.
         :type limit: int
@@ -429,15 +430,15 @@
                 result = self.control.package.find(find_option, projection).limit(limit).skip(skip).sort(sort_key, sort_order)
             else:
                 result = self.control.package.find(find_option, projection).sort(sort_key, sort_order)
 
             count = self.control.package.count_documents(find_option)
 
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error("ERROR: {}".format(e))
             return None
 
         return {
             "result": result or [],
             "count": count or 0,
         }
 
@@ -776,17 +777,16 @@
         :param combiner: name of combiner to delete.
         :type combiner: str
         :return:
         """
         try:
             self.combiners.delete_one({"name": combiner})
         except Exception:
-            print(
-                "WARNING, failed to delete combiner: {}".format(combiner),
-                flush=True,
+            logger.error(
+                "Failed to delete combiner: {}".format(combiner),
             )
 
     def set_client(self, client_data):
         """Set client in statestore.
 
         :param client_data: dictionary of client config.
         :type client_data: dict
@@ -839,15 +839,15 @@
                 result = self.clients.find(find, projection).limit(limit).skip(skip).sort(sort_key, sort_order)
             else:
                 result = self.clients.find(find, projection).sort(sort_key, sort_order)
 
             count = self.clients.count_documents(find)
 
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error("{}".format(e))
 
         return {
             "result": result,
             "count": count,
         }
 
     def list_combiners_data(self, combiners, sort_key="count", sort_order=pymongo.DESCENDING):
@@ -875,15 +875,15 @@
                 {"$group": {"_id": "$combiner", "count": {"$sum": 1}}},
                 {"$sort": {sort_key: sort_order, "_id": pymongo.ASCENDING}}
             ]
 
             result = self.clients.aggregate(pipeline)
 
         except Exception as e:
-            print("ERROR: {}".format(e), flush=True)
+            logger.error(e)
 
         return result
 
     def report_status(self, msg):
         """Write status message to the database.
 
         :param msg: The status message.
```

### Comparing `fedn-0.8.0/fedn/network/storage/statestore/statestorebase.py` & `fedn-0.9.0b1/fedn/network/storage/statestore/statestorebase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/utils/helpers/helperbase.py` & `fedn-0.9.0b1/fedn/utils/helpers/helperbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/utils/helpers/helpers.py` & `fedn-0.9.0b1/fedn/utils/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/utils/helpers/plugins/androidhelper.py` & `fedn-0.9.0b1/fedn/utils/helpers/plugins/androidhelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import struct
 import tempfile
 
 import numpy as np
 
+from fedn.common.log_config import logger
 from fedn.utils.helpers.helperbase import HelperBase
 
 
 class Helper(HelperBase):
     """FEDn helper class for android json model weights."""
 
     def __init__(self):
@@ -82,15 +83,15 @@
 
     def load(self, fh):
         """Load weights from file or filelike.
 
         :param fh: file path, filehandle, filelike.
         :return: List of weights in json format.
         """
-        print("in android helper load")
+        logger.debug("in android helper load")
         if isinstance(fh, str):
             with open(fh, "rb") as file:
                 byte_data = file.read()
         else:
             byte_data = fh.read()
 
         weights = np.array(struct.unpack(f'{len(byte_data) // 4}f', byte_data))
```

### Comparing `fedn-0.8.0/fedn/utils/helpers/plugins/numpyhelper.py` & `fedn-0.9.0b1/fedn/utils/helpers/plugins/numpyhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.8.0/fedn/utils/plots.py` & `fedn-0.9.0b1/fedn/utils/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 
 import numpy
 import plotly
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
+from fedn.common.log_config import logger
 from fedn.network.storage.statestore.mongostatestore import MongoStateStore
 
 
 class Plot:
     """
 
     """
@@ -23,15 +24,15 @@
             self.status = self.mdb['control.status']
             self.round_time = self.mdb["control.round_time"]
             self.combiner_round_time = self.mdb["control.combiner_round_time"]
             self.psutil_usage = self.mdb["control.psutil_monitoring"]
             self.network_clients = self.mdb["network.clients"]
 
         except Exception as e:
-            print("FAILED TO CONNECT TO MONGO, {}".format(e), flush=True)
+            logger.error("FAILED TO CONNECT TO MONGO, {}".format(e))
             self.collection = None
             raise
 
     # plot metrics from DB
     def _scalar_metrics(self, metrics):
         """ Extract all scalar valued metrics from a MODEL_VALIDATON. """
```

### Comparing `fedn-0.8.0/fedn.egg-info/SOURCES.txt` & `fedn-0.9.0b1/fedn.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,30 @@
 fedn/common/certificate/certificate.py
 fedn/common/certificate/certificatemanager.py
 fedn/common/net/__init__.py
 fedn/network/__init__.py
 fedn/network/config.py
 fedn/network/state.py
 fedn/network/api/__init__.py
+fedn/network/api/auth.py
 fedn/network/api/client.py
 fedn/network/api/interface.py
 fedn/network/api/network.py
 fedn/network/api/server.py
 fedn/network/api/tests.py
+fedn/network/api/v1/__init__.py
+fedn/network/api/v1/client_routes.py
+fedn/network/api/v1/combiner_routes.py
+fedn/network/api/v1/model_routes.py
+fedn/network/api/v1/package_routes.py
+fedn/network/api/v1/round_routes.py
+fedn/network/api/v1/session_routes.py
+fedn/network/api/v1/shared.py
+fedn/network/api/v1/status_routes.py
+fedn/network/api/v1/validation_routes.py
 fedn/network/clients/__init__.py
 fedn/network/clients/client.py
 fedn/network/clients/connect.py
 fedn/network/clients/package.py
 fedn/network/clients/state.py
 fedn/network/clients/test_client.py
 fedn/network/combiner/__init__.py
@@ -48,14 +59,15 @@
 fedn/network/combiner/aggregators/aggregatorbase.py
 fedn/network/combiner/aggregators/fedavg.py
 fedn/network/combiner/aggregators/fedopt.py
 fedn/network/controller/__init__.py
 fedn/network/controller/control.py
 fedn/network/controller/controlbase.py
 fedn/network/grpc/__init__.py
+fedn/network/grpc/auth.py
 fedn/network/grpc/fedn_pb2.py
 fedn/network/grpc/fedn_pb2_grpc.py
 fedn/network/grpc/server.py
 fedn/network/loadbalancer/__init__.py
 fedn/network/loadbalancer/firstavailable.py
 fedn/network/loadbalancer/leastpacked.py
 fedn/network/loadbalancer/loadbalancerbase.py
@@ -67,19 +79,32 @@
 fedn/network/storage/s3/__init__.py
 fedn/network/storage/s3/base.py
 fedn/network/storage/s3/miniorepository.py
 fedn/network/storage/s3/repository.py
 fedn/network/storage/statestore/__init__.py
 fedn/network/storage/statestore/mongostatestore.py
 fedn/network/storage/statestore/statestorebase.py
-fedn/tests/__init__.py
+fedn/network/storage/statestore/stores/__init__.py
+fedn/network/storage/statestore/stores/client_store.py
+fedn/network/storage/statestore/stores/combiner_store.py
+fedn/network/storage/statestore/stores/model_store.py
+fedn/network/storage/statestore/stores/package_store.py
+fedn/network/storage/statestore/stores/round_store.py
+fedn/network/storage/statestore/stores/session_store.py
+fedn/network/storage/statestore/stores/shared.py
+fedn/network/storage/statestore/stores/status_store.py
+fedn/network/storage/statestore/stores/store.py
+fedn/network/storage/statestore/stores/validation_store.py
 fedn/utils/__init__.py
 fedn/utils/checksum.py
 fedn/utils/dispatcher.py
+fedn/utils/environment.py
 fedn/utils/plots.py
 fedn/utils/process.py
+fedn/utils/flowercompat/__init__.py
+fedn/utils/flowercompat/client_app_adapter.py
 fedn/utils/helpers/__init__.py
 fedn/utils/helpers/helperbase.py
 fedn/utils/helpers/helpers.py
 fedn/utils/helpers/plugins/__init__.py
 fedn/utils/helpers/plugins/androidhelper.py
 fedn/utils/helpers/plugins/numpyhelper.py
```

### Comparing `fedn-0.8.0/setup.py` & `fedn-0.9.0b1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from setuptools import find_packages, setup
 
 setup(
     name='fedn',
-    version='0.8.0',
+    version='0.9.0b1',
     description="""Scaleout Federated Learning""",
     author='Scaleout Systems AB',
     author_email='contact@scaleoutsystems.com',
     url='https://www.scaleoutsystems.com',
     py_modules=['fedn'],
-    python_requires='>=3.8,<3.11',
+    python_requires='>=3.8,<3.12',
     install_requires=[
-        "PyYAML>=5.4",
         "requests",
         "urllib3>=1.26.4",
         "minio",
-        "python-slugify",
-        "grpcio~=1.57.0",
-        "grpcio-tools~=1.57.0",
+        "grpcio~=1.60.0",
+        "grpcio-tools~=1.60.0",
         "numpy>=1.21.6",
-        "protobuf",
+        "protobuf~=4.25.2",
         "pymongo",
         "Flask",
-        "Flask-WTF",
         "pyjwt",
         "pyopenssl",
-        "ttictoc",
         "psutil",
         "click==8.0.1",
-        "jinja2",
+        "grpcio-health-checking~=1.60.0",
+        "flasgger==0.9.5",
         "plotly",
-        "pandas",
-        "bokeh<3.0.0",
-        "networkx",
-        "grpcio-health-checking~=1.57.0"
+        "virtualenv",
     ],
+    extras_require={
+        'flower': ["flwr==1.8.0"]
+    },
     license='Apache 2.0',
     zip_safe=False,
     entry_points={
         'console_scripts': ["fedn=cli:main"]
     },
     keywords='Federated learning',
     packages=find_packages(exclude=["tests", "tests.*"]),
     classifiers=[
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

