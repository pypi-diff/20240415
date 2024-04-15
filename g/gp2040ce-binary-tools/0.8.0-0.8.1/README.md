# Comparing `tmp/gp2040ce_binary_tools-0.8.0.tar.gz` & `tmp/gp2040ce_binary_tools-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce_binary_tools-0.8.0.tar", last modified: Sun Apr 14 04:34:29 2024, max compression
+gzip compressed data, was "gp2040ce_binary_tools-0.8.1.tar", last modified: Mon Apr 15 04:38:55 2024, max compression
```

## Comparing `gp2040ce_binary_tools-0.8.0.tar` & `gp2040ce_binary_tools-0.8.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.0/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.0/.gitignore
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.539307 gp2040ce_binary_tools-0.8.0/.reuse/
--rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.0/.reuse/dep5
--rw-r--r--   0 bss       (1026) bss       (1000)     5973 2024-04-14 04:20:23.000000 gp2040ce_binary_tools-0.8.0/CHANGELOG.md
--rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.0/LICENSE.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.540307 gp2040ce_binary_tools-0.8.0/LICENSES/
--rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/MIT.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.0/MAINTAINERS.md
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.0/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.554307 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)    18569 2024-04-13 01:06:37.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/gui.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/
--rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    16797 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.0/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.0/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.542307 gp2040ce_binary_tools-0.8.0/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.544307 gp2040ce_binary_tools-0.8.0/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.553307 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.553307 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-binary-source-of-json-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.json
--rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board-with-board-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16077 2024-04-13 01:08:25.000000 gp2040ce_binary_tools-0.8.0/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.0/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/tests/test_rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11220 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.0/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.1/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.1/.gitignore
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.277298 gp2040ce_binary_tools-0.8.1/.reuse/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.1/.reuse/dep5
+-rw-r--r--   0 bss       (1026) bss       (1000)     6244 2024-04-15 04:33:31.000000 gp2040ce_binary_tools-0.8.1/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.1/LICENSE.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.277298 gp2040ce_binary_tools-0.8.1/LICENSES/
+-rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/LICENSES/MIT.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.1/MAINTAINERS.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.1/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.278298 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-15 04:38:55.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    17737 2024-04-15 04:24:05.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/gui.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/
+-rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    17282 2024-04-15 04:22:28.000000 gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.1/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.1/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.1/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-15 04:38:55.292298 gp2040ce_binary_tools-0.8.1/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.279298 gp2040ce_binary_tools-0.8.1/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.281298 gp2040ce_binary_tools-0.8.1/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 04:38:55.291298 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-binary-source-of-json-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.json
+-rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board-with-board-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16263 2024-04-15 04:25:29.000000 gp2040ce_binary_tools-0.8.1/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.1/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.1/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.1/tests/test_rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11246 2024-04-15 03:46:08.000000 gp2040ce_binary_tools-0.8.1/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.1/tox.ini
```

### Comparing `gp2040ce_binary_tools-0.8.0/.gitignore` & `gp2040ce_binary_tools-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/.reuse/dep5` & `gp2040ce_binary_tools-0.8.1/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/CHANGELOG.md` & `gp2040ce_binary_tools-0.8.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # CHANGELOG
 
 Included is a summary of changes to the project. For full details, especially on behind-the-scenes code changes and
 development tools, see the commit history.
 
+## v0.8.1
+
+### Improvements
+
+* `concatenate` no longer writes a padded 2 MB binary (so 4 MB UF2), instead properly indexing the board/user configs
+  separately from the binary, leading to smaller UF2s.
+
+### Bugfixes
+
+* `summarize-gp2040ce` now properly reads UF2 files.
+
 ## v0.8.0
 
 ### Features
 
 * New command, `summarize-gp2040ce`, to get info about a board image or USB device. Details are limited at the moment,
   but more will come as we need them.
 * `dump-config` can now dump the board config rather than only the user config.
