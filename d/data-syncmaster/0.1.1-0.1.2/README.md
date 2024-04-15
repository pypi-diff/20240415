# Comparing `tmp/data_syncmaster-0.1.1.tar.gz` & `tmp/data_syncmaster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_syncmaster-0.1.1.tar", max compression
+gzip compressed data, was "data_syncmaster-0.1.2.tar", max compression
```

## Comparing `data_syncmaster-0.1.1.tar` & `data_syncmaster-0.1.2.tar`

### file list

```diff
@@ -1,110 +1,108 @@
--rw-r--r--   0        0        0    11426 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2325 2024-03-29 12:16:48.740619 data_syncmaster-0.1.1/README.rst
--rw-r--r--   0        0        0     6950 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      247 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/__init__.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/__init__.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/__init__.py
--rw-r--r--   0        0        0      273 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/deps.py
--rw-r--r--   0        0        0      261 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/monitoring.py
--rw-r--r--   0        0        0      349 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/router.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/v1/__init__.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/v1/auth/__init__.py
--rw-r--r--   0        0        0     1302 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/v1/auth/router.py
--rw-r--r--   0        0        0      900 2024-03-29 12:15:50.944471 data_syncmaster-0.1.1/syncmaster/backend/api/v1/auth/utils.py
--rw-r--r--   0        0        0     9815 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/connections.py
--rw-r--r--   0        0        0     7086 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/groups.py
--rw-r--r--   0        0        0     4620 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/queue.py
--rw-r--r--   0        0        0      818 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/router.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/transfers/__init__.py
--rw-r--r--   0        0        0    16672 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/transfers/router.py
--rw-r--r--   0        0        0      877 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/transfers/utils.py
--rw-r--r--   0        0        0     2907 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/api/v1/users.py
--rw-r--r--   0        0        0      632 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/export_openapi_schema.py
--rw-r--r--   0        0        0     7042 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/handler.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/logger.py
--rw-r--r--   0        0        0     1970 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/main.py
--rw-r--r--   0        0        0     2660 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/pre_start.py
--rw-r--r--   0        0        0      234 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/services/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/services/auth.py
--rw-r--r--   0        0        0     1285 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/backend/services/unit_of_work.py
--rw-r--r--   0        0        0     3066 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/config.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/__init__.py
--rw-r--r--   0        0        0      664 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/alembic.ini
--rw-r--r--   0        0        0      975 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/base.py
--rw-r--r--   0        0        0     1049 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/factory.py
--rw-r--r--   0        0        0       58 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/README
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/__init__.py
--rw-r--r--   0        0        0     2258 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/env.py
--rw-r--r--   0        0        0      510 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/script.py.mako
--rw-r--r--   0        0        0    12132 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/versions/2023-11-23_478240cdad4b_init.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1112 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/mixins.py
--rw-r--r--   0        0        0     6349 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/models.py
--rw-r--r--   0        0        0      855 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/__init__.py
--rw-r--r--   0        0        0     4216 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/base.py
--rw-r--r--   0        0        0     4640 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/connection.py
--rw-r--r--   0        0        0     3138 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/credentials_repository.py
--rw-r--r--   0        0        0     8131 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/group.py
--rw-r--r--   0        0        0     6124 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/queue.py
--rw-r--r--   0        0        0     3476 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/repository_with_owner.py
--rw-r--r--   0        0        0     3001 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/run.py
--rw-r--r--   0        0        0     7320 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/transfer.py
--rw-r--r--   0        0        0     2799 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/user.py
--rw-r--r--   0        0        0      576 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/repositories/utils.py
--rw-r--r--   0        0        0      958 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/db/utils.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/dto/__init__.py
--rw-r--r--   0        0        0     1094 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/dto/connections.py
--rw-r--r--   0        0        0      909 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/dto/transfers.py
--rw-r--r--   0        0        0      309 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/__init__.py
--rw-r--r--   0        0        0      254 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/base.py
--rw-r--r--   0        0        0      628 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/connection.py
--rw-r--r--   0        0        0      274 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/credentials.py
--rw-r--r--   0        0        0      514 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/group.py
--rw-r--r--   0        0        0      424 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/queue.py
--rw-r--r--   0        0        0      573 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/run.py
--rw-r--r--   0        0        0      954 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/transfer.py
--rw-r--r--   0        0        0      269 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/exceptions/user.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/__init__.py
--rw-r--r--   0        0        0     1516 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/__init__.py
--rw-r--r--   0        0        0      267 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/auth.py
--rw-r--r--   0        0        0      275 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connection_types.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/__init__.py
--rw-r--r--   0        0        0     4760 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/connection.py
--rw-r--r--   0        0        0      908 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/hdfs.py
--rw-r--r--   0        0        0      852 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/hive.py
--rw-r--r--   0        0        0     1589 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/oracle.py
--rw-r--r--   0        0        0     1184 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/postgres.py
--rw-r--r--   0        0        0     1664 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/s3.py
--rw-r--r--   0        0        0      223 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/file_formats.py
--rw-r--r--   0        0        0      839 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/groups.py
--rw-r--r--   0        0        0     1061 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/page.py
--rw-r--r--   0        0        0      826 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/queue.py
--rw-r--r--   0        0        0      375 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/status.py
--rw-r--r--   0        0        0      197 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfer_types.py
--rw-r--r--   0        0        0     5596 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/__init__.py
--rw-r--r--   0        0        0      554 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/db.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/__init__.py
--rw-r--r--   0        0        0     1638 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/base.py
--rw-r--r--   0        0        0      682 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/hdfs.py
--rw-r--r--   0        0        0      664 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/s3.py
--rw-r--r--   0        0        0      655 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file_format.py
--rw-r--r--   0        0        0      769 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/run.py
--rw-r--r--   0        0        0      364 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/strategy.py
--rw-r--r--   0        0        0      162 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/types.py
--rw-r--r--   0        0        0     2255 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/schemas/v1/users.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/__init__.py
--rw-r--r--   0        0        0      414 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/base.py
--rw-r--r--   0        0        0      476 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/config.py
--rw-r--r--   0        0        0     3820 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/controller.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/__init__.py
--rw-r--r--   0        0        0     1571 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/base.py
--rw-r--r--   0        0        0       99 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/file/__init__.py
--rw-r--r--   0        0        0     1884 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/file/base.py
--rw-r--r--   0        0        0      400 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/file/hdfs.py
--rw-r--r--   0        0        0      742 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/file/s3.py
--rw-r--r--   0        0        0     1305 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/hive.py
--rw-r--r--   0        0        0     1669 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/oracle.py
--rw-r--r--   0        0        0     1641 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/handlers/postgres.py
--rw-r--r--   0        0        0     3127 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/spark.py
--rw-r--r--   0        0        0     3102 2024-03-29 12:15:50.948470 data_syncmaster-0.1.1/syncmaster/worker/transfer.py
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 data_syncmaster-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11426 2024-04-15 10:27:55.872874 data_syncmaster-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2332 2024-04-15 10:28:59.080360 data_syncmaster-0.1.2/README.rst
+-rw-r--r--   0        0        0     6952 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      247 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/__init__.py
+-rw-r--r--   0        0        0     1811 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/__init__.py
+-rwxr-xr-x   0        0        0      814 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/__main__.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/deps.py
+-rw-r--r--   0        0        0      261 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/monitoring.py
+-rw-r--r--   0        0        0      349 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/router.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/auth/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/auth/router.py
+-rw-r--r--   0        0        0      900 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/auth/utils.py
+-rw-r--r--   0        0        0     9815 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/connections.py
+-rw-r--r--   0        0        0     7086 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/groups.py
+-rw-r--r--   0        0        0     4620 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/queue.py
+-rw-r--r--   0        0        0      818 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/router.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/transfers/__init__.py
+-rw-r--r--   0        0        0    16672 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/transfers/router.py
+-rw-r--r--   0        0        0      877 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/transfers/utils.py
+-rw-r--r--   0        0        0     2907 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/api/v1/users.py
+-rw-r--r--   0        0        0      635 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/export_openapi_schema.py
+-rw-r--r--   0        0        0     7042 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/handler.py
+-rw-r--r--   0        0        0      234 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/services/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/services/auth.py
+-rw-r--r--   0        0        0     1285 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/backend/services/unit_of_work.py
+-rw-r--r--   0        0        0     3066 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/config.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/base.py
+-rw-r--r--   0        0        0     1049 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/factory.py
+-rw-r--r--   0        0        0       58 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/README
+-rwxr-xr-x   0        0        0      868 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/__main__.py
+-rw-r--r--   0        0        0      670 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/alembic.ini
+-rw-r--r--   0        0        0     2404 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/env.py
+-rw-r--r--   0        0        0      510 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/script.py.mako
+-rw-r--r--   0        0        0    12132 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/versions/2023-11-23_478240cdad4b_init.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/mixins.py
+-rw-r--r--   0        0        0     6349 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/models.py
+-rw-r--r--   0        0        0      855 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/__init__.py
+-rw-r--r--   0        0        0     4216 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/base.py
+-rw-r--r--   0        0        0     4640 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/connection.py
+-rw-r--r--   0        0        0     3138 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/credentials_repository.py
+-rw-r--r--   0        0        0     8131 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/group.py
+-rw-r--r--   0        0        0     6124 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/queue.py
+-rw-r--r--   0        0        0     3476 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/repository_with_owner.py
+-rw-r--r--   0        0        0     3001 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/run.py
+-rw-r--r--   0        0        0     7320 2024-04-15 10:27:55.876874 data_syncmaster-0.1.2/syncmaster/db/repositories/transfer.py
+-rw-r--r--   0        0        0     2799 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/db/repositories/user.py
+-rw-r--r--   0        0        0      576 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/db/repositories/utils.py
+-rw-r--r--   0        0        0      958 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/db/utils.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/dto/__init__.py
+-rw-r--r--   0        0        0     1094 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/dto/connections.py
+-rw-r--r--   0        0        0      909 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/dto/transfers.py
+-rw-r--r--   0        0        0      309 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/__init__.py
+-rw-r--r--   0        0        0      254 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/base.py
+-rw-r--r--   0        0        0      628 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/connection.py
+-rw-r--r--   0        0        0      274 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/credentials.py
+-rw-r--r--   0        0        0      514 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/group.py
+-rw-r--r--   0        0        0      424 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/queue.py
+-rw-r--r--   0        0        0      573 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/run.py
+-rw-r--r--   0        0        0      954 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/transfer.py
+-rw-r--r--   0        0        0      269 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/exceptions/user.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/__init__.py
+-rw-r--r--   0        0        0     1516 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/auth.py
+-rw-r--r--   0        0        0      275 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connection_types.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/__init__.py
+-rw-r--r--   0        0        0     4760 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/connection.py
+-rw-r--r--   0        0        0      908 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/hdfs.py
+-rw-r--r--   0        0        0      852 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/hive.py
+-rw-r--r--   0        0        0     1589 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/oracle.py
+-rw-r--r--   0        0        0     1184 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/postgres.py
+-rw-r--r--   0        0        0     1664 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/s3.py
+-rw-r--r--   0        0        0      223 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/file_formats.py
+-rw-r--r--   0        0        0      839 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/groups.py
+-rw-r--r--   0        0        0     1061 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/page.py
+-rw-r--r--   0        0        0      826 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/queue.py
+-rw-r--r--   0        0        0      375 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/status.py
+-rw-r--r--   0        0        0      197 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfer_types.py
+-rw-r--r--   0        0        0     5596 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/__init__.py
+-rw-r--r--   0        0        0      554 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/db.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/__init__.py
+-rw-r--r--   0        0        0     1638 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/base.py
+-rw-r--r--   0        0        0      682 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/hdfs.py
+-rw-r--r--   0        0        0      664 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/s3.py
+-rw-r--r--   0        0        0      655 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file_format.py
+-rw-r--r--   0        0        0      769 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/run.py
+-rw-r--r--   0        0        0      364 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/strategy.py
+-rw-r--r--   0        0        0      162 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/types.py
+-rw-r--r--   0        0        0     2255 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/schemas/v1/users.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/base.py
+-rw-r--r--   0        0        0      476 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/config.py
+-rw-r--r--   0        0        0     3820 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/controller.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/__init__.py
+-rw-r--r--   0        0        0     1571 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/base.py
+-rw-r--r--   0        0        0       99 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/file/__init__.py
+-rw-r--r--   0        0        0     1884 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/file/base.py
+-rw-r--r--   0        0        0      400 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/file/hdfs.py
+-rw-r--r--   0        0        0      742 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/file/s3.py
+-rw-r--r--   0        0        0     1305 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/hive.py
+-rw-r--r--   0        0        0     1669 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/oracle.py
+-rw-r--r--   0        0        0     1641 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/handlers/postgres.py
+-rw-r--r--   0        0        0     3127 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/spark.py
+-rw-r--r--   0        0        0     3102 2024-04-15 10:27:55.880874 data_syncmaster-0.1.2/syncmaster/worker/transfer.py
+-rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 data_syncmaster-0.1.2/PKG-INFO
```

### Comparing `data_syncmaster-0.1.1/LICENSE.txt` & `data_syncmaster-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/README.rst` & `data_syncmaster-0.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     :target: https://pypi.org/project/data-syncmaster/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/data-syncmaster.svg
     :target: https://github.com/MobileTeleSystems/syncmaster/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/data-syncmaster.svg
     :target: https://badge.fury.io/py/data-syncmaster
 .. |Docker image| image:: https://img.shields.io/docker/v/mtsrus/syncmaster-backend?sort=semver&label=docker
     :target: https://hub.docker.com/r/mtsrus/syncmaster-backend
