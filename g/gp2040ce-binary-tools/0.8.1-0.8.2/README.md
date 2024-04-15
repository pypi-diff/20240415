# Comparing `tmp/gp2040ce_binary_tools-0.8.1.tar.gz` & `tmp/gp2040ce_binary_tools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce_binary_tools-0.8.1.tar", last modified: Mon Apr 15 04:38:55 2024, max compression
+gzip compressed data, was "gp2040ce_binary_tools-0.8.2.tar", last modified: Mon Apr 15 05:07:25 2024, max compression
```

## Comparing `gp2040ce_binary_tools-0.8.1.tar` & `gp2040ce_binary_tools-0.8.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.1/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.1/.gitignore
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.277298 gp2040ce_binary_tools-0.8.1/.reuse/
--rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.1/.reuse/dep5
--rw-r--r--   0 bss       (1026) bss       (1000)     6244 2024-04-15 04:33:31.000000 gp2040ce_binary_tools-0.8.1/CHANGELOG.md
--rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.1/LICENSE.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.277298 gp2040ce_binary_tools-0.8.1/LICENSES/
--rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/MIT.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.1/MAINTAINERS.md
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.1/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.278298 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)    17737 2024-04-15 04:24:05.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/gui.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/
--rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    17282 2024-04-15 04:22:28.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.1/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.1/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.281298 gp2040ce_binary_tools-0.8.1/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-binary-source-of-json-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.json
--rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board-with-board-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16263 2024-04-15 04:25:29.000000 gp2040ce_binary_tools-0.8.1/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.1/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/tests/test_rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11246 2024-04-15 03:46:08.000000 gp2040ce_binary_tools-0.8.1/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.1/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.588092 gp2040ce_binary_tools-0.8.2/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.2/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.2/.gitignore
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.572092 gp2040ce_binary_tools-0.8.2/.reuse/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.2/.reuse/dep5
+-rw-r--r--   0 bss       (1026) bss       (1000)     6330 2024-04-15 04:51:32.000000 gp2040ce_binary_tools-0.8.2/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.2/LICENSE.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.572092 gp2040ce_binary_tools-0.8.2/LICENSES/
+-rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/LICENSES/MIT.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.2/MAINTAINERS.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 05:07:25.588092 gp2040ce_binary_tools-0.8.2/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.2/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.587092 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.573092 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-15 05:07:25.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    17737 2024-04-15 04:24:05.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/gui.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.574092 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/
+-rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    17331 2024-04-15 04:48:57.000000 gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.2/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.574092 gp2040ce_binary_tools-0.8.2/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.2/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.2/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-15 05:07:25.588092 gp2040ce_binary_tools-0.8.2/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.574092 gp2040ce_binary_tools-0.8.2/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.2/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.577092 gp2040ce_binary_tools-0.8.2/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.586092 gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 05:07:25.586092 gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-binary-source-of-json-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-config.json
+-rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-whole-board-with-board-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.2/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16263 2024-04-15 04:54:54.000000 gp2040ce_binary_tools-0.8.2/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.2/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.2/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.2/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.2/tests/test_rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11246 2024-04-15 05:07:20.000000 gp2040ce_binary_tools-0.8.2/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.2/tox.ini
```

### Comparing `gp2040ce_binary_tools-0.8.1/.gitignore` & `gp2040ce_binary_tools-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/.reuse/dep5` & `gp2040ce_binary_tools-0.8.2/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/CHANGELOG.md` & `gp2040ce_binary_tools-0.8.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # CHANGELOG
 
 Included is a summary of changes to the project. For full details, especially on behind-the-scenes code changes and
 development tools, see the commit history.
 
+## v0.8.2
+
+### Bugfixes
+
+* UF2 files made of parts now have the proper block counts.
+
 ## v0.8.1
 
 ### Improvements
 
 * `concatenate` no longer writes a padded 2 MB binary (so 4 MB UF2), instead properly indexing the board/user configs
   separately from the binary, leading to smaller UF2s.
```

### Comparing `gp2040ce_binary_tools-0.8.1/CONTRIBUTING.md` & `gp2040ce_binary_tools-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/LICENSE.md` & `gp2040ce_binary_tools-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/LICENSES/CC-BY-SA-4.0.txt` & `gp2040ce_binary_tools-0.8.2/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/LICENSES/GPL-3.0-or-later.txt` & `gp2040ce_binary_tools-0.8.2/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/LICENSES/MIT.txt` & `gp2040ce_binary_tools-0.8.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/PKG-INFO` & `gp2040ce_binary_tools-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.1/README.md` & `gp2040ce_binary_tools-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/PKG-INFO` & `gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce_binary_tools-0.8.2/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/__init__.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/builder.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/builder.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/config_tree.css` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/config_tree.css`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/gui.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config.proto` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config_pb2.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums.proto` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums_pb2.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb.proto` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/rp2040.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/storage.py` & `gp2040ce_binary_tools-0.8.2/gp2040ce_bintools/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,33 +61,35 @@
     Args:
         binaries: list of start,binary pairs of binary data to write at the specified memory offset in flash
     Returns:
         the content in UF2 format
     """
     total_blocks = sum([(len(binary) // 256) + 1 if len(binary) % 256 else len(binary) // 256
                         for offset, binary in binaries])
+    block_count = 0
 
     uf2 = bytearray()
     for start, binary in binaries:
         size = len(binary)
         index = 0
         while index < size:
             pad_count = 476 - len(binary[index:index+256])
             uf2 += struct.pack('<LLLLLLLL',
                                UF2_MAGIC_FIRST,                                 # first magic number
                                UF2_MAGIC_SECOND,                                # second magic number
                                0x00002000,                                      # familyID present
                                0x10000000 + start + index,                      # address to write to
                                256,                                             # bytes to write in this block
-                               index // 256,                                    # sequential block number
+                               block_count,                                     # sequential block number
                                total_blocks,                                    # total number of blocks
                                UF2_FAMILY_ID)                                   # family ID
             uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
             uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
             index += 256
+            block_count += 1
     return uf2
 
 
 def convert_uf2_to_binary(uf2: bytearray) -> bytearray:
     """Convert a Microsoft's UF2 payload to a raw binary.
 
     https://github.com/microsoft/uf2/tree/master#overview
```

### Comparing `gp2040ce_binary_tools-0.8.1/pyproject.toml` & `gp2040ce_binary_tools-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/requirements/requirements-dev.txt` & `gp2040ce_binary_tools-0.8.2/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/requirements/requirements.txt` & `gp2040ce_binary_tools-0.8.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/conftest.py` & `gp2040ce_binary_tools-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.2/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/config.proto` & `gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/enums.proto` & `gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/nanopb.proto` & `gp2040ce_binary_tools-0.8.2/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-binary-source-of-json-config.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-binary-source-of-json-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.json` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-config.json`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-firmware.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-storage-area.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board-with-board-config.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-whole-board-with-board-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board.bin` & `gp2040ce_binary_tools-0.8.2/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_builder.py` & `gp2040ce_binary_tools-0.8.2/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_commands.py` & `gp2040ce_binary_tools-0.8.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_gui.py` & `gp2040ce_binary_tools-0.8.2/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_package.py` & `gp2040ce_binary_tools-0.8.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_rp2040.py` & `gp2040ce_binary_tools-0.8.2/tests/test_rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tests/test_storage.py` & `gp2040ce_binary_tools-0.8.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.1/tox.ini` & `gp2040ce_binary_tools-0.8.2/tox.ini`

 * *Files identical despite different names*