```

### Comparing `gp2040ce_binary_tools-0.8.0/CONTRIBUTING.md` & `gp2040ce_binary_tools-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/LICENSE.md` & `gp2040ce_binary_tools-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/LICENSES/CC-BY-SA-4.0.txt` & `gp2040ce_binary_tools-0.8.1/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/LICENSES/GPL-3.0-or-later.txt` & `gp2040ce_binary_tools-0.8.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/LICENSES/MIT.txt` & `gp2040ce_binary_tools-0.8.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/PKG-INFO` & `gp2040ce_binary_tools-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.0/README.md` & `gp2040ce_binary_tools-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/PKG-INFO` & `gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce_binary_tools-0.8.1/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/__init__.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/builder.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,33 +97,23 @@
         firmware_binary = bytearray(firmware.read())
 
     # create a sequential binary for .bin and USB uses, or index it for .uf2
     if usb or combined_filename[-4:] != '.uf2':
         new_binary = combine_firmware_and_config(firmware_binary, board_config_binary, user_config_binary,
                                                  replace_extra=replace_extra)
     else:
-        # this was kind of fine, but combining multiple calls of convert_binary_to_uf2 produced
-        # incorrect total block counts in the file, which picotool handled with some squirrely
-        # double-output behavior that has me worried it'd cause a real issue, so doing the
-        # crude padding + write of empty blocks, for now...
-        #
-        # new_binary = convert_binary_to_uf2(firmware_binary)
-        # if board_config_binary:
-        #     new_binary += convert_binary_to_uf2(pad_config_to_storage_size(board_config_binary),
-        #                                         start=BOARD_CONFIG_BINARY_LOCATION)
-        # if user_config_binary:
-        #     new_binary += convert_binary_to_uf2(pad_config_to_storage_size(user_config_binary),
-        #                                         start=USER_CONFIG_BINARY_LOCATION)
-        #
-        # the correct way to do the above would be to pass a list of {offset,binary_data} to convert...,
-        # and have it calculate the total block size before starting to write, and then iterating over
-        # the three lists. doable, just not on the top of my mind right now
-        new_binary = storage.convert_binary_to_uf2(combine_firmware_and_config(firmware_binary, board_config_binary,
-                                                                               user_config_binary,
-                                                                               replace_extra=replace_extra))
+        binary_list = [(0, firmware_binary)]
+        # we must pad to storage start in order for the UF2 write addresses to make sense
+        if board_config_binary:
+            binary_list.append((storage.BOARD_CONFIG_BINARY_LOCATION,
+                                storage.pad_config_to_storage_size(board_config_binary)))
+        if user_config_binary:
+            binary_list.append((storage.USER_CONFIG_BINARY_LOCATION,
+                                storage.pad_config_to_storage_size(user_config_binary)))
+        new_binary = storage.convert_binary_to_uf2(binary_list)
 
     if combined_filename:
         with open(combined_filename, 'wb') as combined:
             combined.write(new_binary)
 
     if usb:
         endpoint_out, endpoint_in = get_bootsel_endpoints()
@@ -252,16 +242,18 @@
         binary = replace_config_in_binary(bytearray(existing_binary), config_binary)
         with open(filename, 'wb') as file:
             file.write(binary)
     else:
         binary = storage.serialize_config_with_footer(config)
         with open(filename, 'wb') as file:
             if filename[-4:] == '.uf2':