-.. |Documentation| image:: https://readthedocs.org/projects/data-syncmaster/badge/?version=stable
+.. |Documentation| image:: https://readthedocs.org/projects/syncmaster/badge/?version=stable
     :target: https://syncmaster.readthedocs.io
-.. |Build Status| image:: https://github.com/MobileTeleSystems/syncmaster/workflows/Tests/badge.svg
+.. |Build Status| image:: https://github.com/MobileTeleSystems/syncmaster/workflows/Run%20All%20Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/syncmaster/actions
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/syncmaster/graph/badge.svg?token=ky7UyUxolB
     :target: https://codecov.io/gh/MobileTeleSystems/syncmaster
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/syncmaster/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/syncmaster/develop
```

### Comparing `data_syncmaster-0.1.1/pyproject.toml` & `data_syncmaster-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-syncmaster"
-version = "0.1.1"
+version = "0.1.2"
 license = "Apache-2.0"
 description = "Syncmaster REST API + Worker"
 authors = ["DataOps.ETL <onetools@mts.ru>"]
 readme = "README.rst"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Pydantic",
@@ -193,14 +193,16 @@
   "if log.isEnabledFor(logging.DEBUG):",
   "if sys.version_info",
   "@(abc\\.)?abstractmethod",
   "\\.\\.\\.",
   "def downgrade\\(\\)",
 ]
 
