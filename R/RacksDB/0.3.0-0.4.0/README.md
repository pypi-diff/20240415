# Comparing `tmp/RacksDB-0.3.0.tar.gz` & `tmp/racksdb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RacksDB-0.3.0.tar", last modified: Mon Jan 22 11:45:46 2024, max compression
+gzip compressed data, was "racksdb-0.4.0.tar", last modified: Mon Apr 15 12:34:07 2024, max compression
```

## Comparing `RacksDB-0.3.0.tar` & `racksdb-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.802559 RacksDB-0.3.0/
--rw-rw-r--   0 remi      (1000) remi      (1000)    35149 2022-11-18 14:56:05.000000 RacksDB-0.3.0/LICENSE
--rw-r--r--   0 remi      (1000) remi      (1000)     5415 2024-01-22 11:45:46.802559 RacksDB-0.3.0/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)     4412 2024-01-11 20:38:19.000000 RacksDB-0.3.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.802559 RacksDB-0.3.0/RacksDB.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)     5415 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)     1523 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)      105 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/entry_points.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       52 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        8 2024-01-22 11:45:46.000000 RacksDB-0.3.0/RacksDB.egg-info/top_level.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)     1719 2024-01-22 11:09:25.000000 RacksDB-0.3.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.794558 RacksDB-0.3.0/racksdb/
--rw-rw-r--   0 remi      (1000) remi      (1000)     2315 2024-01-20 22:09:55.000000 RacksDB-0.3.0/racksdb/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     3798 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/bases.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.798558 RacksDB-0.3.0/racksdb/drawers/
--rw-rw-r--   0 remi      (1000) remi      (1000)      244 2023-11-01 10:09:45.000000 RacksDB-0.3.0/racksdb/drawers/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     3726 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/drawers/base.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.798558 RacksDB-0.3.0/racksdb/drawers/dtypes/
--rw-rw-r--   0 remi      (1000) remi      (1000)      528 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/drawers/dtypes/hexcolor.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     9386 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/drawers/infrastructure.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     1375 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/drawers/parameters.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     5714 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/drawers/room.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.798558 RacksDB-0.3.0/racksdb/dtypes/
--rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-07-12 12:41:09.000000 RacksDB-0.3.0/racksdb/dtypes/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      550 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/angle.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      622 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/dtypes/bits.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      628 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/dtypes/bytes.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      541 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/dimension.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      388 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/netif_type.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      371 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/rack_height.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      660 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/rack_width.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      384 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/dtypes/storage_type.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      557 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/dtypes/watts.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      157 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     8508 2023-11-13 09:36:04.000000 RacksDB-0.3.0/racksdb/exec.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.798558 RacksDB-0.3.0/racksdb/generic/
--rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-22 14:52:55.000000 RacksDB-0.3.0/racksdb/generic/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)    25580 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/generic/db.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      557 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/generic/definedtype.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.798558 RacksDB-0.3.0/racksdb/generic/dumpers/
--rw-rw-r--   0 remi      (1000) remi      (1000)      883 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/generic/dumpers/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     1022 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/generic/dumpers/_common.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      756 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/generic/dumpers/console.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     4133 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/generic/dumpers/json.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     5302 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/generic/dumpers/yaml.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      338 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/generic/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)    11451 2024-01-22 10:07:36.000000 RacksDB-0.3.0/racksdb/generic/openapi.py
--rw-rw-r--   0 remi      (1000) remi      (1000)    13271 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/generic/schema.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     4370 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/generic/views.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.802559 RacksDB-0.3.0/racksdb/tests/
--rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/tests/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      802 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/tests/test_defined_type_hexcolor.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      893 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/tests/test_defined_type_watts.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     5785 2024-01-20 22:09:55.000000 RacksDB-0.3.0/racksdb/tests/test_drawer.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     7355 2023-10-31 09:24:03.000000 RacksDB-0.3.0/racksdb/tests/test_schema.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      843 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/tests/test_schema_defined_type_loader.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     3263 2024-01-20 22:09:55.000000 RacksDB-0.3.0/racksdb/tests/tests_db_load.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      219 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/version.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     5499 2023-11-09 08:50:19.000000 RacksDB-0.3.0/racksdb/views.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.802559 RacksDB-0.3.0/racksdb/web/
--rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-03 08:22:27.000000 RacksDB-0.3.0/racksdb/web/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     8096 2024-01-22 10:07:36.000000 RacksDB-0.3.0/racksdb/web/app.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.794558 RacksDB-0.3.0/racksdb/web/ui/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.794558 RacksDB-0.3.0/racksdb/web/ui/node_modules/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.794558 RacksDB-0.3.0/racksdb/web/ui/node_modules/flatted/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-01-22 11:45:46.802559 RacksDB-0.3.0/racksdb/web/ui/node_modules/flatted/python/
--rw-rw-r--   0 remi      (1000) remi      (1000)     3879 2023-12-13 10:15:50.000000 RacksDB-0.3.0/racksdb/web/ui/node_modules/flatted/python/flatted.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     2129 2023-12-13 10:15:50.000000 RacksDB-0.3.0/racksdb/web/ui/node_modules/flatted/python/test.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-01-22 11:45:46.802559 RacksDB-0.3.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/
+-rw-rw-r--   0 remi      (1000) remi      (1000)    35149 2022-11-18 14:56:05.000000 racksdb-0.4.0/LICENSE
+-rw-r--r--   0 remi      (1000) remi      (1000)     5665 2024-04-15 12:34:07.392875 racksdb-0.4.0/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4568 2024-04-15 08:02:57.000000 racksdb-0.4.0/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/RacksDB.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)     5665 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1601 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      105 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/entry_points.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       87 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        8 2024-04-15 12:34:07.000000 racksdb-0.4.0/RacksDB.egg-info/top_level.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1449 2024-04-15 08:22:34.000000 racksdb-0.4.0/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.384874 racksdb-0.4.0/racksdb/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2714 2024-04-12 13:51:54.000000 racksdb-0.4.0/racksdb/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5075 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/bases.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.388875 racksdb-0.4.0/racksdb/drawers/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      244 2023-11-01 10:09:45.000000 racksdb-0.4.0/racksdb/drawers/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6121 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/base.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.388875 racksdb-0.4.0/racksdb/drawers/coordinates/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      475 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/coordinates/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      209 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/coordinates/base.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      408 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/coordinates/json.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      407 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/coordinates/yaml.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.388875 racksdb-0.4.0/racksdb/drawers/dtypes/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/dtypes/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      703 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/dtypes/hexcolor.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    21919 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/infrastructure.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1375 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/drawers/parameters.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7871 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/drawers/room.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.388875 racksdb-0.4.0/racksdb/dtypes/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-07-12 12:41:09.000000 racksdb-0.4.0/racksdb/dtypes/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      550 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/angle.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      622 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/dtypes/bits.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      628 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/dtypes/bytes.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      541 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/dimension.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      388 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/netif_type.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      371 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/rack_height.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      660 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/rack_width.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      384 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/dtypes/storage_type.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      557 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/dtypes/watts.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      320 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     9516 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/exec.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/racksdb/generic/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-22 14:52:55.000000 racksdb-0.4.0/racksdb/generic/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    27193 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/db.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      557 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/generic/definedtype.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/racksdb/generic/dumpers/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      883 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/generic/dumpers/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1022 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/generic/dumpers/_common.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      756 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/generic/dumpers/console.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3564 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/dumpers/json.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4705 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/dumpers/yaml.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      338 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/generic/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    11452 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/openapi.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    13429 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/schema.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6649 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/generic/views.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/racksdb/tests/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/tests/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      834 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/tests/test_defined_type_hexcolor.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      893 2023-11-09 08:50:19.000000 racksdb-0.4.0/racksdb/tests/test_defined_type_watts.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5819 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/tests/test_drawer.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7355 2023-10-31 09:24:03.000000 racksdb-0.4.0/racksdb/tests/test_schema.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      843 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/tests/test_schema_defined_type_loader.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3263 2024-02-08 08:40:05.000000 racksdb-0.4.0/racksdb/tests/tests_db_load.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      219 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/version.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6879 2024-04-08 14:39:01.000000 racksdb-0.4.0/racksdb/views.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-15 12:34:07.392875 racksdb-0.4.0/racksdb/web/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-03 08:22:27.000000 racksdb-0.4.0/racksdb/web/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    11194 2024-04-12 13:51:54.000000 racksdb-0.4.0/racksdb/web/app.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-15 12:34:07.392875 racksdb-0.4.0/setup.cfg
```

### Comparing `RacksDB-0.3.0/LICENSE` & `racksdb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/PKG-INFO` & `racksdb-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RacksDB
-Version: 0.3.0
+Version: 0.4.0
 Summary: Modelize your datacenters infrastructures in YAML database
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RacksDB
 Project-URL: Bug Tracker, https://github.com/rackslab/RacksDB/issues
 Keywords: cmdb,inventory,yaml,datacenters,racks,hpc,cluster
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,17 +16,20 @@
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML
 Requires-Dist: ClusterShell
 Requires-Dist: pycairo