-                file.write(storage.convert_binary_to_uf2(storage.pad_config_to_storage_size(binary),
-                                                         start=storage.USER_CONFIG_BINARY_LOCATION))
+                # we must pad to storage start in order for the UF2 write addresses to make sense
+                file.write(storage.convert_binary_to_uf2([
+                    (storage.USER_CONFIG_BINARY_LOCATION, storage.pad_config_to_storage_size(binary)),
+                ]))
             else:
                 file.write(binary)
 
 
 def write_new_config_to_usb(config: Message, endpoint_out: object, endpoint_in: object):
     """Serialize the provided config to a device over USB, in the proper location for a GP2040-CE board.
 
@@ -348,16 +340,15 @@
     input_group.add_argument('--filename', help="input .bin or .uf2 file to inspect")
 
     args, _ = parser.parse_known_args()
     if args.usb:
         content, endpoint, _ = get_gp2040ce_from_usb()
         print(f"USB device {hex(endpoint.device.idVendor)}:{hex(endpoint.device.idProduct)}:\n")
     else:
-        with open(args.filename, 'rb') as file_:
-            content = file_.read()
+        content = storage.get_binary_from_file(args.filename)
         print(f"File {args.filename}:\n")
 
     gp2040ce_version = find_version_string_in_binary(content)
     try:
         board_config = storage.get_config(storage.get_board_storage_section(bytes(content)))
         board_config_version = board_config.boardVersion if board_config.boardVersion else "NOT SPECIFIED"
     except storage.ConfigReadError:
```

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/config_tree.css` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/config_tree.css`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/gui.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config.proto` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config_pb2.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums.proto` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb.proto` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/rp2040.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/storage.py` & `gp2040ce_binary_tools-0.8.1/gp2040ce_bintools/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,44 +49,45 @@
     """Exception raised when a length sanity check fails."""
 
 
 class ConfigMagicError(ConfigReadError):
     """Exception raised when the config section does not have the magic value in its footer."""
 
 
-def convert_binary_to_uf2(binary: bytearray, start: int = 0) -> bytearray:
+def convert_binary_to_uf2(binaries: list[tuple[int, bytearray]]) -> bytearray:
     """Convert a GP2040-CE binary payload to Microsoft's UF2 format.
 
     https://github.com/microsoft/uf2/tree/master#overview
 
     Args:
-        binary: bytearray content to convert to a UF2 payload
-        start: position offset to start at rather than flash start (for creating e.g. user config UF2s)
+        binaries: list of start,binary pairs of binary data to write at the specified memory offset in flash
     Returns:
         the content in UF2 format
     """
-    size = len(binary)
-    blocks = (len(binary) // 256) + 1 if len(binary) % 256 else len(binary) // 256
-    uf2 = bytearray()
+    total_blocks = sum([(len(binary) // 256) + 1 if len(binary) % 256 else len(binary) // 256
+                        for offset, binary in binaries])
 
-    index = 0
-    while index < size:
-        pad_count = 476 - len(binary[index:index+256])
-        uf2 += struct.pack('<LLLLLLLL',
-                           UF2_MAGIC_FIRST,                                 # first magic number
-                           UF2_MAGIC_SECOND,                                # second magic number
-                           0x00002000,                                      # familyID present
-                           0x10000000 + start + index,                      # address to write to
-                           256,                                             # bytes to write in this block
-                           index // 256,                                    # sequential block number
-                           blocks,                                          # total number of blocks
-                           UF2_FAMILY_ID)                                   # family ID
-        uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
-        uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
-        index += 256
+    uf2 = bytearray()
+    for start, binary in binaries:
+        size = len(binary)
+        index = 0
+        while index < size:
+            pad_count = 476 - len(binary[index:index+256])
+            uf2 += struct.pack('<LLLLLLLL',
+                               UF2_MAGIC_FIRST,                                 # first magic number
+                               UF2_MAGIC_SECOND,                                # second magic number
+                               0x00002000,                                      # familyID present
+                               0x10000000 + start + index,                      # address to write to
+                               256,                                             # bytes to write in this block
+                               index // 256,                                    # sequential block number
+                               total_blocks,                                    # total number of blocks
+                               UF2_FAMILY_ID)                                   # family ID
+            uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
+            uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
+            index += 256
     return uf2
 
 
 def convert_uf2_to_binary(uf2: bytearray) -> bytearray:
     """Convert a Microsoft's UF2 payload to a raw binary.
 
     https://github.com/microsoft/uf2/tree/master#overview