+
+
 [tool.poetry.group.docs.dependencies]
 autodoc-pydantic = {version = "^2.0.1", python = ">=3.8"}
 numpydoc = {version = "^1.6.0", python = ">=3.8"}
 sphinx = [
   {version = "^7.1.2", python = ">=3.8"},
   {version = "^7.2.6", python = ">=3.9"},
 ]
```

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/auth/router.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/auth/router.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/auth/utils.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/auth/utils.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/connections.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/connections.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/groups.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/groups.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/queue.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/queue.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/router.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/router.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/transfers/router.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/transfers/router.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/transfers/utils.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/transfers/utils.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/api/v1/users.py` & `data_syncmaster-0.1.2/syncmaster/backend/api/v1/users.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/export_openapi_schema.py` & `data_syncmaster-0.1.2/syncmaster/backend/export_openapi_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import json
 import sys
 
 from fastapi import FastAPI
 
-from syncmaster.backend.main import get_application
+from syncmaster.backend import application_factory
 from syncmaster.config import Settings
 
 
 def get_openapi_schema(app: FastAPI) -> dict:
     return app.openapi()
 
 
 if __name__ == "__main__":
     settings = Settings()
-    app = get_application(settings)
+    app = application_factory(settings)
     schema = get_openapi_schema(app)
     file_path = sys.argv[1]
     if not file_path:
         raise ValueError("File path not sent")
     with open(file_path, "w") as file:
         json.dump(schema, file)
```

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/handler.py` & `data_syncmaster-0.1.2/syncmaster/backend/handler.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/main.py` & `data_syncmaster-0.1.2/syncmaster/backend/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
-import uvicorn
 from fastapi import FastAPI, HTTPException
 from starlette.middleware.cors import CORSMiddleware
 
 from syncmaster.backend.api.deps import (
     AuthMarker,
     DatabaseEngineMarker,
     DatabaseSessionMarker,
@@ -18,15 +17,15 @@
 )
 from syncmaster.backend.services import get_auth_scheme
 from syncmaster.config import Settings
 from syncmaster.db.factory import create_engine, create_session_factory, get_uow
 from syncmaster.exceptions import SyncmasterError
 
 