+Requires-Dist: PyGObject
+Provides-Extra: dev
+Requires-Dist: Flask-Cors; extra == "dev"
 Provides-Extra: web
 Requires-Dist: Flask; extra == "web"
-Requires-Dist: Flask-Cors; extra == "web"
+Requires-Dist: requests-toolbelt; extra == "web"
 
 <img
   src="assets/bitmaps/logo_full_white_medium.png"
   alt="RacksDB Overview"
   align="right"
   width="200px"
   style="margin: 20px;">
@@ -49,17 +52,16 @@
 * **Monitoring**: Synchronize monitoring services with equipments database and
   define dynamic dashboard.
 * **Documentation**: Get updated architecture diagrams and define generic
   adaptative procedures.
 
 <p align="center">
   <img
-    src="docs/modules/overview/images/racksdb_overview.svg"
+    src="docs/modules/overview/images/racksdb_overview.png"
     alt="RacksDB Overview"
-    width="600px"
     style="margin: 0 auto;">
 </p>
 
 Generally speaking, **RacksDB** is a specialized
 [CMDB](https://en.wikipedia.org/wiki/Configuration_management_database)
 dedicated to
 [DCIM](https://en.wikipedia.org/wiki/Data_center_management#Data_center_infrastructure_management).
@@ -81,15 +83,23 @@
 * **Extensibility.** In addition to RacksDB simple format, custom schema
   extensions can be defined to store specific data.
 
 RacksDB provides multiple interfaces to request the database with its
 [CLI tool](https://docs.rackslab.io/racksdb/usage/racksdb.html), a
 [Python library](https://docs.rackslab.io/racksdb/usage/lib.html), a
 [REST API](https://docs.rackslab.io/racksdb/usage/rest.html) and a
-[Web UI](racksdb/web/ui/README.md) (in _beta_).
+[Web UI](https://docs.rackslab.io/racksdb/usage/ui.html).
+
+<p align="center">
+<img
+  src="assets/screenshots/assemblies/bitmaps/screenshots-small.webp"
+  alt="RacksDB web UI"
+  width="600px"
+  style="margin: 0 auto;">
+<p>
 
 For more details, read the
 [full description](https://docs.rackslab.io/racksdb/overview/overview.html)
 of RacksDB.
 
 ## Status
```

### Comparing `RacksDB-0.3.0/README.md` & `racksdb-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 * **Monitoring**: Synchronize monitoring services with equipments database and
   define dynamic dashboard.
 * **Documentation**: Get updated architecture diagrams and define generic
   adaptative procedures.
 
 <p align="center">
   <img
-    src="docs/modules/overview/images/racksdb_overview.svg"
+    src="docs/modules/overview/images/racksdb_overview.png"
     alt="RacksDB Overview"
-    width="600px"
     style="margin: 0 auto;">
 </p>
 
 Generally speaking, **RacksDB** is a specialized
 [CMDB](https://en.wikipedia.org/wiki/Configuration_management_database)
 dedicated to
 [DCIM](https://en.wikipedia.org/wiki/Data_center_management#Data_center_infrastructure_management).
@@ -55,15 +54,23 @@
 * **Extensibility.** In addition to RacksDB simple format, custom schema
   extensions can be defined to store specific data.
 
 RacksDB provides multiple interfaces to request the database with its
 [CLI tool](https://docs.rackslab.io/racksdb/usage/racksdb.html), a
 [Python library](https://docs.rackslab.io/racksdb/usage/lib.html), a
 [REST API](https://docs.rackslab.io/racksdb/usage/rest.html) and a
-[Web UI](racksdb/web/ui/README.md) (in _beta_).
+[Web UI](https://docs.rackslab.io/racksdb/usage/ui.html).
+
+<p align="center">
+<img
+  src="assets/screenshots/assemblies/bitmaps/screenshots-small.webp"
+  alt="RacksDB web UI"
+  width="600px"
+  style="margin: 0 auto;">
+<p>
 
 For more details, read the
 [full description](https://docs.rackslab.io/racksdb/overview/overview.html)
 of RacksDB.
 
 ## Status
```

### Comparing `RacksDB-0.3.0/RacksDB.egg-info/PKG-INFO` & `racksdb-0.4.0/RacksDB.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RacksDB
-Version: 0.3.0
+Version: 0.4.0
 Summary: Modelize your datacenters infrastructures in YAML database
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RacksDB
 Project-URL: Bug Tracker, https://github.com/rackslab/RacksDB/issues
 Keywords: cmdb,inventory,yaml,datacenters,racks,hpc,cluster
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,17 +16,20 @@
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML
 Requires-Dist: ClusterShell
 Requires-Dist: pycairo
+Requires-Dist: PyGObject
+Provides-Extra: dev
+Requires-Dist: Flask-Cors; extra == "dev"
 Provides-Extra: web
 Requires-Dist: Flask; extra == "web"
-Requires-Dist: Flask-Cors; extra == "web"
+Requires-Dist: requests-toolbelt; extra == "web"
 
 <img
   src="assets/bitmaps/logo_full_white_medium.png"
   alt="RacksDB Overview"
   align="right"
   width="200px"
   style="margin: 20px;">
@@ -49,17 +52,16 @@
 * **Monitoring**: Synchronize monitoring services with equipments database and
   define dynamic dashboard.
 * **Documentation**: Get updated architecture diagrams and define generic
   adaptative procedures.
 
 <p align="center">
   <img
-    src="docs/modules/overview/images/racksdb_overview.svg"
+    src="docs/modules/overview/images/racksdb_overview.png"
     alt="RacksDB Overview"
-    width="600px"
     style="margin: 0 auto;">
 </p>
 
 Generally speaking, **RacksDB** is a specialized
 [CMDB](https://en.wikipedia.org/wiki/Configuration_management_database)
 dedicated to
 [DCIM](https://en.wikipedia.org/wiki/Data_center_management#Data_center_infrastructure_management).
@@ -81,15 +83,23 @@
 * **Extensibility.** In addition to RacksDB simple format, custom schema
   extensions can be defined to store specific data.
 
 RacksDB provides multiple interfaces to request the database with its
 [CLI tool](https://docs.rackslab.io/racksdb/usage/racksdb.html), a
 [Python library](https://docs.rackslab.io/racksdb/usage/lib.html), a
 [REST API](https://docs.rackslab.io/racksdb/usage/rest.html) and a
-[Web UI](racksdb/web/ui/README.md) (in _beta_).
+[Web UI](https://docs.rackslab.io/racksdb/usage/ui.html).
+
+<p align="center">
+<img
+  src="assets/screenshots/assemblies/bitmaps/screenshots-small.webp"
+  alt="RacksDB web UI"
+  width="600px"
+  style="margin: 0 auto;">
+<p>
 
 For more details, read the
 [full description](https://docs.rackslab.io/racksdb/overview/overview.html)
 of RacksDB.
 
 ## Status
```

### Comparing `RacksDB-0.3.0/RacksDB.egg-info/SOURCES.txt` & `racksdb-0.4.0/RacksDB.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 racksdb/version.py
 racksdb/views.py
 racksdb/drawers/__init__.py
 racksdb/drawers/base.py
 racksdb/drawers/infrastructure.py
 racksdb/drawers/parameters.py
 racksdb/drawers/room.py
+racksdb/drawers/coordinates/__init__.py
+racksdb/drawers/coordinates/base.py
+racksdb/drawers/coordinates/json.py
+racksdb/drawers/coordinates/yaml.py
+racksdb/drawers/dtypes/__init__.py
 racksdb/drawers/dtypes/hexcolor.py
 racksdb/dtypes/__init__.py
 racksdb/dtypes/angle.py
 racksdb/dtypes/bits.py
 racksdb/dtypes/bytes.py
 racksdb/dtypes/dimension.py
 racksdb/dtypes/netif_type.py
@@ -45,10 +50,8 @@
 racksdb/tests/test_defined_type_hexcolor.py
 racksdb/tests/test_defined_type_watts.py
 racksdb/tests/test_drawer.py
 racksdb/tests/test_schema.py
 racksdb/tests/test_schema_defined_type_loader.py
 racksdb/tests/tests_db_load.py
 racksdb/web/__init__.py
-racksdb/web/app.py
-racksdb/web/ui/node_modules/flatted/python/flatted.py
-racksdb/web/ui/node_modules/flatted/python/test.py
+racksdb/web/app.py
```

### Comparing `RacksDB-0.3.0/pyproject.toml` & `racksdb-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RacksDB"
-version = "0.3.0"
+version = "0.4.0"
 description = "Modelize your datacenters infrastructures in YAML database"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["cmdb", "inventory", "yaml", "datacenters", "racks", "hpc", "cluster"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
 dependencies = [
     "PyYAML",
     "ClusterShell",
     "pycairo",
+    "PyGObject",
 ]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: System Administrators",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Database :: Database Engines/Servers",
     "Topic :: System :: Clustering",
     "Topic :: System :: Systems Administration",
 ]
 
 [project.optional-dependencies]
+dev = [
+    "Flask-Cors",
+]
 web = [
     "Flask",
-    "Flask-Cors",
+    "requests-toolbelt",
 ]
 
 [project.scripts]
 racksdb = "racksdb.exec:RacksDBExec.run"
 racksdb-web = "racksdb.web.app:RacksDBWebApp.run"
 
 [tool.setuptools.packages.find]
 include = ["racksdb*"]
-exclude = ["racksdb.web.ui*"]
 
 [project.urls]
 "Homepage" = "https://github.com/rackslab/RacksDB"
 "Bug Tracker" = "https://github.com/rackslab/RacksDB/issues"
 
-# Do not automatically install all files in package tree as data files. This is
-# especially required for files under UI folder that could be could considered
-# data files even though they are explicitely excluded from packages search
-# paths.
-[tool.setuptools]
-include-package-data = false
-
 [tool.black]
 target-version = ['py36']
 color = 1
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
```

### Comparing `RacksDB-0.3.0/racksdb/__init__.py` & `racksdb-0.4.0/racksdb/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from pathlib import Path
 from typing import Union
 
 from .generic.schema import Schema, SchemaFileLoader, SchemaDefinedTypeLoader
 from .generic.db import GenericDB, DBDict, DBList, DBSplittedFilesLoader
+from .generic.errors import DBSchemaError, DBFormatError
+from .errors import RacksDBFormatError, RacksDBSchemaError
 from . import bases
 
 
 class RacksDB(GenericDB):
 
     DEFAULT_DB = "/var/lib/racksdb"
     DEFAULT_SCHEMA = "/usr/share/racksdb/schemas/racksdb.yml"
     DEFAULT_EXT = "/etc/racksdb/extensions.yml"
+    DEFAULT_UI = "/usr/share/racksdb/frontend"
     PREFIX = "RacksDB"
     DEFINED_TYPES_MODULE = "racksdb.dtypes"
 
     def __init__(self, schema, loader):
         super().__init__(self.PREFIX, schema, bases)
         self._loader = loader
 
@@ -61,14 +64,20 @@
             ext = Path(cls.DEFAULT_EXT)
         elif isinstance(ext, str):
             ext = Path(ext)
         if db is None:
             db = Path(cls.DEFAULT_DB)
         elif isinstance(db, str):
             db = Path(db)
-        _schema = Schema(
-            SchemaFileLoader(schema, ext),
-            SchemaDefinedTypeLoader(cls.DEFINED_TYPES_MODULE),
-        )
-        _db = cls(_schema, DBSplittedFilesLoader(db))
-        super(cls, _db).load(_db._loader)
+        try:
+            _schema = Schema(
+                SchemaFileLoader(schema, ext),
+                SchemaDefinedTypeLoader(cls.DEFINED_TYPES_MODULE),
+            )
+        except DBSchemaError as err:
+            raise RacksDBSchemaError(str(err)) from err
+        try:
+            _db = cls(_schema, DBSplittedFilesLoader(db))
+            super(cls, _db).load(_db._loader)
+        except DBFormatError as err:
+            raise RacksDBFormatError(str(err)) from err
         return _db
```

### Comparing `RacksDB-0.3.0/racksdb/bases.py` & `racksdb-0.4.0/racksdb/bases.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 # Copyright (c) 2022-2023 Rackslab
 #
 # This file is part of RacksDB.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
+import math
+
+try:
+    from functools import cached_property
+except ImportError:
+    # For Python 3.[6-7] compatibility. The dependency to cached_property
+    # external library is not declared in pyproject.toml, it is added
+    # explicitely in packages codes only for distributions stuck with these old
+    # versions of Python.
+    #
+    # This try/except block can be removed when support of Python < 3.8 is
+    # dropped in RacksDB.
+    from cached_property import cached_property
+
 from .generic.db import DBList, DBDict
 
 
 class RacksDBDatacenterBase:
     def _filter(self, name=None, tags=None):
         # filter by name
         if name is not None and name != self.name:
@@ -39,26 +53,41 @@
         if tags is not None:
             for tag in tags:
                 if tag not in self.tags:
                     return False
         return True
 
 
-class RacksDBNodeBase:
+class RacksDBGenericEquipment:
     @property
     def tags(self):
         result = DBList()
         for tag in getattr(self._parent, "tags", []):
             result.append(tag)
-        # RacksDBNodeBase loaded tags are renamed with loaded prefix to avoid
-        # conflict with this property.
+        # RacksDB{Node,StorageEquipment,NetworkEquipment,MiscEquipment} loaded tags are
+        # renamed with loaded prefix to avoid conflict with this property.
         for tag in getattr(self, f"{self.LOADED_PREFIX}tags", []):
-            result.append(tag)
+            # Avoid duplicate tags that could be defined on both parent part and
+            # equipment.
+            if tag not in result:
+                result.append(tag)
         return result
 
+    @cached_property
+    def position(self):
+        obj = self._db.create_object_by_name("EquipmentPosition")
+        obj.height = (
+            self._first.slot
+            - self.rack.type.initial
+            + math.floor((self.slot - self._first.slot) * self.type.width)
+            * self.type.height
+        )
+        obj.width = (self.slot - self._first.slot) % int(1 / self.type.width)
+        return obj
+
     def _filter(self, infrastructure=None, name=None, tags=None):
         # filter by name
         if name is not None and name != self.name:
             return False
         # filter by infrastructure name
         if infrastructure is not None and infrastructure != self.infrastructure.name:
             return False
@@ -66,18 +95,31 @@
         if tags is not None:
             for tag in tags:
                 if tag not in self.tags:
                     return False
         return True
 
 
-class RacksDBRackBase:
+class RacksDBNodeBase(RacksDBGenericEquipment):
+    pass
+
+
+class RacksDBStorageEquipmentBase(RacksDBGenericEquipment):
+    pass
 
-    COMPUTED_PROPERTIES = ["nodes", "fillrate"]
 
+class RacksDBNetworkEquipmentBase(RacksDBGenericEquipment):
+    pass
+
+
+class RacksDBMiscEquipmentBase(RacksDBGenericEquipment):
+    pass
+
+
+class RacksDBRackBase:
     def _filter(self, name=None):
         # filter by name
         if name is not None and name != self.name:
             return False
         return True
 
     @property
@@ -106,14 +148,11 @@
                 if self.name == part.rack.name:
                     for nodes in part.nodes.values():
                         result.append(nodes)
         return result
 
 
 class RacksDBRacksRowBase:
-
-    COMPUTED_PROPERTIES = ["nbracks"]
-
     @property
     def nbracks(self):
         """Return the number of racks in the row."""
         return len(self.racks)
```

### Comparing `RacksDB-0.3.0/racksdb/drawers/dtypes/hexcolor.py` & `racksdb-0.4.0/racksdb/generic/definedtype.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# Copyright (c) 2023 Rackslab
+# Copyright (c) 2022-2023 Rackslab
 #
 # This file is part of RacksDB.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import re
-from typing import Tuple
 
-from racksdb.generic.definedtype import SchemaDefinedType
+from .errors import DBFormatError
 
 
-class SchemaDefinedTypeHexcolor(SchemaDefinedType):
-
-    pattern = r"#[0-9a-fA-F]{6}"
-    native = Tuple[float, float, float]
-
-    def parse(self, value):
-        self._match(value)
-        hexrgb = re.findall("[0-9a-fA-F]{2}", value)
-        rgb = tuple(int(f"0x{_hex}", 16) / 255 for _hex in hexrgb)
-        return rgb
+class SchemaDefinedType:
+    def __init__(self):
+        self.name = self.__class__.__module__
+
+    def __str__(self):
+        return f"~{self.name}"
+
+    def _match(self, value):
+        regex = re.compile(self.pattern)
+        match = regex.match(str(value))
+        if match is None:
+            raise DBFormatError(f"Unable to match {self} pattern with value {value}")
+        return match
```

### Comparing `RacksDB-0.3.0/racksdb/drawers/parameters.py` & `racksdb-0.4.0/racksdb/drawers/parameters.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/angle.py` & `racksdb-0.4.0/racksdb/dtypes/angle.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/bits.py` & `racksdb-0.4.0/racksdb/dtypes/bits.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/bytes.py` & `racksdb-0.4.0/racksdb/dtypes/bytes.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/dimension.py` & `racksdb-0.4.0/racksdb/dtypes/dimension.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/rack_width.py` & `racksdb-0.4.0/racksdb/dtypes/rack_width.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/dtypes/watts.py` & `racksdb-0.4.0/racksdb/dtypes/watts.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/exec.py` & `racksdb-0.4.0/racksdb/exec.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from pathlib import Path
 
 from .version import get_version
 from .generic.errors import DBFormatError, DBSchemaError
 from .generic.db import (
     DBSplittedFilesLoader,
-    DBEmptyLoader,
+    DBDictsLoader,
     DBStdinLoader,
 )
 from .generic.dumpers import DBDumperFactory, SchemaDumperFactory
 from . import RacksDB
 from .drawers import InfrastructureDrawer, RoomDrawer
 from .drawers.parameters import DrawingParameters
 from .errors import RacksDBError
@@ -118,15 +118,18 @@
                     kwargs["action"] = "store_true"
                 else:
                     kwargs["nargs"] = parameter.nargs
                 if parameter.choices is not None:
                     kwargs["choices"] = parameter.choices
                 if parameter.default is not None:
                     kwargs["default"] = parameter.default
-                    kwargs["help"] += " (default: %(default)s)"
+                    if parameter.default_in_help:
+                        kwargs["help"] += " (default: %(default)s)"
+                if parameter.const is not None:
+                    kwargs["const"] = parameter.const
                 if parameter.required:
                     kwargs["required"] = True
                 if parameter.type:
                     kwargs["type"] = parameter.type
                 subparser.add_argument(*args, **kwargs)
                 subparser.set_defaults(func=getattr(self, f"_run_{action.name}"))
 
@@ -214,32 +217,58 @@
                 objects_map=view.objects_map,
                 fold=self.args.fold,
             ).dump(data)
         )
 
     def _run_draw(self):
         file = f"{self.args.name}.{self.args.format}"
+
+        # Handle coordinates opts
+        if self.args.coordinates is False:
+            coordinates_file = None
+        elif self.args.coordinates is True:
+            coordinates_file = f"coordinates.{self.args.coordinates_format}"
+        else:
+            coordinates_file = self.args.coordinates
+        coordinates_fh = (
+            open(coordinates_file, "w+") if coordinates_file is not None else None
+        )
         try:
             if self.args.parameters is None:
-                db_loader = DBEmptyLoader()
+                db_loader = DBDictsLoader()
             elif isinstance(self.args.parameters, str):
                 if self.args.parameters == "-":
                     db_loader = DBStdinLoader()
                 else:
                     db_loader = DBSplittedFilesLoader(Path(self.args.parameters))
             parameters = DrawingParameters.load(db_loader, self.args.drawings_schema)
         except DBSchemaError as err:
             logger.critical("Unable to load drawing parameters schema: %s", str(err))
             sys.exit(1)
         except DBFormatError as err:
             logger.critical("Unable to load drawing parameters: %s", str(err))
             sys.exit(1)
         if self.args.entity == "infrastructure":
             drawer = InfrastructureDrawer(
-                self.db, self.args.name, file, self.args.format, parameters
+                self.db,
+                self.args.name,
+                file,
+                self.args.format,
+                parameters,
+                coordinates_fh,
+                self.args.coordinates_format,
             )
         elif self.args.entity == "room":
             drawer = RoomDrawer(
-                self.db, self.args.name, file, self.args.format, parameters
+                self.db,
+                self.args.name,
+                file,
+                self.args.format,
+                parameters,
+                coordinates_fh,
+                self.args.coordinates_format,
             )
         drawer.draw()
         logger.info("Generated image file %s", file)
+        if self.args.coordinates:
+            logger.info("Generated coordinates file %s", coordinates_file)
+            coordinates_fh.close()
```

### Comparing `RacksDB-0.3.0/racksdb/generic/db.py` & `racksdb-0.4.0/racksdb/generic/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2022-2023 Rackslab
 #
 # This file is part of RacksDB.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
+import copy
 import logging
 
 import yaml
 from ClusterShell.NodeSet import NodeSet
 
 from .errors import DBFormatError
 from .definedtype import SchemaDefinedType
@@ -23,32 +24,39 @@
     SchemaBackReference,
     SchemaProperty,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def deepmerge(a: dict, b: dict, path=[]) -> dict:
+    """Deep-merge dict b into dict a."""
+    for key in b:
+        if key in a:
+            if isinstance(a[key], dict) and isinstance(b[key], dict):
+                deepmerge(a[key], b[key], path + [str(key)])
+            elif a[key] != b[key]:
+                raise Exception("Conflict at " + ".".join(path + [str(key)]))
+        else:
+            a[key] = b[key]
+    return a
+
+
 class DBObject:
     LOADED_PREFIX = "__loaded_"
 
     def __init__(self, db, schema):
         self._db = db
         self._schema = schema
 
     def _filter(self, **kwargs):
         """Abstract filter method, must be overriden in specialized bases module
         classes when filtering is needed."""
         return True
 
-    def _computed_props(self):
-        """Generator to iterate over the list of DBObject computed properties."""
-        if hasattr(self, "COMPUTED_PROPERTIES"):
-            for prop in self.COMPUTED_PROPERTIES:
-                yield prop
-
 
 class DBExpandableObject(DBObject):
     def _attributes(self):
         """Return the dict of stable attributes, range attribues and the pair of range
         attribute and value."""
         stable_attributes = {}
         range_attribute = None
@@ -187,17 +195,25 @@
 
 
 class DBDict(dict):
     def filter(self, **kwargs):
         """Return a copy of the current DBDict without key and values that do not match
         provided filter criteria."""
         result = DBDict()
-        for key, value in self.items():
+
+        def add_match(key, value):
             if value._filter(**kwargs):
                 result[key] = value
+
+        for key, value in self.items():
+            if isinstance(value, DBExpandableObject):
+                for idx, _expanded_value in enumerate(value.objects()):
+                    add_match(key.rangeset[idx], _expanded_value)
+            else:
+                add_match(key, value)
         return result
 
     def __iter__(self):
         for item in self.values():
             if isinstance(item, DBExpandableObject):
                 for expanded_item in item.objects():
                     yield expanded_item
@@ -229,25 +245,34 @@
         return values
 
     def first(self):
         """Return the first expanded object of the dictionnary."""
         return list(self)[0]  # list() calls __iter__()
 
 
-class DBFileLoader:
+class DBLoader:
+    """Abstract DB loader."""
+
+    def __init__(self):
+        self.path = None
+
+
+class DBFileLoader(DBLoader):
     def __init__(self, path):
+        self.path = path
         with open(path) as fh:
             try:
                 self.content = yaml.safe_load(fh)
             except yaml.composer.ComposerError as err:
                 raise DBFormatError(err)
 
 
-class DBSplittedFilesLoader:
+class DBSplittedFilesLoader(DBLoader):
     def __init__(self, path):
+        self.path = path
         # try the parent folder
         if not path.exists():
             raise DBFormatError(f"DB path {path} does not exist")
         elif path.is_file():
             if not path.name.endswith(".yml"):
                 raise DBFormatError(f"DB contains file {path} without .yml extension")
             logger.debug("Loading DB file %s", path)
@@ -260,40 +285,43 @@
             # if directory, load recursively
             self.content = {}
             for item in path.iterdir():
                 logger.debug("Loading DB directory %s", path)
                 self.content[item.stem] = DBSplittedFilesLoader(item).content
 
 
-class DBEmptyLoader:
-    """Loader that loads nothing, just define an empty database with an optional
-    initial content. It is designed to be used to load optional database files
-    when schema defines enough default values to operate or when initial data
-    is loaded by other mean."""
+class DBDictsLoader(DBLoader):
+    """Loader that loads data from an optional set of dictionaries nothing. It accepts
+    any number of dictionaries in argument, they are all deep merged consecutively. It
+    can be used to load optional database files (ie. potentially empty database) when
+    schema defines enough default values to operate or when initial data is loaded by
+    other mean."""
+
+    def __init__(self, *args):
+        self.content = {}
+        for _content in args:
+            self.content = deepmerge(copy.deepcopy(self.content), _content)
 
-    def __init__(self, initial={}):
-        self.content = initial
 
-
-class DBStdinLoader:
+class DBStdinLoader(DBLoader):
     """Load YAML database provided in program's standard input."""
 
     def __init__(self):
         try:
             self.content = yaml.safe_load(sys.stdin.read())
         except yaml.composer.ComposerError as err:
             raise DBFormatError(err)
 
 
-class DBStringLoader:
+class DBStringLoader(DBLoader):
     """Load YAML database provided in a string."""
 
-    def __init__(self, content):
+    def __init__(self, content, initial={}):
         try:
-            self.content = yaml.safe_load(content)
+            self.content = deepmerge(initial, yaml.safe_load(content))
         except yaml.composer.ComposerError as err:
             raise DBFormatError(err)
 
 
 class GenericDB(DBObject):
     def __init__(self, prefix, schema, bases=None):
         super().__init__(self, schema)
@@ -331,21 +359,21 @@
                             f"{native_type.__name__}"
                         )
                     return literal
         elif isinstance(schema_type, SchemaDefinedType):
             return self.load_defined_type(literal, schema_type)
         elif isinstance(schema_type, SchemaExpandable):
             if not isinstance(literal, str):
-                DBFormatError(
+                raise DBFormatError(
                     f"token {token} of {schema_type} is not a valid expandable str"
                 )
             return self.load_expandable(literal)
         elif isinstance(schema_type, SchemaRangeId):
             if not isinstance(literal, int):
-                DBFormatError(
+                raise DBFormatError(
                     f"token {token} of {schema_type} is not a valid rangeid integer"
                 )
             return self.load_rangeid(literal)
         elif isinstance(schema_type, SchemaContainerList):
             return self.load_list(token, literal, schema_type, parent)
         elif isinstance(schema_type, SchemaObject):
             return self.load_object(token, literal, schema_type, parent)
@@ -359,18 +387,16 @@
         raise DBFormatError(
             f"Unknow literal {literal} for token {token} for type {schema_type}"
         )
 
     def load_defined_type(self, literal, schema_type: SchemaDefinedType):
         return schema_type.parse(literal)
 
-    def load_object(
-        self, token, literal, schema_object: SchemaObject, parent: SchemaObject
-    ):
-        logger.debug("Loading object %s with %s (%s)", token, literal, schema_object)
+    def create_object(self, schema_object):
+        """Instanciate DBObject with dynamic instanciation with optional base class."""
         # is it expandable?
         if schema_object.expandable:
             bases = [DBExpandableObject]
             classname = f"{self._prefix}Expandable{schema_object.name}"
         else:
             bases = [DBObject]
             classname = f"{self._prefix}{schema_object.name}"
@@ -382,27 +408,38 @@
             bases.insert(
                 0,
                 getattr(self._bases, f"{self._prefix}{schema_object.name}Base"),
             )
         except AttributeError:
             pass
         # instanciate the object with its dynamically defined class
-        obj = type(classname, tuple(bases), dict())(self, schema_object)
+        return type(classname, tuple(bases), dict())(self, schema_object)
+
+    def create_object_by_name(self, name):
+        """Instanciate DBObject by its name."""
+        return self.create_object(self._schema.find_obj(name))
+
+    def load_object(
+        self, token, literal, schema_object: SchemaObject, parent: SchemaObject
+    ):
+        logger.debug("Loading object %s with %s (%s)", token, literal, schema_object)
+        obj = self.create_object(schema_object)
 
         obj._parent = parent
 
         # load object attributes
         self.load_object_attributes(obj, literal, schema_object)
 
         for prop in schema_object.properties:
             # Check all required properties are properly defined in obj
             # attributes.
             if (
                 not isinstance(prop.type, SchemaBackReference)
                 and prop.required
+                and not prop.computed
                 and not hasattr(obj, prop.name)
             ):
                 raise DBFormatError(
                     f"Property {prop.name} is required in schema for object "
                     f"{schema_object}"
                 )
             # Load back references
@@ -461,14 +498,20 @@
             # pass.
             processed = False
 
             # Iterate over a copy of last pass remaining object attributes
             for token, literal in _content.copy().items():
                 # Get the schema property corresponding to this token
                 token_property = self.token_object_property(token, schema_object)
+                # Check property is not computed or raise error
+                if token_property.computed:
+                    raise DBFormatError(
+                        f"{schema_object.name}>{token} is a computed property, thus it "
+                        "cannot be defined in database."
+                    )
                 # Check if this attribute can be loaded, considering its
                 # references and loaded objects.
                 if not self.loadable_attribute(token, token_property, passes, obj):
                     # The attribute cannot be loaded, jump to next attribute.
                     logger.debug(
                         "Skipping object %s property %s in pass %d",
                         schema_object.name,
```

### Comparing `RacksDB-0.3.0/racksdb/generic/definedtype.py` & `racksdb-0.4.0/racksdb/tests/test_defined_type_hexcolor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# Copyright (c) 2022-2023 Rackslab
+# Copyright (c) 2023 Rackslab
 #
 # This file is part of RacksDB.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-import re
+import unittest
 
-from .errors import DBFormatError
+from racksdb.drawers.dtypes.hexcolor import SchemaDefinedTypeHexcolor
+from racksdb.generic.errors import DBFormatError
 
 
-class SchemaDefinedType:
-    def __init__(self):
-        self.name = self.__class__.__module__
-
-    def __str__(self):
-        return f"~{self.name}"
-
-    def _match(self, value):
-        regex = re.compile(self.pattern)
-        match = regex.match(str(value))
-        if match is None:
-            raise DBFormatError(f"Unable to match {self} pattern with value {value}")
-        return match
+class TestDefinedTypeHexcolor(unittest.TestCase):
+    def test_defined_type_hexcolor(self):
+        defined_type = SchemaDefinedTypeHexcolor()
+        self.assertEqual(defined_type.parse("#004080"), (0, 64 / 255, 128 / 255, 1.0))
+        self.assertEqual(
+            defined_type.parse("#ffb4c5"), (1.0, 180 / 255, 197 / 255, 1.0)
+        )
+
+    def test_defined_type_hexcolor_invalid_values(self):
+        defined_type = SchemaDefinedTypeHexcolor()
+        for value in ["001122", "fail"]:
+            with self.assertRaises(DBFormatError):
+                defined_type.parse(value)
```

### Comparing `RacksDB-0.3.0/racksdb/generic/dumpers/__init__.py` & `racksdb-0.4.0/racksdb/generic/dumpers/__init__.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/generic/dumpers/_common.py` & `racksdb-0.4.0/racksdb/generic/dumpers/_common.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/generic/dumpers/console.py` & `racksdb-0.4.0/racksdb/generic/dumpers/console.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/generic/dumpers/json.py` & `racksdb-0.4.0/racksdb/generic/dumpers/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,33 +53,19 @@
                 # As a DBList is also a standard iterable Python list, json.JSONEncoder
                 # will iterate itself over the DBList, thus expanding potential
                 # expandable objects automatically. There is nothing more to do in this
                 # case.
                 return obj
         elif isinstance(obj, DBObject):
             result = {}
-            for attribute, value in vars(obj).items():
-                # Skip special attributes
-                if attribute in [
-                    "_db",
-                    "_indexes",
-                    "_schema",
-                    "_parent",
-                    "_first",
-                    "_key",
-                ]:
+            for prop in obj._schema.properties:
+                try:
+                    self._fill_obj_dict(result, obj, prop.name, getattr(obj, prop.name))
+                except AttributeError:
                     continue
-                # Replace renamed attribute by overriding property
-                if attribute.startswith(obj.LOADED_PREFIX):
-                    attribute = attribute[len(obj.LOADED_PREFIX) :]
-                    value = getattr(obj, attribute)
-                self._fill_obj_dict(result, obj, attribute, value)
-
-            for prop in obj._computed_props():
-                self._fill_obj_dict(result, obj, prop, getattr(obj, prop))
             return result
         # Let the base class default method raise the TypeError
         return json.JSONEncoder.default(self, obj)
 
 
 class DBDumperJSON:
     def __init__(self, show_types=False, objects_map={}, fold=True):
```

### Comparing `RacksDB-0.3.0/racksdb/generic/dumpers/yaml.py` & `racksdb-0.4.0/racksdb/generic/dumpers/yaml.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,36 +65,22 @@
         if self.show_types:
             tag = f"{data.__class__.__name__}"
         else:
             tag = "tag:yaml.org,2002:map"  # YAML generic mapping type
 
         node = yaml.MappingNode(tag, node_value)
 
-        for item_key, item_value in vars(data).items():
-            # skip special fields
-            if item_key in [
-                "_db",
-                "_indexes",
-                "_schema",
-                "_parent",
-                "_first",
-                "_key",
-            ]:
+        for prop in data._schema.properties:
+            try:
+                self._fill_obj_node_value(
+                    dumper, node_value, data, prop.name, getattr(data, prop.name)
+                )
+            except AttributeError:
                 continue
-            # If the attribute has been renamed with loaded prefix, call bases
-            # module class attribute instead.
-            if item_key.startswith(data.LOADED_PREFIX):
-                item_key = item_key[len(data.LOADED_PREFIX) :]
-                item_value = getattr(data, item_key)
-            self._fill_obj_node_value(dumper, node_value, data, item_key, item_value)
 
-        for prop in data._computed_props():
-            self._fill_obj_node_value(
-                dumper, node_value, data, prop, getattr(data, prop)
-            )
         return node
 
     def _represent_dbobjectrange(self, dumper, data):
         return dumper.represent_data(str(data.rangeset))
 
     def _represent_dbobjectrangeid(self, dumper, data):
         return dumper.represent_data(data.start)
```

### Comparing `RacksDB-0.3.0/racksdb/generic/openapi.py` & `racksdb-0.4.0/racksdb/generic/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                         }
                     }
                 },
             }
         }
 
     def _action_argument_description(self, action, parameter):
-        """Return the OpenAPI description of a DBActionArgument."""
+        """Return the OpenAPI description of a DBActionParameter."""
         result = {
             "name": parameter.name,
             "in": "path" if action.inpath(parameter) else "query",
             "description": parameter.description,
             "required": parameter.required or action.inpath(parameter),
         }
         if parameter.nargs == 0:
```

### Comparing `RacksDB-0.3.0/racksdb/generic/schema.py` & `racksdb-0.4.0/racksdb/generic/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,26 +198,31 @@
         result = f"^{self.obj}"
         if self.prop is not None:
             result += f".{self.prop}"
         return result
 
 
 class SchemaProperty:
-    def __init__(self, name, required, key, default, value_type, description, example):
+    def __init__(
+        self, name, required, key, default, value_type, description, example, computed
+    ):
         self.name = name
         self.required = required
         self.key = key
         self.default = default
         self.type = value_type
         self.description = description
         self.example = example
+        self.computed = computed
 
     def __str__(self):
         if self.required:
             result = "required "
+        elif self.computed:
+            result = "computed"
         else:
             result = "optional "
         if self.key:
             result += "key "
         result += str(self.type)
         if self.default is not None:
             result += f" ({self.default})"
@@ -274,14 +279,15 @@
             name,
             required,
             key,
             default,
             value_type,
             spec.get("description"),
             spec.get("example"),
+            spec.get("computed", False),
         )
 
     def value_type(self, spec):
         # parse native types
         for native_type in (str, int, float, bool):
             if spec == native_type.__name__:
                 return SchemaNativeType(native_type)
```

### Comparing `RacksDB-0.3.0/racksdb/tests/test_defined_type_hexcolor.py` & `racksdb-0.4.0/racksdb/tests/test_schema_defined_type_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright (c) 2023 Rackslab
+# Copyright (c) 2022-2023 Rackslab
 #
 # This file is part of RacksDB.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import unittest
 
-from racksdb.drawers.dtypes.hexcolor import SchemaDefinedTypeHexcolor
-from racksdb.generic.errors import DBFormatError
+from racksdb.generic.schema import SchemaDefinedTypeLoader
+from racksdb.generic.definedtype import SchemaDefinedType
 
 
-class TestDefinedTypeHexcolor(unittest.TestCase):
-    def test_defined_type_hexcolor(self):
-        defined_type = SchemaDefinedTypeHexcolor()
-        self.assertEqual(defined_type.parse("#004080"), (0, 64 / 255, 128 / 255))
-        self.assertEqual(defined_type.parse("#ffb4c5"), (1.0, 180 / 255, 197 / 255))
-
-    def test_defined_type_hexcolor_invalid_values(self):
-        defined_type = SchemaDefinedTypeHexcolor()
-        for value in ["001122", "fail"]:
-            with self.assertRaises(DBFormatError):
-                defined_type.parse(value)
+class TestSchemaDefinedTypeLoader(unittest.TestCase):
+    def test_schema_defined_type_loader(self):
+        # Load defined types provided in RacksDB
+        loader = SchemaDefinedTypeLoader("racksdb.dtypes")
+        # Verify at least one defined type has been loaded
+        self.assertGreater(len(loader.content), 0)
+        # Verify loader content is a dict
+        self.assertIs(type(loader.content), dict)
+        # Verify content values are valid SchemaDefinedType
+        for defined_type in loader.content.values():
+            self.assertIsInstance(defined_type, SchemaDefinedType)
```

### Comparing `RacksDB-0.3.0/racksdb/tests/test_defined_type_watts.py` & `racksdb-0.4.0/racksdb/tests/test_defined_type_watts.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/tests/test_drawer.py` & `racksdb-0.4.0/racksdb/tests/test_drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 import unittest
 from pathlib import Path
 
 from racksdb.drawers.base import Drawer, DefaultEquipmentColorSet, DefaultRackColorSet
 from racksdb.drawers.parameters import DrawingParameters
-from racksdb.generic.db import DBEmptyLoader
+from racksdb.generic.db import DBDictsLoader
 
 
 class FakeEquipmentType:
     def __init__(self, id):
         self.id = id
 
 
@@ -68,37 +68,37 @@
                     {
                         "tags": ["tag1", "tag2"],
                         "pane": "#445566",  # (68, 85, 102)
                     },
                 ],
             }
         }
-        loader = DBEmptyLoader(parameters_raw)
+        loader = DBDictsLoader(parameters_raw)
         parameters = DrawingParameters.load(loader, self.drawings_schema_path)
-        self.drawer = Drawer({}, "output", "format", parameters)
+        self.drawer = Drawer({}, "output", "format", parameters, None, "yaml")
 
     def test_matching_equipment_coloring_rule(self):
         # Equipment with type type1 must match 1st coloring rule.
         self.assertEqual(
             self.drawer._find_equipment_colorset(FakeEquipment("type1", [])).background,
-            (17 / 255, 34 / 255, 51 / 255),
+            (17 / 255, 34 / 255, 51 / 255, 1.0),
         )
         # Equipment with another type must not match any defined coloring rule
         # and fallback to default.
         self.assertEqual(
             self.drawer._find_equipment_colorset(FakeEquipment("type2", [])).background,
             DefaultEquipmentColorSet.background,
         )
         # Equipment with type != type1 and all tag1 and tag2 must match 2nd coloring
         # rule.
         self.assertEqual(
             self.drawer._find_equipment_colorset(
                 FakeEquipment("type2", ["tag1", "tag2"])
             ).border,
-            (68 / 255, 85 / 255, 102 / 255),
+            (68 / 255, 85 / 255, 102 / 255, 1.0),
         )
         # Equipment with type != type1 and only part of 2nd coloring rule tags must not
         # match any defined coloring rule and fallback to default.
         self.assertEqual(
             self.drawer._find_equipment_colorset(
                 FakeEquipment("type2", ["tag1"])
             ).background,
@@ -119,26 +119,26 @@
             DefaultEquipmentColorSet.background,
         )
 
     def test_matching_rack_coloring_rule(self):
         # Rack with type type1 must match 1st coloring rule.
         self.assertEqual(
             self.drawer._find_rack_colorset(FakeRack("type1", [])).frame,
-            (17 / 255, 34 / 255, 51 / 255),
+            (17 / 255, 34 / 255, 51 / 255, 1.0),
         )
         # Rack with another type must not match any defined coloring rule and fallback
         # to default.
         self.assertEqual(
             self.drawer._find_rack_colorset(FakeRack("type2", [])).frame,
             DefaultRackColorSet.frame,
         )
         # Rack with type != type1 and all tag1 and tag2 must match 2nd coloring rule.
         self.assertEqual(
             self.drawer._find_rack_colorset(FakeRack("type2", ["tag1", "tag2"])).pane,
-            (68 / 255, 85 / 255, 102 / 255),
+            (68 / 255, 85 / 255, 102 / 255, 1.0),
         )
         # Rack with type != type1 and only part of 2nd coloring rule tags must not match
         # any defined coloring rule and fallback to default.
         self.assertEqual(
             self.drawer._find_rack_colorset(FakeRack("type2", ["tag1"])).pane,
             DefaultRackColorSet.pane,
         )
```

### Comparing `RacksDB-0.3.0/racksdb/tests/test_schema.py` & `racksdb-0.4.0/racksdb/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/tests/tests_db_load.py` & `racksdb-0.4.0/racksdb/tests/tests_db_load.py`

 * *Files identical despite different names*

### Comparing `RacksDB-0.3.0/racksdb/views.py` & `racksdb-0.4.0/racksdb/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -139,23 +139,55 @@
                 DBActionParameter(
                     "drawings_schema",
                     description="Schema of drawing parameters",
                     _type=Path,
                     default=DrawingParameters.DEFAULT_SCHEMA,
                     specific="cli",
                 ),
+                DBActionParameter(
+                    "coordinates",
+                    description=(
+                        "Dump equipments and racks coordinates in diagrams. When this "
+                        "parameter is set, the mimetype of the response is "
+                        "`multipart/form-data`."
+                    ),
+                    nargs=0,
+                    specific="web",
+                ),
+                DBActionParameter(
+                    "coordinates",
+                    description=(
+                        "Dump equipments and racks coordinates in diagrams (default: "
+                        "disabled, default filename: coordinates.<FORMAT>)"
+                    ),
+                    short="c",
+                    nargs="?",
+                    _type=Path,
+                    default=False,
+                    default_in_help=False,
+                    const=True,
+                    specific="cli",
+                ),
+                DBActionParameter(
+                    "coordinates_format",
+                    description="Format of coordinates",
+                    choices=["json", "yaml"],
+                    default="json",
+                ),
             ],
             responses=[
                 DBActionResponse("image/png", binary=True),
                 DBActionResponse("image/svg+xml"),
                 DBActionResponse("application/pdf", binary=True),
+                DBActionResponse("multipart/form-data", binary=True),
             ],
             errors=[
-                DBActionError(400, "Unable to parse drawing parameters in JSON format"),
                 DBActionError(
-                    415,
-                    "Unsupported drawing parameters format or unable to load drawing "
-                    "parameters schema",
+                    400,
+                    "Unable to load drawing parameters, unsupported coordinates format"
+                    "or unable to load requested entity in database.",
                 ),
+                DBActionError(415, "Unsupported drawing parameters format."),
+                DBActionError(500, "Unable to load drawing parameters schema."),
             ],
         )
     ]
```

### Comparing `RacksDB-0.3.0/racksdb/web/app.py` & `racksdb-0.4.0/racksdb/web/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 import argparse
 from pathlib import Path
 import io
 import logging
 
 from flask import Flask, Blueprint, Response, request, send_file, abort, jsonify
+from requests_toolbelt import MultipartEncoder
 
 from .. import RacksDB
+from ..errors import RacksDBError
 from ..version import get_version
 from ..views import RacksDBViews
-from ..generic.db import DBEmptyLoader, DBStringLoader
+from ..generic.db import DBDictsLoader, DBStringLoader
 from ..generic.openapi import OpenAPIGenerator
 from ..generic.dumpers import DBDumperFactory, SchemaDumperFactory
 from ..generic.schema import Schema, SchemaFileLoader, SchemaDefinedTypeLoader
 from ..generic.errors import DBSchemaError, DBFormatError
 from ..drawers import InfrastructureDrawer, RoomDrawer
 from ..drawers.parameters import DrawingParameters
 
@@ -36,20 +38,22 @@
 
     def __init__(
         self,
         schema=RacksDB.DEFAULT_SCHEMA,
         ext=RacksDB.DEFAULT_EXT,
         db=RacksDB.DEFAULT_DB,
         drawings_schema=DrawingParameters.DEFAULT_SCHEMA,
+        default_drawing_parameters={},
         openapi=False,
     ):
         super().__init__("RacksDB web blueprint", __name__)
         self.db = RacksDB.load(schema=schema, ext=ext, db=db)
         self.views = RacksDBViews()
         self.drawings_schema = drawings_schema
+        self.default_drawing_parameters = default_drawing_parameters
         if openapi:
             self.add_url_rule("/openapi.yaml", view_func=self._openapi, methods=["GET"])
         self.add_url_rule(
             f"/v{get_version()}/<content>", view_func=self._dump_view, methods=["GET"]
         )
         self.add_url_rule(
             f"/v{get_version()}/schema", view_func=self._schema, methods=["GET"]
@@ -61,15 +65,15 @@
         for action in self.views.actions():
             # add path with generic action
             self.add_url_rule(
                 f"/v{get_version()}{action.path}",
                 view_func=getattr(self, f"_{action.name}"),
                 methods=[action.method.upper()],
             )
-        for error in [400, 404, 415]:
+        for error in [400, 404, 415, 500]:
             self.register_error_handler(error, self._handle_bad_request)
 
     def _handle_bad_request(self, error):
         return (
             jsonify(code=error.code, name=error.name, description=error.description),
             error.code,
         )
@@ -108,34 +112,83 @@
         )
         return Response(
             response=dumper.dump(data), mimetype=self.MIMETYPES[dump_format]
         )
 
     def _draw(self, entity, name, format):
         if not len(request.data):
-            db_loader = DBEmptyLoader()
+            db_loader = DBDictsLoader(self.default_drawing_parameters)
         elif request.is_json:
-            db_loader = DBEmptyLoader(request.get_json())
+            db_loader = DBDictsLoader(
+                self.default_drawing_parameters, request.get_json()
+            )
         elif request.content_type == "application/x-yaml":
-            db_loader = DBStringLoader(request.data.decode())
+            db_loader = DBStringLoader(
+                request.data.decode(), initial=self.default_drawing_parameters
+            )
         else:
             abort(415, "Unsupported request body format")
         try:
             parameters = DrawingParameters.load(db_loader, self.drawings_schema)
         except DBSchemaError as err:
-            abort(415, f"Unable to load drawing parameters schema: {str(err)}")
+            abort(500, f"Unable to load drawing parameters schema: {str(err)}")
         except DBFormatError as err:
-            abort(415, f"Unable to load drawing parameters: {str(err)}")
+            abort(400, f"Unable to load drawing parameters: {str(err)}")
+
+        # Handle coordinates query parameters
+        with_coordinates = "coordinates" in request.args
+        coordinates_format = request.args.get("coordinates_format", "json")
+        if coordinates_format not in {"json", "yaml"}:
+            abort(400, "Unsupported coordinates format")
+
+        # Create volatile in-memory file handlers
         file = io.BytesIO()
-        if entity == "infrastructure":
-            drawer = InfrastructureDrawer(self.db, name, file, format, parameters)
-        elif entity == "room":
-            drawer = RoomDrawer(self.db, name, file, format, parameters)
+        coordinates_fh = io.StringIO() if with_coordinates else None
+
+        try:
+            if entity == "infrastructure":
+                drawer = InfrastructureDrawer(
+                    self.db,
+                    name,
+                    file,
+                    format,
+                    parameters,
+                    coordinates_fh,
+                    coordinates_format,
+                )
+            elif entity == "room":
+                drawer = RoomDrawer(
+                    self.db,
+                    name,
+                    file,
+                    format,
+                    parameters,
+                    coordinates_fh,
+                    coordinates_format,
+                )
+        except RacksDBError as err:
+            abort(400, str(err))
         drawer.draw()
         file.seek(0)
+
+        if with_coordinates:
+            coordinates_fh.seek(0)
+            # Send coordinates in multipart response along with generated image.
+            multipart = MultipartEncoder(
+                fields={
+                    "image": (f"{name}.{format}", file, self.MIMETYPES[format]),
+                    "coordinates": (
+                        f"coordinates.{coordinates_format}",
+                        coordinates_fh,
+                        self.MIMETYPES[coordinates_format],
+                    ),
+                }
+            )
+            return Response(multipart.to_string(), mimetype=multipart.content_type)
+
         return send_file(
             file,
             mimetype=self.MIMETYPES[format],
         )
 
     def _openapi(self):
         _drawings_schema = Schema(
@@ -214,32 +267,67 @@
             help="Enable CORS headers",
         )
         parser.add_argument(
             "--openapi",
             action="store_true",
             help="Enable OpenAPI route",
         )
+        parser.add_argument(
+            "--with-ui",
+            help="Enable UI with optional path (default path: %(const)s)",
+            nargs="?",
+            metavar="PATH",
+            const=RacksDB.DEFAULT_UI,
+            type=Path,
+        )
 
         self.args = parser.parse_args()
         self.register_blueprint(
             RacksDBWebBlueprint(
                 self.args.schema,
                 self.args.ext,
                 self.args.db,
                 self.args.drawings_schema,
-                self.args.openapi,
+                openapi=self.args.openapi,
             )
         )
 
+        if self.args.with_ui:
+            self.add_url_rule("/config.json", view_func=self._ui_config)
+            self.static_folder = self.args.with_ui
+            self.add_url_rule("/", view_func=self._ui_files)
+            self.add_url_rule("/<path:name>", view_func=self._ui_files)
+
+    def _ui_config(self):
+        return jsonify(
+            {
+                "API_SERVER": (f"http://{self.args.host}:{self.args.port}/"),
+                "API_VERSION": f"v{get_version()}",
+            }
+        )
+
+    def _ui_files(self, name="index.html"):
+        if (
+            name in ["favicon.ico"]
+            or name.startswith("assets/")
+            or name.startswith("logo/")
+        ):
+            return self.send_static_file(name)
+        else:
+            return self.send_static_file("index.html")
+
     def serve(self):
         logger.info("Running RacksDB web application")
         if self.args.cors:
-            from flask_cors import CORS
+            try:
+                from flask_cors import CORS
 
-            CORS(self)
+                CORS(self)
+            except ImportError:
+                logger.warning("Unable to load CORS module, CORS is disabled.")
         super().run(
             host=self.args.host,
             port=self.args.port,
             debug=self.args.debug,
         )
 
     @classmethod
```