@@ -198,32 +199,47 @@
         raise ConfigCrcError(f"provided content CRC checksum {content_crc} does not match footer's expected CRC "
                              f"checksum {config_crc}!")
 
     logger.debug("detected footer (size:%s, crc:%s, magic:%s", config_size, config_crc, config_magic)
     return config_size, config_crc, config_magic
 
 
+def get_binary_from_file(filename: str) -> bytes:
+    """Read the specified file (.bin or .uf2) and get back its raw binary contents.
+
+    Args:
+        filename: the filename of the file to open and read
+    Returns:
+        the file's content, in raw binary format
+    Raises:
+        FileNotFoundError: if the file was not found
+    """
+    with open(filename, 'rb') as dump:
+        if filename[-4:] == '.uf2':
+            content = bytes(convert_uf2_to_binary(bytearray(dump.read())))
+        else:
+            content = dump.read()
+
+    return content
+
+
 def get_config_from_file(filename: str, whole_board: bool = False, allow_no_file: bool = False,
                          board_config: bool = False) -> Message:
     """Read the specified file (memory dump or whole board dump) and get back its config section.
 
     Args:
         filename: the filename of the file to open and read
         whole_board: optional, if true, attempt to find the storage section from its normal location on a board
         allow_no_file: if true, attempting to open a nonexistent file returns an empty config, else it errors
         board_config: if true, the board config is provided instead of the user config
     Returns:
         the parsed configuration
     """
     try:
-        with open(filename, 'rb') as dump:
-            if filename[-4:] == '.uf2':
-                content = bytes(convert_uf2_to_binary(bytearray(dump.read())))
-            else:
-                content = dump.read()
+        content = get_binary_from_file(filename)
     except FileNotFoundError:
         if not allow_no_file:
             raise
         config_pb2 = get_config_pb2()
         return config_pb2.Config()
 
     if whole_board:
@@ -374,16 +390,17 @@
         config, _, _ = get_board_config_from_usb()
     else:
         config, _, _ = get_user_config_from_usb()
     binary_config = serialize_config_with_footer(config)
     with open(args.filename, 'wb') as out_file:
         if args.filename[-4:] == '.uf2':
             # we must pad to storage start in order for the UF2 write addresses to make sense