-def get_application(settings: Settings) -> FastAPI:
+def application_factory(settings: Settings) -> FastAPI:
     application = FastAPI(
         title=settings.PROJECT_NAME,
         debug=settings.DEBUG,
     )
     application.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
@@ -51,13 +50,7 @@
             DatabaseSessionMarker: lambda: session_factory,
             UnitOfWorkMarker: get_uow(session_factory, settings),
             AuthMarker: auth_scheme,
         }
     )
 
     return application
-
-
-if __name__ == "__main__":
-    settings = Settings()
-    app = get_application(settings=settings)
-    uvicorn.run(app, host="0.0.0.0", port=8000)
```

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/services/auth.py` & `data_syncmaster-0.1.2/syncmaster/backend/services/auth.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/backend/services/unit_of_work.py` & `data_syncmaster-0.1.2/syncmaster/backend/services/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/config.py` & `data_syncmaster-0.1.2/syncmaster/config.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/alembic.ini` & `data_syncmaster-0.1.2/syncmaster/db/migrations/alembic.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [alembic]
-script_location = %(here)s/migrations
+script_location = %(here)s
 file_template = %%(year)d-%%(month).2d-%%(day).2d_%%(rev)s_%%(slug)s
-prepend_sys_path = .
+prepend_sys_path = %(here)s/../../../
 version_path_separator = os
 
 [post_write_hooks]
 
 [loggers]
 keys = root,sqlalchemy,alembic
```