-            out_file.write(convert_binary_to_uf2(pad_config_to_storage_size(binary_config),
-                                                 start=USER_CONFIG_BINARY_LOCATION))
+            out_file.write(convert_binary_to_uf2([
+                (USER_CONFIG_BINARY_LOCATION, pad_config_to_storage_size(binary_config)),
+            ]))
         else:
             out_file.write(binary_config)
 
 
 def visualize():
     """Print the contents of GP2040-CE's storage."""
     parser = argparse.ArgumentParser(
```

### Comparing `gp2040ce_binary_tools-0.8.0/pyproject.toml` & `gp2040ce_binary_tools-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/requirements/requirements-dev.txt` & `gp2040ce_binary_tools-0.8.1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/requirements/requirements.txt` & `gp2040ce_binary_tools-0.8.1/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/conftest.py` & `gp2040ce_binary_tools-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.1/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/config.proto` & `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/enums.proto` & `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/nanopb.proto` & `gp2040ce_binary_tools-0.8.1/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-binary-source-of-json-config.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-binary-source-of-json-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.json` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-config.json`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-firmware.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-storage-area.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board-with-board-config.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board-with-board-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board.bin` & `gp2040ce_binary_tools-0.8.1/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_builder.py` & `gp2040ce_binary_tools-0.8.1/tests/test_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for the image builder module.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
 SPDX-License-Identifier: GPL-3.0-or-later
 """
+import math
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
@@ -113,29 +114,31 @@
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
     builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
                                                    binary_user_config_filename=config_file,
                                                    combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
-    # size of the file should be 2x the binary version, and the binary is 2 MB
-    assert len(content) == 2 * 2 * 1024 * 1024
+    # size of the file should be 2x the padded firmware + 2x the board config space + 2x the user config space
+    assert len(content) == (math.ceil(len(firmware_binary)/256) * 512 +
+                            math.ceil(STORAGE_SIZE/256) * 512 * 2)
 
 
 def test_concatenate_to_uf2_board_only(tmp_path, firmware_binary, config_binary):
     """Test that we write a UF2 file as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.uf2')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
     builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
                                                    combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
-    # size of the file should be 2x the binary version (minus user config space), and the binary is 2 MB - 16KB
-    assert len(content) == 2 * (2 * 1024 * 1024 - 16384)
+    # size of the file should be 2x the padded firmware + 2x the board config space
+    assert len(content) == (math.ceil(len(firmware_binary)/256) * 512 +
+                            math.ceil(STORAGE_SIZE/256) * 512)
 
 
 def test_find_version_string(firmware_binary):
     """Test that we can find a version string in a binary."""
     assert builder.find_version_string_in_binary(firmware_binary) == 'v0.7.5'
```

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_commands.py` & `gp2040ce_binary_tools-0.8.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_gui.py` & `gp2040ce_binary_tools-0.8.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_package.py` & `gp2040ce_binary_tools-0.8.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_rp2040.py` & `gp2040ce_binary_tools-0.8.1/tests/test_rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.0/tests/test_storage.py` & `gp2040ce_binary_tools-0.8.1/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,50 +129,50 @@
     assert config.boardVersion == 'v0.7.5'
     assert config.hotkeyOptions.hotkey01.dpadMask == 0
     assert config.hotkeyOptions.hotkey02.dpadMask == 1
 
 
 def test_convert_binary_to_uf2(whole_board_with_board_config_dump):
     """Do some sanity checks in the attempt to convert a binary to a UF2."""
-    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+    uf2 = storage.convert_binary_to_uf2([{0, whole_board_with_board_config_dump}])
     assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
     assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
     assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
     assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
 
 
 def test_convert_unaligned_binary_to_uf2(firmware_binary):
     """Do some sanity checks in the attempt to convert a binary to a UF2."""
-    uf2 = storage.convert_binary_to_uf2(firmware_binary)
+    uf2 = storage.convert_binary_to_uf2([{0, firmware_binary}])
     assert len(uf2) == math.ceil(len(firmware_binary)/256) * 512    # 256 byte complete/partial chunks -> 512 b chunks
     assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
     assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
     assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
 
 
 def test_convert_binary_to_uf2_with_offsets(whole_board_with_board_config_dump):
     """Do some sanity checks in the attempt to convert a binary to a UF2."""
-    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump, start=storage.USER_CONFIG_BINARY_LOCATION)
+    uf2 = storage.convert_binary_to_uf2([{storage.USER_CONFIG_BINARY_LOCATION, whole_board_with_board_config_dump}])
     assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
     assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
     assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
     assert uf2[524:528] == bytearray(b'\x00\xc1\x1f\x10')   # address to write the second chunk
 
 
 def test_convert_binary_to_uf2_to_binary(whole_board_with_board_config_dump):
     """Do some sanity checks in the attempt to convert a binary to a UF2."""
-    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+    uf2 = storage.convert_binary_to_uf2([{0, whole_board_with_board_config_dump}])
     binary = storage.convert_uf2_to_binary(uf2)
     assert len(binary) == 2097152
     assert whole_board_with_board_config_dump == binary
 
 
 def test_malformed_uf2(whole_board_with_board_config_dump):
     """Check that we expect a properly-formed UF2."""
-    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+    uf2 = storage.convert_binary_to_uf2([{0, whole_board_with_board_config_dump}])
 
     # truncated UF2 --- byte mismatch
     with pytest.raises(ValueError):
         storage.convert_uf2_to_binary(uf2[:-4])
 
     # truncated uf2 --- counter is wrong
     with pytest.raises(ValueError):
```

### Comparing `gp2040ce_binary_tools-0.8.0/tox.ini` & `gp2040ce_binary_tools-0.8.1/tox.ini`

 * *Files identical despite different names*