### Comparing `data_syncmaster-0.1.1/syncmaster/db/base.py` & `data_syncmaster-0.1.2/syncmaster/db/base.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/factory.py` & `data_syncmaster-0.1.2/syncmaster/db/factory.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/migrations/env.py` & `data_syncmaster-0.1.2/syncmaster/db/migrations/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 config = context.config
 
 
 if config.config_file_name is not None:
     fileConfig(config.config_file_name)
 
-config.set_main_option("sqlalchemy.url", Settings().build_db_connection_uri())
+if not config.get_main_option("sqlalchemy.url"):
+    # read application settings only if sqlalchemy.url is not being passed via cli arguments
+    config.set_main_option("sqlalchemy.url", Settings().build_db_connection_uri())
 
 target_metadata = (
     Base.metadata,
     ResultModelBase.metadata,
 )
```

### Comparing `data_syncmaster-0.1.1/syncmaster/db/migrations/versions/2023-11-23_478240cdad4b_init.py` & `data_syncmaster-0.1.2/syncmaster/db/migrations/versions/2023-11-23_478240cdad4b_init.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/mixins.py` & `data_syncmaster-0.1.2/syncmaster/db/mixins.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/models.py` & `data_syncmaster-0.1.2/syncmaster/db/models.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/__init__.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/base.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/base.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/connection.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/connection.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/credentials_repository.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/credentials_repository.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/group.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/group.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/queue.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/queue.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/repository_with_owner.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/repository_with_owner.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/run.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/run.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/transfer.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/transfer.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/user.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/user.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/repositories/utils.py` & `data_syncmaster-0.1.2/syncmaster/db/repositories/utils.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/db/utils.py` & `data_syncmaster-0.1.2/syncmaster/db/utils.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/dto/connections.py` & `data_syncmaster-0.1.2/syncmaster/dto/connections.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/dto/transfers.py` & `data_syncmaster-0.1.2/syncmaster/dto/transfers.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/exceptions/connection.py` & `data_syncmaster-0.1.2/syncmaster/exceptions/connection.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/exceptions/group.py` & `data_syncmaster-0.1.2/syncmaster/exceptions/group.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/exceptions/run.py` & `data_syncmaster-0.1.2/syncmaster/exceptions/run.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/exceptions/transfer.py` & `data_syncmaster-0.1.2/syncmaster/exceptions/transfer.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/__init__.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/connection.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/connection.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/hdfs.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/hdfs.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/hive.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/hive.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/oracle.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/oracle.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/postgres.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/postgres.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/connections/s3.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/connections/s3.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/groups.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/groups.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/page.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/page.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/queue.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/queue.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/__init__.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/db.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/db.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/base.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/base.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/hdfs.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file/s3.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file/s3.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/file_format.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/file_format.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/transfers/run.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/transfers/run.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/schemas/v1/users.py` & `data_syncmaster-0.1.2/syncmaster/schemas/v1/users.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/controller.py` & `data_syncmaster-0.1.2/syncmaster/worker/controller.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/base.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/base.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/file/base.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/file/base.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/file/s3.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/file/s3.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/hive.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/hive.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/oracle.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/oracle.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/handlers/postgres.py` & `data_syncmaster-0.1.2/syncmaster/worker/handlers/postgres.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/spark.py` & `data_syncmaster-0.1.2/syncmaster/worker/spark.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/syncmaster/worker/transfer.py` & `data_syncmaster-0.1.2/syncmaster/worker/transfer.py`

 * *Files identical despite different names*

### Comparing `data_syncmaster-0.1.1/PKG-INFO` & `data_syncmaster-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-syncmaster
-Version: 0.1.1
+Version: 0.1.2
 Summary: Syncmaster REST API + Worker
 License: Apache-2.0
 Keywords: Syncmaster,REST,API,Worker,Replication
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -62,17 +62,17 @@
     :target: https://pypi.org/project/data-syncmaster/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/data-syncmaster.svg
     :target: https://github.com/MobileTeleSystems/syncmaster/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/data-syncmaster.svg
     :target: https://badge.fury.io/py/data-syncmaster
 .. |Docker image| image:: https://img.shields.io/docker/v/mtsrus/syncmaster-backend?sort=semver&label=docker
     :target: https://hub.docker.com/r/mtsrus/syncmaster-backend
-.. |Documentation| image:: https://readthedocs.org/projects/data-syncmaster/badge/?version=stable
+.. |Documentation| image:: https://readthedocs.org/projects/syncmaster/badge/?version=stable
     :target: https://syncmaster.readthedocs.io
-.. |Build Status| image:: https://github.com/MobileTeleSystems/syncmaster/workflows/Tests/badge.svg
+.. |Build Status| image:: https://github.com/MobileTeleSystems/syncmaster/workflows/Run%20All%20Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/syncmaster/actions
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/syncmaster/graph/badge.svg?token=ky7UyUxolB
     :target: https://codecov.io/gh/MobileTeleSystems/syncmaster
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/syncmaster/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/syncmaster/develop
```

