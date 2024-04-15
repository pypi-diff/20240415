# Comparing `tmp/daliuge-translator-4.0.0.tar.gz` & `tmp/daliuge-translator-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-translator-4.0.0.tar", last modified: Mon Mar 25 14:48:22 2024, max compression
+gzip compressed data, was "daliuge-translator-4.0.1.tar", last modified: Mon Apr 15 07:01:40 2024, max compression
```

## Comparing `daliuge-translator-4.0.0.tar` & `daliuge-translator-4.0.1.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.784262 daliuge-translator-4.0.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1089 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/.coveragerc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      180 2023-05-09 13:02:30.000000 daliuge-translator-4.0.0/MANIFEST.in
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      307 2024-03-25 14:48:22.784262 daliuge-translator-4.0.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      157 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2812 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/build_translator.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.684263 daliuge-translator-4.0.0/daliuge_translator.egg-info/
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)      307 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10315 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       62 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      152 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        9 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/daliuge_translator.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.684263 daliuge-translator-4.0.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.684263 daliuge-translator-4.0.0/dlg/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      334 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-01-20 04:39:24.000000 daliuge-translator-4.0.0/dlg/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-02-21 01:56:47.000000 daliuge-translator-4.0.0/dlg/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.684263 daliuge-translator-4.0.0/dlg/dropmake/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1055 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.692263 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      257 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      251 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-11-30 13:05:03.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2046 2023-06-29 09:21:37.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/definition_classes.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12075 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12524 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13319 2023-06-29 09:21:37.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12149 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33214 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33621 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-37.pyc
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)    15078 2024-02-16 06:04:13.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33862 2023-03-20 04:28:33.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-39.pyc
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)    24978 2024-02-16 06:04:13.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg_node.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5103 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5142 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-37.pyc
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)     5408 2024-02-16 06:04:13.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5192 2023-03-02 10:50:42.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4295 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4260 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4282 2022-12-02 06:13:10.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4298 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10593 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10603 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-37.pyc
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)    10641 2024-02-16 06:04:13.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10671 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15161 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15425 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15471 2023-06-29 08:45:42.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15177 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35069 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35137 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35596 2023-06-29 08:45:42.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35179 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3051 2023-06-29 09:21:30.000000 daliuge-translator-4.0.0/dlg/dropmake/definition_classes.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26528 2023-06-29 09:21:30.000000 daliuge-translator-4.0.0/dlg/dropmake/dm_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16917 2024-03-25 11:51:05.000000 daliuge-translator-4.0.0/dlg/dropmake/lg.graph.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35686 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/dlg/dropmake/lg.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35972 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/dlg/dropmake/lg_node.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.692263 daliuge-translator-4.0.0/dlg/dropmake/lib/
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   382436 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/lib/libmetis.dylib
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   495581 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/lib/libmetis.so
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7963 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/dlg/dropmake/pg_generator.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5689 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/pg_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17876 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/dlg/dropmake/pgt.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26019 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/dlg/dropmake/pgtp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    51636 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/dlg/dropmake/scheduler.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.696263 daliuge-translator-4.0.0/dlg/dropmake/utils/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.700263 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      169 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-11-30 13:05:03.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8415 2023-02-19 06:22:54.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/anneal.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4435 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4464 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4434 2023-05-09 13:02:31.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4428 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2429 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2682 2023-03-19 10:33:29.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2717 2023-05-09 13:46:35.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2475 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11713 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/anneal.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5848 2023-05-09 13:02:30.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/antichains.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3470 2023-05-09 13:46:34.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/bash_parameter.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.700263 daliuge-translator-4.0.0/dlg/dropmake/utils/heft/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8068 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/utils/heft/base.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.704263 daliuge-translator-4.0.0/dlg/dropmake/web/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2024-02-27 02:20:53.000000 daliuge-translator-4.0.0/dlg/dropmake/web/LICENSE
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       47 2024-02-27 02:20:53.000000 daliuge-translator-4.0.0/dlg/dropmake/web/VERSION
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.704263 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      161 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-11-30 13:05:03.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18547 2022-11-03 13:04:49.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/lg_web.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25609 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26872 2024-03-18 15:07:08.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25869 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4532 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4487 2023-03-19 10:35:34.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4568 2023-05-09 13:46:35.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4548 2022-12-21 05:50:12.000000 daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   139114 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/d3.v3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11324 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/dlg/dropmake/web/graph_init.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.704263 daliuge-translator-4.0.0/dlg/dropmake/web/img/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14438 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/img/jsoneditor-icons.png
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      878 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/license.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    28184 2024-03-18 15:04:41.000000 daliuge-translator-4.0.0/dlg/dropmake/web/main.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7019 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/dlg/dropmake/web/matrix_vis.html
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)    15050 2023-05-09 13:02:30.000000 daliuge-translator-4.0.0/dlg/dropmake/web/pg_viewer.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17286 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/pure-min.css
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.708263 daliuge-translator-4.0.0/dlg/dropmake/web/src/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5649 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/FileSaver.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.680263 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.712263 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    64548 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   151749 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48488 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   108539 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4897 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    76483 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4021 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    32461 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   192348 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   492048 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155758 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   625953 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.720263 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   222911 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   402249 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78635 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   311949 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   131637 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   250568 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58072 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   190253 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.728263 daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/d3.v5.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/dagre-d3.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/dagre-d3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      806 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/data_prep.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/echarts-dagre.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.736263 daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    69177 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   174048 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    79612 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    60840 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   165349 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/html2canvas.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.740263 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/arrow_right_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      409 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/explore_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/liu.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/liuFavIcon.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1462 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26026 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/translate_green.png
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      423 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/zoom_in_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      370 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/zoom_out_map_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      404 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/zoom_out_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30747 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/jquery-ui.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89500 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/jquery.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.760263 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17804 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/canteen.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1943 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/caseFrame.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12066 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/caseFrame.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7037 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/config.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7545 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/countup.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45411 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/dat.gui.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9813 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/draggable.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5929 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16465 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10407 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16061 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecStat.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   986443 2023-05-09 13:46:34.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/echarts.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7598 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/esl.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3080 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/facePrint.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.760263 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/fflate/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30151 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/fflate/index.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9690 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/frameInsight.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    95957 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/jquery.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9937 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/perlin.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3908 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/rearrange.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/require.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11232 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/requireES.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2984 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/reset.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   320509 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/rollup.browser.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34282 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/testHelper.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16108 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/main.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/dropmake/web/src/require.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39837 2024-03-18 14:56:39.000000 daliuge-translator-4.0.0/dlg/dropmake/web/translator_rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4718 2023-05-09 13:46:34.000000 daliuge-translator-4.0.0/dlg/dropmake/web/translator_utils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.764263 daliuge-translator-4.0.0/dlg/translator/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg/translator/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.764263 daliuge-translator-4.0.0/dlg/translator/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      159 2023-03-19 10:30:52.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-11-30 13:05:03.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-12-21 05:49:48.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11776 2022-12-21 08:43:30.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11757 2024-03-18 15:06:41.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11783 2022-12-21 05:49:48.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      291 2023-02-19 06:22:55.000000 daliuge-translator-4.0.0/dlg/translator/__pycache__/version.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15141 2024-03-18 15:04:41.000000 daliuge-translator-4.0.0/dlg/translator/tool_commands.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      223 2024-03-25 14:48:22.000000 daliuge-translator-4.0.0/dlg/translator/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1043 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/dlg.spec
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.772262 daliuge-translator-4.0.0/docker/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      936 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/docker/Dockerfile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      943 2024-03-18 15:04:41.000000 daliuge-translator-4.0.0/docker/Dockerfile.dev
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      809 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/docker/Dockerfile.ray
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      966 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/docker/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1418 2024-02-15 06:56:33.000000 daliuge-translator-4.0.0/run_translator.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2024-03-25 14:48:22.788262 daliuge-translator-4.0.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3766 2024-03-25 14:36:41.000000 daliuge-translator-4.0.0/setup.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      120 2023-06-29 09:21:30.000000 daliuge-translator-4.0.0/stop_translator.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.772262 daliuge-translator-4.0.0/test/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.772262 daliuge-translator-4.0.0/test/dropmake/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/dropmake/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.776262 daliuge-translator-4.0.0/test/dropmake/logical_graphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58266 2024-03-25 12:28:10.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/ArrayLoop.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11934 2024-03-25 12:32:15.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/HelloWorld_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33969 2024-03-25 14:10:55.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/Plasma_test.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34116 2024-03-25 12:33:25.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/SharedMemoryTest.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   154708 2024-03-25 14:25:47.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/chiles_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   249542 2024-03-25 14:11:04.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/cont_img_mvp.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12121 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.graph.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10861 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.json.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12001 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    66412 2024-03-25 12:31:07.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    50347 2024-03-25 12:31:38.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather_empty.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    80653 2024-03-25 12:31:57.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   197452 2024-03-25 12:32:34.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/lofar_std.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14909 2024-03-25 12:32:52.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/nagsIo.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26265 2024-03-25 12:44:27.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/simpleMKN.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10592 2024-03-25 12:34:22.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/test-20190830-110556.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25187 2024-03-25 12:35:50.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/testLoop.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12288 2024-03-25 12:36:14.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/testScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    87068 2024-03-25 14:10:48.000000 daliuge-translator-4.0.0/test/dropmake/logical_graphs/test_grpby_gather.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1918 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/test/dropmake/test_lg_fill.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18712 2024-03-25 13:58:14.000000 daliuge-translator-4.0.0/test/dropmake/test_lgweb.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8215 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/test/dropmake/test_pg_gen.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4666 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/test/dropmake/test_scheduler.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.784262 daliuge-translator-4.0.0/test/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/reproducibility/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:48:22.784262 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21761 2024-03-25 12:24:08.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSBash.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21543 2024-03-25 14:15:20.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSPython.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21547 2024-03-25 14:15:19.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSPython2.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21750 2024-03-25 12:25:06.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldBash.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21755 2024-03-25 12:25:21.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldBashSplit.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5968 2024-03-25 12:25:40.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldFile.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26854 2024-03-25 14:15:22.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/apps.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13471 2024-03-25 12:22:30.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/files.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10002 2024-03-25 12:23:41.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/groupUse.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33617 2024-03-25 14:15:21.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/groups.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6576 2024-03-25 14:15:17.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/misc.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45065 2024-03-25 12:25:56.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/simpleNoScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45063 2024-03-25 12:26:17.000000 daliuge-translator-4.0.0/test/reproducibility/reproGraphs/simpleScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    99333 2024-03-25 14:23:04.000000 daliuge-translator-4.0.0/test/reproducibility/test_accumulatedata.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21073 2023-05-18 15:50:38.000000 daliuge-translator-4.0.0/test/reproducibility/test_integration.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1472 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/reproducibility/test_json_output.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2107 2023-05-09 13:46:34.000000 daliuge-translator-4.0.0/test/reproducibility/test_repro_inits.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2022-11-30 13:05:02.000000 daliuge-translator-4.0.0/test/reproducibility/test_reprodata_compare.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6045 2023-05-09 13:46:34.000000 daliuge-translator-4.0.0/test/reproducibility/test_scatter_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2898 2023-06-29 08:45:39.000000 daliuge-translator-4.0.0/test/test_tool_trans.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      134 2023-05-18 15:50:38.000000 daliuge-translator-4.0.0/test-requirements.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1089 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/.coveragerc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      180 2023-05-09 13:02:30.000000 daliuge-translator-4.0.1/MANIFEST.in
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      307 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      157 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/README.md
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2845 2024-04-12 16:15:38.000000 daliuge-translator-4.0.1/build_translator.sh
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.580611 daliuge-translator-4.0.1/daliuge_translator.egg-info/
+-rw-r--r--   0 awicenec  (1000) awicenec  (1000)      307 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10315 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       62 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      152 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        9 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/daliuge_translator.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.584611 daliuge-translator-4.0.1/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.584611 daliuge-translator-4.0.1/dlg/__pycache__/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      334 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-01-20 04:39:24.000000 daliuge-translator-4.0.1/dlg/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-02-21 01:56:47.000000 daliuge-translator-4.0.1/dlg/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.584611 daliuge-translator-4.0.1/dlg/dropmake/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1055 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.588611 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      257 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      251 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-11-30 13:05:03.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2046 2023-06-29 09:21:37.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/definition_classes.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12075 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12524 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13319 2023-06-29 09:21:37.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12149 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33214 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33621 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-37.pyc
+-rw-r--r--   0 awicenec  (1000) awicenec  (1000)    15078 2024-02-16 06:04:13.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33862 2023-03-20 04:28:33.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-39.pyc
+-rw-r--r--   0 awicenec  (1000) awicenec  (1000)    24978 2024-02-16 06:04:13.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg_node.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5103 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5142 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5481 2024-04-15 05:52:25.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5192 2023-03-02 10:50:42.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4295 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4260 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4282 2022-12-02 06:13:10.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4298 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10593 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10603 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10695 2024-04-15 05:52:25.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10671 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15161 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15425 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15471 2023-06-29 08:45:42.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15177 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35069 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35137 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35596 2023-06-29 08:45:42.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35179 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3051 2023-06-29 09:21:30.000000 daliuge-translator-4.0.1/dlg/dropmake/definition_classes.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26528 2023-06-29 09:21:30.000000 daliuge-translator-4.0.1/dlg/dropmake/dm_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16917 2024-03-25 11:51:05.000000 daliuge-translator-4.0.1/dlg/dropmake/lg.graph.schema
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35686 2024-02-15 06:56:33.000000 daliuge-translator-4.0.1/dlg/dropmake/lg.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35972 2024-02-15 06:56:33.000000 daliuge-translator-4.0.1/dlg/dropmake/lg_node.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.588611 daliuge-translator-4.0.1/dlg/dropmake/lib/
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   382436 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/lib/libmetis.dylib
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   495581 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/lib/libmetis.so
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8014 2024-04-15 05:51:59.000000 daliuge-translator-4.0.1/dlg/dropmake/pg_generator.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5689 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/pg_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17766 2024-04-15 05:52:24.000000 daliuge-translator-4.0.1/dlg/dropmake/pgt.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26019 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/dlg/dropmake/pgtp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    51636 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/dlg/dropmake/scheduler.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.592611 daliuge-translator-4.0.1/dlg/dropmake/utils/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.592611 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      169 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-11-30 13:05:03.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8415 2023-02-19 06:22:54.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/anneal.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4435 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4464 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4434 2023-05-09 13:02:31.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4428 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2429 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2682 2023-03-19 10:33:29.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2717 2023-05-09 13:46:35.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2475 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11713 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/anneal.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5848 2023-05-09 13:02:30.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/antichains.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3470 2023-05-09 13:46:34.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/bash_parameter.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.592611 daliuge-translator-4.0.1/dlg/dropmake/utils/heft/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8068 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/utils/heft/base.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.592611 daliuge-translator-4.0.1/dlg/dropmake/web/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2024-04-12 15:25:08.000000 daliuge-translator-4.0.1/dlg/dropmake/web/LICENSE
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       59 2024-04-12 15:25:08.000000 daliuge-translator-4.0.1/dlg/dropmake/web/VERSION
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.596611 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      161 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-11-30 13:05:03.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18547 2022-11-03 13:04:49.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/lg_web.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25609 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26649 2024-04-15 01:30:04.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25869 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4532 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4487 2023-03-19 10:35:34.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4574 2024-04-15 01:30:05.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4548 2022-12-21 05:50:12.000000 daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   139114 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/d3.v3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11324 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/dlg/dropmake/web/graph_init.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.596611 daliuge-translator-4.0.1/dlg/dropmake/web/img/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14438 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/img/jsoneditor-icons.png
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      878 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/license.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    28184 2024-04-10 13:44:37.000000 daliuge-translator-4.0.1/dlg/dropmake/web/main.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7019 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/dlg/dropmake/web/matrix_vis.html
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)    15050 2023-05-09 13:02:30.000000 daliuge-translator-4.0.1/dlg/dropmake/web/pg_viewer.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17286 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/pure-min.css
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.596611 daliuge-translator-4.0.1/dlg/dropmake/web/src/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5649 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/FileSaver.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.580611 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.600611 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    64548 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   151749 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48488 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   108539 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4897 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    76483 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4021 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    32461 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   192348 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   492048 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155758 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   625953 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.604611 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   222911 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   402249 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78635 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   311949 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   131637 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   250568 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58072 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   190253 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.604611 daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/d3.v5.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/dagre-d3.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/dagre-d3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      806 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/data_prep.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/echarts-dagre.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.608611 daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    69177 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   174048 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    79612 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    60840 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   165349 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/html2canvas.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.608611 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/arrow_right_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      409 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/explore_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/liu.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/liuFavIcon.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1462 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/settings_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26026 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/translate_green.png
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      423 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/zoom_in_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      370 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/zoom_out_map_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      404 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/zoom_out_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30747 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/jquery-ui.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89500 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/jquery.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.612611 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17804 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/canteen.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1943 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/caseFrame.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12066 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/caseFrame.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7037 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/config.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7545 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/countup.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45411 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/dat.gui.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9813 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/draggable.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5929 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16465 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecSimpleTransform.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10407 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16061 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecStat.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/echarts-dagre.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   986443 2023-05-09 13:46:34.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/echarts.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7598 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/esl.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3080 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/facePrint.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.612611 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/fflate/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30151 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/fflate/index.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9690 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/frameInsight.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    95957 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/jquery.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9937 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/perlin.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3908 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/rearrange.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/require.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11232 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/requireES.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2984 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/reset.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   320509 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/rollup.browser.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34282 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/testHelper.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16108 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/main.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/dropmake/web/src/require.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39143 2024-04-12 16:12:35.000000 daliuge-translator-4.0.1/dlg/dropmake/web/translator_rest.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4730 2024-04-12 16:12:35.000000 daliuge-translator-4.0.1/dlg/dropmake/web/translator_utils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.616611 daliuge-translator-4.0.1/dlg/translator/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg/translator/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.616611 daliuge-translator-4.0.1/dlg/translator/__pycache__/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      159 2023-03-19 10:30:52.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-11-30 13:05:03.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-12-21 05:49:48.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11776 2022-12-21 08:43:30.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-310.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11757 2024-03-18 15:06:41.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11783 2022-12-21 05:49:48.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-39.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      291 2023-02-19 06:22:55.000000 daliuge-translator-4.0.1/dlg/translator/__pycache__/version.cpython-38.pyc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15141 2024-03-18 15:04:41.000000 daliuge-translator-4.0.1/dlg/translator/tool_commands.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      223 2024-04-15 07:01:40.000000 daliuge-translator-4.0.1/dlg/translator/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1043 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/dlg.spec
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.616611 daliuge-translator-4.0.1/docker/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      936 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/docker/Dockerfile
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      910 2024-04-12 16:16:40.000000 daliuge-translator-4.0.1/docker/Dockerfile.dev
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      809 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/docker/Dockerfile.ray
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      966 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/docker/README.md
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1497 2024-04-12 16:16:40.000000 daliuge-translator-4.0.1/run_translator.sh
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3766 2024-04-15 06:59:37.000000 daliuge-translator-4.0.1/setup.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      120 2023-06-29 09:21:30.000000 daliuge-translator-4.0.1/stop_translator.sh
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.616611 daliuge-translator-4.0.1/test/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.616611 daliuge-translator-4.0.1/test/dropmake/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/dropmake/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/test/dropmake/logical_graphs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58266 2024-03-25 12:28:10.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/ArrayLoop.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11934 2024-03-25 12:32:15.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/HelloWorld_simple.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33969 2024-03-25 14:10:55.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/Plasma_test.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34116 2024-03-25 12:33:25.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/SharedMemoryTest.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   154708 2024-04-15 05:48:24.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/chiles_simple.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   249542 2024-03-25 14:11:04.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/cont_img_mvp.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12121 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.graph.schema
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10861 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.json.schema
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12001 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.schema
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    66412 2024-03-25 12:31:07.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    50347 2024-03-25 12:31:38.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather_empty.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    80653 2024-03-25 12:31:57.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather_simple.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   197452 2024-03-25 12:32:34.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/lofar_std.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14909 2024-03-25 12:32:52.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/nagsIo.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26265 2024-03-25 12:44:27.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/simpleMKN.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10592 2024-03-25 12:34:22.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/test-20190830-110556.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25187 2024-03-25 12:35:50.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/testLoop.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12288 2024-03-25 12:36:14.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/testScatter.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    87068 2024-03-25 14:10:48.000000 daliuge-translator-4.0.1/test/dropmake/logical_graphs/test_grpby_gather.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1918 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/test/dropmake/test_lg_fill.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18712 2024-04-10 13:15:34.000000 daliuge-translator-4.0.1/test/dropmake/test_lgweb.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8215 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/test/dropmake/test_pg_gen.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4666 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/test/dropmake/test_scheduler.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/test/reproducibility/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/reproducibility/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:40.620611 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21761 2024-03-25 12:24:08.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSBash.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21543 2024-03-25 14:15:20.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSPython.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21547 2024-03-25 14:15:19.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSPython2.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21750 2024-03-25 12:25:06.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldBash.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21755 2024-03-25 12:25:21.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldBashSplit.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5968 2024-03-25 12:25:40.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldFile.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26854 2024-03-25 14:15:22.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/apps.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13471 2024-03-25 12:22:30.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/files.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10002 2024-03-25 12:23:41.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/groupUse.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33617 2024-03-25 14:15:21.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/groups.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6576 2024-03-25 14:15:17.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/misc.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45065 2024-03-25 12:25:56.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/simpleNoScatter.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45063 2024-03-25 12:26:17.000000 daliuge-translator-4.0.1/test/reproducibility/reproGraphs/simpleScatter.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    99333 2024-03-25 14:23:04.000000 daliuge-translator-4.0.1/test/reproducibility/test_accumulatedata.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21073 2023-05-18 15:50:38.000000 daliuge-translator-4.0.1/test/reproducibility/test_integration.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1472 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/reproducibility/test_json_output.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2107 2023-05-09 13:46:34.000000 daliuge-translator-4.0.1/test/reproducibility/test_repro_inits.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2022-11-30 13:05:02.000000 daliuge-translator-4.0.1/test/reproducibility/test_reprodata_compare.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6045 2023-05-09 13:46:34.000000 daliuge-translator-4.0.1/test/reproducibility/test_scatter_blockdag.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2898 2023-06-29 08:45:39.000000 daliuge-translator-4.0.1/test/test_tool_trans.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      134 2023-05-18 15:50:38.000000 daliuge-translator-4.0.1/test-requirements.txt
```

### Comparing `daliuge-translator-4.0.0/.coveragerc` & `daliuge-translator-4.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/build_translator.sh` & `daliuge-translator-4.0.1/build_translator.sh`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,14 @@
         echo "Building translator slim version ${VCS_TAG}"
         docker build --build-arg VCS_TAG=${VCS_TAG} --no-cache -t icrar/daliuge-translator.big:${VCS_TAG} -f docker/Dockerfile .
         echo "Build finished! Slimming the image now"
         echo ""
         echo ""
         echo ">>>>> docker-slim output <<<<<<<<<"
         docker run -it --rm -v /var/run/docker.sock:/var/run/docker.sock dslim/docker-slim build --include-shell \
-        --include-path /usr/local/lib --include-path /usr/local/bin --include-path /daliuge --include-path /dlg \
+        --include-path /usr/bin/hostname --include-path /usr/local/lib --include-path /usr/local/bin --include-path /daliuge --include-path /dlg \
         --http-probe=false --tag=icrar/daliuge-translator:${VCS_TAG} icrar/daliuge-translator.big:${VCS_TAG}
 	    ;;
     *)
         echo "Usage: build_translator.sh <dep|dev|slim>"
         exit 0;;
 esac
```

### Comparing `daliuge-translator-4.0.0/daliuge_translator.egg-info/SOURCES.txt` & `daliuge-translator-4.0.1/daliuge_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/__init__.py` & `daliuge-translator-4.0.1/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__init__.py` & `daliuge-translator-4.0.1/dlg/dropmake/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/definition_classes.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/definition_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/dm_utils.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/dm_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/lg_node.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/lg_node.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Feb 15 06:56:33 2024 UTC, .py size: 7963 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a1b5 cd65 1b1f 0000  U..........e....
+00000000: 550d 0d0a 0000 0000 7fc0 1c66 4e1f 0000  U..........fN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0014 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
 00000030: 5a00 6501 6401 6b02 7210 6402 5a02 6403  Z.e.d.k.r.d.Z.d.
 00000040: 6404 6c03 5a03 6403 6404 6c04 5a04 6403  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 5a05 6403 6404 6c06 5a06 6403  d.l.Z.d.d.l.Z.d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6403  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6403 6407 6c0c  d.l.m.Z...d.d.l.
@@ -45,294 +45,299 @@
 000002c0: 025a 0464 0353 0029 04da 0b5f 4c47 5465  .Z.d.S.)..._LGTe
 000002d0: 6d70 6c61 7465 fa01 7e7a 125b 5f61 2d7a  mplate..~z.[_a-z
 000002e0: 5d5b 5f61 2d7a 302d 395c 2e5d 2a4e 2905  ][_a-z0-9\.]*N).
 000002f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000300: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000310: 6d65 5f5f da09 6465 6c69 6d69 7465 72da  me__..delimiter.
 00000320: 0969 6470 6174 7465 726e a900 7211 0000  .idpattern..r...
-00000330: 0072 1100 0000 fa3d 2f64 6c67 2f6c 6962  .r.....=/dlg/lib
-00000340: 2f70 7974 686f 6e33 2e38 2f73 6974 652d  /python3.8/site-
-00000350: 7061 636b 6167 6573 2f64 6c67 2f64 726f  packages/dlg/dro
-00000360: 706d 616b 652f 7067 5f67 656e 6572 6174  pmake/pg_generat
-00000370: 6f72 2e70 7972 0a00 0000 2b00 0000 7304  or.pyr....+...s.
-00000380: 0000 0008 0104 0172 0a00 0000 6301 0000  .......r....c...
-00000390: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-000003a0: 0003 0000 0073 5600 0000 7400 7c00 8301  .....sV...t.|...
-000003b0: 7d01 7c00 a001 a100 4400 5d40 5c02 8900  }.|.....D.]@\...
-000003c0: 7d02 7402 7c02 7400 8302 7248 7403 7c02  }.t.|.t...rHt.|.
-000003d0: 8301 7d03 7c01 a004 8700 6601 6401 6402  ..}.|.....f.d.d.
-000003e0: 8408 7c03 a001 a100 4400 8301 a101 0100  ..|.....D.......
-000003f0: 7110 7c02 7c01 8800 3c00 7110 7c01 5300  q.|.|...<.q.|.S.
-00000400: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000410: 0300 0000 0500 0000 1300 0000 731e 0000  ............s...
-00000420: 0069 007c 005d 165c 027d 017d 0264 0088  .i.|.].\.}.}.d..
-00000430: 007c 0166 0216 007c 0293 0271 0453 0029  .|.f...|...q.S.)
-00000440: 017a 0525 732e 2573 7211 0000 0029 03da  .z.%s.%sr....)..
-00000450: 022e 30da 016b da01 76a9 01da 036b 6579  ..0..k..v....key
-00000460: 7211 0000 0072 1200 0000 da0a 3c64 6963  r....r......<dic
-00000470: 7463 6f6d 703e 3500 0000 7306 0000 0006  tcomp>5...s.....
-00000480: 0006 000a 007a 215f 666c 6174 7465 6e5f  .....z!_flatten_
-00000490: 6469 6374 2e3c 6c6f 6361 6c73 3e2e 3c64  dict.<locals>.<d
-000004a0: 6963 7463 6f6d 703e 2905 da04 6469 6374  ictcomp>)...dict
-000004b0: da05 6974 656d 73da 0a69 7369 6e73 7461  ..items..isinsta
-000004c0: 6e63 65da 0d5f 666c 6174 7465 6e5f 6469  nce.._flatten_di
-000004d0: 6374 da06 7570 6461 7465 2904 da01 645a  ct..update)...dZ
-000004e0: 0466 6c61 74da 0576 616c 7565 5a09 666c  .flat..valueZ.fl
-000004f0: 6174 7465 6e65 6472 1100 0000 7216 0000  attenedr....r...
-00000500: 0072 1200 0000 721c 0000 0030 0000 0073  .r....r....0...s
-00000510: 0e00 0000 0001 0801 1001 0a01 0801 1e02  ................
-00000520: 0a01 721c 0000 0063 0200 0000 0000 0000  ..r....c........
-00000530: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000540: 7354 0000 0074 00a0 0164 017c 01a1 0201  sT...t...d.|....
-00000550: 0074 027c 0183 017d 0274 037c 0064 0283  .t.|...}.t.|.d..
-00000560: 0272 287c 00a0 04a1 007d 006e 1474 057c  .r(|.....}.n.t.|
-00000570: 0074 0683 0273 3c74 07a0 087c 00a1 017d  .t...s<t...|...}
-00000580: 0074 097c 0083 01a0 0a7c 02a1 017d 0074  .t.|.....|...}.t
-00000590: 07a0 0b7c 00a1 0153 0029 037a 2e4c 6f67  ...|...S.).z.Log
-000005a0: 6963 616c 2047 7261 7068 202b 2070 6172  ical Graph + par
-000005b0: 616d 7320 2d3e 2046 696c 6c65 6420 4c6f  ams -> Filled Lo
-000005c0: 6769 6361 6c20 4772 6170 687a 2946 696c  gical Graphz)Fil
-000005d0: 6c69 6e67 204c 6f67 6963 616c 2047 7261  ling Logical Gra
-000005e0: 7068 2077 6974 6820 7061 7261 6d65 7465  ph with paramete
-000005f0: 7273 3a20 2572 da04 7265 6164 290c da06  rs: %r..read)...
-00000600: 6c6f 6767 6572 da04 696e 666f 721c 0000  logger..infor...
-00000610: 00da 0768 6173 6174 7472 7220 0000 0072  ...hasattrr ...r
-00000620: 1b00 0000 da03 7374 72da 046a 736f 6eda  ......str..json.
-00000630: 0564 756d 7073 720a 0000 00da 0a73 7562  .dumpsr......sub
-00000640: 7374 6974 7574 65da 056c 6f61 6473 2903  stitute..loads).
-00000650: da02 6c67 da06 7061 7261 6d73 5a0b 666c  ..lg..paramsZ.fl
-00000660: 6174 5f70 6172 616d 7372 1100 0000 7211  at_paramsr....r.
-00000670: 0000 0072 1200 0000 da04 6669 6c6c 3b00  ...r......fill;.
-00000680: 0000 7310 0000 0000 020c 0108 010a 010a  ..s.............
-00000690: 010a 010a 010e 0172 2b00 0000 4663 0400  .......r+...Fc..
-000006a0: 0000 0000 0000 0000 0000 0700 0000 0400  ................
-000006b0: 0000 4300 0000 7398 0000 0074 00a0 00a1  ..C...s....t....
-000006c0: 007d 0474 017c 007c 0164 018d 027d 007c  .}.t.|.|.d...}.|
-000006d0: 00a0 02a1 007d 057c 0272 3a7c 0544 005d  .....}.|.r:|.D.]
-000006e0: 147d 0664 027c 066b 0672 2464 037c 0664  .}.d.|.k.r$d.|.d
-000006f0: 023c 0071 247c 0372 8874 03a0 0464 047c  .<.q$|.r.t...d.|
-00000700: 03a1 0201 007c 0544 005d 387d 0664 057c  .....|.D.]8}.d.|
-00000710: 066b 0672 4e7c 0664 0619 0064 076b 0272  .k.rN|.d...d.k.r
-00000720: 4e7c 037c 0664 053c 0064 087c 066b 0672  N|.|.d.<.d.|.k.r
-00000730: 7e7c 0664 0819 006e 0264 097c 0664 023c  ~|.d...n.d.|.d.<
-00000740: 0071 4e7c 05a0 057c 006a 06a1 0101 007c  .qN|...|.j.....|
-00000750: 0553 0029 0a7a 1755 6e72 6f6c 6c73 2061  .S.).z.Unrolls a
-00000760: 206c 6f67 6963 616c 2067 7261 7068 2901   logical graph).
-00000770: da04 7373 6964 5a0a 736c 6565 705f 7469  ..ssidZ.sleep_ti
-00000780: 6d65 7202 0000 007a 1652 6570 6c61 6369  mer....z.Replaci
-00000790: 6e67 2061 7070 7320 7769 7468 2025 73da  ng apps with %s.
-000007a0: 0964 726f 7063 6c61 7373 da0c 6361 7465  .dropclass..cate
-000007b0: 676f 7279 5479 7065 da0b 4170 706c 6963  goryType..Applic
-000007c0: 6174 696f 6eda 0e65 7865 6375 7469 6f6e  ation..execution
-000007d0: 5f74 696d 65e9 0200 0000 2907 da04 7469  _time.....)...ti
-000007e0: 6d65 7203 0000 005a 0d75 6e72 6f6c 6c5f  mer....Z.unroll_
-000007f0: 746f 5f74 706c 7221 0000 0072 2200 0000  to_tplr!...r"...
-00000800: da06 6170 7065 6e64 da09 7265 7072 6f64  ..append..reprod
-00000810: 6174 6129 0772 2900 0000 da0a 6f69 645f  ata).r).....oid_
-00000820: 7072 6566 6978 da07 7a65 726f 7275 6eda  prefix..zerorun.
-00000830: 0361 7070 da05 7374 6172 745a 0964 726f  .app..startZ.dro
-00000840: 705f 6c69 7374 da08 6472 6f70 7370 6563  p_list..dropspec
-00000850: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000860: 0675 6e72 6f6c 6c47 0000 0073 2a00 0000  .unrollG...s*...
-00000870: 0002 0801 0c01 0801 0401 0801 0801 0a01  ................
-00000880: 0401 0c01 0802 06ff 0202 0afe 0204 0803  ................
-00000890: 06ff 0a02 02fd 0805 0c01 723a 0000 00e9  ..........r:....
-000008a0: 0100 0000 7231 0000 00e9 0300 0000 e904  ....r1..........
-000008b0: 0000 00da 046e 6f6e 65da 056d 6574 6973  .....none..metis
-000008c0: da08 6d79 7361 726b 6172 da0d 6d69 6e5f  ..mysarkar..min_
-000008d0: 6e75 6d5f 7061 7274 73da 0370 736f 6300  num_parts..psoc.
-000008e0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000008f0: 0000 0043 0000 0073 1200 0000 6401 6402  ...C...s....d.d.
-00000900: 8400 7400 a001 a100 4400 8301 5300 2903  ..t.....D...S.).
-00000910: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00000920: 0000 0500 0000 5300 0000 731a 0000 0067  ......S...s....g
-00000930: 007c 005d 127d 0174 007c 0174 0183 0272  .|.].}.t.|.t...r
-00000940: 047c 0191 0271 0453 0072 1100 0000 2902  .|...q.S.r....).
-00000950: 721b 0000 0072 2400 0000 2902 7213 0000  r....r$...).r...
-00000960: 00da 0178 7211 0000 0072 1100 0000 7212  ...xr....r....r.
-00000970: 0000 00da 0a3c 6c69 7374 636f 6d70 3e76  .....<listcomp>v
-00000980: 0000 0073 0600 0000 0600 0200 0a00 7a24  ...s..........z$
-00000990: 6b6e 6f77 6e5f 616c 676f 7269 7468 6d73  known_algorithms
-000009a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000009b0: 6f6d 703e 2902 da0c 5f6b 6e6f 776e 5f61  omp>)..._known_a
-000009c0: 6c67 6f73 da04 6b65 7973 7211 0000 0072  lgos..keysr....r
-000009d0: 1100 0000 7211 0000 0072 1200 0000 da10  ....r....r......
-000009e0: 6b6e 6f77 6e5f 616c 676f 7269 7468 6d73  known_algorithms
-000009f0: 7500 0000 7302 0000 0000 0172 4700 0000  u...s......rG...
-00000a00: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00000a10: 0003 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
-00000a20: a000 7c01 a101 7d03 7c03 6401 6b09 7216  ..|...}.|.d.k.r.
-00000a30: 7c03 5300 7c02 5300 2902 7a4e 0a20 2020  |.S.|.S.).zN.   
-00000a40: 204d 616b 6520 7375 7265 2074 6861 7420   Make sure that 
-00000a50: 6465 6661 756c 7420 6973 2073 6574 2065  default is set e
-00000a60: 7665 6e20 6966 2076 616c 7565 2068 6173  ven if value has
-00000a70: 2062 6565 6e20 7061 7373 6564 2061 7320   been passed as 
-00000a80: 4e6f 6e65 2e0a 2020 2020 4e29 01da 0367  None..    N)...g
-00000a90: 6574 2904 da0b 616c 676f 5f70 6172 616d  et)...algo_param
-00000aa0: 73da 0a70 6172 616d 5f6e 616d 65da 0764  s..param_name..d
-00000ab0: 6566 6175 6c74 da05 7061 7261 6d72 1100  efault..paramr..
-00000ac0: 0000 7211 0000 0072 1200 0000 da0f 5f67  ..r....r......_g
-00000ad0: 6574 5f61 6c67 6f5f 7061 7261 6d79 0000  et_algo_paramy..
-00000ae0: 0073 0400 0000 0004 0a01 724d 0000 00da  .s........rM....
-00000af0: 0970 6172 7469 7469 6f6e 6306 0000 0000  .partitionc.....
-00000b00: 0000 0000 0000 0013 0000 0009 0000 004b  ...............K
-00000b10: 0000 0073 d201 0000 7400 7c01 7401 8302  ...s....t.|.t...
-00000b20: 722e 7c01 7402 6b07 7226 7403 6401 7c01  r.|.t.k.r&t.d.|.
-00000b30: 7402 a004 a100 6602 1600 8301 8201 7402  t.....f.......t.
-00000b40: 7c01 1900 7d01 7c01 7402 6b07 724a 7405  |...}.|.t.k.rJt.
-00000b50: 6402 7c01 7402 a004 a100 6602 1600 8301  d.|.t.....f.....
-00000b60: 8201 7406 a007 6403 7402 7c01 1900 7c02  ..t...d.t.|...|.
-00000b70: 7c03 7c06 a105 0100 6404 7d07 7408 7c06  |.|.....d.}.t.|.
-00000b80: 6405 6406 8303 7d08 7408 7c06 6407 6406  d.d...}.t.|.d.d.
-00000b90: 8303 7d09 7408 7c06 6408 6409 8303 7d0a  ..}.t.|.d.d...}.
-00000ba0: 7408 7c06 640a 640b 8303 7d0b 7408 7c06  t.|.d.d...}.t.|.
-00000bb0: 640c 640d 8303 7d0c 7408 7c06 640e 640f  d.d...}.t.|.d.d.
-00000bc0: 8303 7d0d 7408 7c06 6410 6411 8303 7d0e  ..}.t.|.d.d...}.
-00000bd0: 7408 7c06 6412 6413 8303 7d0f 7408 7c06  t.|.d.d...}.t.|.
-00000be0: 6414 6415 8303 7d10 7c0b 7c0c 6416 9c02  d.d...}.|.|.d...
-00000bf0: 7d11 7c01 7409 6b02 72ec 740a 7c00 8301  }.|.t.k.r.t.|...
-00000c00: 7d00 6eb8 7c01 740b 6b02 9001 7228 6417  }.n.|.t.k...r(d.
-00000c10: 7c0a 1800 6418 1700 7d12 7c12 6406 6b01  |...d...}.|.d.k.
-00000c20: 9001 7210 6418 7d12 740c 7c00 7c02 7c08  ..r.d.}.t.|.|.|.
-00000c30: 7c04 7c09 7c12 7c07 6419 8d07 7d00 6e7c  |.|.|.|.d...}.n|
-00000c40: 7c01 740d 6b02 9001 7246 740e 7c00 7c02  |.t.k...rFt.|.|.
-00000c50: 7c04 7c11 7c07 6419 8d05 7d00 6e5e 7c01  |.|.|.d...}.n^|.
-00000c60: 740f 6b02 9001 7274 6418 7c0d 641a 1b00  t.k...rtd.|.d...
-00000c70: 1800 7d0d 7410 7c00 7c0e 7c02 7c04 7c0b  ..}.t.|.|.|.|.|.
-00000c80: 7c07 7c0d 641b 8d07 7d00 6e30 7c01 7411  |.|.d...}.n0|.t.
-00000c90: 6b02 9001 7296 7412 7c00 7c04 7c11 7c0e  k...r.t.|.|.|.|.
-00000ca0: 7c0f 7c10 7c07 641c 8d07 7d00 6e0e 7405  |.|.|.d...}.n.t.
-00000cb0: 641d a013 7c01 a101 8301 8201 7c00 6a14  d...|.......|.j.
-00000cc0: 641e 7c05 641f 8d02 0100 7c05 9001 73ce  d.|.d.....|...s.
-00000cd0: 7c00 6a15 6700 641e 7c03 7c02 7c03 1700  |.j.g.d.|.|.|...
-00000ce0: 6420 8d04 7d00 7c00 5300 2921 7a24 5061  d ..}.|.S.)!z$Pa
-00000cf0: 7274 6974 696f 6e73 2061 2050 6879 7369  rtitions a Physi
-00000d00: 6361 6c20 4772 6170 6820 5465 6d70 6c61  cal Graph Templa
-00000d10: 7465 7a3c 556e 6b6e 6f77 6e20 7061 7274  tez<Unknown part
-00000d20: 6974 696f 6e69 6e67 2061 6c67 6f72 6974  itioning algorit
-00000d30: 686d 3a20 2573 2e20 4b6e 6f77 6e20 616c  hm: %s. Known al
-00000d40: 676f 7269 7468 6d73 2061 7265 3a20 2572  gorithms are: %r
-00000d50: 7a38 556e 6b6e 6f77 6e20 7061 7274 6974  z8Unknown partit
-00000d60: 696f 6e20 616c 676f 7269 7468 6d3a 2025  ion algorithm: %
-00000d70: 642e 204b 6e6f 776e 2061 6c67 6f72 6974  d. Known algorit
-00000d80: 686d 2061 7265 3a20 2572 7a54 5275 6e6e  hm are: %rzTRunn
-00000d90: 696e 6720 7061 7274 6974 696f 6e69 6e67  ing partitioning
-00000da0: 2077 6974 6820 616c 676f 7269 7468 6d3d   with algorithm=
-00000db0: 2573 2c20 2564 2070 6172 7469 7469 6f6e  %s, %d partition
-00000dc0: 732c 2025 6420 6973 6c61 6e64 732c 2061  s, %d islands, a
-00000dd0: 6e64 2070 6172 616d 6574 6572 733d 2572  nd parameters=%r
-00000de0: 54da 086d 696e 5f67 6f61 6c72 0200 0000  T..min_goalr....
-00000df0: da05 7074 7970 65da 0c6d 6178 5f6c 6f61  ..ptype..max_loa
-00000e00: 645f 696d 62e9 5a00 0000 da07 6d61 785f  d_imb.Z.....max_
-00000e10: 6370 75e9 0800 0000 da07 6d61 785f 6d65  cpu.......max_me
-00000e20: 6d69 e803 0000 da0b 7469 6d65 5f67 7265  mi......time_gre
-00000e30: 6564 79e9 3200 0000 da08 6465 6164 6c69  edy.2.....deadli
-00000e40: 6e65 4eda 0474 6f70 6be9 1e00 0000 da0a  neN..topk.......
-00000e50: 7377 6172 6d5f 7369 7a65 e928 0000 0029  swarm_size.(...)
-00000e60: 02da 086e 756d 5f63 7075 735a 096d 656d  ...num_cpusZ.mem
-00000e70: 5f75 7361 6765 e964 0000 0072 3b00 0000  _usage.d...r;...
-00000e80: 2901 da0b 6d65 7267 655f 7061 7274 7367  )...merge_partsg
-00000e90: 0000 0000 0000 5940 2902 725f 0000 005a  ......Y@).r_...Z
-00000ea0: 116f 7074 696d 6973 7469 635f 6661 6374  .optimistic_fact
-00000eb0: 6f72 2904 7258 0000 0072 5900 0000 725b  or).rX...rY...r[
-00000ec0: 0000 0072 5f00 0000 7a20 556e 6b6e 6f77  ...r_...z Unknow
-00000ed0: 6e20 7061 7274 6974 696f 6e20 616c 676f  n partition algo
-00000ee0: 7269 7468 6d3a 207b 307d 4629 025a 0a73  rithm: {0}F).Z.s
-00000ef0: 7472 696e 675f 7265 705a 0676 6973 7561  tring_repZ.visua
-00000f00: 6c29 03da 0772 6574 5f73 7472 da0b 6e75  l)...ret_str..nu
-00000f10: 6d5f 6973 6c61 6e64 73da 0d74 706c 5f6e  m_islands..tpl_n
-00000f20: 6f64 6573 5f6c 656e 2916 721b 0000 0072  odes_len).r....r
-00000f30: 2400 0000 7245 0000 00da 0a56 616c 7565  $...rE.....Value
-00000f40: 4572 726f 7272 4600 0000 7204 0000 0072  ErrorrF...r....r
-00000f50: 2100 0000 7222 0000 0072 4d00 0000 da09  !...r"...rM.....
-00000f60: 414c 474f 5f4e 4f4e 4572 0500 0000 da0a  ALGO_NONEr......
-00000f70: 414c 474f 5f4d 4554 4953 7206 0000 00da  ALGO_METISr.....
-00000f80: 0e41 4c47 4f5f 4d59 5f53 4152 4b41 5272  .ALGO_MY_SARKARr
-00000f90: 0700 0000 da12 414c 474f 5f4d 494e 5f4e  ......ALGO_MIN_N
-00000fa0: 554d 5f50 4152 5453 7208 0000 00da 0841  UM_PARTSr......A
-00000fb0: 4c47 4f5f 5053 4f72 0900 0000 da06 666f  LGO_PSOr......fo
-00000fc0: 726d 6174 5a0c 746f 5f67 6f6a 735f 6a73  rmatZ.to_gojs_js
-00000fd0: 6f6e da0a 746f 5f70 675f 7370 6563 2913  on..to_pg_spec).
-00000fe0: da03 7067 74da 0461 6c67 6fda 0e6e 756d  ..pgt..algo..num
-00000ff0: 5f70 6172 7469 7469 6f6e 7372 6100 0000  _partitionsra...
-00001000: da0f 7061 7274 6974 696f 6e5f 6c61 6265  ..partition_labe
-00001010: 6c5a 0973 686f 775f 676f 6a73 7249 0000  lZ.show_gojsrI..
-00001020: 005a 0b63 6f75 6c64 5f6d 6572 6765 724f  .Z.could_mergerO
-00001030: 0000 0072 5000 0000 7251 0000 0072 5300  ...rP...rQ...rS.
-00001040: 0000 7255 0000 0072 5600 0000 7258 0000  ..rU...rV...rX..
-00001050: 0072 5900 0000 725b 0000 005a 076d 6178  .rY...r[...Z.max
-00001060: 5f64 6f70 5a07 7566 6163 746f 7272 1100  _dopZ.ufactorr..
-00001070: 0000 7211 0000 0072 1200 0000 724e 0000  ..r....r....rN..
-00001080: 0081 0000 0073 ac00 0000 000b 0a01 0801  .....s..........
-00001090: 0201 0201 0aff 02ff 0404 0802 0801 0201  ................
-000010a0: 0201 0aff 02ff 0405 0401 0202 0601 0201  ................
-000010b0: 0201 02fa 040c 0401 0c01 0c01 0c01 0c01  ................
-000010c0: 0c01 0c01 0c01 0c01 0c02 0a02 0801 0a02  ................
-000010d0: 0a01 0c01 0a01 0401 0201 0201 0201 0201  ................
-000010e0: 0201 0201 0201 02f9 080a 0a01 0201 0201  ................
-000010f0: 0201 0201 0201 02fb 0808 0a01 0c01 0201  ................
-00001100: 0201 0201 0201 0201 0201 0201 02f9 080a  ................
-00001110: 0a01 0201 0201 0201 0201 0201 0201 0201  ................
-00001120: 02f9 080b 0e02 0e01 0601 0401 0201 0201  ................
-00001130: 0201 06fc 0606 5463 0400 0000 0000 0000  ......Tc........
-00001140: 0000 0000 0a00 0000 0800 0000 4300 0000  ............C...
-00001150: 73b2 0000 0074 00a0 0164 017c 019b 0064  s....t...d.|...d
-00001160: 027c 029b 0064 037c 039b 009d 06a1 0101  .|...d.|........
-00001170: 007c 0173 2c64 047d 0474 027c 0483 0182  .|.s,d.}.t.|....
-00001180: 017c 0164 057c 0285 0219 007d 057c 017c  .|.d.|.....}.|.|
-00001190: 0264 0685 0219 007d 0674 037c 0064 0519  .d.....}.t.|.d..
-000011a0: 0083 0174 046b 0872 5c7c 0064 0719 007d  ...t.k.r\|.d...}
-000011b0: 007c 0044 005d 4c7d 077c 0769 006b 0372  .|.D.]L}.|.i.k.r
-000011c0: 6074 057c 0764 0819 0064 0764 0685 0219  `t.|.d...d.d....
-000011d0: 0083 017d 087c 067c 0819 007c 0764 083c  ...}.|.|...|.d.<
-000011e0: 0074 057c 0764 0919 0064 0764 0685 0219  .t.|.d...d.d....
-000011f0: 0083 017d 097c 057c 0919 007c 0764 093c  ...}.|.|...|.d.<
-00001200: 0071 607c 0053 0029 0a7a 2f4d 6170 7320  .q`|.S.).z/Maps 
-00001210: 6120 5068 7973 6963 616c 2047 7261 7068  a Physical Graph
-00001220: 2054 656d 706c 6174 6520 6070 6774 6020   Template `pgt` 
-00001230: 746f 2060 6e6f 6465 7360 7a24 5265 736f  to `nodes`z$Reso
-00001240: 7572 6365 206d 6170 7069 6e67 2063 616c  urce mapping cal
-00001250: 6c65 6420 7769 7468 206e 6f64 6573 3a20  led with nodes: 
-00001260: 7a0b 2c20 6973 6c61 6e64 733a 207a 1220  z., islands: z. 
-00001270: 616e 6420 636f 5f68 6f73 745f 6469 6d3a  and co_host_dim:
-00001280: 207a 2b45 6d70 7479 206e 6f64 655f 6c69   z+Empty node_li
-00001290: 7374 2c20 6361 6e6e 6f74 206d 6170 2074  st, cannot map t
-000012a0: 6865 2050 4720 7465 6d70 6c61 7465 7202  he PG templater.
-000012b0: 0000 004e 723b 0000 00da 046e 6f64 65da  ...Nr;.....node.
-000012c0: 0669 736c 616e 6429 0672 2100 0000 7222  .island).r!...r"
-000012d0: 0000 0072 6300 0000 da04 7479 7065 7224  ...rc.....typer$
-000012e0: 0000 00da 0369 6e74 290a 726b 0000 00da  .....int).rk....
-000012f0: 056e 6f64 6573 7261 0000 00da 0b63 6f5f  .nodesra.....co_
-00001300: 686f 7374 5f64 696d 5a08 6572 725f 696e  host_dimZ.err_in
-00001310: 666f 5a08 6469 6d5f 6c69 7374 5a07 6e6d  foZ.dim_listZ.nm
-00001320: 5f6c 6973 745a 0964 726f 705f 7370 6563  _listZ.drop_spec
-00001330: 5a04 6e69 6478 5a04 6969 6478 7211 0000  Z.nidxZ.iidxr...
-00001340: 0072 1100 0000 7212 0000 00da 0c72 6573  .r....r......res
-00001350: 6f75 7263 655f 6d61 70f2 0000 0073 2200  ource_map....s".
-00001360: 0000 0003 0401 14ff 0403 0401 0401 0803  ................
-00001370: 0c01 0c01 1001 0801 0801 0801 1401 0c01  ................
-00001380: 1401 0e02 7275 0000 0029 034e 464e 2904  ....ru...).NFN).
-00001390: 723b 0000 0072 3b00 0000 724e 0000 0046  r;...r;...rN...F
-000013a0: 2902 723b 0000 0054 2922 da07 5f5f 646f  ).r;...T)"..__do
-000013b0: 635f 5f72 0c00 0000 da0b 5f5f 7061 636b  c__r......__pack
-000013c0: 6167 655f 5f72 2500 0000 da07 6c6f 6767  age__r%.....logg
-000013d0: 696e 67da 0673 7472 696e 6772 3200 0000  ing..stringr2...
-000013e0: da0f 646c 672e 6472 6f70 6d61 6b65 2e6c  ..dlg.dropmake.l
-000013f0: 6772 0300 0000 7204 0000 005a 1064 6c67  gr....r....Z.dlg
-00001400: 2e64 726f 706d 616b 652e 7067 7472 0500  .dropmake.pgtr..
-00001410: 0000 5a11 646c 672e 6472 6f70 6d61 6b65  ..Z.dlg.dropmake
-00001420: 2e70 6774 7072 0600 0000 7207 0000 0072  .pgtpr....r....r
-00001430: 0800 0000 7209 0000 00da 0967 6574 4c6f  ....r......getLo
-00001440: 6767 6572 7221 0000 00da 0854 656d 706c  ggerr!.....Templ
-00001450: 6174 6572 0a00 0000 721c 0000 0072 2b00  ater....r....r+.
-00001460: 0000 723a 0000 0072 6400 0000 7265 0000  ..r:...rd...re..
-00001470: 0072 6600 0000 7267 0000 0072 6800 0000  .rf...rg...rh...
-00001480: 7245 0000 0072 4700 0000 724d 0000 0072  rE...rG...rM...r
-00001490: 4e00 0000 7275 0000 0072 1100 0000 7211  N...ru...r....r.
-000014a0: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
-000014b0: 6d6f 6475 6c65 3e16 0000 0073 6000 0000  module>....s`...
-000014c0: 0406 0801 0402 0801 0801 0801 0802 1001  ................
-000014d0: 0c01 1802 0a03 1205 080b 080c 0a1a 0401  ................
-000014e0: 0401 0401 0401 0403 0200 0201 0200 0201  ................
-000014f0: 0200 0201 0200 0201 0200 0201 0200 0201  ................
-00001500: 0200 0201 0200 0201 0200 0201 0200 02f6  ................
-00001510: 040e 0804 080b 0001 0001 0001 00fa 0a71  ...............q
+00000330: 0072 1100 0000 fa4a 2f68 6f6d 652f 6177  .r.....J/home/aw
+00000340: 6963 656e 6563 2f67 6974 2f64 616c 6975  icenec/git/daliu
+00000350: 6765 2f64 616c 6975 6765 2d74 7261 6e73  ge/daliuge-trans
+00000360: 6c61 746f 722f 646c 672f 6472 6f70 6d61  lator/dlg/dropma
+00000370: 6b65 2f70 675f 6765 6e65 7261 746f 722e  ke/pg_generator.
+00000380: 7079 720a 0000 002b 0000 0073 0400 0000  pyr....+...s....
+00000390: 0801 0401 720a 0000 0063 0100 0000 0000  ....r....c......
+000003a0: 0000 0000 0000 0400 0000 0600 0000 0300  ................
+000003b0: 0000 7356 0000 0074 007c 0083 017d 017c  ..sV...t.|...}.|
+000003c0: 00a0 01a1 0044 005d 405c 0289 007d 0274  .....D.]@\...}.t
+000003d0: 027c 0274 0083 0272 4874 037c 0283 017d  .|.t...rHt.|...}
+000003e0: 037c 01a0 0487 0066 0164 0164 0284 087c  .|.....f.d.d...|
+000003f0: 03a0 01a1 0044 0083 01a1 0101 0071 107c  .....D.......q.|
+00000400: 027c 0188 003c 0071 107c 0153 0029 034e  .|...<.q.|.S.).N
+00000410: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000420: 0005 0000 0013 0000 0073 1e00 0000 6900  .........s....i.
+00000430: 7c00 5d16 5c02 7d01 7d02 6400 8800 7c01  |.].\.}.}.d...|.
+00000440: 6602 1600 7c02 9302 7104 5300 2901 7a05  f...|...q.S.).z.
+00000450: 2573 2e25 7372 1100 0000 2903 da02 2e30  %s.%sr....)....0
+00000460: da01 6bda 0176 a901 da03 6b65 7972 1100  ..k..v....keyr..
+00000470: 0000 7212 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
+00000480: 6d70 3e35 0000 0073 0600 0000 0600 0600  mp>5...s........
+00000490: 0a00 7a21 5f66 6c61 7474 656e 5f64 6963  ..z!_flatten_dic
+000004a0: 742e 3c6c 6f63 616c 733e 2e3c 6469 6374  t.<locals>.<dict
+000004b0: 636f 6d70 3e29 05da 0464 6963 74da 0569  comp>)...dict..i
+000004c0: 7465 6d73 da0a 6973 696e 7374 616e 6365  tems..isinstance
+000004d0: da0d 5f66 6c61 7474 656e 5f64 6963 74da  .._flatten_dict.
+000004e0: 0675 7064 6174 6529 04da 0164 da04 666c  .update)...d..fl
+000004f0: 6174 da05 7661 6c75 655a 0966 6c61 7474  at..valueZ.flatt
+00000500: 656e 6564 7211 0000 0072 1600 0000 7212  enedr....r....r.
+00000510: 0000 0072 1c00 0000 3000 0000 730e 0000  ...r....0...s...
+00000520: 0000 0108 0110 010a 0108 011e 020a 0172  ...............r
+00000530: 1c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000540: 0003 0000 0004 0000 0043 0000 0073 5400  .........C...sT.
+00000550: 0000 7400 a001 6401 7c01 a102 0100 7402  ..t...d.|.....t.
+00000560: 7c01 8301 7d02 7403 7c00 6402 8302 7228  |...}.t.|.d...r(
+00000570: 7c00 a004 a100 7d00 6e14 7405 7c00 7406  |.....}.n.t.|.t.
+00000580: 8302 733c 7407 a008 7c00 a101 7d00 7409  ..s<t...|...}.t.
+00000590: 7c00 8301 a00a 7c02 a101 7d00 7407 a00b  |.....|...}.t...
+000005a0: 7c00 a101 5300 2903 7a2e 4c6f 6769 6361  |...S.).z.Logica
+000005b0: 6c20 4772 6170 6820 2b20 7061 7261 6d73  l Graph + params
+000005c0: 202d 3e20 4669 6c6c 6564 204c 6f67 6963   -> Filled Logic
+000005d0: 616c 2047 7261 7068 7a29 4669 6c6c 696e  al Graphz)Fillin
+000005e0: 6720 4c6f 6769 6361 6c20 4772 6170 6820  g Logical Graph 
+000005f0: 7769 7468 2070 6172 616d 6574 6572 733a  with parameters:
+00000600: 2025 72da 0472 6561 6429 0cda 066c 6f67   %r..read)...log
+00000610: 6765 72da 0469 6e66 6f72 1c00 0000 da07  ger..infor......
+00000620: 6861 7361 7474 7272 2100 0000 721b 0000  hasattrr!...r...
+00000630: 00da 0373 7472 da04 6a73 6f6e da05 6475  ...str..json..du
+00000640: 6d70 7372 0a00 0000 da0a 7375 6273 7469  mpsr......substi
+00000650: 7475 7465 da05 6c6f 6164 7329 03da 026c  tute..loads)...l
+00000660: 67da 0670 6172 616d 735a 0b66 6c61 745f  g..paramsZ.flat_
+00000670: 7061 7261 6d73 7211 0000 0072 1100 0000  paramsr....r....
+00000680: 7212 0000 00da 0466 696c 6c3b 0000 0073  r......fill;...s
+00000690: 1000 0000 0002 0c01 0801 0a01 0a01 0a01  ................
+000006a0: 0a01 0e01 722c 0000 0046 6304 0000 0000  ....r,...Fc.....
+000006b0: 0000 0000 0000 0007 0000 0004 0000 0043  ...............C
+000006c0: 0000 0073 9800 0000 7400 a000 a100 7d04  ...s....t.....}.
+000006d0: 7401 7c00 7c01 6401 8d02 7d00 7c00 a002  t.|.|.d...}.|...
+000006e0: a100 7d05 7c02 723a 7c05 4400 5d14 7d06  ..}.|.r:|.D.].}.
+000006f0: 6402 7c06 6b06 7224 6403 7c06 6402 3c00  d.|.k.r$d.|.d.<.
+00000700: 7124 7c03 7288 7403 a004 6404 7c03 a102  q$|.r.t...d.|...
+00000710: 0100 7c05 4400 5d38 7d06 6405 7c06 6b06  ..|.D.]8}.d.|.k.
+00000720: 724e 7c06 6406 1900 6407 6b02 724e 7c03  rN|.d...d.k.rN|.
+00000730: 7c06 6405 3c00 6408 7c06 6b06 727e 7c06  |.d.<.d.|.k.r~|.
+00000740: 6408 1900 6e02 6409 7c06 6402 3c00 714e  d...n.d.|.d.<.qN
+00000750: 7c05 a005 7c00 6a06 a101 0100 7c05 5300  |...|.j.....|.S.
+00000760: 290a 7a17 556e 726f 6c6c 7320 6120 6c6f  ).z.Unrolls a lo
+00000770: 6769 6361 6c20 6772 6170 6829 015a 0473  gical graph).Z.s
+00000780: 7369 645a 0a73 6c65 6570 5f74 696d 6572  sidZ.sleep_timer
+00000790: 0200 0000 7a16 5265 706c 6163 696e 6720  ....z.Replacing 
+000007a0: 6170 7073 2077 6974 6820 2573 5a09 6472  apps with %sZ.dr
+000007b0: 6f70 636c 6173 73da 0c63 6174 6567 6f72  opclass..categor
+000007c0: 7954 7970 65da 0b41 7070 6c69 6361 7469  yType..Applicati
+000007d0: 6f6e 5a0e 6578 6563 7574 696f 6e5f 7469  onZ.execution_ti
+000007e0: 6d65 e902 0000 0029 07da 0474 696d 6572  me.....)...timer
+000007f0: 0300 0000 5a0d 756e 726f 6c6c 5f74 6f5f  ....Z.unroll_to_
+00000800: 7470 6c72 2200 0000 7223 0000 00da 0661  tplr"...r#.....a
+00000810: 7070 656e 645a 0972 6570 726f 6461 7461  ppendZ.reprodata
+00000820: 2907 722a 0000 005a 0a6f 6964 5f70 7265  ).r*...Z.oid_pre
+00000830: 6669 785a 077a 6572 6f72 756e da03 6170  fixZ.zerorun..ap
+00000840: 70da 0573 7461 7274 5a09 6472 6f70 5f6c  p..startZ.drop_l
+00000850: 6973 74da 0864 726f 7073 7065 6372 1100  ist..dropspecr..
+00000860: 0000 7211 0000 0072 1200 0000 da06 756e  ..r....r......un
+00000870: 726f 6c6c 4700 0000 7320 0000 0000 0208  rollG...s ......
+00000880: 010c 0108 0104 0108 0108 010a 0104 010c  ................
+00000890: 0108 0114 0108 0212 ff08 030c 0172 3500  .............r5.
+000008a0: 0000 e901 0000 0072 2f00 0000 e903 0000  .......r/.......
+000008b0: 00e9 0400 0000 da04 6e6f 6e65 5a05 6d65  ........noneZ.me
+000008c0: 7469 735a 086d 7973 6172 6b61 725a 0d6d  tisZ.mysarkarZ.m
+000008d0: 696e 5f6e 756d 5f70 6172 7473 5a03 7073  in_num_partsZ.ps
+000008e0: 6f63 0000 0000 0000 0000 0000 0000 0000  oc..............
+000008f0: 0000 0300 0000 4300 0000 7312 0000 0064  ......C...s....d
+00000900: 0164 0284 0074 00a0 01a1 0044 0083 0153  .d...t.....D...S
+00000910: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000920: 0002 0000 0005 0000 0053 0000 0073 1a00  .........S...s..
+00000930: 0000 6700 7c00 5d12 7d01 7400 7c01 7401  ..g.|.].}.t.|.t.
+00000940: 8302 7204 7c01 9102 7104 5300 7211 0000  ..r.|...q.S.r...
+00000950: 0029 0272 1b00 0000 7225 0000 0029 0272  .).r....r%...).r
+00000960: 1300 0000 da01 7872 1100 0000 7211 0000  ......xr....r...
+00000970: 0072 1200 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000980: 703e 7100 0000 7306 0000 0006 0002 000a  p>q...s.........
+00000990: 007a 246b 6e6f 776e 5f61 6c67 6f72 6974  .z$known_algorit
+000009a0: 686d 732e 3c6c 6f63 616c 733e 2e3c 6c69  hms.<locals>.<li
+000009b0: 7374 636f 6d70 3e29 02da 0c5f 6b6e 6f77  stcomp>)..._know
+000009c0: 6e5f 616c 676f 73da 046b 6579 7372 1100  n_algos..keysr..
+000009d0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000009e0: 00da 106b 6e6f 776e 5f61 6c67 6f72 6974  ...known_algorit
+000009f0: 686d 7370 0000 0073 0200 0000 0001 723e  hmsp...s......r>
+00000a00: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000a10: 0400 0000 0300 0000 4300 0000 731a 0000  ........C...s...
+00000a20: 007c 00a0 007c 01a1 017d 037c 0364 016b  .|...|...}.|.d.k
+00000a30: 0972 167c 0353 007c 0253 0029 027a 4e0a  .r.|.S.|.S.).zN.
+00000a40: 2020 2020 4d61 6b65 2073 7572 6520 7468      Make sure th
+00000a50: 6174 2064 6566 6175 6c74 2069 7320 7365  at default is se
+00000a60: 7420 6576 656e 2069 6620 7661 6c75 6520  t even if value 
+00000a70: 6861 7320 6265 656e 2070 6173 7365 6420  has been passed 
+00000a80: 6173 204e 6f6e 652e 0a20 2020 204e 2901  as None..    N).
+00000a90: da03 6765 7429 04da 0b61 6c67 6f5f 7061  ..get)...algo_pa
+00000aa0: 7261 6d73 da0a 7061 7261 6d5f 6e61 6d65  rams..param_name
+00000ab0: da07 6465 6661 756c 74da 0570 6172 616d  ..default..param
+00000ac0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000ad0: 0f5f 6765 745f 616c 676f 5f70 6172 616d  ._get_algo_param
+00000ae0: 7400 0000 7304 0000 0000 040a 0172 4400  t...s........rD.
+00000af0: 0000 da09 7061 7274 6974 696f 6e63 0600  ....partitionc..
+00000b00: 0000 0000 0000 0000 0000 1300 0000 0900  ................
+00000b10: 0000 4b00 0000 73d2 0100 0074 007c 0174  ..K...s....t.|.t
+00000b20: 0183 0272 2e7c 0174 026b 0772 2674 0364  ...r.|.t.k.r&t.d
+00000b30: 017c 0174 02a0 04a1 0066 0216 0083 0182  .|.t.....f......
+00000b40: 0174 027c 0119 007d 017c 0174 026b 0772  .t.|...}.|.t.k.r
+00000b50: 4a74 0564 027c 0174 02a0 04a1 0066 0216  Jt.d.|.t.....f..
+00000b60: 0083 0182 0174 06a0 0764 0374 027c 0119  .....t...d.t.|..
+00000b70: 007c 027c 037c 06a1 0501 0064 047d 0774  .|.|.|.....d.}.t
+00000b80: 087c 0664 0564 0683 037d 0874 087c 0664  .|.d.d...}.t.|.d
+00000b90: 0764 0683 037d 0974 087c 0664 0864 0983  .d...}.t.|.d.d..
+00000ba0: 037d 0a74 087c 0664 0a64 0b83 037d 0b74  .}.t.|.d.d...}.t
+00000bb0: 087c 0664 0c64 0d83 037d 0c74 087c 0664  .|.d.d...}.t.|.d
+00000bc0: 0e64 0f83 037d 0d74 087c 0664 1064 1183  .d...}.t.|.d.d..
+00000bd0: 037d 0e74 087c 0664 1264 1383 037d 0f74  .}.t.|.d.d...}.t
+00000be0: 087c 0664 1464 1583 037d 107c 0b7c 0c64  .|.d.d...}.|.|.d
+00000bf0: 169c 027d 117c 0174 096b 0272 ec74 0a7c  ...}.|.t.k.r.t.|
+00000c00: 0083 017d 006e b87c 0174 0b6b 0290 0172  ...}.n.|.t.k...r
+00000c10: 2864 177c 0a18 0064 1817 007d 127c 1264  (d.|...d...}.|.d
+00000c20: 066b 0190 0172 1064 187d 1274 0c7c 007c  .k...r.d.}.t.|.|
+00000c30: 027c 087c 047c 097c 127c 0764 198d 077d  .|.|.|.|.|.d...}
+00000c40: 006e 7c7c 0174 0d6b 0290 0172 4674 0e7c  .n||.t.k...rFt.|
+00000c50: 007c 027c 047c 117c 0764 198d 057d 006e  .|.|.|.|.d...}.n
+00000c60: 5e7c 0174 0f6b 0290 0172 7464 187c 0d64  ^|.t.k...rtd.|.d
+00000c70: 1a1b 0018 007d 0d74 107c 007c 0e7c 027c  .....}.t.|.|.|.|
+00000c80: 047c 0b7c 077c 0d64 1b8d 077d 006e 307c  .|.|.|.d...}.n0|
+00000c90: 0174 116b 0290 0172 9674 127c 007c 047c  .t.k...r.t.|.|.|
+00000ca0: 117c 0e7c 0f7c 107c 0764 1c8d 077d 006e  .|.|.|.|.d...}.n
+00000cb0: 0e74 0564 1da0 137c 01a1 0183 0182 017c  .t.d...|.......|
+00000cc0: 006a 1464 1e7c 0564 1f8d 0201 007c 0590  .j.d.|.d.....|..
+00000cd0: 0173 ce7c 006a 1567 0064 1e7c 037c 027c  .s.|.j.g.d.|.|.|
+00000ce0: 0317 0064 208d 047d 007c 0053 0029 217a  ...d ..}.|.S.)!z
+00000cf0: 2450 6172 7469 7469 6f6e 7320 6120 5068  $Partitions a Ph
+00000d00: 7973 6963 616c 2047 7261 7068 2054 656d  ysical Graph Tem
+00000d10: 706c 6174 657a 3c55 6e6b 6e6f 776e 2070  platez<Unknown p
+00000d20: 6172 7469 7469 6f6e 696e 6720 616c 676f  artitioning algo
+00000d30: 7269 7468 6d3a 2025 732e 204b 6e6f 776e  rithm: %s. Known
+00000d40: 2061 6c67 6f72 6974 686d 7320 6172 653a   algorithms are:
+00000d50: 2025 727a 3855 6e6b 6e6f 776e 2070 6172   %rz8Unknown par
+00000d60: 7469 7469 6f6e 2061 6c67 6f72 6974 686d  tition algorithm
+00000d70: 3a20 2564 2e20 4b6e 6f77 6e20 616c 676f  : %d. Known algo
+00000d80: 7269 7468 6d20 6172 653a 2025 727a 5452  rithm are: %rzTR
+00000d90: 756e 6e69 6e67 2070 6172 7469 7469 6f6e  unning partition
+00000da0: 696e 6720 7769 7468 2061 6c67 6f72 6974  ing with algorit
+00000db0: 686d 3d25 732c 2025 6420 7061 7274 6974  hm=%s, %d partit
+00000dc0: 696f 6e73 2c20 2564 2069 736c 616e 6473  ions, %d islands
+00000dd0: 2c20 616e 6420 7061 7261 6d65 7465 7273  , and parameters
+00000de0: 3d25 7254 da08 6d69 6e5f 676f 616c 7202  =%rT..min_goalr.
+00000df0: 0000 00da 0570 7479 7065 da0c 6d61 785f  .....ptype..max_
+00000e00: 6c6f 6164 5f69 6d62 e95a 0000 00da 076d  load_imb.Z.....m
+00000e10: 6178 5f63 7075 e908 0000 00da 076d 6178  ax_cpu.......max
+00000e20: 5f6d 656d 69e8 0300 00da 0b74 696d 655f  _memi......time_
+00000e30: 6772 6565 6479 e932 0000 00da 0864 6561  greedy.2.....dea
+00000e40: 646c 696e 654e da04 746f 706b e91e 0000  dlineN..topk....
+00000e50: 00da 0a73 7761 726d 5f73 697a 65e9 2800  ...swarm_size.(.
+00000e60: 0000 2902 5a08 6e75 6d5f 6370 7573 5a09  ..).Z.num_cpusZ.
+00000e70: 6d65 6d5f 7573 6167 65e9 6400 0000 7236  mem_usage.d...r6
+00000e80: 0000 0029 01da 0b6d 6572 6765 5f70 6172  ...)...merge_par
+00000e90: 7473 6700 0000 0000 0059 4029 0272 5500  tsg......Y@).rU.
+00000ea0: 0000 5a11 6f70 7469 6d69 7374 6963 5f66  ..Z.optimistic_f
+00000eb0: 6163 746f 7229 0472 4f00 0000 7250 0000  actor).rO...rP..
+00000ec0: 0072 5200 0000 7255 0000 007a 2055 6e6b  .rR...rU...z Unk
+00000ed0: 6e6f 776e 2070 6172 7469 7469 6f6e 2061  nown partition a
+00000ee0: 6c67 6f72 6974 686d 3a20 7b30 7d46 2902  lgorithm: {0}F).
+00000ef0: 5a0a 7374 7269 6e67 5f72 6570 5a06 7669  Z.string_repZ.vi
+00000f00: 7375 616c 2903 5a07 7265 745f 7374 72da  sual).Z.ret_str.
+00000f10: 0b6e 756d 5f69 736c 616e 6473 5a0d 7470  .num_islandsZ.tp
+00000f20: 6c5f 6e6f 6465 735f 6c65 6e29 1672 1b00  l_nodes_len).r..
+00000f30: 0000 7225 0000 0072 3c00 0000 da0a 5661  ..r%...r<.....Va
+00000f40: 6c75 6545 7272 6f72 723d 0000 0072 0400  lueErrorr=...r..
+00000f50: 0000 7222 0000 0072 2300 0000 7244 0000  ..r"...r#...rD..
+00000f60: 00da 0941 4c47 4f5f 4e4f 4e45 7205 0000  ...ALGO_NONEr...
+00000f70: 00da 0a41 4c47 4f5f 4d45 5449 5372 0600  ...ALGO_METISr..
+00000f80: 0000 da0e 414c 474f 5f4d 595f 5341 524b  ....ALGO_MY_SARK
+00000f90: 4152 7207 0000 00da 1241 4c47 4f5f 4d49  ARr......ALGO_MI
+00000fa0: 4e5f 4e55 4d5f 5041 5254 5372 0800 0000  N_NUM_PARTSr....
+00000fb0: da08 414c 474f 5f50 534f 7209 0000 00da  ..ALGO_PSOr.....
+00000fc0: 0666 6f72 6d61 745a 0c74 6f5f 676f 6a73  .formatZ.to_gojs
+00000fd0: 5f6a 736f 6e5a 0a74 6f5f 7067 5f73 7065  _jsonZ.to_pg_spe
+00000fe0: 6329 13da 0370 6774 5a04 616c 676f 5a0e  c)...pgtZ.algoZ.
+00000ff0: 6e75 6d5f 7061 7274 6974 696f 6e73 7256  num_partitionsrV
+00001000: 0000 005a 0f70 6172 7469 7469 6f6e 5f6c  ...Z.partition_l
+00001010: 6162 656c 5a09 7368 6f77 5f67 6f6a 7372  abelZ.show_gojsr
+00001020: 4000 0000 5a0b 636f 756c 645f 6d65 7267  @...Z.could_merg
+00001030: 6572 4600 0000 7247 0000 0072 4800 0000  erF...rG...rH...
+00001040: 724a 0000 0072 4c00 0000 724d 0000 0072  rJ...rL...rM...r
+00001050: 4f00 0000 7250 0000 0072 5200 0000 5a07  O...rP...rR...Z.
+00001060: 6d61 785f 646f 705a 0775 6661 6374 6f72  max_dopZ.ufactor
+00001070: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00001080: 4500 0000 7c00 0000 73ac 0000 0000 0b0a  E...|...s.......
+00001090: 0108 0102 0102 010a ff02 ff04 0408 0208  ................
+000010a0: 0102 0102 010a ff02 ff04 0504 0102 0206  ................
+000010b0: 0102 0102 0102 fa04 0c04 010c 010c 010c  ................
+000010c0: 010c 010c 010c 010c 010c 010c 020a 0208  ................
+000010d0: 010a 020a 010c 010a 0104 0102 0102 0102  ................
+000010e0: 0102 0102 0102 0102 0102 f908 0a0a 0102  ................
+000010f0: 0102 0102 0102 0102 0102 fb08 080a 010c  ................
+00001100: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001110: f908 0a0a 0102 0102 0102 0102 0102 0102  ................
+00001120: 0102 0102 f908 0b0e 020e 0106 0104 0102  ................
+00001130: 0102 0102 0106 fc06 0654 6304 0000 0000  .........Tc.....
+00001140: 0000 0000 0000 000a 0000 0008 0000 0043  ...............C
+00001150: 0000 0073 d000 0000 7400 a001 6401 7c01  ...s....t...d.|.
+00001160: 9b00 6402 7c02 9b00 6403 7c03 9b00 9d06  ..d.|...d.|.....
+00001170: a101 0100 7c01 732c 6404 7d04 7402 7c04  ....|.s,d.}.t.|.
+00001180: 8301 8201 7c01 6405 7c02 8502 1900 7d05  ....|.d.|.....}.
+00001190: 7c01 7c02 6406 8502 1900 7d06 7403 7c00  |.|.d.....}.t.|.
+000011a0: 6405 1900 8301 7404 6b08 725c 7c00 6407  d.....t.k.r\|.d.
+000011b0: 1900 7d00 7c00 4400 5d6a 7d07 7c07 6900  ..}.|.D.]j}.|.i.
+000011c0: 6b03 7260 7405 7c07 6408 1900 6407 6406  k.r`t.|.d...d.d.
+000011d0: 8502 1900 8301 7d08 7c06 7c08 1900 7c07  ......}.|.|...|.
+000011e0: 6408 3c00 7405 7c07 6409 1900 6407 6406  d.<.t.|.d...d.d.
+000011f0: 8502 1900 8301 7d09 7c05 7c09 1900 a006  ......}.|.|.....
+00001200: 640a a101 6405 1900 640b 1700 7c07 6409  d...d...d...|.d.
+00001210: 3c00 7400 a007 640c 7c07 6409 1900 a102  <.t...d.|.d.....
+00001220: 0100 7160 7c00 5300 290d 7a2f 4d61 7073  ..q`|.S.).z/Maps
+00001230: 2061 2050 6879 7369 6361 6c20 4772 6170   a Physical Grap
+00001240: 6820 5465 6d70 6c61 7465 2060 7067 7460  h Template `pgt`
+00001250: 2074 6f20 606e 6f64 6573 607a 2452 6573   to `nodes`z$Res
+00001260: 6f75 7263 6520 6d61 7070 696e 6720 6361  ource mapping ca
+00001270: 6c6c 6564 2077 6974 6820 6e6f 6465 733a  lled with nodes:
+00001280: 207a 0b2c 2069 736c 616e 6473 3a20 7a12   z., islands: z.
+00001290: 2061 6e64 2063 6f5f 686f 7374 5f64 696d   and co_host_dim
+000012a0: 3a20 7a2b 456d 7074 7920 6e6f 6465 5f6c  : z+Empty node_l
+000012b0: 6973 742c 2063 616e 6e6f 7420 6d61 7020  ist, cannot map 
+000012c0: 7468 6520 5047 2074 656d 706c 6174 6572  the PG templater
+000012d0: 0200 0000 4e72 3600 0000 da04 6e6f 6465  ....Nr6.....node
+000012e0: 5a06 6973 6c61 6e64 fa01 3a7a 053a 3830  Z.island..:z.:80
+000012f0: 3031 7a0a 4973 6c61 6e64 3a20 2573 2908  01z.Island: %s).
+00001300: 7222 0000 0072 2300 0000 7257 0000 00da  r"...r#...rW....
+00001310: 0474 7970 6572 2500 0000 da03 696e 74da  .typer%.....int.
+00001320: 0573 706c 6974 da05 6465 6275 6729 0a72  .split..debug).r
+00001330: 5e00 0000 da05 6e6f 6465 7372 5600 0000  ^.....nodesrV...
+00001340: 5a0b 636f 5f68 6f73 745f 6469 6d5a 0865  Z.co_host_dimZ.e
+00001350: 7272 5f69 6e66 6f5a 0864 696d 5f6c 6973  rr_infoZ.dim_lis
+00001360: 745a 076e 6d5f 6c69 7374 5a09 6472 6f70  tZ.nm_listZ.drop
+00001370: 5f73 7065 635a 046e 6964 785a 0469 6964  _specZ.nidxZ.iid
+00001380: 7872 1100 0000 7211 0000 0072 1200 0000  xr....r....r....
+00001390: da0c 7265 736f 7572 6365 5f6d 6170 ed00  ..resource_map..
+000013a0: 0000 7326 0000 0000 0304 0114 ff04 0304  ..s&............
+000013b0: 0104 0108 030c 010c 0110 0108 0108 0108  ................
+000013c0: 0114 010c 0114 0214 ff06 0312 0272 6600  .............rf.
+000013d0: 0000 2903 4e46 4e29 0472 3600 0000 7236  ..).NFN).r6...r6
+000013e0: 0000 0072 4500 0000 4629 0272 3600 0000  ...rE...F).r6...
+000013f0: 5429 22da 075f 5f64 6f63 5f5f 720c 0000  T)"..__doc__r...
+00001400: 00da 0b5f 5f70 6163 6b61 6765 5f5f 7226  ...__package__r&
+00001410: 0000 00da 076c 6f67 6769 6e67 da06 7374  .....logging..st
+00001420: 7269 6e67 7230 0000 005a 0f64 6c67 2e64  ringr0...Z.dlg.d
+00001430: 726f 706d 616b 652e 6c67 7203 0000 0072  ropmake.lgr....r
+00001440: 0400 0000 5a10 646c 672e 6472 6f70 6d61  ....Z.dlg.dropma
+00001450: 6b65 2e70 6774 7205 0000 005a 1164 6c67  ke.pgtr....Z.dlg
+00001460: 2e64 726f 706d 616b 652e 7067 7470 7206  .dropmake.pgtpr.
+00001470: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
+00001480: 0000 da09 6765 744c 6f67 6765 7272 2200  ....getLoggerr".
+00001490: 0000 da08 5465 6d70 6c61 7465 720a 0000  ....Templater...
+000014a0: 0072 1c00 0000 722c 0000 0072 3500 0000  .r....r,...r5...
+000014b0: 7258 0000 0072 5900 0000 725a 0000 0072  rX...rY...rZ...r
+000014c0: 5b00 0000 725c 0000 0072 3c00 0000 723e  [...r\...r<...r>
+000014d0: 0000 0072 4400 0000 7245 0000 0072 6600  ...rD...rE...rf.
+000014e0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+000014f0: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001500: 1600 0000 7360 0000 0004 0608 0104 0208  ....s`..........
+00001510: 0108 0108 0108 0210 010c 0118 020a 0312  ................
+00001520: 0508 0b08 0c0a 1504 0104 0104 0104 0104  ................
+00001530: 0302 0002 0102 0002 0102 0002 0102 0002  ................
+00001540: 0102 0002 0102 0002 0102 0002 0102 0002  ................
+00001550: 0102 0002 0102 0002 f604 0e08 0408 0b00  ................
+00001560: 0100 0100 0100 fa0a 71                   ........q
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_generator.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_generator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pg_manager.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pg_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Feb 15 06:56:33 2024 UTC, .py size: 17876 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a1b5 cd65 d445 0000  U..........e.E..
+00000000: 550d 0d0a 0000 0000 98c0 1c66 6645 0000  U..........ffE..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6501 6401 6b02 7210 6402 5a02 6403  Z.e.d.k.r.d.Z.d.
 00000040: 6404 6c03 5a03 6403 6404 6c04 5a04 6403  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 5a05 6403 6405 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6406 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6504  d.l.m.Z.m.Z...e.
@@ -34,633 +34,636 @@
 00000210: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
 00000220: 0c00 0000 6500 5a01 6400 5a02 6401 5300  ....e.Z.d.Z.d.S.
 00000230: 2902 da18 4750 4754 4e6f 4e65 6564 4d65  )...GPGTNoNeedMe
 00000240: 7267 6545 7863 6570 7469 6f6e 4ea9 03da  rgeExceptionN...
 00000250: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 00000260: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00000270: 655f 5fa9 0072 0c00 0000 720c 0000 00fa  e__..r....r.....
-00000280: 342f 646c 672f 6c69 622f 7079 7468 6f6e  4/dlg/lib/python
-00000290: 332e 382f 7369 7465 2d70 6163 6b61 6765  3.8/site-package
-000002a0: 732f 646c 672f 6472 6f70 6d61 6b65 2f70  s/dlg/dropmake/p
-000002b0: 6774 2e70 7972 0700 0000 2b00 0000 7302  gt.pyr....+...s.
-000002c0: 0000 0008 0172 0700 0000 6300 0000 0000  .....r....c.....
-000002d0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-000002e0: 0000 0073 0c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000002f0: 6401 5300 2902 da0d 4750 4754 4578 6365  d.S.)...GPGTExce
-00000300: 7074 696f 6e4e 7208 0000 0072 0c00 0000  ptionNr....r....
-00000310: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000320: 0e00 0000 2f00 0000 7302 0000 0008 0172  ..../...s......r
-00000330: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000340: 0000 0000 0004 0000 0040 0000 0073 be00  .........@...s..
-00000350: 0000 6500 5a01 6400 5a02 6401 5a03 6429  ..e.Z.d.Z.d.Z.d)
-00000360: 6403 6404 8401 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
-00000370: 6506 6407 6408 8400 8301 5a07 6409 640a  e.d.d.....Z.d.d.
-00000380: 8400 5a08 640b 640c 8400 5a09 640d 640e  ..Z.d.d...Z.d.d.
-00000390: 8400 5a0a 642a 640f 6410 8401 5a0b 6411  ..Z.d*d.d...Z.d.
-000003a0: 6412 8400 5a0c 6506 6413 6414 8400 8301  d...Z.e.d.d.....
-000003b0: 5a0d 6506 6415 6416 8400 8301 5a0e 642b  Z.e.d.d.....Z.d+
-000003c0: 6419 641a 8401 5a0f 6506 641b 641c 8400  d.d...Z.e.d.d...
-000003d0: 8301 5a10 6506 641d 641e 8400 8301 5a11  ..Z.e.d.d.....Z.
-000003e0: 6511 6a12 641f 641e 8400 8301 5a11 642c  e.j.d.d.....Z.d,
-000003f0: 6421 6422 8401 5a13 642d 6424 6425 8401  d!d"..Z.d-d$d%..
-00000400: 5a14 642e 6427 6428 8401 5a15 6426 5300  Z.d.d'd(..Z.d&S.
-00000410: 292f da03 5047 547a 3a0a 2020 2020 4120  )/..PGTz:.    A 
-00000420: 4452 4f50 2072 6570 7265 7365 6e74 6174  DROP representat
-00000430: 696f 6e20 6f66 2050 6879 7369 6361 6c20  ion of Physical 
-00000440: 4772 6170 6820 5465 6d70 6c61 7465 0a20  Graph Template. 
-00000450: 2020 2054 6303 0000 0000 0000 0000 0000     Tc...........
-00000460: 0003 0000 0003 0000 0043 0000 0073 7a00  .........C...sz.
-00000470: 0000 7c01 7c00 5f00 7401 7c01 8301 7c00  ..|.|._.t.|...|.
-00000480: 5f02 6700 7c00 5f03 7c02 7226 7404 a005  _.g.|._.|.r&t...
-00000490: 7c00 6a00 a101 6e02 6400 7c00 5f06 6400  |.j...n.d.|._.d.
-000004a0: 7c00 5f07 7408 8300 7c00 5f09 7408 8300  |._.t...|._.t...
-000004b0: 7c00 5f0a 6401 7c00 5f0b 6401 7c00 5f0c  |._.d.|._.d.|._.
-000004c0: 6700 7c00 5f0d 6402 7c00 5f0e 6403 7c00  g.|._.d.|._.d.|.
-000004d0: 5f0f 6404 6405 6702 7c00 5f10 6400 7c00  _.d.d.g.|._.d.|.
-000004e0: 5f11 6900 7c00 5f12 6400 5300 2906 4e72  _.i.|._.d.S.).Nr
-000004f0: 0200 0000 e700 0000 0000 0024 4046 da04  ...........$@F..
-00000500: 4461 7461 5a07 436f 6d70 7574 6529 13da  DataZ.Compute)..
-00000510: 0a5f 6472 6f70 5f6c 6973 74da 036c 656e  ._drop_list..len
-00000520: 5a0e 5f64 726f 705f 6c69 7374 5f6c 656e  Z._drop_list_len
-00000530: da0c 5f65 7874 7261 5f64 726f 7073 7204  .._extra_dropsr.
-00000540: 0000 00da 1462 7569 6c64 5f64 6167 5f66  .....build_dag_f
-00000550: 726f 6d5f 6472 6f70 73da 045f 6461 67da  rom_drops.._dag.
-00000560: 095f 6a73 6f6e 5f73 7472 da04 6469 6374  ._json_str..dict
-00000570: da0c 5f6f 6964 5f67 6964 5f6d 6170 da12  .._oid_gid_map..
-00000580: 5f67 6964 5f69 736c 616e 645f 6964 5f6d  _gid_island_id_m
-00000590: 6170 da0f 5f6e 756d 5f70 6172 7473 5f64  ap.._num_parts_d
-000005a0: 6f6e 65da 115f 7061 7274 6974 696f 6e5f  one.._partition_
-000005b0: 6d65 7267 6564 5a0c 5f69 6e6e 6572 5f70  mergedZ._inner_p
-000005c0: 6172 7473 5a09 5f62 775f 7261 7469 6fda  artsZ._bw_ratio.
-000005d0: 0c5f 6d65 7267 655f 7061 7274 735a 0e5f  ._merge_partsZ._
-000005e0: 6973 6c61 6e64 5f6c 6162 656c 73da 0e5f  island_labels.._
-000005f0: 6461 7461 5f6d 6f76 656d 656e 74da 0a5f  data_movement.._
-00000600: 7265 7072 6f64 6174 6129 03da 0473 656c  reprodata)...sel
-00000610: 66da 0964 726f 705f 6c69 7374 5a09 6275  f..drop_listZ.bu
-00000620: 696c 645f 6461 6772 0c00 0000 720c 0000  ild_dagr....r...
-00000630: 0072 0d00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
-00000640: 3800 0000 7324 0000 0000 0106 010a 0106  8...s$..........
-00000650: 0302 ff0e 0202 fd04 0506 0108 0108 0106  ................
-00000660: 0106 0106 0206 0206 010a 0106 017a 0c50  .............z.P
-00000670: 4754 2e5f 5f69 6e69 745f 5f63 0200 0000  GT.__init__c....
-00000680: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00000690: 4300 0000 7366 0000 007c 0164 016b 0172  C...sf...|.d.k.r
-000006a0: 1674 0064 02a0 017c 01a1 0183 0182 017c  .t.d...|.......|
-000006b0: 006a 0273 2e74 0064 03a0 017c 006a 036a  .j.s.t.d...|.j.j
-000006c0: 04a1 0183 0182 017c 006a 057c 016b 0172  .......|.j.|.k.r
-000006d0: 5074 0664 04a0 017c 006a 036a 047c 006a  Pt.d...|.j.j.|.j
-000006e0: 057c 01a1 0383 0182 017c 006a 077c 016b  .|.......|.j.|.k
-000006f0: 0272 5e64 0553 0064 0653 0064 0053 0029  .r^d.S.d.S.d.S.)
-00000700: 074e 7202 0000 007a 1949 6e76 616c 6964  .Nr....z.Invalid
-00000710: 206e 6577 5f6e 756d 5f70 6172 7473 207b   new_num_parts {
-00000720: 307d 7a25 5468 6973 207b 307d 2050 4754  0}z%This {0} PGT
-00000730: 5020 6973 206e 6f74 206d 6164 6520 666f  P is not made fo
-00000740: 7220 6d65 7267 696e 677a 2a4e 6f20 6e65  r mergingz*No ne
-00000750: 6564 2074 6f20 6d65 7267 6520 7468 6973  ed to merge this
-00000760: 207b 307d 2050 4754 503a 207b 317d 203c   {0} PGTP: {1} <
-00000770: 3d20 7b32 7d46 5429 0872 0e00 0000 da06  = {2}FT).r......
-00000780: 666f 726d 6174 721d 0000 00da 095f 5f63  formatr......__c
-00000790: 6c61 7373 5f5f 7209 0000 0072 1b00 0000  lass__r....r....
-000007a0: 7207 0000 0072 1c00 0000 2902 7220 0000  r....r....).r ..
-000007b0: 00da 0d6e 6577 5f6e 756d 5f70 6172 7473  ...new_num_parts
-000007c0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-000007d0: 0a5f 6361 6e5f 6d65 7267 654f 0000 0073  ._can_mergeO...s
-000007e0: 2a00 0000 0001 0801 0201 08ff 0403 0601  *...............
-000007f0: 0201 0401 06ff 02ff 0405 0a01 0201 0401  ................
-00000800: 0601 0401 02fd 02ff 0407 0a01 0402 7a0e  ..............z.
-00000810: 5047 542e 5f63 616e 5f6d 6572 6765 6301  PGT._can_mergec.
-00000820: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000830: 0000 0043 0000 0073 2000 0000 7c00 6a00  ...C...s ...|.j.
-00000840: 6400 6b08 7210 7c00 6a01 5300 7c00 6a01  d.k.r.|.j.S.|.j.
-00000850: 7c00 6a00 1700 5300 6400 5300 a901 4e29  |.j...S.d.S...N)
-00000860: 0272 1400 0000 7212 0000 00a9 0172 2000  .r....r......r .
-00000870: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000880: 00da 0564 726f 7073 6700 0000 7306 0000  ...dropsg...s...
-00000890: 0000 020a 0106 027a 0950 4754 2e64 726f  .......z.PGT.dro
-000008a0: 7073 6302 0000 0000 0000 0000 0000 0002  psc.............
-000008b0: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
-000008c0: 7400 6401 8301 8201 6402 5300 2903 7a41  t.d.....d.S.).zA
-000008d0: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-000008e0: 2074 6f20 666f 726d 6174 2066 6f72 206d   to format for m
-000008f0: 6170 7069 6e67 2061 6e64 2064 6563 6f6d  apping and decom
-00000900: 706f 7369 7469 6f6e 0a20 2020 2020 2020  position.       
-00000910: 207a 2a4d 7573 7420 6265 2069 6d70 6c65   z*Must be imple
-00000920: 6d65 6e74 6564 2062 7920 5047 5450 2073  mented by PGTP s
-00000930: 7562 2d63 6c61 7373 206f 6e6c 794e 2901  ub-class onlyN).
-00000940: 720e 0000 0029 0272 2000 0000 da04 6f75  r....).r .....ou
-00000950: 7466 720c 0000 0072 0c00 0000 720d 0000  tfr....r....r...
-00000960: 00da 1274 6f5f 7061 7274 6974 696f 6e5f  ...to_partition_
-00000970: 696e 7075 746e 0000 0073 0200 0000 0004  inputn...s......
-00000980: 7a16 5047 542e 746f 5f70 6172 7469 7469  z.PGT.to_partiti
-00000990: 6f6e 5f69 6e70 7574 6301 0000 0000 0000  on_inputc.......
-000009a0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-000009b0: 0073 1c00 0000 7400 7c00 6a01 8301 7d01  .s....t.|.j...}.
-000009c0: 7402 7403 a004 7c01 6401 1b00 a101 8301  t.t...|.d.......
-000009d0: 5300 2902 7a1f 0a20 2020 2020 2020 2064  S.).z..        d
-000009e0: 756d 6d79 2066 6f72 206e 6f77 0a20 2020  ummy for now.   
-000009f0: 2020 2020 2072 1000 0000 2905 7213 0000       r....).r...
-00000a00: 0072 1200 0000 da03 696e 74da 046d 6174  .r......int..mat
-00000a10: 68da 0463 6569 6c29 0272 2000 0000 da04  h..ceil).r .....
-00000a20: 6c65 6e67 720c 0000 0072 0c00 0000 720d  lengr....r....r.
-00000a30: 0000 00da 1167 6574 5f6f 7074 5f6e 756d  .....get_opt_num
-00000a40: 5f70 6172 7473 7400 0000 7304 0000 0000  _partst...s.....
-00000a50: 040a 017a 1550 4754 2e67 6574 5f6f 7074  ...z.PGT.get_opt
-00000a60: 5f6e 756d 5f70 6172 7473 6301 0000 0000  _num_partsc.....
-00000a70: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000a80: 0000 0073 0400 0000 6401 5300 2902 4e5a  ...s....d.S.).NZ
-00000a90: 0d52 6177 5f75 6e72 6f6c 6c69 6e67 720c  .Raw_unrollingr.
-00000aa0: 0000 0072 2800 0000 720c 0000 0072 0c00  ...r(...r....r..
-00000ab0: 0000 720d 0000 00da 1267 6574 5f70 6172  ..r......get_par
-00000ac0: 7469 7469 6f6e 5f69 6e66 6f7b 0000 0073  tition_info{...s
-00000ad0: 0200 0000 0006 7a16 5047 542e 6765 745f  ......z.PGT.get_
-00000ae0: 7061 7274 6974 696f 6e5f 696e 666f 6302  partition_infoc.
-00000af0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000b00: 0000 0043 0000 0073 6800 0000 6900 7d02  ...C...sh...i.}.
-00000b10: 7c00 a000 a100 7c02 6401 3c00 7c00 6a01  |.....|.d.<.|.j.
-00000b20: 6402 7c01 0c00 6403 8d02 7c02 6404 3c00  d.|...d...|.d.<.
-00000b30: 7c00 6a02 7c02 6405 3c00 7c00 6a01 7c01  |.j.|.d.<.|.j.|.
-00000b40: 0c00 6406 8d01 7c02 6407 3c00 7c00 6a03  ..d...|.d.<.|.j.
-00000b50: 725a 7c00 6a04 6408 6b04 725a 7c00 6a04  rZ|.j.d.k.rZ|.j.
-00000b60: 7c02 6409 3c00 7c00 a005 7c02 a101 0100  |.d.<.|...|.....
-00000b70: 7c02 5300 290a 4eda 0461 6c67 6f54 2902  |.S.).N..algoT).
-00000b80: da0d 6170 705f 6472 6f70 5f6f 6e6c 79da  ..app_drop_only.
-00000b90: 0c66 6f72 6365 5f61 6e73 7765 725a 0d6d  .force_answerZ.m
-00000ba0: 696e 5f65 7865 635f 7469 6d65 5a13 746f  in_exec_timeZ.to
-00000bb0: 7461 6c5f 6461 7461 5f6d 6f76 656d 656e  tal_data_movemen
-00000bc0: 7429 0172 3400 0000 5a09 6578 6563 5f74  t).r4...Z.exec_t
-00000bd0: 696d 6572 0200 0000 da0b 6e75 6d5f 6973  imer......num_is
-00000be0: 6c61 6e64 7329 0672 3100 0000 da0e 7072  lands).r1.....pr
-00000bf0: 6564 5f65 7865 635f 7469 6d65 da0d 6461  ed_exec_time..da
-00000c00: 7461 5f6d 6f76 656d 656e 7472 1d00 0000  ta_movementr....
-00000c10: 721c 0000 00da 0d5f 6578 7472 615f 7265  r......_extra_re
-00000c20: 7375 6c74 2903 7220 0000 00da 046c 617a  sult).r .....laz
-00000c30: 79da 0372 6574 720c 0000 0072 0c00 0000  y..retr....r....
-00000c40: 720d 0000 00da 0672 6573 756c 7483 0000  r......result...
-00000c50: 0073 1800 0000 0001 0401 0c01 0401 0200  .s..............
-00000c60: 04ff 0a03 0a01 1201 1001 0a01 0a01 7a0a  ..............z.
-00000c70: 5047 542e 7265 7375 6c74 6302 0000 0000  PGT.resultc.....
-00000c80: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
-00000c90: 0000 0073 0400 0000 6400 5300 7227 0000  ...s....d.S.r'..
-00000ca0: 0072 0c00 0000 2902 7220 0000 0072 3a00  .r....).r ...r:.
-00000cb0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000cc0: 0072 3800 0000 9000 0000 7302 0000 0000  .r8.......s.....
-00000cd0: 017a 1150 4754 2e5f 6578 7472 615f 7265  .z.PGT._extra_re
-00000ce0: 7375 6c74 6301 0000 0000 0000 0000 0000  sultc...........
-00000cf0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000d00: 0000 7c00 6a00 5300 2901 7afb 0a20 2020  ..|.j.S.).z..   
-00000d10: 2020 2020 2020 2020 2052 6574 7572 6e20           Return 
-00000d20: 7468 6520 6e65 7477 6f72 6b78 206e 782e  the networkx nx.
-00000d30: 4469 4772 6170 6820 6f62 6a65 6374 0a0a  DiGraph object..
-00000d40: 2020 2020 2020 2020 5468 6520 7765 6967          The weig
-00000d50: 6874 206f 6620 7468 6520 7361 6d65 2065  ht of the same e
-00000d60: 6467 6520 2875 2c20 7629 2061 6c73 6f20  dge (u, v) also 
-00000d70: 6465 7065 6e64 732e 0a20 2020 2020 2020  depends..       
-00000d80: 2049 6620 6974 2069 7320 6361 6c6c 6564   If it is called
-00000d90: 2061 6674 6572 2074 6865 2070 6172 7469   after the parti
-00000da0: 7469 6f6e 696e 672c 2069 7420 636f 756c  tioning, it coul
-00000db0: 6420 6861 7665 2062 6565 6e20 7a65 726f  d have been zero
-00000dc0: 6564 0a20 2020 2020 2020 2069 6620 626f  ed.        if bo
-00000dd0: 7468 2075 2061 6e64 2076 2069 7320 616c  th u and v is al
-00000de0: 6c6f 6361 7465 6420 746f 2074 6865 2073  located to the s
-00000df0: 616d 6520 4472 6f70 4973 6c61 6e64 0a20  ame DropIsland. 
-00000e00: 2020 2020 2020 2029 0172 1600 0000 7228         ).r....r(
-00000e10: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000e20: 0000 da03 6461 6793 0000 0073 0200 0000  ....dag....s....
-00000e30: 0009 7a07 5047 542e 6461 6763 0100 0000  ..z.PGT.dagc....
-00000e40: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000e50: 4300 0000 7342 0000 007c 006a 0064 016b  C...sB...|.j.d.k
-00000e60: 0972 107c 006a 0053 007c 006a 0164 016b  .r.|.j.S.|.j.d.k
-00000e70: 0972 3c7c 006a 017d 0174 0264 0264 0384  .r<|.j.}.t.d.d..
-00000e80: 007c 016a 0364 0464 058d 0144 0083 0183  .|.j.d.d...D....
-00000e90: 017c 005f 007c 006a 0053 0029 067a 300a  .|._.|.j.S.).z0.
-00000ea0: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-00000eb0: 6865 2054 4f54 414c 2064 6174 6120 6d6f  he TOTAL data mo
-00000ec0: 7665 6d65 6e74 0a20 2020 2020 2020 204e  vement.        N
-00000ed0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000ee0: 0005 0000 0073 0000 0073 1e00 0000 7c00  .....s...s....|.
-00000ef0: 5d16 7d01 7c01 6400 1900 a000 6401 6402  ].}.|.d.....d.d.
-00000f00: a102 5600 0100 7102 6403 5300 2904 e902  ..V...q.d.S.)...
-00000f10: 0000 00da 0677 6569 6768 7472 0200 0000  .....weightr....
-00000f20: 4e29 01da 0367 6574 2902 da02 2e30 da01  N)...get)....0..
-00000f30: 6572 0c00 0000 720c 0000 0072 0d00 0000  er....r....r....
-00000f40: da09 3c67 656e 6578 7072 3ea7 0000 0073  ..<genexpr>....s
-00000f50: 0400 0000 0401 0200 7a24 5047 542e 6461  ........z$PGT.da
-00000f60: 7461 5f6d 6f76 656d 656e 742e 3c6c 6f63  ta_movement.<loc
-00000f70: 616c 733e 2e3c 6765 6e65 7870 723e 5429  als>.<genexpr>T)
-00000f80: 01da 0464 6174 6129 0472 1e00 0000 723c  ...data).r....r<
-00000f90: 0000 00da 0373 756d da05 6564 6765 7329  .....sum..edges)
-00000fa0: 0272 2000 0000 da01 4772 0c00 0000 720c  .r .....Gr....r.
-00000fb0: 0000 0072 0d00 0000 7237 0000 009e 0000  ...r....r7......
-00000fc0: 0073 1000 0000 0005 0a01 0601 0a01 0601  .s..............
-00000fd0: 0801 0aff 0a03 7a11 5047 542e 6461 7461  ......z.PGT.data
-00000fe0: 5f6d 6f76 656d 656e 7446 723e 0000 0063  _movementFr>...c
-00000ff0: 0400 0000 0000 0000 0000 0000 0500 0000  ................
-00001000: 0400 0000 0300 0000 7370 0000 007c 006a  ........sp...|.j
-00001010: 0089 0088 0064 016b 0872 2c7c 0372 2874  .....d.k.r,|.r(t
-00001020: 01a0 027c 006a 03a1 017c 005f 047c 006a  ...|.j...|._.|.j
-00001030: 0089 006e 0464 0153 007c 0172 5a74 016a  ...n.d.S.|.rZt.j
-00001040: 0588 0064 0264 038d 0264 0419 007d 0474  ...d.d...d...}.t
-00001050: 0687 0087 0166 0264 0564 0684 087c 0444  .....f.d.d...|.D
-00001060: 0083 0183 0153 0074 016a 0588 0064 0764  .....S.t.j...d.d
-00001070: 038d 0264 0819 0053 0064 0153 0029 097a  ...d...S.d.S.).z
-00001080: 460a 2020 2020 2020 2020 5072 6564 6963  F.        Predic
-00001090: 7420 6578 6563 7574 696f 6e20 7469 6d65  t execution time
-000010a0: 2075 7369 6e67 2074 6865 206c 6f6e 6765   using the longe
-000010b0: 7374 2070 6174 6820 6c65 6e67 7468 0a20  st path length. 
-000010c0: 2020 2020 2020 204e 5429 015a 0973 686f         NT).Z.sho
-000010d0: 775f 7061 7468 7202 0000 0063 0100 0000  w_pathr....c....
-000010e0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000010f0: 3300 0000 7320 0000 007c 005d 187d 0188  3...s ...|.].}..
-00001100: 006a 007c 0119 00a0 0188 0164 00a1 0256  .j.|.......d...V
-00001110: 0001 0071 0264 0153 0029 0272 0200 0000  ...q.d.S.).r....
-00001120: 4e29 02da 056e 6f64 6573 723f 0000 0029  N)...nodesr?...)
-00001130: 0272 4000 0000 da01 75a9 0272 4600 0000  .r@.....u..rF...
-00001140: da02 776b 720c 0000 0072 0d00 0000 7242  ..wkr....r....rB
-00001150: 0000 00bb 0000 0073 0400 0000 0400 0200  .......s........
-00001160: 7a25 5047 542e 7072 6564 5f65 7865 635f  z%PGT.pred_exec_
-00001170: 7469 6d65 2e3c 6c6f 6361 6c73 3e2e 3c67  time.<locals>.<g
-00001180: 656e 6578 7072 3e46 e901 0000 0029 0772  enexpr>F.....).r
-00001190: 3c00 0000 7204 0000 0072 1500 0000 7212  <...r....r....r.
-000011a0: 0000 0072 1600 0000 5a10 6765 745f 6c6f  ...r....Z.get_lo
-000011b0: 6e67 6573 745f 7061 7468 7244 0000 0029  ngest_pathrD...)
-000011c0: 0572 2000 0000 7233 0000 0072 4a00 0000  .r ...r3...rJ...
-000011d0: 7234 0000 005a 026c 7072 0c00 0000 7249  r4...Z.lpr....rI
-000011e0: 0000 0072 0d00 0000 7236 0000 00ac 0000  ...r....r6......
-000011f0: 0073 1400 0000 0006 0601 0801 0401 0e01  .s..............
-00001200: 0802 0401 0401 1201 1802 7a12 5047 542e  ..........z.PGT.
-00001210: 7072 6564 5f65 7865 635f 7469 6d65 6301  pred_exec_timec.
-00001220: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001230: 0000 0043 0000 0073 1e00 0000 7c00 6a00  ...C...s....|.j.
-00001240: 6401 6b08 7218 7c00 6a01 6402 6403 8d01  d.k.r.|.j.d.d...
-00001250: 7c00 5f00 7c00 6a00 5300 2904 7a5c 0a20  |._.|.j.S.).z\. 
-00001260: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-00001270: 6520 4a53 4f4e 2073 7472 696e 6720 7265  e JSON string re
-00001280: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-00001290: 7468 6520 5047 540a 2020 2020 2020 2020  the PGT.        
-000012a0: 666f 7220 7669 7375 616c 6973 6174 696f  for visualisatio
-000012b0: 6e0a 2020 2020 2020 2020 4e54 2901 da06  n.        NT)...
-000012c0: 7669 7375 616c 2902 7217 0000 00da 0c74  visual).r......t
-000012d0: 6f5f 676f 6a73 5f6a 736f 6e72 2800 0000  o_gojs_jsonr(...
-000012e0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-000012f0: 046a 736f 6ebf 0000 0073 0600 0000 0006  .json....s......
-00001300: 0a01 0e02 7a08 5047 542e 6a73 6f6e 6301  ....z.PGT.jsonc.
-00001310: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001320: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00001330: 5300 7227 0000 00a9 0172 1f00 0000 7228  S.r'.....r....r(
-00001340: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00001350: 0000 da09 7265 7072 6f64 6174 61cb 0000  ....reprodata...
-00001360: 0073 0200 0000 0002 7a0d 5047 542e 7265  .s......z.PGT.re
-00001370: 7072 6f64 6174 6163 0200 0000 0000 0000  prodatac........
-00001380: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00001390: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
-000013a0: 2700 0000 724f 0000 0029 0272 2000 0000  '...rO...).r ...
-000013b0: da05 7661 6c75 6572 0c00 0000 720c 0000  ..valuer....r...
-000013c0: 0072 0d00 0000 7250 0000 00cf 0000 0073  .r....rP.......s
-000013d0: 0200 0000 0002 7202 0000 0063 0500 0000  ......r....c....
-000013e0: 0000 0000 0000 0000 0500 0000 0200 0000  ................
-000013f0: 4300 0000 730c 0000 0074 0064 0183 0182  C...s....t.d....
-00001400: 0164 0053 0029 024e 7a1f 4e6f 7420 696d  .d.S.).Nz.Not im
-00001410: 706c 656d 656e 7465 642e 2043 616c 6c20  plemented. Call 
-00001420: 7375 622d 636c 6173 7329 01da 0945 7863  sub-class)...Exc
-00001430: 6570 7469 6f6e 2905 7220 0000 0072 2500  eption).r ...r%.
-00001440: 0000 da0b 666f 726d 5f69 736c 616e 645a  ....form_islandZ
-00001450: 0b69 736c 616e 645f 7479 7065 724c 0000  .island_typerL..
-00001460: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00001470: da10 6d65 7267 655f 7061 7274 6974 696f  ..merge_partitio
-00001480: 6e73 d300 0000 7302 0000 0000 037a 1450  ns....s......z.P
-00001490: 4754 2e6d 6572 6765 5f70 6172 7469 7469  GT.merge_partiti
-000014a0: 6f6e 7372 4b00 0000 6306 0000 0000 0000  onsrK...c.......
-000014b0: 0000 0000 0014 0000 0008 0000 0043 0000  .............C..
-000014c0: 0073 3002 0000 7400 a001 6401 7c04 7c01  .s0...t...d.|.|.
-000014d0: a103 0100 7402 7c01 8301 6402 6b02 7230  ....t.|...d.k.r0
-000014e0: 7c04 6402 6b04 7230 7403 7c04 8301 7d01  |.d.k.r0t.|...}.
-000014f0: 6403 7d06 6e04 6404 7d06 6402 7c00 6a04  d.}.n.d.}.d.|.j.
-00001500: 6b02 7246 7405 6405 8301 8201 7c01 6406  k.rFt.d.....|.d.
-00001510: 6b08 735a 6402 7402 7c01 8301 6b02 7262  k.sZd.t.|...k.rb
-00001520: 7405 6407 8301 8201 7402 7c01 8301 7d07  t.d.....t.|...}.
-00001530: 7a0c 7406 7c03 8301 7d03 5700 6e1a 0100  z.t.|...}.W.n...
-00001540: 0100 0100 7405 6408 a007 7c03 a101 8301  ....t.d...|.....
-00001550: 8201 5900 6e02 5800 7c03 6409 6b00 729e  ..Y.n.X.|.d.k.r.
-00001560: 6409 7d03 7c03 7c07 6b04 72ae 7405 640a  d.}.|.|.k.r.t.d.
-00001570: 8301 8201 7c03 6409 6b04 7d08 7c07 6409  ....|.d.k.}.|.d.
-00001580: 6b00 72cc 7405 640b a007 7c07 a101 8301  k.r.t.d...|.....
-00001590: 8201 7c00 6a04 7d09 7c00 6a08 7d0a 7c05  ..|.j.}.|.j.}.|.
-000015a0: 9001 7312 7c08 72f8 7c09 7c07 6b04 72f8  ..s.|.r.|.|.k.r.
-000015b0: 7405 640c a007 7c07 a101 8301 8201 7c01  t.d...|.......|.
-000015c0: 6402 7c03 8502 1900 7d0b 7c01 7c03 6406  d.|.....}.|.|.d.
-000015d0: 8502 1900 7d0c 6e2a 7c08 9001 7234 7c03  ....}.n*|...r4|.
-000015e0: 7c09 1700 7c07 6b04 9001 7234 7405 640c  |...|.k...r4t.d.
-000015f0: a007 7c07 a101 8301 8201 7c01 7d0b 7c01  ..|.......|.}.|.
-00001600: 7d0c 7402 7c0c 8301 7d0d 7400 a009 640d  }.t.|...}.t...d.
-00001610: 7402 7c0a 8301 7c09 7c07 7402 7c0b 8301  t.|...|.|.t.|...
-00001620: a105 0100 7c08 9001 7274 7c00 6a0a 7c03  ....|...rt|.j.|.
-00001630: 6403 640e 8d02 0100 6e1c 7c0d 7c09 6b00  d.d.....n.|.|.k.
-00001640: 9001 7290 7c00 6a0a 7c0d 6404 640e 8d02  ..r.|.j.|.d.d...
-00001650: 0100 7c0d 7d09 7c00 6a0b 7d0e 7c00 6a0c  ..|.}.|.j.}.|.j.
-00001660: 7d0f 7c06 9001 72ca 640f 6410 8400 7403  }.|...r.d.d...t.
-00001670: 7c0d 8301 4400 8301 7d0c 6411 6410 8400  |...D...}.d.d...
-00001680: 7403 7402 7c0b 8301 8301 4400 8301 7d0b  t.t.|.....D...}.
-00001690: 7c0a 4400 5d44 7d10 7c10 6412 1900 7d11  |.D.]D}.|.d...}.
-000016a0: 7c0e 7c11 1900 7d12 7c0c 7c12 1900 7c10  |.|...}.|.|...|.
-000016b0: 6413 3c00 7c08 9002 7200 7c0f 7c12 1900  d.<.|...r.|.|...
-000016c0: 7c03 1600 6e02 6402 7d13 7c0b 7c13 1900  |...n.d.}.|.|...
-000016d0: 7c10 6414 3c00 9001 71ce 7c02 9002 7228  |.d.<...q.|...r(
-000016e0: 740d 6a0e 7c0a 6415 6416 8d02 5300 7c0a  t.j.|.d.d...S.|.
-000016f0: 5300 6406 5300 2917 6129 0300 000a 2020  S.d.S.).a)....  
-00001700: 2020 2020 2020 636f 6e76 6572 7420 7067        convert pg
-00001710: 7420 746f 2070 6720 7370 6563 6966 6963  t to pg specific
-00001720: 6174 696f 6e2c 2061 6e64 206d 6170 2074  ation, and map t
-00001730: 6861 7420 746f 2074 6865 2068 6172 6477  hat to the hardw
-00001740: 6172 6520 7265 736f 7572 6365 730a 0a20  are resources.. 
-00001750: 2020 2020 2020 206e 6f64 655f 6c69 7374         node_list
-00001760: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-00001770: 6c69 7374 206f 6620 6e6f 6465 7320 286c  list of nodes (l
-00001780: 6973 7429 2c20 7768 6f73 6520 6c65 6e67  ist), whose leng
-00001790: 7468 203d 3d20 286e 756d 5f69 736c 616e  th == (num_islan
-000017a0: 6473 202b 206e 756d 5f6e 6f64 655f 6d67  ds + num_node_mg
-000017b0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-000017c0: 6966 2063 6f5f 6c6f 6361 7465 5f69 736c  if co_locate_isl
-000017d0: 616e 6473 203d 2046 616c 7365 2e0a 2020  ands = False..  
-000017e0: 2020 2020 2020 2020 2020 5765 2061 7373            We ass
-000017f0: 756d 6520 7468 6174 2074 6865 204d 6173  ume that the Mas
-00001800: 7465 7244 726f 704d 616e 6167 6572 2773  terDropManager's
-00001810: 206e 6f64 6520 6973 204e 4f54 2069 6e20   node is NOT in 
-00001820: 7468 6520 6e6f 6465 5f6c 6973 740a 0a20  the node_list.. 
-00001830: 2020 2020 2020 206e 756d 5f69 736c 616e         num_islan
-00001840: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-00001850: 2d20 3e31 2050 6172 7469 7469 6f6e 7320  - >1 Partitions 
-00001860: 6172 6520 2263 6f6e 6365 7074 7561 6c6c  are "conceptuall
-00001870: 7922 2063 6c75 7374 6572 6564 2069 6e74  y" clustered int
-00001880: 6f20 4973 6c61 6e64 730a 2020 2020 2020  o Islands.      
-00001890: 2020 2020 2020 2d20 3120 5061 7274 6974        - 1 Partit
-000018a0: 696f 6e73 204d 4159 2042 4520 7068 7973  ions MAY BE phys
-000018b0: 6963 616c 6c79 206d 6572 6765 6420 7769  ically merged wi
-000018c0: 7468 6f75 7420 6765 6e65 7261 7469 6e67  thout generating
-000018d0: 2069 736c 616e 6473 0a20 2020 2020 2020   islands.       
-000018e0: 2020 2020 2020 2064 6570 656e 6469 6e67         depending
-000018f0: 206f 6e20 7468 6520 6c65 6e67 7468 206f   on the length o
-00001900: 6620 6e6f 6465 5f6c 6973 740a 2020 2020  f node_list.    
-00001910: 2020 2020 2020 2020 2d20 6e75 6d5f 6973          - num_is
-00001920: 6c61 6e64 7320 6361 6e27 7420 6265 203c  lands can't be <
-00001930: 2031 0a0a 2020 2020 2020 2020 7470 6c5f   1..        tpl_
-00001940: 6e6f 6465 735f 6c65 6e3a 2069 6620 7468  nodes_len: if th
-00001950: 6973 2069 7320 6769 7665 6e20 7765 2067  is is given we g
-00001960: 656e 6572 6174 6520 6120 7067 5f73 7065  enerate a pg_spe
-00001970: 6320 7465 6d70 6c61 7465 0a20 2020 2020  c template.     
-00001980: 2020 2020 2020 2054 6865 2070 675f 7370         The pg_sp
-00001990: 6563 2074 656d 706c 6174 6520 6973 2077  ec template is w
-000019a0: 6861 7420 6e65 6564 7320 746f 2062 6520  hat needs to be 
-000019b0: 7365 6e64 2074 6f20 6120 6465 6665 7272  send to a deferr
-000019c0: 6564 2064 6570 6c6f 7965 6d6e 740a 2020  ed deployemnt.  
-000019d0: 2020 2020 2020 2020 2020 7768 6572 6520            where 
-000019e0: 7468 6520 6461 6c69 7567 6520 7379 7374  the daliuge syst
-000019f0: 656d 2069 7320 7374 6172 7465 6420 7570  em is started up
-00001a00: 2061 6665 7220 7375 626d 6973 7369 6f6e   afer submission
-00001a10: 2028 652e 672e 2053 4c55 524d 290a 2020   (e.g. SLURM).  
-00001a20: 2020 2020 2020 7a2c 2320 776f 726b 6572        z,# worker
-00001a30: 206e 6f64 6573 3a20 2573 2c20 6e6f 6465   nodes: %s, node
-00001a40: 5f6c 6973 7428 696e 636c 2e20 4449 4d29  _list(incl. DIM)
-00001a50: 3a20 2573 7202 0000 0054 467a 2654 6865  : %sr....TFz&The
-00001a60: 2067 7261 7068 2068 6173 206e 6f74 2062   graph has not b
-00001a70: 6565 6e20 7061 7274 6974 696f 6e65 6420  een partitioned 
-00001a80: 7965 744e 7a13 4e6f 6465 206c 6973 7420  yetNz.Node list 
-00001a90: 6973 2065 6d70 7479 217a 1d49 6e76 616c  is empty!z.Inval
-00001aa0: 6964 206e 756d 5f69 736c 616e 6473 2073  id num_islands s
-00001ab0: 7065 633a 207b 307d 724b 0000 007a 374e  pec: {0}rK...z7N
-00001ac0: 756d 6265 7220 6f66 2069 736c 616e 6473  umber of islands
-00001ad0: 206d 7573 7420 6265 203c 3d20 6e75 6d62   must be <= numb
-00001ae0: 6572 206f 6620 7370 6563 6966 6965 6420  er of specified 
-00001af0: 6e6f 6465 7321 7a12 546f 6f20 6665 7720  nodes!z.Too few 
-00001b00: 6e6f 6465 733a 207b 307d 7a21 496e 7375  nodes: {0}z!Insu
-00001b10: 6666 6963 6965 6e74 206e 756d 6265 7220  fficient number 
-00001b20: 6f66 206e 6f64 6573 3a20 7b30 7d7a 4844  of nodes: {0}zHD
-00001b30: 726f 7073 2063 6f75 6e74 3a20 2564 2c20  rops count: %d, 
-00001b40: 7061 7274 6974 696f 6e73 2063 6f75 6e74  partitions count
-00001b50: 3a20 2564 2c20 6e6f 6465 7320 636f 756e  : %d, nodes coun
-00001b60: 743a 2025 642c 2069 736c 616e 6420 636f  t: %d, island co
-00001b70: 756e 743a 2025 6429 0172 5300 0000 6301  unt: %d).rS...c.
-00001b80: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001b90: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00001ba0: 5d0c 7d01 6400 7c01 1600 9102 7104 5300  ].}.d.|.....q.S.
-00001bb0: a901 7a03 2325 7372 0c00 0000 a902 7240  ..z.#%sr......r@
-00001bc0: 0000 00da 0178 720c 0000 0072 0c00 0000  .....xr....r....
-00001bd0: 720d 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00001be0: 3e45 0100 0073 0400 0000 0601 0200 7a22  >E...s........z"
-00001bf0: 5047 542e 746f 5f70 675f 7370 6563 2e3c  PGT.to_pg_spec.<
-00001c00: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00001c10: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-00001c20: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-00001c30: 6700 7c00 5d0c 7d01 6400 7c01 1600 9102  g.|.].}.d.|.....
-00001c40: 7104 5300 7255 0000 0072 0c00 0000 7256  q.S.rU...r....rV
-00001c50: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00001c60: 0000 7258 0000 0048 0100 0073 0400 0000  ..rX...H...s....
-00001c70: 0601 0200 da03 6f69 64da 046e 6f64 65da  ......oid..node.
-00001c80: 0669 736c 616e 6472 3d00 0000 a901 da06  .islandr=.......
-00001c90: 696e 6465 6e74 290f da06 6c6f 6767 6572  indent)...logger
-00001ca0: da05 6465 6275 6772 1300 0000 da05 7261  ..debugr......ra
-00001cb0: 6e67 6572 1b00 0000 720e 0000 0072 2c00  nger....r....r,.
-00001cc0: 0000 7223 0000 0072 2900 0000 da04 696e  ..r#...r).....in
-00001cd0: 666f 7254 0000 0072 1900 0000 721a 0000  forT...r....r...
-00001ce0: 0072 4e00 0000 da05 6475 6d70 7329 1472  .rN.....dumps).r
-00001cf0: 2000 0000 da09 6e6f 6465 5f6c 6973 74da   .....node_list.
-00001d00: 0772 6574 5f73 7472 7235 0000 00da 0d74  .ret_strr5.....t
-00001d10: 706c 5f6e 6f64 6573 5f6c 656e da0b 636f  pl_nodes_len..co
-00001d20: 5f68 6f73 745f 6469 6d5a 0674 706c 5f66  _host_dimZ.tpl_f
-00001d30: 6c5a 096e 6f64 6573 5f6c 656e 7253 0000  lZ.nodes_lenrS..
-00001d40: 005a 096e 756d 5f70 6172 7473 7221 0000  .Z.num_partsr!..
-00001d50: 005a 0769 735f 6c69 7374 da07 6e6d 5f6c  .Z.is_list..nm_l
-00001d60: 6973 745a 066e 6d5f 6c65 6e5a 026c 6d5a  istZ.nm_lenZ.lmZ
-00001d70: 036c 6d32 da04 6472 6f70 7259 0000 00da  .lm2..droprY....
-00001d80: 0367 6964 5a04 6973 6964 720c 0000 0072  .gidZ.isidr....r
-00001d90: 0c00 0000 720d 0000 00da 0a74 6f5f 7067  ....r......to_pg
-00001da0: 5f73 7065 63d8 0000 0073 9c00 0000 001a  _spec....s......
-00001db0: 0401 0201 0201 02fd 0406 0aff 0201 06ff  ................
-00001dc0: 0203 0801 0602 0402 0a01 0802 1401 0801  ................
-00001dd0: 0802 0201 0c01 0601 0201 08ff 0a03 0801  ................
-00001de0: 0401 0801 0201 02ff 0403 0801 0801 0e02  ................
-00001df0: 0601 0603 0601 0c01 0201 08ff 0403 0c01  ................
-00001e00: 0e02 1401 0201 08ff 0403 0401 0401 0801  ................
-00001e10: 0401 0201 0601 0201 0201 06fb 0408 0601  ................
-00001e20: 1003 0a01 0e01 0402 0601 060a 0601 0601  ................
-00001e30: 06ff 0603 0601 0aff 0604 0801 0804 0801  ................
-00001e40: 0c01 1601 1002 0601 0e02 7a0e 5047 542e  ..........z.PGT.
-00001e50: 746f 5f70 675f 7370 6563 4e63 0400 0000  to_pg_specNc....
-00001e60: 0000 0000 0000 0000 1e00 0000 0c00 0000  ................
-00001e70: 4300 0000 73e8 0300 007c 006a 007d 0474  C...s....|.j.}.t
-00001e80: 0183 007d 0564 017c 0564 023c 0067 007d  ...}.d.|.d.<.g.}
-00001e90: 0667 007d 0774 0183 007d 0874 027c 006a  .g.}.t...}.t.|.j
-00001ea0: 0383 0144 005d 7a5c 027d 097d 0a7c 0a64  ...D.]z\.}.}.|.d
-00001eb0: 0319 007d 0b74 0183 007d 0c7c 0964 0417  ...}.t...}.|.d..
-00001ec0: 007c 0c64 053c 007c 0964 0417 007c 087c  .|.d.<.|.d...|.|
-00001ed0: 0b3c 007c 0b7c 0c64 033c 007c 0a64 0619  .<.|.|.d.<.|.d..
-00001ee0: 007d 0d74 046a 057c 0d6b 0272 7e64 077c  .}.t.j.|.k.r~d.|
-00001ef0: 0c64 083c 006e 1274 046a 067c 0d6b 0272  .d.<.n.t.j.|.k.r
-00001f00: 9064 097c 0c64 083c 007c 0a64 0a19 007c  .d.|.d.<.|.d...|
-00001f10: 0c64 0a3c 007c 06a0 077c 0ca1 0101 0071  .d.<.|...|.....q
-00001f20: 2c7c 006a 0864 0b6b 0890 0272 e267 007d  ,|.j.d.k...r.g.}
-00001f30: 0e67 007d 0f67 007d 1067 007d 117c 006a  .g.}.g.}.g.}.|.j
-00001f40: 0344 0090 015d c47d 0a7c 0a64 0319 007d  .D...].}.|.d...}
-00001f50: 0b7c 087c 0b19 007d 1274 027c 04a0 097c  .|.|...}.t.|...|
-00001f60: 12a1 0183 0144 0090 015d 9e5c 027d 097d  .....D...].\.}.}
-00001f70: 1374 0183 007d 147c 127c 1464 0c3c 007c  .t...}.|.|.d.<.|
-00001f80: 0a64 0619 0074 046a 0564 0d66 026b 0690  .d...t.j.d.f.k..
-00001f90: 0172 1e64 0e6e 0264 047d 157c 046a 0a7c  .r.d.n.d.}.|.j.|
-00001fa0: 1319 0064 0f19 007d 167c 157c 166b 0290  ...d...}.|.|.k..
-00001fb0: 0272 7c7c 046a 0a7c 1319 0064 1019 007d  .r||.j.|...d...}
-00001fc0: 177c 1564 0e6b 0290 0172 a264 11a0 0b7c  .|.d.k...r.d...|
-00001fd0: 0b7c 09a1 027d 1874 0c7c 1874 046a 0664  .|...}.t.|.t.j.d
-00001fe0: 1264 1364 0464 149c 0583 017d 197c 0aa0  .d.d.d.....}.|..
-00001ff0: 0d7c 19a1 0101 007c 19a0 0e7c 0aa1 0101  .|.....|...|....
-00002000: 007c 19a0 0f7c 17a1 0101 007c 17a0 107c  .|...|.....|...|
-00002010: 19a1 0101 0064 047d 1a6e 4e64 15a0 0b7c  .....d.}.nNd...|
-00002020: 0b7c 09a1 027d 1874 0c7c 1874 046a 0564  .|...}.t.|.t.j.d
-00002030: 1664 1764 0464 149c 0583 017d 197c 0aa0  .d.d.d.....}.|..
-00002040: 0f7c 19a1 0101 007c 19a0 107c 0aa1 0101  .|.....|...|....
-00002050: 007c 19a0 0d7c 17a1 0101 007c 17a0 0e7c  .|...|.....|...|
-00002060: 19a1 0101 0064 0e7d 1a7c 0ea0 077c 19a1  .....d.}.|...|..
-00002070: 0101 0074 117c 0e83 0164 1814 007d 1b7c  ...t.|...d...}.|
-00002080: 1b7c 1464 193c 0074 0183 007d 1c7c 1b7c  .|.d.<.t...}.|.|
-00002090: 1c64 0c3c 007c 137c 1c64 193c 007c 07a0  .d.<.|.|.d.<.|..
-000020a0: 077c 1ca1 0101 007c 11a0 077c 1b64 047c  .|.....|...|.d.|
-000020b0: 1a7c 197c 046a 0a7c 1319 00a0 1264 1a64  .|.|.j.|.....d.d
-000020c0: 0ba1 0266 05a1 0101 007c 0fa0 077c 127c  ...f.....|...|.|
-000020d0: 1366 02a1 0101 007c 10a0 077c 127c 1b66  .f.....|...|.|.f
-000020e0: 02a1 0101 007c 10a0 077c 1b7c 1366 02a1  .....|...|.|.f..
-000020f0: 0101 006e 087c 137c 1464 193c 007c 07a0  ...n.|.|.d.<.|..
-00002100: 077c 14a1 0101 0071 ee71 ca7c 1144 005d  .|.....q.q.|.D.]
-00002110: 2e7d 1d7c 046a 137c 1d64 0e19 007c 1d64  .}.|.j.|.d...|.d
-00002120: 0419 007c 1d64 1b19 007c 1d64 1c19 007c  ...|.d...|.d...|
-00002130: 1d64 1d19 0064 1e8d 0501 0090 0271 967c  .d...d.......q.|
-00002140: 04a0 147c 0fa1 0101 007c 04a0 157c 10a1  ...|.....|...|..
-00002150: 0101 007c 0e7c 005f 086e 507c 006a 0344  ...|.|._.nP|.j.D
-00002160: 005d 487d 0a7c 0a64 0319 007d 0b7c 087c  .]H}.|.d...}.|.|
-00002170: 0b19 007d 127c 04a0 097c 12a1 0144 005d  ...}.|...|...D.]
-00002180: 267d 1374 0183 007d 147c 127c 1464 0c3c  &}.t...}.|.|.d.<
-00002190: 007c 137c 1464 193c 007c 07a0 077c 14a1  .|.|.d.<.|...|..
-000021a0: 0101 0090 0371 0690 0271 e874 027c 006a  .....q...q.t.|.j
-000021b0: 0883 0144 005d 785c 027d 097d 0a7c 0a64  ...D.]x\.}.}.|.d
-000021c0: 0319 007d 0b74 0183 007d 0c7c 0964 0417  ...}.t...}.|.d..
-000021d0: 0064 1814 007c 0c64 053c 007c 0b7c 0c64  .d...|.d.<.|.|.d
-000021e0: 033c 007c 0a64 0619 007d 0d7c 0d74 046a  .<.|.d...}.|.t.j
-000021f0: 056b 0290 0372 8864 077c 0c64 083c 006e  .k...r.d.|.d.<.n
-00002200: 147c 0d74 046a 066b 0290 0372 9c64 1f7c  .|.t.j.k...r.d.|
-00002210: 0c64 083c 007c 0a64 0a19 007c 0c64 0a3c  .d.<.|.d...|.d.<
-00002220: 007c 06a0 077c 0ca1 0101 0090 0371 3c7c  .|...|.......q<|
-00002230: 067c 0564 203c 007c 077c 0564 213c 007c  .|.d <.|.|.d!<.|
-00002240: 057c 005f 167c 0190 0372 e074 176a 187c  .|._.|...r.t.j.|
-00002250: 0564 1b64 228d 0253 007c 0553 0064 0b53  .d.d"..S.|.S.d.S
-00002260: 0029 237a e80a 2020 2020 2020 2020 436f  .)#z..        Co
-00002270: 6e76 6572 7420 5047 5420 2877 6974 686f  nvert PGT (witho
-00002280: 7574 2061 6e79 2070 6172 7469 7469 6f6e  ut any partition
-00002290: 7329 2074 6f20 4a53 4f4e 2066 6f72 2076  s) to JSON for v
-000022a0: 6973 7561 6c69 7361 7469 6f6e 2069 6e20  isualisation in 
-000022b0: 474f 4a53 0a0a 2020 2020 2020 2020 5375  GOJS..        Su
-000022c0: 622d 636c 6173 7320 5047 5450 7320 7769  b-class PGTPs wi
-000022d0: 6c6c 206f 7665 7272 6964 6520 7468 6973  ll override this
-000022e0: 2066 756e 6374 696f 6e2c 2061 6e64 2072   function, and r
-000022f0: 6570 6c61 6365 2074 6869 7320 7769 7468  eplace this with
-00002300: 0a20 2020 2020 2020 2061 6374 7561 6c20  .        actual 
-00002310: 7061 7274 6974 696f 6e69 6e67 2c20 616e  partitioning, an
-00002320: 6420 7468 6520 7669 7375 6c69 7361 7469  d the visulisati
-00002330: 6f6e 2062 6563 6f6d 6573 2061 6e20 6f70  on becomes an op
-00002340: 7469 6f6e 0a20 2020 2020 2020 207a 1267  tion.        z.g
-00002350: 6f2e 4772 6170 684c 696e 6b73 4d6f 6465  o.GraphLinksMode
-00002360: 6cda 0563 6c61 7373 7259 0000 0072 4b00  l..classrY...rK.
-00002370: 0000 da03 6b65 79da 0c63 6174 6567 6f72  ....key..categor
-00002380: 7954 7970 6572 1100 0000 da08 6361 7465  yTyper......cate
-00002390: 676f 7279 da0b 4170 706c 6963 6174 696f  gory..Applicatio
-000023a0: 6eda 046e 616d 654e da04 6672 6f6d 7243  n..nameN..fromrC
-000023b0: 0000 0072 0200 0000 da09 6472 6f70 5f74  ...r......drop_t
-000023c0: 7970 65da 0964 726f 705f 7370 6563 7a10  ype..drop_specz.
-000023d0: 7b30 7d5f 5472 616e 7341 7070 5f7b 317d  {0}_TransApp_{1}
-000023e0: 7a17 646c 672e 6472 6f70 2e42 6172 7269  z.dlg.drop.Barri
-000023f0: 6572 4170 7044 524f 505a 0667 6f5f 6170  erAppDROPZ.go_ap
-00002400: 7029 0572 5900 0000 726d 0000 00da 0964  p).rY...rm.....d
-00002410: 726f 7063 6c61 7373 7270 0000 0072 3e00  ropclassrp...r>.
-00002420: 0000 7a11 7b30 7d5f 5472 616e 7344 6174  ..z.{0}_TransDat
-00002430: 615f 7b31 7d7a 2264 6c67 2e64 6174 612e  a_{1}z"dlg.data.
-00002440: 6472 6f70 732e 6d65 6d6f 7279 2e49 6e4d  drops.memory.InM
-00002450: 656d 6f72 7944 524f 505a 0767 6f5f 6461  emoryDROPZ.go_da
-00002460: 7461 e9ff ffff ffda 0274 6f72 6900 0000  ta.......tori...
-00002470: 723d 0000 00e9 0300 0000 e904 0000 0029  r=.............)
-00002480: 0472 3e00 0000 7272 0000 0072 7300 0000  .r>...rr...rs...
-00002490: 7269 0000 00da 0950 7974 686f 6e41 7070  ri.....PythonApp
-000024a0: da0d 6e6f 6465 4461 7461 4172 7261 79da  ..nodeDataArray.
-000024b0: 0d6c 696e 6b44 6174 6141 7272 6179 725c  .linkDataArrayr\
-000024c0: 0000 0029 1972 3c00 0000 7218 0000 00da  ...).r<...r.....
-000024d0: 0965 6e75 6d65 7261 7465 7212 0000 0072  .enumerater....r
-000024e0: 0500 0000 da04 4441 5441 da0b 4150 504c  ......DATA..APPL
-000024f0: 4943 4154 494f 4eda 0661 7070 656e 6472  ICATION..appendr
-00002500: 1400 0000 5a0a 7375 6363 6573 736f 7273  ....Z.successors
-00002510: 7247 0000 0072 2300 0000 7206 0000 00da  rG...r#...r.....
-00002520: 0b61 6464 436f 6e73 756d 6572 da08 6164  .addConsumer..ad
-00002530: 6449 6e70 7574 da09 6164 644f 7574 7075  dInput..addOutpu
-00002540: 74da 0b61 6464 5072 6f64 7563 6572 7213  t..addProducerr.
-00002550: 0000 0072 3f00 0000 5a08 6164 645f 6e6f  ...r?...Z.add_no
-00002560: 6465 5a11 7265 6d6f 7665 5f65 6467 6573  deZ.remove_edges
-00002570: 5f66 726f 6d5a 0e61 6464 5f65 6467 6573  _fromZ.add_edges
-00002580: 5f66 726f 6dda 0e5f 676f 6a73 5f6a 736f  _from.._gojs_jso
-00002590: 6e5f 6f62 6a72 4e00 0000 7262 0000 0029  n_objrN...rb...)
-000025a0: 1e72 2000 0000 da0a 7374 7269 6e67 5f72  .r .....string_r
-000025b0: 6570 5a07 6f75 7464 6963 7472 4c00 0000  epZ.outdictrL...
-000025c0: 7246 0000 0072 3a00 0000 7247 0000 00da  rF...r:...rG....
-000025d0: 056c 696e 6b73 5a08 6b65 795f 6469 6374  .linksZ.key_dict
-000025e0: da01 6972 6800 0000 7259 0000 0072 5a00  ..irh...rY...rZ.
-000025f0: 0000 da02 7474 5a0b 6578 7472 615f 6472  ....ttZ.extra_dr
-00002600: 6f70 735a 0c72 656d 6f76 655f 6564 6765  opsZ.remove_edge
-00002610: 735a 0961 6464 5f65 6467 6573 5a09 6164  sZ.add_edgesZ.ad
-00002620: 645f 6e6f 6465 735a 036d 796b 5a03 6f75  d_nodesZ.mykZ.ou
-00002630: 70da 046c 696e 6b5a 0766 726f 6d5f 6474  p..linkZ.from_dt
-00002640: 5a05 746f 5f64 745a 0774 6f5f 6472 6f70  Z.to_dtZ.to_drop
-00002650: 5a09 6578 7472 615f 6f69 645a 0864 726f  Z.extra_oidZ.dro
-00002660: 7053 7065 635a 046d 7964 74da 036c 6964  pSpecZ.mydt..lid
-00002670: 5a07 656e 646c 696e 6b5a 0267 6e72 0c00  Z.endlinkZ.gnr..
-00002680: 0000 720c 0000 0072 0d00 0000 724d 0000  ..r....r....rM..
-00002690: 005b 0100 0073 f600 0000 0007 0601 0601  .[...s..........
-000026a0: 0801 0401 0401 0602 1201 0801 0601 0c01  ................
-000026b0: 0c01 0801 0801 0a01 0a01 0a01 0801 0c01  ................
-000026c0: 0c02 0c01 0401 0401 0401 0401 0c01 0801  ................
-000026d0: 0801 1801 0601 0803 10ff 0802 02fd 0205  ................
-000026e0: 0e01 0a01 0e01 0a02 0c01 0202 0201 0401  ................
-000026f0: 0201 0201 02fb 04ff 040a 0a01 0a01 0a01  ................
-00002700: 0a01 0603 0c01 0202 0201 0401 0201 0201  ................
-00002710: 02fb 04ff 0409 0a01 0a01 0a01 0a01 0401  ................
-00002720: 0a01 0c01 0801 0601 0801 0801 0a03 0402  ................
-00002730: 0201 0201 0201 0201 10fb 02ff 0409 0e01  ................
-00002740: 0e01 1002 0801 0e01 0802 0401 0601 0601  ................
-00002750: 0601 0601 06fb 0a07 0a01 0a01 0802 0a01  ................
-00002760: 0801 0801 0e01 0601 0801 0801 1203 1201  ................
-00002770: 0801 0601 1001 0801 0801 0c01 0a01 0c01  ................
-00002780: 0801 0c01 0e02 0801 0801 0601 0601 0e02  ................
-00002790: 7a10 5047 542e 746f 5f67 6f6a 735f 6a73  z.PGT.to_gojs_js
-000027a0: 6f6e 2901 5429 0154 2903 4672 3e00 0000  on).T).T).Fr>...
-000027b0: 4629 0346 7202 0000 0046 2904 5472 4b00  F).Fr....F).TrK.
-000027c0: 0000 7202 0000 0054 2903 544e 4629 1672  ..r....T).TNF).r
-000027d0: 0900 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
-000027e0: 5f5f 646f 635f 5f72 2200 0000 7226 0000  __doc__r"...r&..
-000027f0: 00da 0870 726f 7065 7274 7972 2900 0000  ...propertyr)...
-00002800: 722b 0000 0072 3000 0000 7231 0000 0072  r+...r0...r1...r
-00002810: 3b00 0000 7238 0000 0072 3c00 0000 7237  ;...r8...r<...r7
-00002820: 0000 0072 3600 0000 724e 0000 0072 5000  ...r6...rN...rP.
-00002830: 0000 da06 7365 7474 6572 7254 0000 0072  ....setterrT...r
-00002840: 6a00 0000 724d 0000 0072 0c00 0000 720c  j...rM...r....r.
-00002850: 0000 0072 0c00 0000 720d 0000 0072 0f00  ...r....r....r..
-00002860: 0000 3300 0000 7346 0000 0008 0104 040a  ..3...sF........
-00002870: 1708 1802 010a 0608 0608 0708 080a 0d08  ................
-00002880: 0302 010a 0a02 010a 0e00 0000 0000 ff0a  ................
-00002890: 1302 010a 0b02 010a 0304 010a 0400 0000  ................
-000028a0: 0000 ff0a 0800 0100 0100 0100 fa0a 7f00  ................
-000028b0: 0472 0f00 0000 2913 728b 0000 0072 0900  .r....).r....r..
-000028c0: 0000 da0b 5f5f 7061 636b 6167 655f 5f72  ....__package__r
-000028d0: 4e00 0000 da07 6c6f 6767 696e 6772 2d00  N.....loggingr-.
-000028e0: 0000 da0f 646c 672e 6472 6f70 6d61 6b65  ....dlg.dropmake
-000028f0: 2e6c 6772 0300 0000 da16 646c 672e 6472  .lgr......dlg.dr
-00002900: 6f70 6d61 6b65 2e73 6368 6564 756c 6572  opmake.scheduler
-00002910: 7204 0000 00da 0a64 6c67 2e63 6f6d 6d6f  r......dlg.commo
-00002920: 6e72 0500 0000 7206 0000 00da 0967 6574  nr....r......get
-00002930: 4c6f 6767 6572 725e 0000 0072 0700 0000  Loggerr^...r....
-00002940: 720e 0000 00da 066f 626a 6563 7472 0f00  r......objectr..
-00002950: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00002960: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002970: 1600 0000 7318 0000 0004 0608 0104 0308  ....s...........
-00002980: 0108 0108 020c 010c 0110 020a 0310 0410  ................
-00002990: 04                                       .
+00000280: 412f 686f 6d65 2f61 7769 6365 6e65 632f  A/home/awicenec/
+00000290: 6769 742f 6461 6c69 7567 652f 6461 6c69  git/daliuge/dali
+000002a0: 7567 652d 7472 616e 736c 6174 6f72 2f64  uge-translator/d
+000002b0: 6c67 2f64 726f 706d 616b 652f 7067 742e  lg/dropmake/pgt.
+000002c0: 7079 7207 0000 002b 0000 0073 0200 0000  pyr....+...s....
+000002d0: 0801 7207 0000 0063 0000 0000 0000 0000  ..r....c........
+000002e0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+000002f0: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
+00000300: 0029 02da 0d47 5047 5445 7863 6570 7469  .)...GPGTExcepti
+00000310: 6f6e 4e72 0800 0000 720c 0000 0072 0c00  onNr....r....r..
+00000320: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000330: 002f 0000 0073 0200 0000 0801 720e 0000  ./...s......r...
+00000340: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000350: 0000 0400 0000 4000 0000 73be 0000 0065  ......@...s....e
+00000360: 005a 0164 005a 0264 015a 0364 2964 0364  .Z.d.Z.d.Z.d)d.d
+00000370: 0484 015a 0464 0564 0684 005a 0565 0664  ...Z.d.d...Z.e.d
+00000380: 0764 0884 0083 015a 0764 0964 0a84 005a  .d.....Z.d.d...Z
+00000390: 0864 0b64 0c84 005a 0964 0d64 0e84 005a  .d.d...Z.d.d...Z
+000003a0: 0a64 2a64 0f64 1084 015a 0b64 1164 1284  .d*d.d...Z.d.d..
+000003b0: 005a 0c65 0664 1364 1484 0083 015a 0d65  .Z.e.d.d.....Z.e
+000003c0: 0664 1564 1684 0083 015a 0e64 2b64 1964  .d.d.....Z.d+d.d
+000003d0: 1a84 015a 0f65 0664 1b64 1c84 0083 015a  ...Z.e.d.d.....Z
+000003e0: 1065 0664 1d64 1e84 0083 015a 1165 116a  .e.d.d.....Z.e.j
+000003f0: 1264 1f64 1e84 0083 015a 1164 2c64 2164  .d.d.....Z.d,d!d
+00000400: 2284 015a 1364 2d64 2464 2584 015a 1464  "..Z.d-d$d%..Z.d
+00000410: 2e64 2764 2884 015a 1564 2653 0029 2fda  .d'd(..Z.d&S.)/.
+00000420: 0350 4754 7a3a 0a20 2020 2041 2044 524f  .PGTz:.    A DRO
+00000430: 5020 7265 7072 6573 656e 7461 7469 6f6e  P representation
+00000440: 206f 6620 5068 7973 6963 616c 2047 7261   of Physical Gra
+00000450: 7068 2054 656d 706c 6174 650a 2020 2020  ph Template.    
+00000460: 5463 0300 0000 0000 0000 0000 0000 0300  Tc..............
+00000470: 0000 0300 0000 4300 0000 737a 0000 007c  ......C...sz...|
+00000480: 017c 005f 0074 017c 0183 017c 005f 0267  .|._.t.|...|._.g
+00000490: 007c 005f 037c 0272 2674 04a0 057c 006a  .|._.|.r&t...|.j
+000004a0: 00a1 016e 0264 007c 005f 0664 007c 005f  ...n.d.|._.d.|._
+000004b0: 0774 0883 007c 005f 0974 0883 007c 005f  .t...|._.t...|._
+000004c0: 0a64 017c 005f 0b64 017c 005f 0c67 007c  .d.|._.d.|._.g.|
+000004d0: 005f 0d64 027c 005f 0e64 037c 005f 0f64  ._.d.|._.d.|._.d
+000004e0: 0464 0567 027c 005f 1064 007c 005f 1169  .d.g.|._.d.|._.i
+000004f0: 007c 005f 1264 0053 0029 064e 7202 0000  .|._.d.S.).Nr...
+00000500: 00e7 0000 0000 0000 2440 46da 0444 6174  ........$@F..Dat
+00000510: 615a 0743 6f6d 7075 7465 2913 da0a 5f64  aZ.Compute)..._d
+00000520: 726f 705f 6c69 7374 da03 6c65 6e5a 0e5f  rop_list..lenZ._
+00000530: 6472 6f70 5f6c 6973 745f 6c65 6eda 0c5f  drop_list_len.._
+00000540: 6578 7472 615f 6472 6f70 7372 0400 0000  extra_dropsr....
+00000550: da14 6275 696c 645f 6461 675f 6672 6f6d  ..build_dag_from
+00000560: 5f64 726f 7073 da04 5f64 6167 da09 5f6a  _drops.._dag.._j
+00000570: 736f 6e5f 7374 72da 0464 6963 74da 0c5f  son_str..dict.._
+00000580: 6f69 645f 6769 645f 6d61 70da 125f 6769  oid_gid_map.._gi
+00000590: 645f 6973 6c61 6e64 5f69 645f 6d61 70da  d_island_id_map.
+000005a0: 0f5f 6e75 6d5f 7061 7274 735f 646f 6e65  ._num_parts_done
+000005b0: da11 5f70 6172 7469 7469 6f6e 5f6d 6572  .._partition_mer
+000005c0: 6765 645a 0c5f 696e 6e65 725f 7061 7274  gedZ._inner_part
+000005d0: 735a 095f 6277 5f72 6174 696f da0c 5f6d  sZ._bw_ratio.._m
+000005e0: 6572 6765 5f70 6172 7473 5a0e 5f69 736c  erge_partsZ._isl
+000005f0: 616e 645f 6c61 6265 6c73 da0e 5f64 6174  and_labels.._dat
+00000600: 615f 6d6f 7665 6d65 6e74 da0a 5f72 6570  a_movement.._rep
+00000610: 726f 6461 7461 2903 da04 7365 6c66 da09  rodata)...self..
+00000620: 6472 6f70 5f6c 6973 745a 0962 7569 6c64  drop_listZ.build
+00000630: 5f64 6167 720c 0000 0072 0c00 0000 720d  _dagr....r....r.
+00000640: 0000 00da 085f 5f69 6e69 745f 5f38 0000  .....__init__8..
+00000650: 0073 1e00 0000 0001 0601 0a01 0601 1601  .s..............
+00000660: 0601 0801 0801 0601 0601 0602 0602 0601  ................
+00000670: 0a01 0601 7a0c 5047 542e 5f5f 696e 6974  ....z.PGT.__init
+00000680: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
+00000690: 0000 0006 0000 0043 0000 0073 6600 0000  .......C...sf...
+000006a0: 7c01 6401 6b01 7216 7400 6402 a001 7c01  |.d.k.r.t.d...|.
+000006b0: a101 8301 8201 7c00 6a02 732e 7400 6403  ......|.j.s.t.d.
+000006c0: a001 7c00 6a03 6a04 a101 8301 8201 7c00  ..|.j.j.......|.
+000006d0: 6a05 7c01 6b01 7250 7406 6404 a001 7c00  j.|.k.rPt.d...|.
+000006e0: 6a03 6a04 7c00 6a05 7c01 a103 8301 8201  j.j.|.j.|.......
+000006f0: 7c00 6a07 7c01 6b02 725e 6405 5300 6406  |.j.|.k.r^d.S.d.
+00000700: 5300 6400 5300 2907 4e72 0200 0000 7a19  S.d.S.).Nr....z.
+00000710: 496e 7661 6c69 6420 6e65 775f 6e75 6d5f  Invalid new_num_
+00000720: 7061 7274 7320 7b30 7d7a 2554 6869 7320  parts {0}z%This 
+00000730: 7b30 7d20 5047 5450 2069 7320 6e6f 7420  {0} PGTP is not 
+00000740: 6d61 6465 2066 6f72 206d 6572 6769 6e67  made for merging
+00000750: 7a2a 4e6f 206e 6565 6420 746f 206d 6572  z*No need to mer
+00000760: 6765 2074 6869 7320 7b30 7d20 5047 5450  ge this {0} PGTP
+00000770: 3a20 7b31 7d20 3c3d 207b 327d 4654 2908  : {1} <= {2}FT).
+00000780: 720e 0000 00da 0666 6f72 6d61 7472 1d00  r......formatr..
+00000790: 0000 da09 5f5f 636c 6173 735f 5f72 0900  ....__class__r..
+000007a0: 0000 721b 0000 0072 0700 0000 721c 0000  ..r....r....r...
+000007b0: 0029 0272 2000 0000 da0d 6e65 775f 6e75  .).r .....new_nu
+000007c0: 6d5f 7061 7274 7372 0c00 0000 720c 0000  m_partsr....r...
+000007d0: 0072 0d00 0000 da0a 5f63 616e 5f6d 6572  .r......_can_mer
+000007e0: 6765 4b00 0000 7322 0000 0000 0108 010e  geK...s"........
+000007f0: 0106 0102 010c ff04 030a 0102 0104 0106  ................
+00000800: 0104 0102 fd02 ff04 070a 0104 027a 0e50  .............z.P
+00000810: 4754 2e5f 6361 6e5f 6d65 7267 6563 0100  GT._can_mergec..
+00000820: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000830: 0000 4300 0000 7320 0000 007c 006a 0064  ..C...s ...|.j.d
+00000840: 006b 0872 107c 006a 0153 007c 006a 017c  .k.r.|.j.S.|.j.|
+00000850: 006a 0017 0053 0064 0053 00a9 014e 2902  .j...S.d.S...N).
+00000860: 7214 0000 0072 1200 0000 a901 7220 0000  r....r......r ..
+00000870: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000880: da05 6472 6f70 735f 0000 0073 0600 0000  ..drops_...s....
+00000890: 0002 0a01 0602 7a09 5047 542e 6472 6f70  ......z.PGT.drop
+000008a0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+000008b0: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
+000008c0: 0064 0183 0182 0164 0253 0029 037a 410a  .d.....d.S.).zA.
+000008d0: 2020 2020 2020 2020 436f 6e76 6572 7420          Convert 
+000008e0: 746f 2066 6f72 6d61 7420 666f 7220 6d61  to format for ma
+000008f0: 7070 696e 6720 616e 6420 6465 636f 6d70  pping and decomp
+00000900: 6f73 6974 696f 6e0a 2020 2020 2020 2020  osition.        
+00000910: 7a2a 4d75 7374 2062 6520 696d 706c 656d  z*Must be implem
+00000920: 656e 7465 6420 6279 2050 4754 5020 7375  ented by PGTP su
+00000930: 622d 636c 6173 7320 6f6e 6c79 4e29 0172  b-class onlyN).r
+00000940: 0e00 0000 2902 7220 0000 00da 046f 7574  ....).r .....out
+00000950: 6672 0c00 0000 720c 0000 0072 0d00 0000  fr....r....r....
+00000960: da12 746f 5f70 6172 7469 7469 6f6e 5f69  ..to_partition_i
+00000970: 6e70 7574 6600 0000 7302 0000 0000 047a  nputf...s......z
+00000980: 1650 4754 2e74 6f5f 7061 7274 6974 696f  .PGT.to_partitio
+00000990: 6e5f 696e 7075 7463 0100 0000 0000 0000  n_inputc........
+000009a0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+000009b0: 731c 0000 0074 007c 006a 0183 017d 0174  s....t.|.j...}.t
+000009c0: 0274 03a0 047c 0164 011b 00a1 0183 0153  .t...|.d.......S
+000009d0: 0029 027a 1f0a 2020 2020 2020 2020 6475  .).z..        du
+000009e0: 6d6d 7920 666f 7220 6e6f 770a 2020 2020  mmy for now.    
+000009f0: 2020 2020 7210 0000 0029 0572 1300 0000      r....).r....
+00000a00: 7212 0000 00da 0369 6e74 da04 6d61 7468  r......int..math
+00000a10: da04 6365 696c 2902 7220 0000 00da 046c  ..ceil).r .....l
+00000a20: 656e 6772 0c00 0000 720c 0000 0072 0d00  engr....r....r..
+00000a30: 0000 da11 6765 745f 6f70 745f 6e75 6d5f  ....get_opt_num_
+00000a40: 7061 7274 736c 0000 0073 0400 0000 0004  partsl...s......
+00000a50: 0a01 7a15 5047 542e 6765 745f 6f70 745f  ..z.PGT.get_opt_
+00000a60: 6e75 6d5f 7061 7274 7363 0100 0000 0000  num_partsc......
+00000a70: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000a80: 0000 7304 0000 0064 0153 0029 024e 5a0d  ..s....d.S.).NZ.
+00000a90: 5261 775f 756e 726f 6c6c 696e 6772 0c00  Raw_unrollingr..
+00000aa0: 0000 7228 0000 0072 0c00 0000 720c 0000  ..r(...r....r...
+00000ab0: 0072 0d00 0000 da12 6765 745f 7061 7274  .r......get_part
+00000ac0: 6974 696f 6e5f 696e 666f 7300 0000 7302  ition_infos...s.
+00000ad0: 0000 0000 067a 1650 4754 2e67 6574 5f70  .....z.PGT.get_p
+00000ae0: 6172 7469 7469 6f6e 5f69 6e66 6f63 0200  artition_infoc..
+00000af0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000b00: 0000 4300 0000 7368 0000 0069 007d 027c  ..C...sh...i.}.|
+00000b10: 00a0 00a1 007c 0264 013c 007c 006a 0164  .....|.d.<.|.j.d
+00000b20: 027c 010c 0064 038d 027c 0264 043c 007c  .|...d...|.d.<.|
+00000b30: 006a 027c 0264 053c 007c 006a 017c 010c  .j.|.d.<.|.j.|..
+00000b40: 0064 068d 017c 0264 073c 007c 006a 0372  .d...|.d.<.|.j.r
+00000b50: 5a7c 006a 0464 086b 0472 5a7c 006a 047c  Z|.j.d.k.rZ|.j.|
+00000b60: 0264 093c 007c 00a0 057c 02a1 0101 007c  .d.<.|...|.....|
+00000b70: 0253 0029 0a4e da04 616c 676f 5429 02da  .S.).N..algoT)..
+00000b80: 0d61 7070 5f64 726f 705f 6f6e 6c79 da0c  .app_drop_only..
+00000b90: 666f 7263 655f 616e 7377 6572 5a0d 6d69  force_answerZ.mi
+00000ba0: 6e5f 6578 6563 5f74 696d 655a 1374 6f74  n_exec_timeZ.tot
+00000bb0: 616c 5f64 6174 615f 6d6f 7665 6d65 6e74  al_data_movement
+00000bc0: 2901 7234 0000 005a 0965 7865 635f 7469  ).r4...Z.exec_ti
+00000bd0: 6d65 7202 0000 00da 0b6e 756d 5f69 736c  mer......num_isl
+00000be0: 616e 6473 2906 7231 0000 00da 0e70 7265  ands).r1.....pre
+00000bf0: 645f 6578 6563 5f74 696d 65da 0d64 6174  d_exec_time..dat
+00000c00: 615f 6d6f 7665 6d65 6e74 721d 0000 0072  a_movementr....r
+00000c10: 1c00 0000 da0d 5f65 7874 7261 5f72 6573  ......_extra_res
+00000c20: 756c 7429 0372 2000 0000 5a04 6c61 7a79  ult).r ...Z.lazy
+00000c30: da03 7265 7472 0c00 0000 720c 0000 0072  ..retr....r....r
+00000c40: 0d00 0000 da06 7265 7375 6c74 7b00 0000  ......result{...
+00000c50: 7318 0000 0000 0104 010c 0104 0102 0004  s...............
+00000c60: ff0a 030a 0112 0110 010a 010a 017a 0a50  .............z.P
+00000c70: 4754 2e72 6573 756c 7463 0200 0000 0000  GT.resultc......
+00000c80: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00000c90: 0000 7304 0000 0064 0053 0072 2700 0000  ..s....d.S.r'...
+00000ca0: 720c 0000 0029 0272 2000 0000 7239 0000  r....).r ...r9..
+00000cb0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000cc0: 7238 0000 0088 0000 0073 0200 0000 0001  r8.......s......
+00000cd0: 7a11 5047 542e 5f65 7874 7261 5f72 6573  z.PGT._extra_res
+00000ce0: 756c 7463 0100 0000 0000 0000 0000 0000  ultc............
+00000cf0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00000d00: 007c 006a 0053 0029 017a fb0a 2020 2020  .|.j.S.).z..    
+00000d10: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+00000d20: 6865 206e 6574 776f 726b 7820 6e78 2e44  he networkx nx.D
+00000d30: 6947 7261 7068 206f 626a 6563 740a 0a20  iGraph object.. 
+00000d40: 2020 2020 2020 2054 6865 2077 6569 6768         The weigh
+00000d50: 7420 6f66 2074 6865 2073 616d 6520 6564  t of the same ed
+00000d60: 6765 2028 752c 2076 2920 616c 736f 2064  ge (u, v) also d
+00000d70: 6570 656e 6473 2e0a 2020 2020 2020 2020  epends..        
+00000d80: 4966 2069 7420 6973 2063 616c 6c65 6420  If it is called 
+00000d90: 6166 7465 7220 7468 6520 7061 7274 6974  after the partit
+00000da0: 696f 6e69 6e67 2c20 6974 2063 6f75 6c64  ioning, it could
+00000db0: 2068 6176 6520 6265 656e 207a 6572 6f65   have been zeroe
+00000dc0: 640a 2020 2020 2020 2020 6966 2062 6f74  d.        if bot
+00000dd0: 6820 7520 616e 6420 7620 6973 2061 6c6c  h u and v is all
+00000de0: 6f63 6174 6564 2074 6f20 7468 6520 7361  ocated to the sa
+00000df0: 6d65 2044 726f 7049 736c 616e 640a 2020  me DropIsland.  
+00000e00: 2020 2020 2020 2901 7216 0000 0072 2800        ).r....r(.
+00000e10: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000e20: 00da 0364 6167 8b00 0000 7302 0000 0000  ...dag....s.....
+00000e30: 097a 0750 4754 2e64 6167 6301 0000 0000  .z.PGT.dagc.....
+00000e40: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000e50: 0000 0073 4200 0000 7c00 6a00 6401 6b09  ...sB...|.j.d.k.
+00000e60: 7210 7c00 6a00 5300 7c00 6a01 6401 6b09  r.|.j.S.|.j.d.k.
+00000e70: 723c 7c00 6a01 7d01 7402 6402 6403 8400  r<|.j.}.t.d.d...
+00000e80: 7c01 6a03 6404 6405 8d01 4400 8301 8301  |.j.d.d...D.....
+00000e90: 7c00 5f00 7c00 6a00 5300 2906 7a30 0a20  |._.|.j.S.).z0. 
+00000ea0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+00000eb0: 6520 544f 5441 4c20 6461 7461 206d 6f76  e TOTAL data mov
+00000ec0: 656d 656e 740a 2020 2020 2020 2020 4e63  ement.        Nc
+00000ed0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000ee0: 0500 0000 7300 0000 731e 0000 007c 005d  ....s...s....|.]
+00000ef0: 167d 017c 0164 0019 00a0 0064 0164 02a1  .}.|.d.....d.d..
+00000f00: 0256 0001 0071 0264 0353 0029 04e9 0200  .V...q.d.S.)....
+00000f10: 0000 da06 7765 6967 6874 7202 0000 004e  ....weightr....N
+00000f20: 2901 da03 6765 7429 02da 022e 30da 0165  )...get)....0..e
+00000f30: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000f40: 093c 6765 6e65 7870 723e 9f00 0000 7304  .<genexpr>....s.
+00000f50: 0000 0004 0002 007a 2450 4754 2e64 6174  .......z$PGT.dat
+00000f60: 615f 6d6f 7665 6d65 6e74 2e3c 6c6f 6361  a_movement.<loca
+00000f70: 6c73 3e2e 3c67 656e 6578 7072 3e54 2901  ls>.<genexpr>T).
+00000f80: da04 6461 7461 2904 721e 0000 0072 3b00  ..data).r....r;.
+00000f90: 0000 da03 7375 6dda 0565 6467 6573 2902  ....sum..edges).
+00000fa0: 7220 0000 00da 0147 720c 0000 0072 0c00  r .....Gr....r..
+00000fb0: 0000 720d 0000 0072 3700 0000 9600 0000  ..r....r7.......
+00000fc0: 730c 0000 0000 050a 0106 010a 0106 011c  s...............
+00000fd0: 017a 1150 4754 2e64 6174 615f 6d6f 7665  .z.PGT.data_move
+00000fe0: 6d65 6e74 4672 3d00 0000 6304 0000 0000  mentFr=...c.....
+00000ff0: 0000 0000 0000 0005 0000 0004 0000 0003  ................
+00001000: 0000 0073 7000 0000 7c00 6a00 8900 8800  ...sp...|.j.....
+00001010: 6401 6b08 722c 7c03 7228 7401 a002 7c00  d.k.r,|.r(t...|.
+00001020: 6a03 a101 7c00 5f04 7c00 6a00 8900 6e04  j...|._.|.j...n.
+00001030: 6401 5300 7c01 725a 7401 6a05 8800 6402  d.S.|.rZt.j...d.
+00001040: 6403 8d02 6404 1900 7d04 7406 8700 8701  d...d...}.t.....
+00001050: 6602 6405 6406 8408 7c04 4400 8301 8301  f.d.d...|.D.....
+00001060: 5300 7401 6a05 8800 6407 6403 8d02 6408  S.t.j...d.d...d.
+00001070: 1900 5300 6401 5300 2909 7a46 0a20 2020  ..S.d.S.).zF.   
+00001080: 2020 2020 2050 7265 6469 6374 2065 7865       Predict exe
+00001090: 6375 7469 6f6e 2074 696d 6520 7573 696e  cution time usin
+000010a0: 6720 7468 6520 6c6f 6e67 6573 7420 7061  g the longest pa
+000010b0: 7468 206c 656e 6774 680a 2020 2020 2020  th length.      
+000010c0: 2020 4e54 2901 5a09 7368 6f77 5f70 6174    NT).Z.show_pat
+000010d0: 6872 0200 0000 6301 0000 0000 0000 0000  hr....c.........
+000010e0: 0000 0002 0000 0005 0000 0033 0000 0073  ...........3...s
+000010f0: 2000 0000 7c00 5d18 7d01 8800 6a00 7c01   ...|.].}...j.|.
+00001100: 1900 a001 8801 6400 a102 5600 0100 7102  ......d...V...q.
+00001110: 6401 5300 2902 7202 0000 004e 2902 da05  d.S.).r....N)...
+00001120: 6e6f 6465 7372 3e00 0000 2902 723f 0000  nodesr>...).r?..
+00001130: 00da 0175 a902 7245 0000 00da 0277 6b72  ...u..rE.....wkr
+00001140: 0c00 0000 720d 0000 0072 4100 0000 af00  ....r....rA.....
+00001150: 0000 7304 0000 0004 0002 007a 2550 4754  ..s........z%PGT
+00001160: 2e70 7265 645f 6578 6563 5f74 696d 652e  .pred_exec_time.
+00001170: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00001180: 723e 46e9 0100 0000 2907 723b 0000 0072  r>F.....).r;...r
+00001190: 0400 0000 7215 0000 0072 1200 0000 7216  ....r....r....r.
+000011a0: 0000 005a 1067 6574 5f6c 6f6e 6765 7374  ...Z.get_longest
+000011b0: 5f70 6174 6872 4300 0000 2905 7220 0000  _pathrC...).r ..
+000011c0: 0072 3300 0000 7249 0000 0072 3400 0000  .r3...rI...r4...
+000011d0: 5a02 6c70 720c 0000 0072 4800 0000 720d  Z.lpr....rH...r.
+000011e0: 0000 0072 3600 0000 a200 0000 7314 0000  ...r6.......s...
+000011f0: 0000 0406 0108 0104 010e 0108 0204 0104  ................
+00001200: 0112 0118 027a 1250 4754 2e70 7265 645f  .....z.PGT.pred_
+00001210: 6578 6563 5f74 696d 6563 0100 0000 0000  exec_timec......
+00001220: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001230: 0000 731e 0000 007c 006a 0064 016b 0872  ..s....|.j.d.k.r
+00001240: 187c 006a 0164 0264 038d 017c 005f 007c  .|.j.d.d...|._.|
+00001250: 006a 0053 0029 047a 5c0a 2020 2020 2020  .j.S.).z\.      
+00001260: 2020 5265 7475 726e 2074 6865 204a 534f    Return the JSO
+00001270: 4e20 7374 7269 6e67 2072 6570 7265 7365  N string represe
+00001280: 6e74 6174 696f 6e20 6f66 2074 6865 2050  ntation of the P
+00001290: 4754 0a20 2020 2020 2020 2066 6f72 2076  GT.        for v
+000012a0: 6973 7561 6c69 7361 7469 6f6e 0a20 2020  isualisation.   
+000012b0: 2020 2020 204e 5429 01da 0676 6973 7561       NT)...visua
+000012c0: 6c29 0272 1700 0000 da0c 746f 5f67 6f6a  l).r......to_goj
+000012d0: 735f 6a73 6f6e 7228 0000 0072 0c00 0000  s_jsonr(...r....
+000012e0: 720c 0000 0072 0d00 0000 da04 6a73 6f6e  r....r......json
+000012f0: b300 0000 7306 0000 0000 060a 010e 027a  ....s..........z
+00001300: 0850 4754 2e6a 736f 6e63 0100 0000 0000  .PGT.jsonc......
+00001310: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00001320: 0000 7306 0000 007c 006a 0053 0072 2700  ..s....|.j.S.r'.
+00001330: 0000 a901 721f 0000 0072 2800 0000 720c  ....r....r(...r.
+00001340: 0000 0072 0c00 0000 720d 0000 00da 0972  ...r....r......r
+00001350: 6570 726f 6461 7461 bf00 0000 7302 0000  eprodata....s...
+00001360: 0000 027a 0d50 4754 2e72 6570 726f 6461  ...z.PGT.reproda
+00001370: 7461 6302 0000 0000 0000 0000 0000 0002  tac.............
+00001380: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00001390: 7c01 7c00 5f00 6400 5300 7227 0000 0072  |.|._.d.S.r'...r
+000013a0: 4e00 0000 2902 7220 0000 00da 0576 616c  N...).r .....val
+000013b0: 7565 720c 0000 0072 0c00 0000 720d 0000  uer....r....r...
+000013c0: 0072 4f00 0000 c300 0000 7302 0000 0000  .rO.......s.....
+000013d0: 0272 0200 0000 6305 0000 0000 0000 0000  .r....c.........
+000013e0: 0000 0005 0000 0002 0000 0043 0000 0073  ...........C...s
+000013f0: 0c00 0000 7400 6401 8301 8201 6400 5300  ....t.d.....d.S.
+00001400: 2902 4e7a 1f4e 6f74 2069 6d70 6c65 6d65  ).Nz.Not impleme
+00001410: 6e74 6564 2e20 4361 6c6c 2073 7562 2d63  nted. Call sub-c
+00001420: 6c61 7373 2901 da09 4578 6365 7074 696f  lass)...Exceptio
+00001430: 6e29 0572 2000 0000 7225 0000 00da 0b66  n).r ...r%.....f
+00001440: 6f72 6d5f 6973 6c61 6e64 5a0b 6973 6c61  orm_islandZ.isla
+00001450: 6e64 5f74 7970 6572 4b00 0000 720c 0000  nd_typerK...r...
+00001460: 0072 0c00 0000 720d 0000 00da 106d 6572  .r....r......mer
+00001470: 6765 5f70 6172 7469 7469 6f6e 73c7 0000  ge_partitions...
+00001480: 0073 0200 0000 0003 7a14 5047 542e 6d65  .s......z.PGT.me
+00001490: 7267 655f 7061 7274 6974 696f 6e73 724a  rge_partitionsrJ
+000014a0: 0000 0063 0600 0000 0000 0000 0000 0000  ...c............
+000014b0: 1400 0000 0800 0000 4300 0000 7362 0200  ........C...sb..
+000014c0: 0074 00a0 0164 017c 047c 01a1 0301 0074  .t...d.|.|.....t
+000014d0: 027c 0183 0164 026b 0272 307c 0464 026b  .|...d.k.r0|.d.k
+000014e0: 0472 3074 037c 0483 017d 0164 037d 066e  .r0t.|...}.d.}.n
+000014f0: 0464 047d 0664 027c 006a 046b 0272 4674  .d.}.d.|.j.k.rFt
+00001500: 0564 0583 0182 017c 0164 066b 0873 5a64  .d.....|.d.k.sZd
+00001510: 0274 027c 0183 016b 0272 6274 0564 0783  .t.|...k.rbt.d..
+00001520: 0182 0174 027c 0183 017d 077a 0c74 067c  ...t.|...}.z.t.|
+00001530: 0383 017d 0357 006e 1a01 0001 0001 0074  ...}.W.n.......t
+00001540: 0564 08a0 077c 03a1 0183 0182 0159 006e  .d...|.......Y.n
+00001550: 0258 007c 0364 096b 0072 9e64 097d 037c  .X.|.d.k.r.d.}.|
+00001560: 037c 076b 0472 ae74 0564 0a83 0182 017c  .|.k.r.t.d.....|
+00001570: 0364 096b 047d 087c 0764 096b 0072 cc74  .d.k.}.|.d.k.r.t
+00001580: 0564 0ba0 077c 07a1 0183 0182 017c 006a  .d...|.......|.j
+00001590: 047d 097c 006a 087d 0a7c 0590 0173 127c  .}.|.j.}.|...s.|
+000015a0: 0872 f87c 097c 076b 0472 f874 0564 0ca0  .r.|.|.k.r.t.d..
+000015b0: 077c 07a1 0183 0182 017c 0164 027c 0385  .|.......|.d.|..
+000015c0: 0219 007d 0b7c 017c 0364 0685 0219 007d  ...}.|.|.d.....}
+000015d0: 0c6e 5a7c 0890 0172 347c 037c 0917 007c  .nZ|...r4|.|...|
+000015e0: 076b 0490 0172 3474 0564 0ca0 077c 07a1  .k...r4t.d...|..
+000015f0: 0183 0182 017c 017d 0b74 097c 0174 0a83  .....|.}.t.|.t..
+00001600: 0290 0172 6874 027c 0183 0164 096b 0490  ...rht.|...d.k..
+00001610: 0172 687c 0164 0919 0067 017c 0164 0964  .rh|.d...g.|.d.d
+00001620: 0685 0219 0017 006e 027c 017d 0c74 027c  .......n.|.}.t.|
+00001630: 0c83 017d 0d74 00a0 0b64 0d74 027c 0a83  ...}.t...d.t.|..
+00001640: 017c 097c 0774 027c 0b83 017c 05a1 0601  .|.|.t.|...|....
+00001650: 007c 0890 0172 a67c 006a 0c7c 0364 0364  .|...r.|.j.|.d.d
+00001660: 0e8d 0201 006e 1c7c 0d7c 096b 0090 0172  .....n.|.|.k...r
+00001670: c27c 006a 0c7c 0d64 0464 0e8d 0201 007c  .|.j.|.d.d.....|
+00001680: 0d7d 097c 006a 0d7d 0e7c 006a 0e7d 0f7c  .}.|.j.}.|.j.}.|
+00001690: 0690 0172 fc64 0f64 1084 0074 037c 0d83  ...r.d.d...t.|..
+000016a0: 0144 0083 017d 0c64 1164 1084 0074 0374  .D...}.d.d...t.t
+000016b0: 027c 0b83 0183 0144 0083 017d 0b7c 0a44  .|.....D...}.|.D
+000016c0: 005d 447d 107c 1064 1219 007d 117c 0e7c  .]D}.|.d...}.|.|
+000016d0: 1119 007d 127c 0c7c 1219 007c 1064 133c  ...}.|.|...|.d.<
+000016e0: 007c 0890 0272 327c 0f7c 1219 007c 0316  .|...r2|.|...|..
+000016f0: 006e 0264 027d 137c 0b7c 1319 007c 1064  .n.d.}.|.|...|.d
+00001700: 143c 0090 0271 007c 0290 0272 5a74 0f6a  .<...q.|...rZt.j
+00001710: 107c 0a64 1564 168d 0253 007c 0a53 0064  .|.d.d...S.|.S.d
+00001720: 0653 0029 1761 2903 0000 0a20 2020 2020  .S.).a)....     
+00001730: 2020 2063 6f6e 7665 7274 2070 6774 2074     convert pgt t
+00001740: 6f20 7067 2073 7065 6369 6669 6361 7469  o pg specificati
+00001750: 6f6e 2c20 616e 6420 6d61 7020 7468 6174  on, and map that
+00001760: 2074 6f20 7468 6520 6861 7264 7761 7265   to the hardware
+00001770: 2072 6573 6f75 7263 6573 0a0a 2020 2020   resources..    
+00001780: 2020 2020 6e6f 6465 5f6c 6973 743a 0a20      node_list:. 
+00001790: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
+000017a0: 7420 6f66 206e 6f64 6573 2028 6c69 7374  t of nodes (list
+000017b0: 292c 2077 686f 7365 206c 656e 6774 6820  ), whose length 
+000017c0: 3d3d 2028 6e75 6d5f 6973 6c61 6e64 7320  == (num_islands 
+000017d0: 2b20 6e75 6d5f 6e6f 6465 5f6d 6772 7329  + num_node_mgrs)
+000017e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000017f0: 636f 5f6c 6f63 6174 655f 6973 6c61 6e64  co_locate_island
+00001800: 7320 3d20 4661 6c73 652e 0a20 2020 2020  s = False..     
+00001810: 2020 2020 2020 2057 6520 6173 7375 6d65         We assume
+00001820: 2074 6861 7420 7468 6520 4d61 7374 6572   that the Master
+00001830: 4472 6f70 4d61 6e61 6765 7227 7320 6e6f  DropManager's no
+00001840: 6465 2069 7320 4e4f 5420 696e 2074 6865  de is NOT in the
+00001850: 206e 6f64 655f 6c69 7374 0a0a 2020 2020   node_list..    
+00001860: 2020 2020 6e75 6d5f 6973 6c61 6e64 733a      num_islands:
+00001870: 0a20 2020 2020 2020 2020 2020 202d 203e  .            - >
+00001880: 3120 5061 7274 6974 696f 6e73 2061 7265  1 Partitions are
+00001890: 2022 636f 6e63 6570 7475 616c 6c79 2220   "conceptually" 
+000018a0: 636c 7573 7465 7265 6420 696e 746f 2049  clustered into I
+000018b0: 736c 616e 6473 0a20 2020 2020 2020 2020  slands.         
+000018c0: 2020 202d 2031 2050 6172 7469 7469 6f6e     - 1 Partition
+000018d0: 7320 4d41 5920 4245 2070 6879 7369 6361  s MAY BE physica
+000018e0: 6c6c 7920 6d65 7267 6564 2077 6974 686f  lly merged witho
+000018f0: 7574 2067 656e 6572 6174 696e 6720 6973  ut generating is
+00001900: 6c61 6e64 730a 2020 2020 2020 2020 2020  lands.          
+00001910: 2020 2020 6465 7065 6e64 696e 6720 6f6e      depending on
+00001920: 2074 6865 206c 656e 6774 6820 6f66 206e   the length of n
+00001930: 6f64 655f 6c69 7374 0a20 2020 2020 2020  ode_list.       
+00001940: 2020 2020 202d 206e 756d 5f69 736c 616e       - num_islan
+00001950: 6473 2063 616e 2774 2062 6520 3c20 310a  ds can't be < 1.
+00001960: 0a20 2020 2020 2020 2074 706c 5f6e 6f64  .        tpl_nod
+00001970: 6573 5f6c 656e 3a20 6966 2074 6869 7320  es_len: if this 
+00001980: 6973 2067 6976 656e 2077 6520 6765 6e65  is given we gene
+00001990: 7261 7465 2061 2070 675f 7370 6563 2074  rate a pg_spec t
+000019a0: 656d 706c 6174 650a 2020 2020 2020 2020  emplate.        
+000019b0: 2020 2020 5468 6520 7067 5f73 7065 6320      The pg_spec 
+000019c0: 7465 6d70 6c61 7465 2069 7320 7768 6174  template is what
+000019d0: 206e 6565 6473 2074 6f20 6265 2073 656e   needs to be sen
+000019e0: 6420 746f 2061 2064 6566 6572 7265 6420  d to a deferred 
+000019f0: 6465 706c 6f79 656d 6e74 0a20 2020 2020  deployemnt.     
+00001a00: 2020 2020 2020 2077 6865 7265 2074 6865         where the
+00001a10: 2064 616c 6975 6765 2073 7973 7465 6d20   daliuge system 
+00001a20: 6973 2073 7461 7274 6564 2075 7020 6166  is started up af
+00001a30: 6572 2073 7562 6d69 7373 696f 6e20 2865  er submission (e
+00001a40: 2e67 2e20 534c 5552 4d29 0a20 2020 2020  .g. SLURM).     
+00001a50: 2020 207a 2c23 2077 6f72 6b65 7220 6e6f     z,# worker no
+00001a60: 6465 733a 2025 732c 206e 6f64 655f 6c69  des: %s, node_li
+00001a70: 7374 2869 6e63 6c2e 2044 494d 293a 2025  st(incl. DIM): %
+00001a80: 7372 0200 0000 5446 7a26 5468 6520 6772  sr....TFz&The gr
+00001a90: 6170 6820 6861 7320 6e6f 7420 6265 656e  aph has not been
+00001aa0: 2070 6172 7469 7469 6f6e 6564 2079 6574   partitioned yet
+00001ab0: 4e7a 134e 6f64 6520 6c69 7374 2069 7320  Nz.Node list is 
+00001ac0: 656d 7074 7921 7a1d 496e 7661 6c69 6420  empty!z.Invalid 
+00001ad0: 6e75 6d5f 6973 6c61 6e64 7320 7370 6563  num_islands spec
+00001ae0: 3a20 7b30 7d72 4a00 0000 7a37 4e75 6d62  : {0}rJ...z7Numb
+00001af0: 6572 206f 6620 6973 6c61 6e64 7320 6d75  er of islands mu
+00001b00: 7374 2062 6520 3c3d 206e 756d 6265 7220  st be <= number 
+00001b10: 6f66 2073 7065 6369 6669 6564 206e 6f64  of specified nod
+00001b20: 6573 217a 1254 6f6f 2066 6577 206e 6f64  es!z.Too few nod
+00001b30: 6573 3a20 7b30 7d7a 2149 6e73 7566 6669  es: {0}z!Insuffi
+00001b40: 6369 656e 7420 6e75 6d62 6572 206f 6620  cient number of 
+00001b50: 6e6f 6465 733a 207b 307d 7a4b 4472 6f70  nodes: {0}zKDrop
+00001b60: 7320 636f 756e 743a 2025 642c 2070 6172  s count: %d, par
+00001b70: 7469 7469 6f6e 7320 636f 756e 743a 2025  titions count: %
+00001b80: 642c 206e 6f64 6573 2063 6f75 6e74 3a20  d, nodes count: 
+00001b90: 2564 2c20 6973 6c61 6e64 2063 6f75 6e74  %d, island count
+00001ba0: 3a20 2564 2025 7329 0172 5200 0000 6301  : %d %s).rR...c.
+00001bb0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001bc0: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00001bd0: 5d0c 7d01 6400 7c01 1600 9102 7104 5300  ].}.d.|.....q.S.
+00001be0: a901 7a03 2325 7372 0c00 0000 a902 723f  ..z.#%sr......r?
+00001bf0: 0000 00da 0178 720c 0000 0072 0c00 0000  .....xr....r....
+00001c00: 720d 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00001c10: 3e3a 0100 0073 0400 0000 0600 0200 7a22  >:...s........z"
+00001c20: 5047 542e 746f 5f70 675f 7370 6563 2e3c  PGT.to_pg_spec.<
+00001c30: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001c40: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+00001c50: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
+00001c60: 6700 7c00 5d0c 7d01 6400 7c01 1600 9102  g.|.].}.d.|.....
+00001c70: 7104 5300 7254 0000 0072 0c00 0000 7255  q.S.rT...r....rU
+00001c80: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00001c90: 0000 7257 0000 003b 0100 0073 0400 0000  ..rW...;...s....
+00001ca0: 0601 0200 da03 6f69 64da 046e 6f64 65da  ......oid..node.
+00001cb0: 0669 736c 616e 6472 3c00 0000 a901 da06  .islandr<.......
+00001cc0: 696e 6465 6e74 2911 da06 6c6f 6767 6572  indent)...logger
+00001cd0: da05 6465 6275 6772 1300 0000 da05 7261  ..debugr......ra
+00001ce0: 6e67 6572 1b00 0000 720e 0000 0072 2c00  nger....r....r,.
+00001cf0: 0000 7223 0000 0072 2900 0000 da0a 6973  ..r#...r).....is
+00001d00: 696e 7374 616e 6365 da04 6c69 7374 da04  instance..list..
+00001d10: 696e 666f 7253 0000 0072 1900 0000 721a  inforS...r....r.
+00001d20: 0000 0072 4d00 0000 da05 6475 6d70 7329  ...rM.....dumps)
+00001d30: 1472 2000 0000 5a09 6e6f 6465 5f6c 6973  .r ...Z.node_lis
+00001d40: 74da 0772 6574 5f73 7472 7235 0000 00da  t..ret_strr5....
+00001d50: 0d74 706c 5f6e 6f64 6573 5f6c 656e da0b  .tpl_nodes_len..
+00001d60: 636f 5f68 6f73 745f 6469 6d5a 0674 706c  co_host_dimZ.tpl
+00001d70: 5f66 6c5a 096e 6f64 6573 5f6c 656e 7252  _flZ.nodes_lenrR
+00001d80: 0000 005a 096e 756d 5f70 6172 7473 7221  ...Z.num_partsr!
+00001d90: 0000 005a 0769 735f 6c69 7374 da07 6e6d  ...Z.is_list..nm
+00001da0: 5f6c 6973 745a 066e 6d5f 6c65 6e5a 026c  _listZ.nm_lenZ.l
+00001db0: 6d5a 036c 6d32 da04 6472 6f70 7258 0000  mZ.lm2..droprX..
+00001dc0: 00da 0367 6964 5a04 6973 6964 720c 0000  ...gidZ.isidr...
+00001dd0: 0072 0c00 0000 720d 0000 00da 0a74 6f5f  .r....r......to_
+00001de0: 7067 5f73 7065 63cc 0000 0073 9a00 0000  pg_spec....s....
+00001df0: 001a 0401 0201 0201 02fd 0405 1401 0801  ................
+00001e00: 0602 0402 0a01 0802 1401 0801 0802 0201  ................
+00001e10: 0c01 0601 1401 0801 0401 0801 0201 02ff  ................
+00001e20: 0403 0801 0801 0e02 0601 0603 0601 0c01  ................
+00001e30: 0201 08ff 0403 0c01 0e02 1401 0201 08ff  ................
+00001e40: 0403 0403 08ff 0401 0aff 1a02 02fd 0205  ................
+00001e50: 0801 0401 0201 0601 0201 0201 0601 02fa  ................
+00001e60: 0409 0601 1003 0a01 0e01 0402 0601 060a  ................
+00001e70: 0601 1201 0601 0aff 0604 0801 0804 0801  ................
+00001e80: 0c01 1601 1002 0601 0e02 7a0e 5047 542e  ..........z.PGT.
+00001e90: 746f 5f70 675f 7370 6563 4e63 0400 0000  to_pg_specNc....
+00001ea0: 0000 0000 0000 0000 1e00 0000 0c00 0000  ................
+00001eb0: 4300 0000 73e8 0300 007c 006a 007d 0474  C...s....|.j.}.t
+00001ec0: 0183 007d 0564 017c 0564 023c 0067 007d  ...}.d.|.d.<.g.}
+00001ed0: 0667 007d 0774 0183 007d 0874 027c 006a  .g.}.t...}.t.|.j
+00001ee0: 0383 0144 005d 7a5c 027d 097d 0a7c 0a64  ...D.]z\.}.}.|.d
+00001ef0: 0319 007d 0b74 0183 007d 0c7c 0964 0417  ...}.t...}.|.d..
+00001f00: 007c 0c64 053c 007c 0964 0417 007c 087c  .|.d.<.|.d...|.|
+00001f10: 0b3c 007c 0b7c 0c64 033c 007c 0a64 0619  .<.|.|.d.<.|.d..
+00001f20: 007d 0d74 046a 057c 0d6b 0272 7e64 077c  .}.t.j.|.k.r~d.|
+00001f30: 0c64 083c 006e 1274 046a 067c 0d6b 0272  .d.<.n.t.j.|.k.r
+00001f40: 9064 097c 0c64 083c 007c 0a64 0a19 007c  .d.|.d.<.|.d...|
+00001f50: 0c64 0a3c 007c 06a0 077c 0ca1 0101 0071  .d.<.|...|.....q
+00001f60: 2c7c 006a 0864 0b6b 0890 0272 e267 007d  ,|.j.d.k...r.g.}
+00001f70: 0e67 007d 0f67 007d 1067 007d 117c 006a  .g.}.g.}.g.}.|.j
+00001f80: 0344 0090 015d c47d 0a7c 0a64 0319 007d  .D...].}.|.d...}
+00001f90: 0b7c 087c 0b19 007d 1274 027c 04a0 097c  .|.|...}.t.|...|
+00001fa0: 12a1 0183 0144 0090 015d 9e5c 027d 097d  .....D...].\.}.}
+00001fb0: 1374 0183 007d 147c 127c 1464 0c3c 007c  .t...}.|.|.d.<.|
+00001fc0: 0a64 0619 0074 046a 0564 0d66 026b 0690  .d...t.j.d.f.k..
+00001fd0: 0172 1e64 0e6e 0264 047d 157c 046a 0a7c  .r.d.n.d.}.|.j.|
+00001fe0: 1319 0064 0f19 007d 167c 157c 166b 0290  ...d...}.|.|.k..
+00001ff0: 0272 7c7c 046a 0a7c 1319 0064 1019 007d  .r||.j.|...d...}
+00002000: 177c 1564 0e6b 0290 0172 a264 11a0 0b7c  .|.d.k...r.d...|
+00002010: 0b7c 09a1 027d 1874 0c7c 1874 046a 0664  .|...}.t.|.t.j.d
+00002020: 1264 1364 0464 149c 0583 017d 197c 0aa0  .d.d.d.....}.|..
+00002030: 0d7c 19a1 0101 007c 19a0 0e7c 0aa1 0101  .|.....|...|....
+00002040: 007c 19a0 0f7c 17a1 0101 007c 17a0 107c  .|...|.....|...|
+00002050: 19a1 0101 0064 047d 1a6e 4e64 15a0 0b7c  .....d.}.nNd...|
+00002060: 0b7c 09a1 027d 1874 0c7c 1874 046a 0564  .|...}.t.|.t.j.d
+00002070: 1664 1764 0464 149c 0583 017d 197c 0aa0  .d.d.d.....}.|..
+00002080: 0f7c 19a1 0101 007c 19a0 107c 0aa1 0101  .|.....|...|....
+00002090: 007c 19a0 0d7c 17a1 0101 007c 17a0 0e7c  .|...|.....|...|
+000020a0: 19a1 0101 0064 0e7d 1a7c 0ea0 077c 19a1  .....d.}.|...|..
+000020b0: 0101 0074 117c 0e83 0164 1814 007d 1b7c  ...t.|...d...}.|
+000020c0: 1b7c 1464 193c 0074 0183 007d 1c7c 1b7c  .|.d.<.t...}.|.|
+000020d0: 1c64 0c3c 007c 137c 1c64 193c 007c 07a0  .d.<.|.|.d.<.|..
+000020e0: 077c 1ca1 0101 007c 11a0 077c 1b64 047c  .|.....|...|.d.|
+000020f0: 1a7c 197c 046a 0a7c 1319 00a0 1264 1a64  .|.|.j.|.....d.d
+00002100: 0ba1 0266 05a1 0101 007c 0fa0 077c 127c  ...f.....|...|.|
+00002110: 1366 02a1 0101 007c 10a0 077c 127c 1b66  .f.....|...|.|.f
+00002120: 02a1 0101 007c 10a0 077c 1b7c 1366 02a1  .....|...|.|.f..
+00002130: 0101 006e 087c 137c 1464 193c 007c 07a0  ...n.|.|.d.<.|..
+00002140: 077c 14a1 0101 0071 ee71 ca7c 1144 005d  .|.....q.q.|.D.]
+00002150: 2e7d 1d7c 046a 137c 1d64 0e19 007c 1d64  .}.|.j.|.d...|.d
+00002160: 0419 007c 1d64 1b19 007c 1d64 1c19 007c  ...|.d...|.d...|
+00002170: 1d64 1d19 0064 1e8d 0501 0090 0271 967c  .d...d.......q.|
+00002180: 04a0 147c 0fa1 0101 007c 04a0 157c 10a1  ...|.....|...|..
+00002190: 0101 007c 0e7c 005f 086e 507c 006a 0344  ...|.|._.nP|.j.D
+000021a0: 005d 487d 0a7c 0a64 0319 007d 0b7c 087c  .]H}.|.d...}.|.|
+000021b0: 0b19 007d 127c 04a0 097c 12a1 0144 005d  ...}.|...|...D.]
+000021c0: 267d 1374 0183 007d 147c 127c 1464 0c3c  &}.t...}.|.|.d.<
+000021d0: 007c 137c 1464 193c 007c 07a0 077c 14a1  .|.|.d.<.|...|..
+000021e0: 0101 0090 0371 0690 0271 e874 027c 006a  .....q...q.t.|.j
+000021f0: 0883 0144 005d 785c 027d 097d 0a7c 0a64  ...D.]x\.}.}.|.d
+00002200: 0319 007d 0b74 0183 007d 0c7c 0964 0417  ...}.t...}.|.d..
+00002210: 0064 1814 007c 0c64 053c 007c 0b7c 0c64  .d...|.d.<.|.|.d
+00002220: 033c 007c 0a64 0619 007d 0d7c 0d74 046a  .<.|.d...}.|.t.j
+00002230: 056b 0290 0372 8864 077c 0c64 083c 006e  .k...r.d.|.d.<.n
+00002240: 147c 0d74 046a 066b 0290 0372 9c64 1f7c  .|.t.j.k...r.d.|
+00002250: 0c64 083c 007c 0a64 0a19 007c 0c64 0a3c  .d.<.|.d...|.d.<
+00002260: 007c 06a0 077c 0ca1 0101 0090 0371 3c7c  .|...|.......q<|
+00002270: 067c 0564 203c 007c 077c 0564 213c 007c  .|.d <.|.|.d!<.|
+00002280: 057c 005f 167c 0190 0372 e074 176a 187c  .|._.|...r.t.j.|
+00002290: 0564 1b64 228d 0253 007c 0553 0064 0b53  .d.d"..S.|.S.d.S
+000022a0: 0029 237a e80a 2020 2020 2020 2020 436f  .)#z..        Co
+000022b0: 6e76 6572 7420 5047 5420 2877 6974 686f  nvert PGT (witho
+000022c0: 7574 2061 6e79 2070 6172 7469 7469 6f6e  ut any partition
+000022d0: 7329 2074 6f20 4a53 4f4e 2066 6f72 2076  s) to JSON for v
+000022e0: 6973 7561 6c69 7361 7469 6f6e 2069 6e20  isualisation in 
+000022f0: 474f 4a53 0a0a 2020 2020 2020 2020 5375  GOJS..        Su
+00002300: 622d 636c 6173 7320 5047 5450 7320 7769  b-class PGTPs wi
+00002310: 6c6c 206f 7665 7272 6964 6520 7468 6973  ll override this
+00002320: 2066 756e 6374 696f 6e2c 2061 6e64 2072   function, and r
+00002330: 6570 6c61 6365 2074 6869 7320 7769 7468  eplace this with
+00002340: 0a20 2020 2020 2020 2061 6374 7561 6c20  .        actual 
+00002350: 7061 7274 6974 696f 6e69 6e67 2c20 616e  partitioning, an
+00002360: 6420 7468 6520 7669 7375 6c69 7361 7469  d the visulisati
+00002370: 6f6e 2062 6563 6f6d 6573 2061 6e20 6f70  on becomes an op
+00002380: 7469 6f6e 0a20 2020 2020 2020 207a 1267  tion.        z.g
+00002390: 6f2e 4772 6170 684c 696e 6b73 4d6f 6465  o.GraphLinksMode
+000023a0: 6cda 0563 6c61 7373 7258 0000 0072 4a00  l..classrX...rJ.
+000023b0: 0000 da03 6b65 79da 0c63 6174 6567 6f72  ....key..categor
+000023c0: 7954 7970 6572 1100 0000 da08 6361 7465  yTyper......cate
+000023d0: 676f 7279 da0b 4170 706c 6963 6174 696f  gory..Applicatio
+000023e0: 6eda 046e 616d 654e da04 6672 6f6d 7242  n..nameN..fromrB
+000023f0: 0000 0072 0200 0000 da09 6472 6f70 5f74  ...r......drop_t
+00002400: 7970 65da 0964 726f 705f 7370 6563 7a10  ype..drop_specz.
+00002410: 7b30 7d5f 5472 616e 7341 7070 5f7b 317d  {0}_TransApp_{1}
+00002420: 7a17 646c 672e 6472 6f70 2e42 6172 7269  z.dlg.drop.Barri
+00002430: 6572 4170 7044 524f 505a 0667 6f5f 6170  erAppDROPZ.go_ap
+00002440: 7029 0572 5800 0000 726d 0000 00da 0964  p).rX...rm.....d
+00002450: 726f 7063 6c61 7373 7270 0000 0072 3d00  ropclassrp...r=.
+00002460: 0000 7a11 7b30 7d5f 5472 616e 7344 6174  ..z.{0}_TransDat
+00002470: 615f 7b31 7d7a 2264 6c67 2e64 6174 612e  a_{1}z"dlg.data.
+00002480: 6472 6f70 732e 6d65 6d6f 7279 2e49 6e4d  drops.memory.InM
+00002490: 656d 6f72 7944 524f 505a 0767 6f5f 6461  emoryDROPZ.go_da
+000024a0: 7461 e9ff ffff ffda 0274 6f72 6900 0000  ta.......tori...
+000024b0: 723c 0000 00e9 0300 0000 e904 0000 0029  r<.............)
+000024c0: 0472 3d00 0000 7272 0000 0072 7300 0000  .r=...rr...rs...
+000024d0: 7269 0000 00da 0950 7974 686f 6e41 7070  ri.....PythonApp
+000024e0: da0d 6e6f 6465 4461 7461 4172 7261 79da  ..nodeDataArray.
+000024f0: 0d6c 696e 6b44 6174 6141 7272 6179 725b  .linkDataArrayr[
+00002500: 0000 0029 1972 3b00 0000 7218 0000 00da  ...).r;...r.....
+00002510: 0965 6e75 6d65 7261 7465 7212 0000 0072  .enumerater....r
+00002520: 0500 0000 da04 4441 5441 da0b 4150 504c  ......DATA..APPL
+00002530: 4943 4154 494f 4eda 0661 7070 656e 6472  ICATION..appendr
+00002540: 1400 0000 5a0a 7375 6363 6573 736f 7273  ....Z.successors
+00002550: 7246 0000 0072 2300 0000 7206 0000 00da  rF...r#...r.....
+00002560: 0b61 6464 436f 6e73 756d 6572 da08 6164  .addConsumer..ad
+00002570: 6449 6e70 7574 da09 6164 644f 7574 7075  dInput..addOutpu
+00002580: 74da 0b61 6464 5072 6f64 7563 6572 7213  t..addProducerr.
+00002590: 0000 0072 3e00 0000 5a08 6164 645f 6e6f  ...r>...Z.add_no
+000025a0: 6465 5a11 7265 6d6f 7665 5f65 6467 6573  deZ.remove_edges
+000025b0: 5f66 726f 6d5a 0e61 6464 5f65 6467 6573  _fromZ.add_edges
+000025c0: 5f66 726f 6d5a 0e5f 676f 6a73 5f6a 736f  _fromZ._gojs_jso
+000025d0: 6e5f 6f62 6a72 4d00 0000 7263 0000 0029  n_objrM...rc...)
+000025e0: 1e72 2000 0000 da0a 7374 7269 6e67 5f72  .r .....string_r
+000025f0: 6570 5a07 6f75 7464 6963 7472 4b00 0000  epZ.outdictrK...
+00002600: 7245 0000 0072 3900 0000 7246 0000 00da  rE...r9...rF....
+00002610: 056c 696e 6b73 5a08 6b65 795f 6469 6374  .linksZ.key_dict
+00002620: da01 6972 6800 0000 7258 0000 0072 5900  ..irh...rX...rY.
+00002630: 0000 da02 7474 5a0b 6578 7472 615f 6472  ....ttZ.extra_dr
+00002640: 6f70 735a 0c72 656d 6f76 655f 6564 6765  opsZ.remove_edge
+00002650: 735a 0961 6464 5f65 6467 6573 5a09 6164  sZ.add_edgesZ.ad
+00002660: 645f 6e6f 6465 735a 036d 796b 5a03 6f75  d_nodesZ.mykZ.ou
+00002670: 70da 046c 696e 6b5a 0766 726f 6d5f 6474  p..linkZ.from_dt
+00002680: 5a05 746f 5f64 745a 0774 6f5f 6472 6f70  Z.to_dtZ.to_drop
+00002690: 5a09 6578 7472 615f 6f69 645a 0864 726f  Z.extra_oidZ.dro
+000026a0: 7053 7065 635a 046d 7964 74da 036c 6964  pSpecZ.mydt..lid
+000026b0: 5a07 656e 646c 696e 6b5a 0267 6e72 0c00  Z.endlinkZ.gnr..
+000026c0: 0000 720c 0000 0072 0d00 0000 724c 0000  ..r....r....rL..
+000026d0: 004e 0100 0073 f200 0000 0007 0601 0601  .N...s..........
+000026e0: 0801 0401 0401 0602 1201 0801 0601 0c01  ................
+000026f0: 0c01 0801 0801 0a01 0a01 0a01 0801 0c01  ................
+00002700: 0c02 0c01 0401 0401 0401 0401 0c01 0801  ................
+00002710: 0801 1801 0601 0802 1aff 0203 0e01 0a01  ................
+00002720: 0e01 0a02 0c01 0202 0201 0401 0201 0201  ................
+00002730: 02fb 04ff 040a 0a01 0a01 0a01 0a01 0603  ................
+00002740: 0c01 0202 0201 0401 0201 0201 02fb 04ff  ................
+00002750: 0409 0a01 0a01 0a01 0a01 0401 0a01 0c01  ................
+00002760: 0801 0601 0801 0801 0a03 0402 0201 0201  ................
+00002770: 0201 0201 10fb 02ff 0409 0e01 0e01 1002  ................
+00002780: 0801 0e01 0802 0401 0601 0601 0601 0601  ................
+00002790: 06fb 0a07 0a01 0a01 0802 0a01 0801 0801  ................
+000027a0: 0e01 0601 0801 0801 1203 1201 0801 0601  ................
+000027b0: 1001 0801 0801 0c01 0a01 0c01 0801 0c01  ................
+000027c0: 0e02 0801 0801 0601 0601 0e02 7a10 5047  ............z.PG
+000027d0: 542e 746f 5f67 6f6a 735f 6a73 6f6e 2901  T.to_gojs_json).
+000027e0: 5429 0154 2903 4672 3d00 0000 4629 0346  T).T).Fr=...F).F
+000027f0: 7202 0000 0046 2904 5472 4a00 0000 7202  r....F).TrJ...r.
+00002800: 0000 0054 2903 544e 4629 1672 0900 0000  ...T).TNF).r....
+00002810: 720a 0000 0072 0b00 0000 da07 5f5f 646f  r....r......__do
+00002820: 635f 5f72 2200 0000 7226 0000 00da 0870  c__r"...r&.....p
+00002830: 726f 7065 7274 7972 2900 0000 722b 0000  ropertyr)...r+..
+00002840: 0072 3000 0000 7231 0000 0072 3a00 0000  .r0...r1...r:...
+00002850: 7238 0000 0072 3b00 0000 7237 0000 0072  r8...r;...r7...r
+00002860: 3600 0000 724d 0000 0072 4f00 0000 da06  6...rM...rO.....
+00002870: 7365 7474 6572 7253 0000 0072 6a00 0000  setterrS...rj...
+00002880: 724c 0000 0072 0c00 0000 720c 0000 0072  rL...r....r....r
+00002890: 0c00 0000 720d 0000 0072 0f00 0000 3300  ....r....r....3.
+000028a0: 0000 7340 0000 0008 0104 040a 1308 1402  ..s@............
+000028b0: 010a 0608 0608 0708 080a 0d08 0302 010a  ................
+000028c0: 0a02 010a 0b0a 1102 010a 0b02 010a 0304  ................
+000028d0: 010a 0400 0000 0000 ff0a 0800 0100 0100  ................
+000028e0: 0100 fa0a 7f00 0372 0f00 0000 2913 728a  .......r....).r.
+000028f0: 0000 0072 0900 0000 da0b 5f5f 7061 636b  ...r......__pack
+00002900: 6167 655f 5f72 4d00 0000 da07 6c6f 6767  age__rM.....logg
+00002910: 696e 6772 2d00 0000 da0f 646c 672e 6472  ingr-.....dlg.dr
+00002920: 6f70 6d61 6b65 2e6c 6772 0300 0000 5a16  opmake.lgr....Z.
+00002930: 646c 672e 6472 6f70 6d61 6b65 2e73 6368  dlg.dropmake.sch
+00002940: 6564 756c 6572 7204 0000 00da 0a64 6c67  edulerr......dlg
+00002950: 2e63 6f6d 6d6f 6e72 0500 0000 7206 0000  .commonr....r...
+00002960: 00da 0967 6574 4c6f 6767 6572 725d 0000  ...getLoggerr]..
+00002970: 0072 0700 0000 720e 0000 00da 066f 626a  .r....r......obj
+00002980: 6563 7472 0f00 0000 720c 0000 0072 0c00  ectr....r....r..
+00002990: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
+000029a0: 6f64 756c 653e 1600 0000 7318 0000 0004  odule>....s.....
+000029b0: 0608 0104 0308 0108 0108 020c 010c 0110  ................
+000029c0: 020a 0310 0410 04                        .......
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgt.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/pgtp.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/pgtp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/__pycache__/scheduler.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/__pycache__/scheduler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/definition_classes.py` & `daliuge-translator-4.0.1/dlg/dropmake/definition_classes.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/dm_utils.py` & `daliuge-translator-4.0.1/dlg/dropmake/dm_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/lg.graph.schema` & `daliuge-translator-4.0.1/dlg/dropmake/lg.graph.schema`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/lg.py` & `daliuge-translator-4.0.1/dlg/dropmake/lg.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/lg_node.py` & `daliuge-translator-4.0.1/dlg/dropmake/lg_node.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/lib/libmetis.dylib` & `daliuge-translator-4.0.1/dlg/dropmake/lib/libmetis.dylib`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/lib/libmetis.so` & `daliuge-translator-4.0.1/dlg/dropmake/lib/libmetis.so`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/pg_generator.py` & `daliuge-translator-4.0.1/dlg/dropmake/pg_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,18 @@
     if zerorun:
         for dropspec in drop_list:
             if "sleep_time" in dropspec:
                 dropspec["sleep_time"] = 0
     if app:
         logger.info("Replacing apps with %s", app)
         for dropspec in drop_list:
-            if (
-                "dropclass" in dropspec
-                and dropspec["categoryType"] == "Application"
-            ):
+            if "dropclass" in dropspec and dropspec["categoryType"] == "Application":
                 dropspec["dropclass"] = app
                 dropspec["sleep_time"] = (
-                    dropspec["execution_time"]
-                    if "execution_time" in dropspec
-                    else 2
+                    dropspec["execution_time"] if "execution_time" in dropspec else 2
                 )
     drop_list.append(lg.reprodata)
     return drop_list
 
 
 ALGO_NONE = 0
 ALGO_METIS = 1
@@ -255,10 +250,13 @@
     if type(pgt[0]) is str:
         pgt = pgt[1]  # remove the graph name TODO: we may want to retain that
     for drop_spec in pgt:
         if drop_spec != {}:
             nidx = int(drop_spec["node"][1:])  # skip '#'
             drop_spec["node"] = nm_list[nidx]
             iidx = int(drop_spec["island"][1:])  # skip '#'
-            drop_spec["island"] = dim_list[iidx]
+            drop_spec["island"] = (
+                dim_list[iidx].split(":")[0] + ":8001"
+            )  # TODO: just for test
+            logger.debug("Island: %s", drop_spec["island"])
 
     return pgt  # now it's a PG
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/pg_manager.py` & `daliuge-translator-4.0.1/dlg/dropmake/pg_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/pgt.py` & `daliuge-translator-4.0.1/dlg/dropmake/pgt.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,15 @@
     A DROP representation of Physical Graph Template
     """
 
     def __init__(self, drop_list, build_dag=True):
         self._drop_list = drop_list
         self._drop_list_len = len(drop_list)
         self._extra_drops = []  # artifacts DROPs produced during L2G mapping
-        self._dag = (
-            DAGUtil.build_dag_from_drops(self._drop_list)
-            if build_dag
-            else None
-        )
+        self._dag = DAGUtil.build_dag_from_drops(self._drop_list) if build_dag else None
         self._json_str = None
         self._oid_gid_map = dict()
         self._gid_island_id_map = dict()
         self._num_parts_done = 0
         self._partition_merged = 0
         self._inner_parts = []  # a list of inner partitions (e.g. nodes)
         # for visualisation only
@@ -74,22 +70,18 @@
         self._merge_parts = False
         self._island_labels = ["Data", "Compute"]
         self._data_movement = None
         self._reprodata = {}
 
     def _can_merge(self, new_num_parts):
         if new_num_parts <= 0:
-            raise GPGTException(
-                "Invalid new_num_parts {0}".format(new_num_parts)
-            )
+            raise GPGTException("Invalid new_num_parts {0}".format(new_num_parts))
         if not self._merge_parts:
             raise GPGTException(
-                "This {0} PGTP is not made for merging".format(
-                    self.__class__.__name__
-                )
+                "This {0} PGTP is not made for merging".format(self.__class__.__name__)
             )
         if self._num_parts_done <= new_num_parts:
             raise GPGTNoNeedMergeException(
                 "No need to merge this {0} PGTP: {1} <= {2}".format(
                     self.__class__.__name__,
                     self._num_parts_done,
                     new_num_parts,
@@ -160,22 +152,18 @@
         """
         Return the TOTAL data movement
         """
         if self._data_movement is not None:
             return self._data_movement
         elif self.dag is not None:
             G = self.dag
-            self._data_movement = sum(
-                e[2].get("weight", 0) for e in G.edges(data=True)
-            )
+            self._data_movement = sum(e[2].get("weight", 0) for e in G.edges(data=True))
         return self._data_movement
 
-    def pred_exec_time(
-        self, app_drop_only=False, wk="weight", force_answer=False
-    ):
+    def pred_exec_time(self, app_drop_only=False, wk="weight", force_answer=False):
         """
         Predict execution time using the longest path length
         """
         G = self.dag
         if G is None:
             if force_answer:
                 self._dag = DAGUtil.build_dag_from_drops(self._drop_list)
@@ -240,17 +228,15 @@
             where the daliuge system is started up afer submission (e.g. SLURM)
         """
         logger.debug(
             "# worker nodes: %s, node_list(incl. DIM): %s",
             tpl_nodes_len,
             node_list,
         )
-        if (
-            len(node_list) == 0 and tpl_nodes_len > 0
-        ):  # generate pg_spec template
+        if len(node_list) == 0 and tpl_nodes_len > 0:  # generate pg_spec template
             node_list = range(tpl_nodes_len)  # create a fake list for now
             tpl_fl = True
         else:
             tpl_fl = False
 
         if 0 == self._num_parts_done:
             raise GPGTException("The graph has not been partitioned yet")
@@ -258,17 +244,15 @@
         if node_list is None or 0 == len(node_list):
             raise GPGTException("Node list is empty!")
         nodes_len = len(node_list)
 
         try:
             num_islands = int(num_islands)
         except:
-            raise GPGTException(
-                "Invalid num_islands spec: {0}".format(num_islands)
-            )
+            raise GPGTException("Invalid num_islands spec: {0}".format(num_islands))
         if num_islands < 1:
             num_islands = 1  # need at least one island manager
         if num_islands > nodes_len:
             raise GPGTException(
                 "Number of islands must be <= number of specified nodes!"
             )
         form_island = num_islands > 1
@@ -288,22 +272,27 @@
             nm_list = node_list[num_islands:]
         else:
             if form_island and num_islands + num_parts > nodes_len:
                 raise GPGTException(
                     "Insufficient number of nodes: {0}".format(nodes_len)
                 )
             is_list = node_list
-            nm_list = node_list
+            nm_list = (
+                [node_list[1]] + node_list[1:]
+                if isinstance(node_list, list) and len(node_list) > 1
+                else node_list
+            )
         nm_len = len(nm_list)
         logger.info(
-            "Drops count: %d, partitions count: %d, nodes count: %d, island count: %d",
+            "Drops count: %d, partitions count: %d, nodes count: %d, island count: %d %s",
             len(drop_list),
             num_parts,
             nodes_len,
             len(is_list),
+            co_host_dim,
         )
 
         if form_island:
             self.merge_partitions(num_islands, form_island=True)
             # from Eq.1 we know that num_parts <= nm_len
             # so no need to update its value
         elif nm_len < num_parts:
@@ -318,17 +307,15 @@
         # then the test_metis_pgtp_gen_pg_island fails. This needs more investigation
         # but is a corner case.
         # values = set(dict(lm).values()) # old unique values
         # values = dict(zip(values,range(len(values)))) # dict with new values
         # lm = {k:values[v] for (k, v) in lm.items()} # replace old values with new
 
         if tpl_fl:
-            nm_list = [
-                "#%s" % x for x in range(nm_len)
-            ]  # so that nm_list[i] == '#i'
+            nm_list = ["#%s" % x for x in range(nm_len)]  # so that nm_list[i] == '#i'
             is_list = [
                 "#%s" % x for x in range(len(is_list))
             ]  # so that is_list[i] == '#i'
 
         for drop in drop_list:
             oid = drop["oid"]
             # For now, simply round robin, but need to consider
@@ -380,17 +367,15 @@
             for drop in self._drop_list:
                 oid = drop["oid"]
                 myk = key_dict[oid]
                 for i, oup in enumerate(G.successors(myk)):
                     link = dict()
                     link["from"] = myk
                     from_dt = (
-                        0
-                        if drop["categoryType"] in [CategoryType.DATA, "data"]
-                        else 1
+                        0 if drop["categoryType"] in [CategoryType.DATA, "data"] else 1
                     )
                     to_dt = G.nodes[oup]["drop_type"]
                     if from_dt == to_dt:
                         to_drop = G.nodes[oup]["drop_spec"]
                         if from_dt == 0:
                             # add an extra app DROP
                             extra_oid = "{0}_TransApp_{1}".format(oid, i)
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/pgtp.py` & `daliuge-translator-4.0.1/dlg/dropmake/pgtp.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/scheduler.py` & `daliuge-translator-4.0.1/dlg/dropmake/scheduler.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__init__.py` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/anneal.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/anneal.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/antichains.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/antichains.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/anneal.py` & `daliuge-translator-4.0.1/dlg/dropmake/utils/anneal.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/antichains.py` & `daliuge-translator-4.0.1/dlg/dropmake/utils/antichains.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/bash_parameter.py` & `daliuge-translator-4.0.1/dlg/dropmake/utils/bash_parameter.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/utils/heft/base.py` & `daliuge-translator-4.0.1/dlg/dropmake/utils/heft/base.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/LICENSE` & `daliuge-translator-4.0.1/dlg/dropmake/web/LICENSE`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__init__.py` & `daliuge-translator-4.0.1/dlg/dropmake/web/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/lg_web.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/lg_web.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Mar 18 14:56:39 2024 UTC, .py size: 39837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2756 f865 9d9b 0000  U.......'V.e....
+00000000: 550d 0d0a 0000 0000 735d 1966 e798 0000  U.......s].f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 7209 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
@@ -312,1369 +312,1355 @@
 00001370: 696c 65da 0165 a900 725a 0000 00fa 512f  ile..e..rZ....Q/
 00001380: 686f 6d65 2f61 7769 6365 6e65 632f 6769  home/awicenec/gi
 00001390: 742f 6461 6c69 7567 652f 6461 6c69 7567  t/daliuge/daliug
 000013a0: 652d 7472 616e 736c 6174 6f72 2f64 6c67  e-translator/dlg
 000013b0: 2f64 726f 706d 616b 652f 7765 622f 7472  /dropmake/web/tr
 000013c0: 616e 736c 6174 6f72 5f72 6573 742e 7079  anslator_rest.py
 000013d0: da10 6a73 6f6e 626f 6479 5f70 6f73 745f  ..jsonbody_post_
-000013e0: 6c67 9200 0000 7330 0000 0000 0b0a 0102  lg....s0........
+000013e0: 6c67 9000 0000 732a 0000 0000 090a 0102  lg....s*........
 000013f0: 0102 0102 fe06 0402 010e 010e 0112 010a  ................
 00001400: 010c 0108 0104 010c 011e 0110 0102 0102  ................
-00001410: 0104 0102 0006 ff02 fe1c 0772 5c00 0000  ...........r\...
-00001420: 7a24 5468 6520 6e61 6d65 206f 6620 7468  z$The name of th
-00001430: 6520 6c67 2074 6f20 6c6f 6164 2066 726f  e lg to load fro
-00001440: 6d20 6669 6c65 2902 723f 0000 0072 3300  m file).r?...r3.
-00001450: 0000 2901 7240 0000 0063 0100 0000 0000  ..).r@...c......
-00001460: 0000 0000 0000 0700 0000 0900 0000 4300  ..............C.
-00001470: 0000 73b6 0000 007c 0064 016b 0873 1474  ..s....|.d.k.s.t
-00001480: 007c 0083 0164 026b 0272 6474 0174 0283  .|...d.k.rdt.t..
-00001490: 017d 017a 2874 0374 047c 0183 0183 017d  .}.z(t.t.|.....}
-000014a0: 027c 0264 0317 007c 017c 0219 0064 0219  .|.d...|.|...d..
-000014b0: 0017 007d 037c 037d 0057 006e 1e04 0074  ...}.|.}.W.n...t
-000014c0: 056b 0a72 6201 0001 0001 0064 04a0 0674  .k.rb......d...t
-000014d0: 07a1 0106 0059 0053 0058 0074 0874 027c  .....Y.S.X.t.t.|
-000014e0: 0083 0272 a074 0774 027c 0083 027d 0474  ...r.t.t.|...}.t
-000014f0: 097c 0464 0583 028f 107d 0574 0aa0 0b7c  .|.d.....}.t...|
-00001500: 05a1 017d 0657 0035 0051 0052 0058 0074  ...}.W.5.Q.R.X.t
-00001510: 0c7c 0683 0153 0074 0d64 0664 07a0 067c  .|...S.t.d.d...|
-00001520: 00a1 0164 088d 0282 0164 0153 0029 097a  ...d.....d.S.).z
-00001530: 3d0a 2020 2020 5265 7475 726e 7320 4a53  =.    Returns JS
-00001540: 4f4e 2072 6570 7265 7365 6e74 6174 696f  ON representatio
-00001550: 6e20 6f66 2073 6176 6564 206c 6f67 6963  n of saved logic
-00001560: 616c 2067 7261 7068 2e0a 2020 2020 4e72  al graph..    Nr
-00001570: 0100 0000 fa01 2f7a 184e 6f74 6869 6e67  ....../z.Nothing
-00001580: 2066 6f75 6e64 2069 6e20 6469 7220 7b30   found in dir {0
-00001590: 7dda 0172 7243 0000 007a 194a 534f 4e20  }..rrC...z.JSON 
-000015a0: 6772 6170 6820 7b30 7d20 6e6f 7420 666f  graph {0} not fo
-000015b0: 756e 640a 7244 0000 0029 0eda 036c 656e  und.rD...)...len
-000015c0: 7227 0000 0072 4900 0000 da04 6e65 7874  r'...rI.....next
-000015d0: da04 6974 6572 da0d 5374 6f70 4974 6572  ..iter..StopIter
-000015e0: 6174 696f 6e72 5700 0000 7228 0000 0072  ationrW...r(...r
-000015f0: 2900 0000 7253 0000 0072 4a00 0000 da04  )...rS...rJ.....
-00001600: 6c6f 6164 720e 0000 0072 0a00 0000 2907  loadr....r....).
-00001610: 7240 0000 005a 0761 6c6c 5f6c 6773 da09  r@...Z.all_lgs..
-00001620: 6669 7273 745f 6469 725a 0866 6972 7374  first_dirZ.first
-00001630: 5f6c 67da 036c 6770 da01 66da 0464 6174  _lg..lgp..f..dat
-00001640: 6172 5a00 0000 725a 0000 0072 5b00 0000  arZ...rZ...r[...
-00001650: da0f 6a73 6f6e 626f 6479 5f67 6574 5f6c  ..jsonbody_get_l
-00001660: 67b7 0000 0073 2200 0000 0009 1401 0801  g....s".........
-00001670: 0201 0c01 1401 0801 0e01 1001 0a02 0a01  ................
-00001680: 0c01 1401 0802 0201 0201 08fe 7268 0000  ............rh..
-00001690: 007a 0d2f 7067 745f 6a73 6f6e 626f 6479  .z./pgt_jsonbody
-000016a0: 2902 da0e 7265 7370 6f6e 7365 5f63 6c61  )...response_cla
-000016b0: 7373 723e 0000 007a 2554 6865 206e 616d  ssr>...z%The nam
-000016c0: 6520 6f66 2074 6865 2070 6774 2074 6f20  e of the pgt to 
-000016d0: 6c6f 6164 2066 726f 6d20 6669 6c65 2901  load from file).
-000016e0: da08 7067 745f 6e61 6d65 6301 0000 0000  ..pgt_namec.....
-000016f0: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
-00001700: 0000 0073 5000 0000 7400 7401 7c00 8302  ...sP...t.t.|...
-00001710: 723a 7402 7401 7c00 8302 7d01 7403 7c01  r:t.t.|...}.t.|.
-00001720: 6401 8302 8f0e 7d02 7c02 a004 a100 7d03  d.....}.|.....}.
-00001730: 5700 3500 5100 5200 5800 7405 7c03 8301  W.5.Q.R.X.t.|...
-00001740: 5300 7406 6402 6403 a007 7c00 a101 6404  S.t.d.d...|...d.
-00001750: 8d02 8201 6405 5300 2906 7a41 0a20 2020  ....d.S.).zA.   
-00001760: 2052 6574 7572 6e20 4a53 4f4e 2072 6570   Return JSON rep
-00001770: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
-00001780: 2070 6879 7369 6361 6c20 6772 6170 6820   physical graph 
-00001790: 7465 6d70 6c61 7465 0a20 2020 2072 5e00  template.    r^.
-000017a0: 0000 7243 0000 007a 184a 534f 4e20 6772  ..rC...z.JSON gr
-000017b0: 6170 6820 7b30 7d20 6e6f 7420 666f 756e  aph {0} not foun
-000017c0: 6472 4400 0000 4e29 0872 2a00 0000 da07  drD...N).r*.....
-000017d0: 7067 745f 6469 7272 2b00 0000 7253 0000  pgt_dirr+...rS..
-000017e0: 00da 0472 6561 6472 0e00 0000 720a 0000  ...readr....r...
-000017f0: 0072 5700 0000 2904 726a 0000 00da 0370  .rW...).rj.....p
-00001800: 6774 7266 0000 0072 6700 0000 725a 0000  gtrf...rg...rZ..
-00001810: 0072 5a00 0000 725b 0000 00da 106a 736f  .rZ...r[.....jso
-00001820: 6e62 6f64 795f 6765 745f 7067 74d5 0000  nbody_get_pgt...
-00001830: 0073 1200 0000 0007 0a02 0a01 0c01 1201  .s..............
-00001840: 0802 0201 0200 08ff 726e 0000 007a 0a2f  ........rn...z./
-00001850: 7067 5f76 6965 7765 727a 2954 6865 2073  pg_viewerz)The s
-00001860: 7472 696e 6720 6f66 2074 6865 2074 7970  tring of the typ
-00001870: 6520 6f66 2076 6965 7720 746f 2070 726f  e of view to pro
-00001880: 7669 6465 2902 da07 7265 7175 6573 74da  vide)...request.
-00001890: 0d70 6774 5f76 6965 775f 6e61 6d65 6302  .pgt_view_namec.
-000018a0: 0000 0000 0000 0000 0000 0005 0000 0009  ................
-000018b0: 0000 0043 0000 0073 9a00 0000 7c01 6401  ...C...s....|.d.
-000018c0: 6b08 7314 7400 7c01 8301 6402 6b02 725c  k.s.t.|...d.k.r\
-000018d0: 7401 7402 8301 7d02 7a26 7403 7404 7c02  t.t...}.z&t.t.|.
-000018e0: 8301 8301 7d03 7c03 7405 6a06 1700 7c02  ....}.|.t.j...|.
-000018f0: 7c03 1900 6402 1900 1700 7d01 5700 6e18  |...d.....}.W.n.
-00001900: 0400 7407 6b0a 725a 0100 0100 0100 6401  ..t.k.rZ......d.
-00001910: 7d01 5900 6e02 5800 7408 7402 7c01 8302  }.Y.n.X.t.t.|...
-00001920: 7282 7409 a00a 6403 7c00 7c01 6401 6404  r.t...d.|.|.d.d.
-00001930: 6401 6405 9c05 a102 7d04 7c04 5300 740b  d.d.....}.|.S.t.
-00001940: 6406 6407 a00c 7c01 7402 a102 6408 8d02  d.d...|.t...d...
-00001950: 8201 6401 5300 2909 7a29 0a20 2020 204c  ..d.S.).z).    L
-00001960: 6f61 6473 2074 6865 2070 6879 7369 6361  oads the physica
-00001970: 6c20 6772 6170 6820 7669 6577 6572 0a20  l graph viewer. 
-00001980: 2020 204e 7201 0000 00fa 0e70 675f 7669     Nr......pg_vi
-00001990: 6577 6572 2e68 746d 6cfa 1750 6879 7369  ewer.html..Physi
-000019a0: 6361 6c20 4772 6170 6820 5465 6d70 6c61  cal Graph Templa
-000019b0: 7465 a905 726f 0000 00da 1270 6774 5f76  te..ro.....pgt_v
-000019c0: 6965 775f 6a73 6f6e 5f6e 616d 655a 0e70  iew_json_nameZ.p
-000019d0: 6172 7469 7469 6f6e 5f69 6e66 6f72 3700  artition_infor7.
-000019e0: 0000 da05 6572 726f 7272 4300 0000 7a2e  ....errorrC...z.
-000019f0: 5068 7973 6963 616c 2067 7261 7068 2074  Physical graph t
-00001a00: 656d 706c 6174 6520 7669 6577 207b 307d  emplate view {0}
-00001a10: 206e 6f74 2066 6f75 6e64 207b 317d 7244   not found {1}rD
-00001a20: 0000 0029 0d72 5f00 0000 722c 0000 0072  ...).r_...r,...r
-00001a30: 6b00 0000 7260 0000 0072 6100 0000 da02  k...r`...ra.....
-00001a40: 6f73 da03 7365 7072 6200 0000 722a 0000  os..seprb...r*..
-00001a50: 00da 0974 656d 706c 6174 6573 da10 5465  ...templates..Te
-00001a60: 6d70 6c61 7465 5265 7370 6f6e 7365 720a  mplateResponser.
-00001a70: 0000 0072 5700 0000 2905 726f 0000 0072  ...rW...).ro...r
-00001a80: 7000 0000 5a08 616c 6c5f 7067 7473 7264  p...Z.all_pgtsrd
-00001a90: 0000 00da 0374 706c 725a 0000 0072 5a00  .....tplrZ...rZ.
-00001aa0: 0000 725b 0000 00da 0e6c 6f61 645f 7067  ..r[.....load_pg
-00001ab0: 5f76 6965 7765 72e8 0000 0073 3200 0000  _viewer....s2...
-00001ac0: 000a 1401 0801 0201 0c01 1a01 0e01 0a01  ................
-00001ad0: 0a01 0401 0202 0201 0201 0201 0201 02fb  ................
-00001ae0: 04fe 040a 0402 0201 0201 0401 0200 02ff  ................
-00001af0: 02fe 727b 0000 007a 112f 7368 6f77 5f67  ..r{...z./show_g
-00001b00: 616e 7474 5f63 6861 7274 7a32 5468 6520  antt_chartz2The 
-00001b10: 7067 745f 6964 2075 7365 6420 746f 2069  pgt_id used to i
-00001b20: 6e74 6572 6e61 6c6c 7920 7265 6665 7265  nternally refere
-00001b30: 6e63 6520 7468 6973 2067 7261 7068 2902  nce this graph).
-00001b40: 726f 0000 00da 0670 6774 5f69 6463 0200  ro.....pgt_idc..
-00001b50: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-00001b60: 0000 4300 0000 7318 0000 0074 00a0 0164  ..C...s....t...d
-00001b70: 017c 007c 0164 0264 039c 03a1 027d 027c  .|.|.d.d.....}.|
-00001b80: 0253 0029 047a 2b0a 2020 2020 496e 7465  .S.).z+.    Inte
-00001b90: 7266 6163 6520 746f 2073 686f 7720 7468  rface to show th
-00001ba0: 6520 6761 6e74 7420 6368 6172 740a 2020  e gantt chart.  
-00001bb0: 2020 fa0f 6d61 7472 6978 5f76 6973 2e68    ..matrix_vis.h
-00001bc0: 746d 6c5a 0f70 6774 5f67 616e 7474 5f63  tmlZ.pgt_gantt_c
-00001bd0: 6861 7274 a903 726f 0000 0072 7400 0000  hart..ro...rt...
-00001be0: 5a0a 7669 735f 6163 7469 6f6e a902 7278  Z.vis_action..rx
-00001bf0: 0000 0072 7900 0000 a903 726f 0000 0072  ...ry.....ro...r
-00001c00: 7c00 0000 727a 0000 0072 5a00 0000 725a  |...rz...rZ...rZ
-00001c10: 0000 0072 5b00 0000 da10 7368 6f77 5f67  ...r[.....show_g
-00001c20: 616e 7474 5f63 6861 7274 0e01 0000 7310  antt_chart....s.
-00001c30: 0000 0000 0a04 0102 0202 0102 0102 fd04  ................
-00001c40: fe04 0872 8100 0000 7a10 2f70 6774 5f67  ...r....z./pgt_g
-00001c50: 616e 7474 5f63 6861 7274 2901 727c 0000  antt_chart).r|..
-00001c60: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-00001c70: 0000 0a00 0000 4300 0000 734c 0000 007a  ......C...sL...z
-00001c80: 1074 00a0 017c 00a1 017d 017c 0157 0053  .t...|...}.|.W.S
-00001c90: 0004 0074 026b 0a72 4601 007d 0201 007a  ...t.k.rF..}...z
-00001ca0: 1874 0364 0164 02a0 047c 007c 02a1 0264  .t.d.d...|.|...d
-00001cb0: 038d 0282 0157 0035 0064 047d 027e 0258  .....W.5.d.}.~.X
-00001cc0: 0059 006e 0258 0064 0453 0029 057a 4a0a  .Y.n.X.d.S.).zJ.
-00001cd0: 2020 2020 496e 7465 7266 6163 6520 746f      Interface to
-00001ce0: 2072 6574 7269 6576 6520 6120 4761 6e74   retrieve a Gant
-00001cf0: 7420 4368 6172 7420 6d61 7472 6978 2061  t Chart matrix a
-00001d00: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
-00001d10: 2050 4754 0a20 2020 2072 4800 0000 7a2b   PGT.    rH...z+
-00001d20: 4661 696c 6564 2074 6f20 6765 6e65 7261  Failed to genera
-00001d30: 7465 2047 616e 7474 2063 6861 7274 2066  te Gantt chart f
-00001d40: 6f72 207b 307d 3a20 7b31 7d72 4400 0000  or {0}: {1}rD...
-00001d50: 4e29 05da 0670 675f 6d67 72da 0f67 6574  N)...pg_mgr..get
-00001d60: 5f67 616e 7474 5f63 6861 7274 7223 0000  _gantt_chartr#..
-00001d70: 0072 0a00 0000 7257 0000 0029 0372 7c00  .r....rW...).r|.
-00001d80: 0000 da03 7265 74da 0267 6572 5a00 0000  ....ret..gerZ...
-00001d90: 725a 0000 0072 5b00 0000 7283 0000 0023  rZ...r[...r....#
-00001da0: 0100 0073 1600 0000 0009 0201 0a01 0601  ...s............
-00001db0: 1001 0201 0201 0401 0200 02ff 02fe 7283  ..............r.
-00001dc0: 0000 007a 122f 7368 6f77 5f73 6368 6564  ...z./show_sched
-00001dd0: 756c 655f 6d61 7463 0200 0000 0000 0000  ule_matc........
-00001de0: 0000 0000 0300 0000 0700 0000 4300 0000  ............C...
-00001df0: 7318 0000 0074 00a0 0164 017c 007c 0164  s....t...d.|.|.d
-00001e00: 0264 039c 03a1 027d 027c 0253 0029 047a  .d.....}.|.S.).z
-00001e10: 2c0a 2020 2020 496e 7465 7266 6163 6520  ,.    Interface 
-00001e20: 746f 2073 686f 7720 7468 6520 7363 6865  to show the sche
-00001e30: 6475 6c65 206d 6174 0a20 2020 2072 7d00  dule mat.    r}.
-00001e40: 0000 5a10 7067 745f 7363 6865 6475 6c65  ..Z.pgt_schedule
-00001e50: 5f6d 6174 727e 0000 0072 7f00 0000 7280  _matr~...r....r.
-00001e60: 0000 0072 5a00 0000 725a 0000 0072 5b00  ...rZ...rZ...r[.
-00001e70: 0000 da14 7368 6f77 5f73 6368 6564 756c  ....show_schedul
-00001e80: 655f 6d61 7472 6978 3801 0000 7310 0000  e_matrix8...s...
-00001e90: 0000 0a04 0102 0202 0102 0102 fd04 fe04  ................
-00001ea0: 0872 8600 0000 7a16 2f67 6574 5f73 6368  .r....z./get_sch
-00001eb0: 6564 756c 655f 6d61 7472 6963 6573 6301  edule_matricesc.
-00001ec0: 0000 0000 0000 0000 0000 0003 0000 000a  ................
-00001ed0: 0000 0043 0000 0073 4c00 0000 7a10 7400  ...C...sL...z.t.
-00001ee0: a001 7c00 a101 7d01 7c01 5700 5300 0400  ..|...}.|.W.S...
-00001ef0: 7402 6b0a 7246 0100 7d02 0100 7a18 7403  t.k.rF..}...z.t.
-00001f00: 6401 6402 a004 7c00 7c02 a102 6403 8d02  d.d...|.|...d...
-00001f10: 8201 5700 3500 6404 7d02 7e02 5800 5900  ..W.5.d.}.~.X.Y.
-00001f20: 6e02 5800 6404 5300 2905 7a47 0a20 2020  n.X.d.S.).zG.   
-00001f30: 2049 6e74 6572 6661 6365 2074 6f20 7265   Interface to re
-00001f40: 7475 726e 2061 6c6c 2073 6368 6564 756c  turn all schedul
-00001f50: 6520 6d61 7472 6963 6573 2066 6f72 2061  e matrices for a
-00001f60: 2073 696e 676c 6520 7067 745f 6964 0a20   single pgt_id. 
-00001f70: 2020 2072 4800 0000 7a2c 4661 696c 6564     rH...z,Failed
-00001f80: 2074 6f20 6765 7420 7363 6865 6475 6c65   to get schedule
-00001f90: 206d 6174 7269 6365 7320 666f 7220 7b30   matrices for {0
-00001fa0: 7d3a 207b 317d 7244 0000 004e 2905 7282  }: {1}rD...N).r.
-00001fb0: 0000 00da 1567 6574 5f73 6368 6564 756c  .....get_schedul
-00001fc0: 655f 6d61 7472 6963 6573 7256 0000 0072  e_matricesrV...r
-00001fd0: 0a00 0000 7257 0000 0029 0372 7c00 0000  ....rW...).r|...
-00001fe0: 7284 0000 0072 5900 0000 725a 0000 0072  r....rY...rZ...r
-00001ff0: 5a00 0000 725b 0000 0072 8700 0000 4d01  Z...r[...r....M.
-00002000: 0000 7316 0000 0000 0902 010a 0106 0110  ..s.............
-00002010: 0102 0102 0104 0102 0002 ff02 fe72 8700  .............r..
-00002020: 0000 7a08 2f67 656e 5f70 6774 7a3d 4966  ..z./gen_pgtz=If
-00002030: 2070 7265 7365 6e74 2c20 7472 616e 736c   present, transl
-00002040: 6174 6f72 2077 696c 6c20 6174 7465 6d70  ator will attemp
-00002050: 7420 746f 206c 6f61 6420 7468 6973 206c  t to load this l
-00002060: 6720 6672 6f6d 2066 696c 657a 6b52 6570  g from filezkRep
-00002070: 726f 6475 6369 6269 6c69 7479 206d 6f64  roducibility mod
-00002080: 6520 7365 7474 696e 6720 6c65 7665 6c20  e setting level 
-00002090: 6f66 2070 726f 7665 6e61 6e63 6520 7472  of provenance tr
-000020a0: 6163 6b69 6e67 2e20 5265 6665 7220 746f  acking. Refer to
-000020b0: 206d 6169 6e20 646f 6375 6d65 6e74 6174   main documentat
-000020c0: 696f 6e20 666f 7220 6d6f 7265 2069 6e66  ion for more inf
-000020d0: 6f72 6d61 7469 6f6e da05 6661 6c73 657a  ormation..falsez
-000020e0: 2c49 6620 2774 7275 6527 2c20 7769 6c6c  ,If 'true', will
-000020f0: 2072 6570 6c61 6365 2061 6c6c 2061 7070   replace all app
-00002100: 7320 7769 7468 2073 6c65 6570 737a 2a54  s with sleepsz*T
-00002110: 6865 206e 756d 6265 7220 6f66 2064 6174  he number of dat
-00002120: 6120 7061 7274 6974 696f 6e73 2069 6e20  a partitions in 
-00002130: 7468 6520 6772 6170 68da 056d 6574 6973  the graph..metis
-00002140: 7a36 5468 6520 7363 6865 6475 6c69 6e67  z6The scheduling
-00002150: 2061 6c67 6f72 6974 686d 2075 7365 6420   algorithm used 
-00002160: 7768 656e 2075 6e72 6f6c 6c69 6e67 2074  when unrolling t
-00002170: 6865 2067 7261 7068 7a27 5468 6520 6e75  he graphz'The nu
-00002180: 6d62 6572 206f 6620 6461 7461 2d69 736c  mber of data-isl
-00002190: 616e 6473 2074 6f20 7061 7274 6974 696f  ands to partitio
-000021a0: 6e5a 0950 6172 7469 7469 6f6e 7a2e 5468  nZ.Partitionz.Th
-000021b0: 6520 6c61 6265 6c20 7072 6566 6978 6564  e label prefixed
-000021c0: 2074 6f20 6561 6368 2067 656e 6572 6174   to each generat
-000021d0: 6564 2070 6172 7469 7469 6f6e 2908 726f  ed partition).ro
-000021e0: 0000 0072 4000 0000 7242 0000 00da 0474  ...r@...rB.....t
-000021f0: 6573 74da 076e 756d 5f70 6172 da04 616c  est..num_par..al
-00002200: 676f da0b 6e75 6d5f 6973 6c61 6e64 73da  go..num_islands.
-00002210: 0970 6172 5f6c 6162 656c 6308 0000 0000  .par_labelc.....
-00002220: 0000 0000 0000 0011 0000 000a 0000 0043  ...............C
-00002230: 0000 0073 7401 0000 7400 7401 7c01 8302  ...st...t.t.|...
-00002240: 731c 7402 6401 6402 a003 7c01 a101 6403  s.t.d.d...|...d.
-00002250: 8d02 8201 7a90 7404 7405 7401 7c01 8302  ....z.t.t.t.|...
-00002260: 7c02 8302 7d08 7c03 a006 a100 6404 6b02  |...}.|.....d.k.
-00002270: 7d03 7407 7c08 7c03 7c05 7c04 7c06 7c07  }.t.|.|.|.|.|.|.
-00002280: 7c00 6a08 a009 a100 8307 7d09 6405 7d0a  |.j.......}.d.}.
-00002290: 740a a00b 7c09 7c01 a102 7d0b 6406 a00c  t...|.|...}.d...
-000022a0: 6407 6408 8400 7c09 a00d a100 a009 a100  d.d...|.........
-000022b0: 4400 8301 a101 7d0c 740e a00f 6409 7c00  D.....}.t...d.|.
-000022c0: 7c0b 7c0c 640a 7c0a 6405 6b02 729a 640b  |.|.d.|.d.k.r.d.
-000022d0: 6e02 640c 1600 6400 640d 9c05 a102 7d0d  n.d...d.d.....}.
-000022e0: 7c0d 5700 5300 0400 7410 6b0a 72f0 0100  |.W.S...t.k.r...
-000022f0: 7d0e 0100 7a26 7411 a012 640e a101 0100  }...z&t...d.....
-00002300: 7402 640f 6410 a003 7413 7c0e 8301 7c01  t.d.d...t.|...|.
-00002310: a102 6403 8d02 8201 5700 3500 6400 7d0e  ..d.....W.5.d.}.
-00002320: 7e0e 5800 5900 6e80 0400 7414 6b0a 9001  ~.X.Y.n...t.k...
-00002330: 7234 0100 7d0f 0100 7a26 7411 a012 6411  r4..}...z&t...d.
-00002340: a101 0100 7402 640f 6412 a003 7413 7c0f  ....t.d.d...t.|.
-00002350: 8301 7c01 a102 6403 8d02 8201 5700 3500  ..|...d.....W.5.
-00002360: 6400 7d0f 7e0f 5800 5900 6e3c 0400 7415  d.}.~.X.Y.n<..t.
-00002370: 6b0a 9001 726e 0100 0100 0100 7411 a012  k...rn......t...
-00002380: 6413 a101 0100 7416 a017 a100 7d10 7402  d.....t.....}.t.
-00002390: 640f 6414 a003 7c10 7c01 a102 6403 8d02  d.d...|.|...d...
-000023a0: 8201 5900 6e02 5800 6400 5300 2915 4e72  ..Y.n.X.d.S.).Nr
-000023b0: 4300 0000 7a1d 4c6f 6769 6361 6c20 6772  C...z.Logical gr
-000023c0: 6170 6820 277b 307d 2720 6e6f 7420 666f  aph '{0}' not fo
-000023d0: 756e 6472 4400 0000 da04 7472 7565 7201  undrD.....truer.
-000023e0: 0000 00fa 0320 2d20 6301 0000 0000 0000  ..... - c.......
-000023f0: 0000 0000 0003 0000 0006 0000 0053 0000  .............S..
-00002400: 0073 1c00 0000 6700 7c00 5d14 5c02 7d01  .s....g.|.].\.}.
-00002410: 7d02 6400 a000 7c01 7c02 a102 9102 7104  }.d...|.|.....q.
-00002420: 5300 a901 7a07 7b30 7d3a 7b31 7da9 0172  S...z.{0}:{1}..r
-00002430: 5700 0000 a903 da02 2e30 da01 6bda 0176  W........0..k..v
-00002440: 725a 0000 0072 5a00 0000 725b 0000 00da  rZ...rZ...r[....
-00002450: 0a3c 6c69 7374 636f 6d70 3e98 0100 0073  .<listcomp>....s
-00002460: 0400 0000 0600 0600 7a1b 6765 6e5f 7067  ........z.gen_pg
-00002470: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
-00002480: 636f 6d70 3e72 7100 0000 fa19 5068 7973  comp>rq.....Phys
-00002490: 6963 616c 2047 7261 7068 2054 656d 706c  ical Graph Templ
-000024a0: 6174 6525 73da 00da 0c50 6172 7469 7469  ate%s....Partiti
-000024b0: 6f6e 696e 6772 7300 0000 7a0f 4772 6170  oningrs...z.Grap
-000024c0: 6820 4578 6365 7074 696f 6e72 4800 0000  h ExceptionrH...
-000024d0: fa1e 496e 7661 6c69 6420 4c6f 6769 6361  ..Invalid Logica
-000024e0: 6c20 4772 6170 6820 7b31 7d3a 207b 307d  l Graph {1}: {0}
-000024f0: 7a12 5363 6865 6475 6c65 2045 7863 6570  z.Schedule Excep
-00002500: 7469 6f6e fa23 4772 6170 6820 7363 6865  tion.#Graph sche
-00002510: 6475 6c69 6e67 2065 7863 6570 7469 6f6e  duling exception
-00002520: 207b 317d 3a20 7b30 7d7a 1b50 6172 7469   {1}: {0}z.Parti
-00002530: 7469 6f6e 202f 204f 7468 6572 2065 7863  tion / Other exc
-00002540: 6570 7469 6f6e fa22 4772 6170 6820 7061  eption."Graph pa
-00002550: 7274 6974 696f 6e20 6578 6365 7074 696f  rtition exceptio
-00002560: 6e20 7b31 7d3a 207b 307d 2918 7229 0000  n {1}: {0}).r)..
-00002570: 0072 4900 0000 720a 0000 0072 5700 0000  .rI...r....rW...
-00002580: 722d 0000 0072 2800 0000 da05 6c6f 7765  r-...r(.....lowe
-00002590: 7272 2e00 0000 5a0c 7175 6572 795f 7061  rr....Z.query_pa
-000025a0: 7261 6d73 da05 6974 656d 7372 8200 0000  rams..itemsr....
-000025b0: da07 6164 645f 7067 74da 046a 6f69 6eda  ..add_pgt..join.
-000025c0: 0672 6573 756c 7472 7800 0000 7279 0000  .resultrx...ry..
-000025d0: 0072 2300 0000 724c 0000 00da 0469 6e66  .r#...rL.....inf
-000025e0: 6f72 5800 0000 7225 0000 0072 5600 0000  orX...r%...rV...
-000025f0: da09 7472 6163 6562 6163 6bda 0a66 6f72  ..traceback..for
-00002600: 6d61 745f 6578 6329 1172 6f00 0000 7240  mat_exc).ro...r@
-00002610: 0000 0072 4200 0000 728a 0000 0072 8b00  ...rB...r....r..
-00002620: 0000 728c 0000 0072 8d00 0000 728e 0000  ..r....r....r...
-00002630: 005a 036c 6774 726d 0000 00da 0e6e 756d  .Z.lgtrm.....num
-00002640: 5f70 6172 7469 7469 6f6e 7372 7c00 0000  _partitionsr|...
-00002650: da09 7061 7274 5f69 6e66 6f72 7a00 0000  ..part_inforz...
-00002660: 7285 0000 00da 0273 65da 0974 7261 6365  r......se..trace
-00002670: 5f6d 7367 725a 0000 0072 5a00 0000 725b  _msgrZ...rZ...r[
-00002680: 0000 00da 0767 656e 5f70 6774 6501 0000  .....gen_pgte...
-00002690: 7376 0000 0000 1d0a 0102 0102 0108 fe06  sv..............
-000026a0: 0402 0110 010c 0102 0102 0102 0102 0102  ................
-000026b0: 0102 0102 0108 f904 0904 020c 0204 0114  ................
-000026c0: ff04 0304 0102 0202 0102 0102 0102 010e  ................
-000026d0: ff02 0202 fa04 fe04 0b06 0110 010a 0102  ................
-000026e0: 0102 010e fe16 0412 010a 0102 0102 0104  ................
-000026f0: 0106 0002 ff02 fe16 0610 010a 0108 0102  ................
-00002700: 0102 0104 0102 0002 ff02 fe72 aa00 0000  ...........r....
-00002710: 7a2c 5468 6520 6772 6170 6820 6461 7461  z,The graph data
-00002720: 2075 7365 6420 6173 2074 6865 2067 7261   used as the gra
-00002730: 7068 2069 6620 7375 7070 6c69 6564 2912  ph if supplied).
-00002740: 726f 0000 0072 4000 0000 da09 6a73 6f6e  ro...r@.....json
-00002750: 5f64 6174 6172 4200 0000 728a 0000 0072  _datarB...r....r
-00002760: 8c00 0000 728b 0000 0072 8d00 0000 728e  ....r....r....r.
-00002770: 0000 00da 086d 696e 5f67 6f61 6cda 0570  .....min_goal..p
-00002780: 7479 7065 da0c 6d61 785f 6c6f 6164 5f69  type..max_load_i
-00002790: 6d62 da07 6d61 785f 6370 75da 0b74 696d  mb..max_cpu..tim
-000027a0: 655f 6772 6565 6479 da08 6465 6164 6c69  e_greedy..deadli
-000027b0: 6e65 da04 746f 706b da0a 7377 6172 6d5f  ne..topk..swarm_
-000027c0: 7369 7a65 da07 6d61 785f 6d65 6d63 1200  size..max_memc..
-000027d0: 0000 0000 0000 0000 0000 1d00 0000 0a00  ................
-000027e0: 0000 c300 0000 73b8 0100 007c 04a0 00a1  ......s....|....
-000027f0: 0064 016b 027d 047a e274 01a0 027c 02a1  .d.k.}.z.t...|..
-00002800: 017d 127a 0e74 037c 1274 0483 0201 0057  .}.z.t.|.t.....W
-00002810: 006e 3c04 0074 056b 0a72 6201 007d 1301  .n<..t.k.rb..}..
-00002820: 007a 1e64 02a0 0674 077c 1383 017c 01a1  .z.d...t.|...|..
-00002830: 027d 1474 08a0 097c 14a1 0101 0057 0035  .}.t...|.....W.5
-00002840: 0064 037d 137e 1358 0059 006e 0258 0074  .d.}.~.X.Y.n.X.t
-00002850: 0a7c 127c 0383 027d 1274 0b7c 097c 0a7c  .|.|...}.t.|.|.|
-00002860: 0b7c 0c7c 0d7c 0e7c 0f7c 107c 1183 097d  .|.|.|.|.|.|...}
-00002870: 1574 0c7c 127c 047c 057c 067c 077c 087c  .t.|.|.|.|.|.|.|
-00002880: 1583 077d 1674 0da0 0e7c 167c 01a1 027d  ...}.t...|.|...}
-00002890: 1764 04a0 0f64 0564 0684 007c 16a0 10a1  .d...d.d...|....
-000028a0: 00a0 11a1 0044 0083 01a1 017d 1874 12a0  .....D.....}.t..
-000028b0: 1364 077c 007c 177c 1864 087c 0664 096b  .d.|.|.|.d.|.d.k
-000028c0: 0272 dc64 0a6e 0264 0b16 0064 0364 0c9c  .r.d.n.d...d.d..
-000028d0: 05a1 027d 197c 1957 0053 0004 0074 146b  ...}.|.W.S...t.k
-000028e0: 0a90 0172 3401 007d 1a01 007a 2674 08a0  ...r4..}...z&t..
-000028f0: 1564 0da1 0101 0074 1664 0e64 0fa0 0674  .d.....t.d.d...t
-00002900: 077c 1a83 017c 01a1 0264 108d 0282 0157  .|...|...d.....W
-00002910: 0035 0064 037d 1a7e 1a58 0059 006e 8004  .5.d.}.~.X.Y.n..
-00002920: 0074 176b 0a90 0172 7801 007d 1b01 007a  .t.k...rx..}...z
-00002930: 2674 08a0 1564 11a1 0101 0074 1664 0e64  &t...d.....t.d.d
-00002940: 12a0 0674 077c 1b83 017c 01a1 0264 108d  ...t.|...|...d..
-00002950: 0282 0157 0035 0064 037d 1b7e 1b58 0059  ...W.5.d.}.~.X.Y
-00002960: 006e 3c04 0074 186b 0a90 0172 b201 0001  .n<..t.k...r....
-00002970: 0001 0074 08a0 1564 13a1 0101 0074 19a0  ...t...d.....t..
-00002980: 1aa1 007d 1c74 1664 0e64 14a0 067c 1c7c  ...}.t.d.d...|.|
-00002990: 01a1 0264 108d 0282 0159 006e 0258 0064  ...d.....Y.n.X.d
-000029a0: 0353 0029 157a ee0a 2020 2020 5472 616e  .S.).z..    Tran
-000029b0: 736c 6174 696e 6720 4c6f 6769 6361 6c20  slating Logical 
-000029c0: 4772 6170 6873 2074 6f20 5068 7973 6963  Graphs to Physic
-000029d0: 616c 2047 7261 7068 732e 0a20 2020 2044  al Graphs..    D
-000029e0: 6966 6665 7273 2066 726f 6d20 6765 745f  iffers from get_
-000029f0: 7067 7420 6162 6f76 6520 6279 2074 6865  pgt above by the
-00002a00: 2066 6163 7420 7468 6174 2074 6865 206c   fact that the l
-00002a10: 6f67 6963 616c 2067 7261 7068 2064 6174  ogical graph dat
-00002a20: 6120 6973 2050 4f53 5465 640a 2020 2020  a is POSTed.    
-00002a30: 746f 2074 6869 7320 726f 7574 6520 696e  to this route in
-00002a40: 2061 2048 5454 5020 666f 726d 2c20 7768   a HTTP form, wh
-00002a50: 6572 6561 7320 6765 6e5f 7067 7420 6c6f  ereas gen_pgt lo
-00002a60: 6164 7320 7468 6520 6c6f 6769 6361 6c20  ads the logical 
-00002a70: 6772 6170 6820 6461 7461 0a20 2020 2066  graph data.    f
-00002a80: 726f 6d20 6120 6c6f 6361 6c20 6669 6c65  rom a local file
-00002a90: 0a20 2020 2072 8f00 0000 7a19 5661 6c69  .    r....z.Vali
-00002aa0: 6461 7469 6f6e 2045 7272 6f72 207b 317d  dation Error {1}
-00002ab0: 3a20 7b30 7d4e 7290 0000 0063 0100 0000  : {0}Nr....c....
-00002ac0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00002ad0: 5300 0000 731c 0000 0067 007c 005d 145c  S...s....g.|.].\
-00002ae0: 027d 017d 0264 00a0 007c 017c 02a1 0291  .}.}.d...|.|....
-00002af0: 0271 0453 0072 9100 0000 7292 0000 0072  .q.S.r....r....r
-00002b00: 9300 0000 725a 0000 0072 5a00 0000 725b  ....rZ...rZ...r[
-00002b10: 0000 0072 9700 0000 1002 0000 7304 0000  ...r........s...
-00002b20: 0006 0006 007a 2067 656e 5f70 6774 5f70  .....z gen_pgt_p
-00002b30: 6f73 742e 3c6c 6f63 616c 733e 2e3c 6c69  ost.<locals>.<li
-00002b40: 7374 636f 6d70 3e72 7100 0000 7298 0000  stcomp>rq...r...
-00002b50: 0072 0100 0000 7299 0000 0072 9a00 0000  .r....r....r....
-00002b60: 7273 0000 007a 0f47 5241 5048 2045 5843  rs...z.GRAPH EXC
-00002b70: 4550 5449 4f4e 7248 0000 0072 9b00 0000  EPTIONrH...r....
-00002b80: 7244 0000 007a 1253 4348 4544 554c 4520  rD...z.SCHEDULE 
-00002b90: 4558 4345 5054 494f 4e72 9c00 0000 7a0f  EXCEPTIONr....z.
-00002ba0: 4f54 4845 5220 4558 4345 5054 494f 4e72  OTHER EXCEPTIONr
-00002bb0: 9d00 0000 291b 729e 0000 0072 4a00 0000  ....).r....rJ...
-00002bc0: 724b 0000 0072 1200 0000 da09 4c47 5f53  rK...r......LG_S
-00002bd0: 4348 454d 4172 1300 0000 7257 0000 0072  CHEMAr....rW...r
-00002be0: 5800 0000 724c 0000 0072 7500 0000 722d  X...rL...ru...r-
-00002bf0: 0000 0072 2f00 0000 722e 0000 0072 8200  ...r/...r....r..
-00002c00: 0000 72a0 0000 0072 a100 0000 72a2 0000  ..r....r....r...
-00002c10: 0072 9f00 0000 7278 0000 0072 7900 0000  .r....rx...ry...
-00002c20: 7223 0000 0072 a300 0000 720a 0000 0072  r#...r....r....r
-00002c30: 2500 0000 7256 0000 0072 a400 0000 72a5  %...rV...r....r.
-00002c40: 0000 0029 1d72 6f00 0000 7240 0000 0072  ...).ro...r@...r
-00002c50: ab00 0000 7242 0000 0072 8a00 0000 728c  ....rB...r....r.
-00002c60: 0000 0072 8b00 0000 728d 0000 0072 8e00  ...r....r....r..
-00002c70: 0000 72ac 0000 0072 ad00 0000 72ae 0000  ..r....r....r...
-00002c80: 0072 af00 0000 72b0 0000 0072 b100 0000  .r....r....r....
-00002c90: 72b2 0000 0072 b300 0000 72b4 0000 00da  r....r....r.....
-00002ca0: 0d6c 6f67 6963 616c 5f67 7261 7068 da02  .logical_graph..
-00002cb0: 7665 7275 0000 00da 0b61 6c67 6f5f 7061  veru.....algo_pa
-00002cc0: 7261 6d73 726d 0000 0072 7c00 0000 72a7  ramsrm...r|...r.
-00002cd0: 0000 0072 7a00 0000 7285 0000 0072 a800  ...rz...r....r..
-00002ce0: 0000 72a9 0000 0072 5a00 0000 725a 0000  ..r....rZ...rZ..
-00002cf0: 0072 5b00 0000 da0c 6765 6e5f 7067 745f  .r[.....gen_pgt_
-00002d00: 706f 7374 bf01 0000 738c 0000 0000 2f0c  post....s...../.
-00002d10: 0102 010a 0102 010e 0110 0110 011c 020a  ................
-00002d20: 0302 0102 0102 0102 0102 0102 0102 0102  ................
-00002d30: 0102 0102 f704 0b02 0102 0102 0102 0102  ................
-00002d40: 0102 0102 0102 f904 090c 0104 0114 ff04  ................
-00002d50: 0304 0102 0202 0102 0102 0102 010e ff02  ................
-00002d60: 0202 fa04 fe04 0b06 0112 010a 0102 0102  ................
-00002d70: 010e fe16 0412 010a 0102 0102 0104 0106  ................
-00002d80: 0002 ff02 fe16 0610 010a 0108 0102 0102  ................
-00002d90: 0104 0102 0002 ff02 fe72 b900 0000 7a07  .........r....z.
-00002da0: 2f67 656e 5f70 677a 6c49 6620 7375 7070  /gen_pgzlIf supp
-00002db0: 6c69 6564 2c20 7468 6973 2065 6e64 706f  lied, this endpo
-00002dc0: 696e 7420 7769 6c6c 2061 7474 656d 7074  int will attempt
-00002dd0: 2074 6f20 6465 706c 6f79 2074 6865 2067   to deploy the g
-00002de0: 7261 7068 2069 7320 7468 6520 646c 675f  raph is the dlg_
-00002df0: 7067 745f 7572 6c20 6f72 2064 6c67 5f6d  pgt_url or dlg_m
-00002e00: 6772 5f68 6f73 742f 706f 7274 2065 6e64  gr_host/port end
-00002e10: 706f 696e 747a 2a54 6865 2044 414c 6975  pointz*The DALiu
-00002e20: 4745 206d 616e 6167 6572 2074 6f20 6465  GE manager to de
-00002e30: 706c 6f79 2074 6865 2067 7261 7068 2074  ploy the graph t
-00002e40: 6f7a 3254 6865 2044 414c 6975 4745 206d  oz2The DALiuGE m
-00002e50: 616e 6167 6572 2062 6173 6520 4950 2074  anager base IP t
-00002e60: 6f20 6465 706c 6f79 2074 6865 2067 7261  o deploy the gra
-00002e70: 7068 2074 6f7a 2f54 6865 2044 414c 6975  ph toz/The DALiu
-00002e80: 4745 206d 616e 6167 6572 2070 6f72 7420  GE manager port 
-00002e90: 746f 2064 6570 6c6f 7920 7468 6520 6772  to deploy the gr
-00002ea0: 6170 6820 746f 7a35 5468 6520 6e75 6d62  aph toz5The numb
-00002eb0: 6572 206f 6620 6e6f 6465 7320 746f 2075  er of nodes to u
-00002ec0: 6e72 6f6c 6c20 7468 6520 6772 6170 6820  nroll the graph 
-00002ed0: 7061 7274 6974 696f 6e20 666f 7229 0772  partition for).r
-00002ee0: 6f00 0000 727c 0000 00da 0e64 6c67 5f6d  o...r|.....dlg_m
-00002ef0: 6772 5f64 6570 6c6f 79da 0b64 6c67 5f6d  gr_deploy..dlg_m
-00002f00: 6772 5f75 726c da0c 646c 675f 6d67 725f  gr_url..dlg_mgr_
-00002f10: 686f 7374 da0c 646c 675f 6d67 725f 706f  host..dlg_mgr_po
-00002f20: 7274 da0d 7470 6c5f 6e6f 6465 735f 6c65  rt..tpl_nodes_le
-00002f30: 6e63 0700 0000 0000 0000 0000 0000 1900  nc..............
-00002f40: 0000 0a00 0000 4300 0000 739a 0200 0064  ......C...s....d
-00002f50: 017d 0764 027d 087c 0364 036b 0972 8474  .}.d.}.|.d.k.r.t
-00002f60: 007c 0383 017d 097a 1c7c 096a 01a0 0264  .|...}.z.|.j...d
-00002f70: 04a1 015c 027d 0a7d 0874 037c 0883 017d  ...\.}.}.t.|...}
-00002f80: 0857 006e 3001 0001 0001 007c 096a 017d  .W.n0......|.j.}
-00002f90: 0a7c 096a 0464 056b 0272 5264 067d 086e  .|.j.d.k.rRd.}.n
-00002fa0: 0e7c 096a 0464 076b 0272 6064 027d 0859  .|.j.d.k.r`d.}.Y
-00002fb0: 006e 0258 007c 096a 057d 077c 07a0 0664  .n.X.|.j.}.|...d
-00002fc0: 08a1 0172 9a7c 0764 0364 0985 0219 007d  ...r.|.d.d.....}
-00002fd0: 076e 167c 047d 0a7c 0564 036b 0972 967c  .n.|.}.|.d.k.r.|
-00002fe0: 057d 086e 0464 027d 0874 07a0 0864 0a7c  .}.n.d.}.t...d.|
-00002ff0: 0aa1 0201 0074 07a0 0864 0b7c 08a1 0201  .....t...d.|....
-00003000: 0074 07a0 0864 0c7c 07a1 0201 007c 0264  .t...d.|.....|.d
-00003010: 036b 097d 0b74 09a0 0a7c 01a1 017d 0c7c  .k.}.t...|...}.|
-00003020: 0c64 036b 0872 ea74 0b64 0d64 0ea0 0c7c  .d.k.r.t.d.d...|
-00003030: 01a1 0164 0f8d 0282 017c 0c6a 0d7d 0d7c  ...d.....|.j.}.|
-00003040: 0c6a 0e7d 0e74 0f74 1074 1164 1064 1184  .j.}.t.t.t.d.d..
-00003050: 007c 0d64 1219 0083 0283 0183 017d 0f7c  .|.d.........}.|
-00003060: 0a64 036b 0890 0172 587c 0664 136b 0490  .d.k...rX|.d.k..
-00003070: 0172 2a7c 0f7d 106e 0c74 0b64 1464 1564  .r*|.}.n.t.d.d.d
-00003080: 0f8d 0282 017c 0c6a 1267 0064 167c 1064  .....|.j.g.d.|.d
-00003090: 178d 037d 117c 11a0 137c 0ea1 0101 0074  ...}.|...|.....t
-000030a0: 147c 1183 0153 007a c274 157c 0a7c 087c  .|...S.z.t.|.|.|
-000030b0: 0764 1864 198d 047d 127c 12a0 16a1 007d  .d.d...}.|.....}
-000030c0: 137c 0c6a 127c 1364 1664 1a8d 027d 117c  .|.j.|.d.d...}.|
-000030d0: 0b90 0272 0e74 176a 17a0 18a1 00a0 1964  ...r.t.j.......d
-000030e0: 1ba1 017d 1464 1ca0 0c7c 01a0 0264 1da1  ...}.d...|...d..
-000030f0: 0164 1319 00a0 0264 1ea1 0164 1319 00a0  .d.....d...d....
-00003100: 0264 08a1 0164 0919 007c 14a1 027d 157c  .d...d...|...}.|
-00003110: 12a0 1a7c 15a1 0101 0074 1ba0 1c7c 11a1  ...|.....t...|..
-00003120: 017d 167c 11a0 137c 0ea1 0101 007c 12a0  .}.|...|.....|..
-00003130: 1d7c 157c 11a1 0201 007c 126a 1e7c 157c  .|.|.....|.j.|.|
-00003140: 1664 1f8d 0201 0074 1f64 20a0 0c7c 0a7c  .d.....t.d ..|.|
-00003150: 087c 077c 15a1 0483 0157 0053 0074 147c  .|.|.....W.S.t.|
-00003160: 1183 0157 0053 0057 006e 7a04 0074 206a  ...W.S.W.nz..t j
-00003170: 216b 0a90 0272 5201 007d 1701 007a 1674  !k...rR..}...z.t
-00003180: 0b64 1464 21a0 0c7c 17a1 0164 0f8d 0282  .d.d!..|...d....
-00003190: 0157 0035 0064 037d 177e 1758 0059 006e  .W.5.d.}.~.X.Y.n
-000031a0: 4404 0074 226b 0a90 0272 9401 007d 1801  D..t"k...r...}..
-000031b0: 007a 2474 07a0 2374 24a0 25a1 00a1 0101  .z$t..#t$.%.....
-000031c0: 0074 0b64 1464 22a0 0c7c 18a1 0164 0f8d  .t.d.d"..|...d..
-000031d0: 0282 0157 0035 0064 037d 187e 1858 0059  ...W.5.d.}.~.X.Y
-000031e0: 006e 0258 0064 0353 0029 237a 750a 2020  .n.X.d.S.)#zu.  
-000031f0: 2020 5245 5354 6675 6c20 696e 7465 7266    RESTful interf
-00003200: 6163 6520 746f 2063 6f6e 7665 7274 2061  ace to convert a
-00003210: 2050 4754 2850 2920 696e 746f 2050 4720   PGT(P) into PG 
-00003220: 6279 206d 6170 7069 6e67 0a20 2020 2050  by mapping.    P
-00003230: 4754 2850 2920 6f6e 746f 2061 2067 6976  GT(P) onto a giv
-00003240: 656e 2073 6574 206f 6620 6176 6169 6c61  en set of availa
-00003250: 626c 6520 7265 736f 7572 6365 730a 2020  ble resources.  
-00003260: 2020 7299 0000 0069 bb01 0000 4efa 013a    r....i....N..:
-00003270: da04 6874 7470 e950 0000 00da 0568 7474  ..http.P.....htt
-00003280: 7073 725d 0000 00e9 ffff ffff 7a10 4d61  psr]........z.Ma
-00003290: 6e61 6765 7220 686f 7374 3a20 2573 7a10  nager host: %sz.
-000032a0: 4d61 6e61 6765 7220 706f 7274 3a20 2573  Manager port: %s
-000032b0: 7a12 4d61 6e61 6765 7220 7072 6566 6978  z.Manager prefix
-000032c0: 3a20 2573 7243 0000 00fa 3a50 4754 2850  : %srC....:PGT(P
-000032d0: 2920 7769 7468 2069 6420 7b30 7d20 6e6f  ) with id {0} no
-000032e0: 7420 666f 756e 6420 696e 2074 6865 2050  t found in the P
-000032f0: 6879 7369 6361 6c20 4772 6170 6820 4d61  hysical Graph Ma
-00003300: 6e61 6765 7272 4400 0000 6301 0000 0000  nagerrD...c.....
-00003310: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-00003320: 0000 0073 0800 0000 6401 7c00 6b06 5300  ...s....d.|.k.S.
-00003330: a902 4e5a 0769 7347 726f 7570 725a 0000  ..NZ.isGrouprZ..
-00003340: 00a9 01da 016e 725a 0000 0072 5a00 0000  .....nrZ...rZ...
-00003350: 725b 0000 00da 083c 6c61 6d62 6461 3e7e  r[.....<lambda>~
-00003360: 0200 00f3 0000 0000 7a18 6765 6e5f 7067  ........z.gen_pg
-00003370: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00003380: 613e da0d 6e6f 6465 4461 7461 4172 7261  a>..nodeDataArra
-00003390: 7972 0100 0000 7248 0000 007a 324d 7573  yr....rH...z2Mus
-000033a0: 7420 7370 6563 6966 7920 4441 4c69 7547  t specify DALiuG
-000033b0: 4520 6d61 6e61 6765 7220 686f 7374 206f  E manager host o
-000033c0: 7220 7470 6c5f 6e6f 6465 735f 6c65 6e46  r tpl_nodes_lenF
-000033d0: 2902 da07 7265 745f 7374 7272 be00 0000  )...ret_strr....
-000033e0: e91e 0000 0029 04da 0468 6f73 74da 0470  .....)...host..p
-000033f0: 6f72 745a 0a75 726c 5f70 7265 6669 78da  ortZ.url_prefix.
-00003400: 0774 696d 656f 7574 2901 72cb 0000 007a  .timeout).r....z
-00003410: 1425 592d 256d 2d25 6454 2548 2d25 4d2d  .%Y-%m-%dT%H-%M-
-00003420: 2553 2e25 667a 077b 307d 5f7b 317d 7a06  %S.%fz.{0}_{1}z.
-00003430: 2e67 7261 7068 5a04 5f70 6774 2901 da0e  .graphZ._pgt)...
-00003440: 636f 6d70 6c65 7465 645f 7569 6473 7a27  completed_uidsz'
-00003450: 6874 7470 3a2f 2f7b 307d 3a7b 317d 7b32  http://{0}:{1}{2
-00003460: 7d2f 7365 7373 696f 6e3f 7365 7373 696f  }/session?sessio
-00003470: 6e49 643d 7b33 7d7a 3146 6169 6c65 6420  nId={3}z1Failed 
-00003480: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
-00003490: 2044 414c 6955 4745 2044 726f 7020 4d61   DALiUGE Drop Ma
-000034a0: 6e61 6765 723a 207b 307d fa24 4661 696c  nager: {0}.$Fail
-000034b0: 6564 2074 6f20 6465 706c 6f79 2070 6879  ed to deploy phy
-000034c0: 7369 6361 6c20 6772 6170 683a 207b 307d  sical graph: {0}
-000034d0: 2926 7205 0000 00da 066e 6574 6c6f 63da  )&r......netloc.
-000034e0: 0573 706c 6974 da03 696e 74da 0673 6368  .split..int..sch
-000034f0: 656d 65da 0470 6174 68da 0865 6e64 7377  eme..path..endsw
-00003500: 6974 6872 4c00 0000 da05 6465 6275 6772  ithrL.....debugr
-00003510: 8200 0000 da07 6765 745f 7067 7472 0a00  ......get_pgtr..
-00003520: 0000 7257 0000 00da 0e5f 676f 6a73 5f6a  ..rW....._gojs_j
-00003530: 736f 6e5f 6f62 6ada 0972 6570 726f 6461  son_obj..reproda
-00003540: 7461 725f 0000 00da 046c 6973 74da 0666  tar_.....list..f
-00003550: 696c 7465 72da 0a74 6f5f 7067 5f73 7065  ilter..to_pg_spe
-00003560: 63da 0661 7070 656e 6472 0e00 0000 7217  c..appendr....r.
-00003570: 0000 00da 056e 6f64 6573 da08 6461 7465  .....nodes..date
-00003580: 7469 6d65 da03 6e6f 77da 0873 7472 6674  time..now..strft
-00003590: 696d 65da 0e63 7265 6174 655f 7365 7373  ime..create_sess
-000035a0: 696f 6e72 1600 0000 da09 6765 745f 726f  ionr......get_ro
-000035b0: 6f74 73da 0c61 7070 656e 645f 6772 6170  ots..append_grap
-000035c0: 68da 0e64 6570 6c6f 795f 7365 7373 696f  h..deploy_sessio
-000035d0: 6e72 0f00 0000 7215 0000 00da 1352 6573  nr....r......Res
-000035e0: 7443 6c69 656e 7445 7863 6570 7469 6f6e  tClientException
-000035f0: 7256 0000 0072 7500 0000 72a4 0000 0072  rV...ru...r....r
-00003600: a500 0000 2919 726f 0000 0072 7c00 0000  ....).ro...r|...
-00003610: 72ba 0000 0072 bb00 0000 72bc 0000 0072  r....r....r....r
-00003620: bd00 0000 72be 0000 00da 076d 7072 6566  ....r......mpref
-00003630: 6978 da05 6d70 6f72 745a 066d 7061 7273  ix..mportZ.mpars
-00003640: 65da 056d 686f 7374 5a06 6465 706c 6f79  e..mhostZ.deploy
-00003650: da04 7067 7470 da05 7067 7470 6a72 db00  ..pgtp..pgtpjr..
-00003660: 0000 72a6 0000 005a 066e 6e6f 6465 73da  ..r....Z.nnodes.
-00003670: 0770 675f 7370 6563 5a0a 6d67 725f 636c  .pg_specZ.mgr_cl
-00003680: 6965 6e74 da09 6e6f 6465 5f6c 6973 74da  ient..node_list.
-00003690: 0264 745a 0473 7369 6472 d000 0000 da02  .dtZ.ssidr......
-000036a0: 7265 da02 6578 725a 0000 0072 5a00 0000  re..exrZ...rZ...
-000036b0: 725b 0000 00da 0667 656e 5f70 6737 0200  r[.....gen_pg7..
-000036c0: 0073 b200 0000 001e 0401 0401 0801 0801  .s..............
-000036d0: 0201 1001 0c01 0601 0601 0a01 0601 0a01  ................
-000036e0: 0a01 0601 0a01 0e02 0401 0801 0602 0402  ................
-000036f0: 0c01 0c01 0c03 0801 0a01 0801 0201 0201  ................
-00003700: 0401 02ff 02fe 0607 0601 0601 0201 14ff  ................
-00003710: 0404 0a01 0a01 0602 0201 0201 02fe 0605  ................
-00003720: 1001 0a01 0801 0201 0201 0200 0200 0200  ................
-00003730: 02ff 0604 0802 0e02 0601 1001 0401 2000  .............. .
-00003740: 02ff 0403 0a02 0a01 0a01 0c02 0e04 0201  ................
-00003750: 0401 0200 0200 0200 02ff 02ff 0606 0e01  ................
-00003760: 1401 0201 0201 0401 02ff 02fe 1606 1201  ................
-00003770: 0e01 0201 0201 08fe 72f3 0000 007a 0c2f  ........r....z./
-00003780: 6765 6e5f 7067 5f73 7065 637a 3054 6865  gen_pg_specz0The
-00003790: 206c 6973 7420 6f66 2064 616c 6975 6765   list of daliuge
-000037a0: 206e 6f64 6573 2074 6f20 7375 626d 6974   nodes to submit
-000037b0: 2074 6865 2067 7261 7068 2074 6f7a 4454   the graph tozDT
-000037c0: 6865 2061 6464 7265 7373 206f 6620 7468  he address of th
-000037d0: 6520 6d61 6e61 6765 7220 686f 7374 2077  e manager host w
-000037e0: 6865 7265 2074 6865 2067 7261 7068 2077  here the graph w
-000037f0: 696c 6c20 6265 2064 6570 6c6f 7965 6420  ill be deployed 
-00003800: 746f 2e7a 2a54 6865 206e 756d 6265 7220  to.z*The number 
-00003810: 6f66 206e 6f64 6573 2072 6571 7565 7374  of nodes request
-00003820: 6564 2062 7920 7468 6520 6772 6170 6829  ed by the graph)
-00003830: 0472 7c00 0000 72ef 0000 00da 0c6d 616e  .r|...r......man
-00003840: 6167 6572 5f68 6f73 7472 be00 0000 6304  ager_hostr....c.
-00003850: 0000 0000 0000 0000 0000 0009 0000 000a  ................
-00003860: 0000 0043 0000 0073 3801 0000 7a20 7c02  ...C...s8...z |.
-00003870: 6401 6b02 720e 6401 7d02 7400 a001 6402  d.k.r.d.}.t...d.
-00003880: 7402 7c00 8301 a102 0100 5700 6e44 0400  t.|.......W.nD..
-00003890: 7403 6b0a 7264 0100 7d04 0100 7a26 7400  t.k.rd..}...z&t.
-000038a0: a004 6403 7405 a006 a100 a102 0100 7407  ..d.t.........t.
-000038b0: 6404 6405 a008 7c04 a101 6406 8d02 8201  d.d...|...d.....
-000038c0: 5700 3500 6407 7d04 7e04 5800 5900 6e02  W.5.d.}.~.X.Y.n.
-000038d0: 5800 7409 a00a 7c00 a101 7d05 7c05 6407  X.t...|...}.|.d.
-000038e0: 6b08 728a 7407 6408 6409 a008 7c00 a101  k.r.t.d.d...|...
-000038f0: 6406 8d02 8201 7c01 6407 6b08 729e 7407  d.....|.d.k.r.t.
-00003900: 6404 640a 6406 8d02 8201 7a4e 7c05 6a0b  d.d.d.....zN|.j.
-00003910: 7c02 6701 7c01 1700 7c03 640b 640c 8d03  |.g.|...|.d.d...
-00003920: 7d06 740c a00d 7c06 a101 7d07 7400 a001  }.t...|...}.t...
-00003930: 640d 740e 7c07 8301 a102 0100 740f 7410  d.t.|.......t.t.
-00003940: a011 7c06 740e 7c07 8301 640e 9c02 a101  ..|.t.|...d.....
-00003950: 8301 7d08 7c08 5700 5300 0400 7403 6b0a  ..}.|.W.S...t.k.
-00003960: 9001 7232 0100 7d04 0100 7a26 7400 a004  ..r2..}...z&t...
-00003970: 6403 7405 a006 a100 a102 0100 7407 6404  d.t.........t.d.
-00003980: 640f a008 7c04 a101 6406 8d02 8201 5700  d...|...d.....W.
-00003990: 3500 6407 7d04 7e04 5800 5900 6e02 5800  5.d.}.~.X.Y.n.X.
-000039a0: 6407 5300 2910 7a34 0a20 2020 2049 6e74  d.S.).z4.    Int
-000039b0: 6572 6661 6365 2074 6f20 636f 6e76 6572  erface to conver
-000039c0: 7420 6120 5047 5428 5029 2069 6e74 6f20  t a PGT(P) into 
-000039d0: 7067 5f73 7065 630a 2020 2020 da09 6c6f  pg_spec.    ..lo
-000039e0: 6361 6c68 6f73 747a 0a70 6774 5f69 643a  calhostz.pgt_id:
-000039f0: 2025 737a 0225 7372 4800 0000 7a35 556e   %sz.%srH...z5Un
-00003a00: 6162 6c65 2074 6f20 7061 7273 6520 6a73  able to parse js
-00003a10: 6f6e 2062 6f64 7920 6f66 2072 6571 7565  on body of reque
-00003a20: 7374 2066 6f72 2070 675f 7370 6563 3a20  st for pg_spec: 
-00003a30: 7b30 7d72 4400 0000 4e72 4300 0000 72c4  {0}rD...NrC...r.
-00003a40: 0000 007a 1f4d 7573 7420 7370 6563 6966  ...z.Must specif
-00003a50: 7920 4441 4c69 7547 4520 6e6f 6465 7320  y DALiuGE nodes 
-00003a60: 6c69 7374 4629 0272 be00 0000 72cb 0000  listF).r....r...
-00003a70: 007a 0d52 6f6f 7420 5549 4473 3a20 2573  .z.Root UIDs: %s
-00003a80: 2902 72ee 0000 00da 0972 6f6f 745f 7569  ).r......root_ui
-00003a90: 6473 7a1f 4661 696c 6564 2074 6f20 6765  dsz.Failed to ge
-00003aa0: 6e65 7261 7465 2070 675f 7370 6563 3a20  nerate pg_spec: 
-00003ab0: 7b30 7d29 1272 4c00 0000 72d8 0000 0072  {0}).rL...r....r
-00003ac0: 5800 0000 7256 0000 0072 7500 0000 72a4  X...rV...ru...r.
-00003ad0: 0000 0072 a500 0000 720a 0000 0072 5700  ...r....r....rW.
-00003ae0: 0000 7282 0000 0072 d900 0000 72de 0000  ..r....r....r...
-00003af0: 0072 1600 0000 72e5 0000 0072 dc00 0000  .r....r....r....
-00003b00: 720e 0000 0072 4a00 0000 7255 0000 0029  r....rJ...rU...)
-00003b10: 0972 7c00 0000 72ef 0000 0072 f400 0000  .r|...r....r....
-00003b20: 72be 0000 0072 f200 0000 72ec 0000 0072  r....r....r....r
-00003b30: ee00 0000 72f6 0000 00da 0872 6573 706f  ....r......respo
-00003b40: 6e73 6572 5a00 0000 725a 0000 0072 5b00  nserZ...rZ...r[.
-00003b50: 0000 da0b 6765 6e5f 7067 5f73 7065 63bb  ....gen_pg_spec.
-00003b60: 0200 0073 5a00 0000 0014 0201 0801 0401  ...sZ...........
-00003b70: 1402 1001 1001 0201 0201 0401 02ff 02fe  ................
-00003b80: 1806 0a01 0801 0201 0201 0401 02ff 02fe  ................
-00003b90: 0606 0801 0201 0200 02ff 0604 0201 0401  ................
-00003ba0: 0801 0201 02fd 0605 0a01 1001 0201 0401  ................
-00003bb0: 0cff 02ff 0405 0601 1201 1001 0201 0201  ................
-00003bc0: 08fe 72f8 0000 007a 0c2f 6765 6e5f 7067  ..r....z./gen_pg
-00003bd0: 5f68 656c 6d63 0100 0000 0000 0000 0000  _helmc..........
-00003be0: 0000 0600 0000 0a00 0000 4300 0000 73b6  ..........C...s.
-00003bf0: 0000 0064 0164 026c 006d 017d 0101 0074  ...d.d.l.m.}...t
-00003c00: 02a0 037c 00a1 017d 027c 0264 036b 0872  ...|...}.|.d.k.r
-00003c10: 3074 0464 0464 05a0 057c 00a1 0164 068d  0t.d.d...|...d..
-00003c20: 0282 017c 026a 067d 0374 07a0 0864 077c  ...|.j.}.t...d.|
-00003c30: 03a1 0201 0074 0974 0a74 0b64 0864 0984  .....t.t.t.d.d..
-00003c40: 007c 0364 0a19 0083 0283 0183 017d 047a  .|.d.........}.z
-00003c50: 107c 017c 027c 0474 0c83 0301 0057 006e  .|.|.|.t.....W.n
-00003c60: 4404 0074 0d6a 0e6b 0a72 b001 007d 0501  D..t.j.k.r...}..
-00003c70: 007a 2474 07a0 0f74 10a0 11a1 00a1 0101  .z$t...t........
-00003c80: 0074 0464 0b64 0ca0 057c 05a1 0164 068d  .t.d.d...|...d..
-00003c90: 0282 0157 0035 0064 037d 057e 0558 0059  ...W.5.d.}.~.X.Y
-00003ca0: 006e 0258 0064 0d53 0029 0e7a 2c0a 2020  .n.X.d.S.).z,.  
-00003cb0: 2020 4465 706c 6f79 7320 6120 5047 5420    Deploys a PGT 
-00003cc0: 6173 2061 204b 3873 2068 656c 6d20 6368  as a K8s helm ch
-00003cd0: 6172 742e 0a20 2020 20e9 0300 0000 2901  art..    .....).
-00003ce0: da0a 7374 6172 745f 6865 6c6d 4e72 4300  ..start_helmNrC.
-00003cf0: 0000 72c4 0000 0072 4400 0000 7a08 5047  ..r....rD...z.PG
-00003d00: 5450 3a20 2573 6301 0000 0000 0000 0000  TP: %sc.........
-00003d10: 0000 0001 0000 0002 0000 0053 0000 0073  ...........S...s
-00003d20: 0800 0000 6401 7c00 6b06 5300 72c5 0000  ....d.|.k.S.r...
-00003d30: 0072 5a00 0000 72c6 0000 0072 5a00 0000  .rZ...r....rZ...
-00003d40: 725a 0000 0072 5b00 0000 72c8 0000 0017  rZ...r[...r.....
-00003d50: 0300 0072 c900 0000 7a1d 6765 6e5f 7067  ...r....z.gen_pg
-00003d60: 5f68 656c 6d2e 3c6c 6f63 616c 733e 2e3c  _helm.<locals>.<
-00003d70: 6c61 6d62 6461 3e72 ca00 0000 7248 0000  lambda>r....rH..
-00003d80: 0072 d100 0000 7a30 496e 7370 6563 7420  .r....z0Inspect 
-00003d90: 796f 7572 206b 3873 2064 6173 6862 6f61  your k8s dashboa
-00003da0: 7264 2066 6f72 2064 6570 6c6f 796d 656e  rd for deploymen
-00003db0: 7420 7374 6174 7573 2912 5a19 6465 706c  t status).Z.depl
-00003dc0: 6f79 2e73 7461 7274 5f68 656c 6d5f 636c  oy.start_helm_cl
-00003dd0: 7573 7465 7272 fa00 0000 7282 0000 0072  usterr....r....r
-00003de0: d900 0000 720a 0000 0072 5700 0000 72da  ....r....rW...r.
-00003df0: 0000 0072 4c00 0000 72a3 0000 0072 5f00  ...rL...r....r_.
-00003e00: 0000 72dc 0000 0072 dd00 0000 726b 0000  ..r....r....rk..
-00003e10: 0072 1500 0000 72e8 0000 0072 7500 0000  .r....r....ru...
-00003e20: 72a4 0000 0072 a500 0000 2906 727c 0000  r....r....).r|..
-00003e30: 0072 fa00 0000 72ec 0000 0072 ed00 0000  .r....r....r....
-00003e40: 72a6 0000 0072 f200 0000 725a 0000 0072  r....r....rZ...r
-00003e50: 5a00 0000 725b 0000 00da 0b67 656e 5f70  Z...r[.....gen_p
-00003e60: 675f 6865 6c6d ff02 0000 732e 0000 0000  g_helm....s.....
-00003e70: 0a0c 020a 0108 0102 0102 0104 0102 ff02  ................
-00003e80: fe06 0706 010c 0102 0114 ff04 0402 0110  ................
-00003e90: 0112 010e 0102 0102 0108 fe18 0572 fb00  .............r..
-00003ea0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00003eb0: 0000 0003 0000 0040 0000 0073 c600 0000  .......@...s....
-00003ec0: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-00003ed0: 5a04 6505 6506 6402 6602 1900 6507 6403  Z.e.e.d.f...e.d.
-00003ee0: 3c00 6402 5a08 6505 6506 6402 6602 1900  <.d.Z.e.e.d.f...
-00003ef0: 6507 6404 3c00 6402 5a09 6505 6506 6402  e.d.<.d.Z.e.e.d.
-00003f00: 6602 1900 6507 6405 3c00 6402 5a0a 6505  f...e.d.<.d.Z.e.
-00003f10: 6506 6402 6602 1900 6507 6406 3c00 6402  e.d.f...e.d.<.d.
-00003f20: 5a0b 6505 6506 6402 6602 1900 6507 6407  Z.e.e.d.f...e.d.
-00003f30: 3c00 6402 5a0c 6505 6506 6402 6602 1900  <.d.Z.e.e.d.f...
-00003f40: 6507 6408 3c00 6402 5a0d 6505 6506 6402  e.d.<.d.Z.e.e.d.
-00003f50: 6602 1900 6507 6409 3c00 6402 5a0e 6505  f...e.d.<.d.Z.e.
-00003f60: 6506 6402 6602 1900 6507 640a 3c00 6402  e.d.f...e.d.<.d.
-00003f70: 5a0f 6505 6506 6402 6602 1900 6507 640b  Z.e.e.d.f...e.d.
-00003f80: 3c00 6402 5300 290c da0a 416c 676f 5061  <.d.S.)...AlgoPa
-00003f90: 7261 6d73 7a88 0a20 2020 2053 6574 206f  ramsz..    Set o
-00003fa0: 6620 7363 6865 6475 6c69 6e67 2061 6c67  f scheduling alg
-00003fb0: 6f72 6974 686d 2070 6172 616d 6574 6572  orithm parameter
-00003fc0: 732c 206e 6f74 2061 6c6c 2061 7070 6c79  s, not all apply
-00003fd0: 2074 6f20 616c 6c20 616c 676f 7269 7468   to all algorith
-00003fe0: 6d73 2e0a 2020 2020 5265 6665 7220 746f  ms..    Refer to
-00003ff0: 206d 6169 6e20 646f 6375 6d65 6e74 6174   main documentat
-00004000: 696f 6e20 666f 7220 6d6f 7265 2069 6e66  ion for more inf
-00004010: 6f72 6d61 7469 6f6e 2e0a 2020 2020 4e72  ormation..    Nr
-00004020: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
-00004030: 0000 0072 b000 0000 72b1 0000 0072 b200  ...r....r....r..
-00004040: 0000 72b3 0000 0072 b400 0000 2910 da08  ..r....r....)...
-00004050: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00004060: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00004070: 5f5f da07 5f5f 646f 635f 5f72 ac00 0000  __..__doc__r....
-00004080: 7204 0000 0072 d400 0000 da0f 5f5f 616e  r....r......__an
-00004090: 6e6f 7461 7469 6f6e 735f 5f72 ad00 0000  notations__r....
-000040a0: 72ae 0000 0072 af00 0000 72b0 0000 0072  r....r....r....r
-000040b0: b100 0000 72b2 0000 0072 b300 0000 72b4  ....r....r....r.
-000040c0: 0000 0072 5a00 0000 725a 0000 0072 5a00  ...rZ...rZ...rZ.
-000040d0: 0000 725b 0000 0072 fc00 0000 2903 0000  ..r[...r....)...
-000040e0: 7314 0000 000a 0104 0514 0114 0114 0114  s...............
-000040f0: 0114 0114 0114 0114 0172 fc00 0000 6300  .........r....c.
-00004100: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00004110: 0000 0040 0000 0073 2400 0000 6500 5a01  ...@...s$...e.Z.
-00004120: 6400 5a02 6401 5a03 6402 5a04 6403 5a05  d.Z.d.Z.d.Z.d.Z.
-00004130: 6404 5a06 6405 5a07 6406 5a08 6407 5300  d.Z.d.Z.d.Z.d.S.
-00004140: 2908 da0f 4b6e 6f77 6e41 6c67 6f72 6974  )...KnownAlgorit
-00004150: 686d 737a 540a 2020 2020 4c69 7374 206f  hmszT.    List o
-00004160: 6620 6b6e 6f77 6e20 7363 6865 6475 6c69  f known scheduli
-00004170: 6e67 2061 6c67 6f72 6974 686d 732e 0a20  ng algorithms.. 
-00004180: 2020 2057 696c 6c20 6e65 6564 2074 6f20     Will need to 
-00004190: 6265 2075 7064 6174 6564 206d 616e 7561  be updated manua
-000041a0: 6c6c 792e 0a20 2020 2029 01da 046e 6f6e  lly..    )...non
-000041b0: 6529 0172 8900 0000 2901 5a08 6d79 7361  e).r....).Z.mysa
-000041c0: 726b 6172 2901 5a0d 6d69 6e5f 6e75 6d5f  rkar).Z.min_num_
-000041d0: 7061 7274 735a 0370 736f 4e29 0972 fd00  partsZ.psoN).r..
-000041e0: 0000 72fe 0000 0072 ff00 0000 7200 0100  ..r....r....r...
-000041f0: 005a 0941 4c47 4f5f 4e4f 4e45 5a0a 414c  .Z.ALGO_NONEZ.AL
-00004200: 474f 5f4d 4554 4953 5a0e 414c 474f 5f4d  GO_METISZ.ALGO_M
-00004210: 595f 5341 524b 4152 5a12 414c 474f 5f4d  Y_SARKARZ.ALGO_M
-00004220: 494e 5f4e 554d 5f50 4152 5453 5a08 414c  IN_NUM_PARTSZ.AL
-00004230: 474f 5f50 534f 725a 0000 0072 5a00 0000  GO_PSOrZ...rZ...
-00004240: 725a 0000 0072 5b00 0000 7202 0100 003a  rZ...r[...r....:
-00004250: 0300 0073 0c00 0000 0801 0405 0401 0401  ...s............
-00004260: 0401 0401 7202 0100 0029 02da 0d67 7261  ....r....)...gra
-00004270: 7068 5f63 6f6e 7465 6e74 da0a 6772 6170  ph_content..grap
-00004280: 685f 6e61 6d65 6302 0000 0000 0000 0000  h_namec.........
-00004290: 0000 0006 0000 000b 0000 0043 0000 0073  ...........C...s
-000042a0: f200 0000 6900 7d02 7c00 6400 6b09 7220  ....i.}.|.d.k.r 
-000042b0: 7c01 6400 6b09 7220 7400 6401 6402 6403  |.d.k.r t.d.d.d.
-000042c0: 8d02 8201 7401 7402 7c01 8302 7386 7c00  ....t.t.|...s.|.
-000042d0: 733c 7400 6401 6404 6403 8d02 8201 71ee  s<t.d.d.d.....q.
-000042e0: 7a0e 7403 a004 7c00 a101 7d02 5700 71ee  z.t...|...}.W.q.
-000042f0: 0400 7405 6b0a 7282 0100 7d03 0100 7a1a  ..t.k.r...}...z.
-00004300: 7406 a007 7c03 a101 0100 7400 6401 6405  t...|.....t.d.d.
-00004310: 6403 8d02 8201 5700 3500 6400 7d03 7e03  d.....W.5.d.}.~.
-00004320: 5800 5900 71ee 5800 6e68 7408 7402 7c01  X.Y.q.X.nht.t.|.
-00004330: 8302 7d04 7409 7c04 6406 8302 8f4e 7d05  ..}.t.|.d....N}.
-00004340: 7a0e 7403 a00a 7c05 a101 7d02 5700 6e38  z.t...|...}.W.n8
-00004350: 0400 7405 6b0a 72e2 0100 7d03 0100 7a1a  ..t.k.r...}...z.
-00004360: 7406 a007 7c03 a101 0100 7400 6407 6408  t...|.....t.d.d.
-00004370: 6403 8d02 8201 5700 3500 6400 7d03 7e03  d.....W.5.d.}.~.
-00004380: 5800 5900 6e02 5800 5700 3500 5100 5200  X.Y.n.X.W.5.Q.R.
-00004390: 5800 7c02 5300 2909 4ee9 9001 0000 7a35  X.|.S.).N.....z5
-000043a0: 4e65 6564 2074 6f20 7375 7070 6c79 2065  Need to supply e
-000043b0: 6974 6865 7220 616e 206e 616d 6520 6f72  ither an name or
-000043c0: 2063 6f6e 7465 6e74 2062 7574 206e 6f74   content but not
-000043d0: 2062 6f74 6872 4400 0000 7a19 4c47 2063   bothrD...z.LG c
-000043e0: 6f6e 7465 6e74 2069 7320 6e6f 6e65 7869  ontent is nonexi
-000043f0: 7374 656e 747a 174c 4720 636f 6e74 656e  stentz.LG conten
-00004400: 7420 6973 206d 616c 666f 726d 6564 725e  t is malformedr^
-00004410: 0000 0072 4800 0000 7a21 4c47 2067 7261  ...rH...z!LG gra
-00004420: 7068 206f 6e20 6669 6c65 2063 616e 6e6f  ph on file canno
-00004430: 7420 6265 206c 6f61 6465 6429 0b72 0a00  t be loaded).r..
-00004440: 0000 7229 0000 0072 4900 0000 724a 0000  ..r)...rI...rJ..
-00004450: 0072 4b00 0000 7203 0000 0072 4c00 0000  .rK...r....rL...
-00004460: 7275 0000 0072 2800 0000 7253 0000 0072  ru...r(...rS...r
-00004470: 6300 0000 2906 7204 0100 0072 0501 0000  c...).r....r....
-00004480: 5a09 6f75 745f 6772 6170 68da 066a 6572  Z.out_graph..jer
-00004490: 726f 7272 6500 0000 7266 0000 0072 5a00  rorre...rf...rZ.
-000044a0: 0000 725a 0000 0072 5b00 0000 da0a 6c6f  ..rZ...r[.....lo
-000044b0: 6164 5f67 7261 7068 4703 0000 733e 0000  ad_graphG...s>..
-000044c0: 0000 0104 0110 0102 0102 0102 fe06 040a  ................
-000044d0: 0104 0102 0102 0002 ff08 0402 010e 0110  ................
-000044e0: 010a 0102 0102 0002 ff1a 040a 010c 0102  ................
-000044f0: 010e 0110 010a 0102 0102 0002 ff22 0372  .............".r
-00004500: 0801 0000 7a08 2f6c 675f 6669 6c6c 7a40  ....z./lg_fillz@
-00004510: 4966 2070 7265 7365 6e74 2c20 7472 616e  If present, tran
-00004520: 736c 6174 6f72 2077 696c 6c20 7573 6520  slator will use 
-00004530: 7468 6973 2073 7472 696e 6720 6173 2074  this string as t
-00004540: 6865 2067 7261 7068 2063 6f6e 7465 6e74  he graph content
-00004550: 7a02 7b7d 7a27 4a53 4f4e 206b 6579 3a20  z.{}z'JSON key: 
-00004560: 7661 6c75 6520 7374 6f72 6520 6f66 2067  value store of g
-00004570: 7261 7068 2070 6172 616d 7465 7263 0100  raph paramterc..
-00004580: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00004590: 0000 4300 0000 7312 0000 0067 007c 005d  ..C...s....g.|.]
-000045a0: 0a7d 017c 016a 0091 0271 0453 0072 5a00  .}.|.j...q.S.rZ.
-000045b0: 0000 723b 0000 0029 0272 9400 0000 5a07  ..r;...).r....Z.
-000045c0: 726f 7074 696f 6e72 5a00 0000 725a 0000  roptionrZ...rZ..
-000045d0: 0072 5b00 0000 7297 0000 0077 0300 0073  .r[...r....w...s
-000045e0: 0400 0000 0602 02ff 7297 0000 0029 02da  ........r....)..
-000045f0: 0465 6e75 6d72 3300 0000 2904 7240 0000  .enumr3...).r@..
-00004600: 0072 4100 0000 da0a 7061 7261 6d65 7465  .rA.....paramete
-00004610: 7273 7242 0000 0063 0400 0000 0000 0000  rsrB...c........
-00004620: 0000 0000 0800 0000 0a00 0000 4300 0000  ............C...
-00004630: 7378 0000 0074 007c 017c 0083 027d 047a  sx...t.|.|...}.z
-00004640: 0e74 01a0 027c 02a1 017d 0557 006e 3804  .t...|...}.W.n8.
-00004650: 0074 036b 0a72 5001 007d 0601 007a 1a74  .t.k.rP..}...z.t
-00004660: 04a0 057c 06a1 0101 0074 0664 0164 0264  ...|.....t.d.d.d
-00004670: 038d 0282 0157 0035 0064 047d 067e 0658  .....W.5.d.}.~.X
-00004680: 0059 006e 0258 0074 076a 086a 09a0 0a7c  .Y.n.X.t.j.j...|
-00004690: 047c 05a1 027d 0774 0b74 0c7c 077c 0383  .|...}.t.t.|.|..
-000046a0: 0283 017d 0774 0d7c 0783 0153 0029 057a  ...}.t.|...S.).z
-000046b0: 950a 2020 2020 5769 6c6c 2066 696c 6c20  ..    Will fill 
-000046c0: 6120 6c6f 6769 6361 6c20 6772 6170 6820  a logical graph 
-000046d0: 6279 2072 6570 6c61 6369 6e67 2066 6965  by replacing fie
-000046e0: 6c64 7320 7769 7468 2073 7570 706c 6965  lds with supplie
-000046f0: 6420 7061 7261 6d65 7465 7273 2e0a 0a20  d parameters... 
-00004700: 2020 204f 6e65 206f 6620 6c67 5f6e 616d     One of lg_nam
-00004710: 6520 6f72 206c 675f 636f 6e74 656e 742c  e or lg_content,
-00004720: 2062 7574 206e 6f74 2062 6f74 682c 206d   but not both, m
-00004730: 7573 7420 6265 2073 7065 6369 6669 6564  ust be specified
-00004740: 2e0a 2020 2020 7206 0100 007a 1b50 6172  ..    r....z.Par
-00004750: 616d 6574 6572 2073 7472 696e 6720 6973  ameter string is
-00004760: 2069 6e76 616c 6964 7244 0000 004e 290e   invalidrD...N).
-00004770: 7208 0100 0072 4a00 0000 724b 0000 0072  r....rJ...rK...r
-00004780: 0300 0000 724c 0000 0072 7500 0000 720a  ....rL...ru...r.
-00004790: 0000 00da 0364 6c67 da08 6472 6f70 6d61  .....dlg..dropma
-000047a0: 6b65 da0c 7067 5f67 656e 6572 6174 6f72  ke..pg_generator
-000047b0: da04 6669 6c6c 721c 0000 0072 1b00 0000  ..fillr....r....
-000047c0: 720e 0000 0029 0872 4000 0000 7241 0000  r....).r@...rA..
-000047d0: 0072 0a01 0000 7242 0000 00da 086c 675f  .r....rB.....lg_
-000047e0: 6772 6170 68da 0670 6172 616d 7372 0701  graph..paramsr..
-000047f0: 0000 5a0c 6f75 7470 7574 5f67 7261 7068  ..Z.output_graph
-00004800: 725a 0000 0072 5a00 0000 725b 0000 00da  rZ...rZ...r[....
-00004810: 076c 675f 6669 6c6c 6803 0000 7318 0000  .lg_fillh...s...
-00004820: 0000 1b0a 0102 010e 0110 010a 0102 0102  ................
-00004830: 0002 ff18 0310 010e 0172 1101 0000 7a07  .........r....z.
-00004840: 2f75 6e72 6f6c 6c7a 2449 4420 7072 6566  /unrollz$ID pref
-00004850: 6978 2061 7070 656e 6465 6420 746f 2075  ix appended to u
-00004860: 6e72 6f6c 6c65 6420 6e6f 6465 737a 2e49  nrolled nodesz.I
-00004870: 6620 7472 7565 2c20 6170 7073 2077 696c  f true, apps wil
-00004880: 6c20 6265 2072 6570 6c61 6365 6420 7769  l be replaced wi
-00004890: 7468 2073 6c65 6570 2061 7070 737a 2e49  th sleep appsz.I
-000048a0: 6620 7365 742c 2077 696c 6c20 6368 616e  f set, will chan
-000048b0: 6765 2061 6c6c 2061 7070 7320 746f 2074  ge all apps to t
-000048c0: 6869 7320 6170 7020 636c 6173 7329 0572  his app class).r
-000048d0: 4000 0000 7241 0000 00da 0a6f 6964 5f70  @...rA.....oid_p
-000048e0: 7265 6669 78da 087a 6572 6f5f 7275 6eda  refix..zero_run.
-000048f0: 0b64 6566 6175 6c74 5f61 7070 6305 0000  .default_appc...
-00004900: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-00004910: 0043 0000 0073 2e00 0000 7400 7c01 7c00  .C...s....t.|.|.
-00004920: 8302 7d05 7401 6a02 6a03 a004 7c05 7c02  ..}.t.j.j...|.|.
-00004930: 7c03 7c04 a104 7d06 7405 7c06 8301 7d06  |.|...}.t.|...}.
-00004940: 7406 7c06 8301 5300 2901 7a8d 0a20 2020  t.|...S.).z..   
-00004950: 2057 696c 6c20 756e 726f 6c6c 2061 206c   Will unroll a l
-00004960: 6f67 6963 616c 2067 7261 7068 2069 6e74  ogical graph int
-00004970: 6f20 6120 7068 7973 6963 616c 2067 7261  o a physical gra
-00004980: 7068 2074 656d 706c 6174 652e 0a0a 2020  ph template...  
-00004990: 2020 4f6e 6520 6f66 206c 675f 6e61 6d65    One of lg_name
-000049a0: 206f 7220 6c67 5f63 6f6e 7465 6e74 2c20   or lg_content, 
-000049b0: 6275 7420 6e6f 7420 626f 7468 2c20 6e65  but not both, ne
-000049c0: 6564 7320 746f 2062 6520 7370 6563 6966  eds to be specif
-000049d0: 6965 642e 0a20 2020 2029 0772 0801 0000  ied..    ).r....
-000049e0: 720b 0100 0072 0c01 0000 720d 0100 00da  r....r....r.....
-000049f0: 0675 6e72 6f6c 6c72 1e00 0000 720e 0000  .unrollr....r...
-00004a00: 0029 0772 4000 0000 7241 0000 0072 1201  .).r@...rA...r..
-00004a10: 0000 7213 0100 0072 1401 0000 720f 0100  ..r....r....r...
-00004a20: 0072 6d00 0000 725a 0000 0072 5a00 0000  .rm...rZ...rZ...
-00004a30: 725b 0000 00da 096c 675f 756e 726f 6c6c  r[.....lg_unroll
-00004a40: 9003 0000 7312 0000 0000 1b0a 0108 0102  ....s...........
-00004a50: 0002 0002 0002 ff04 0308 0172 1601 0000  ...........r....
-00004a60: 7a0a 2f70 6172 7469 7469 6f6e 7a3d 4966  z./partitionz=If
-00004a70: 2073 7065 6369 6669 6564 2c20 7472 616e   specified, tran
-00004a80: 736c 6174 6f72 2077 696c 6c20 6174 7465  slator will atte
-00004a90: 6d70 7420 746f 206c 6f61 6420 6772 6170  mpt to load grap
-00004aa0: 6820 6672 6f6d 2066 696c 657a 2f4e 756d  h from filez/Num
-00004ab0: 6265 7220 6f66 2070 6172 7469 7469 6f6e  ber of partition
-00004ac0: 7320 746f 2075 6e72 6f6c 6c20 7468 6520  s to unroll the 
-00004ad0: 6772 6170 6820 6163 726f 7373 7a27 4e75  graph acrossz'Nu
-00004ae0: 6d62 6572 206f 6620 6461 7461 2069 736c  mber of data isl
-00004af0: 616e 6473 2074 6f20 7061 7274 6974 696f  ands to partitio
-00004b00: 6e20 666f 727a 2154 6865 2073 656c 6563  n forz!The selec
-00004b10: 7465 6420 7363 6865 6475 6c69 6e67 2061  ted scheduling a
-00004b20: 6c67 6f72 6974 686d 7a62 5468 6520 7061  lgorithmzbThe pa
-00004b30: 7261 6d65 7465 7220 7661 6c75 6573 2070  rameter values p
-00004b40: 6173 7365 6420 746f 2074 6865 2073 6368  assed to the sch
-00004b50: 6564 756c 696e 6720 616c 676f 7269 7468  eduling algorith
-00004b60: 6d2e 2052 6571 7569 7265 6420 7061 7261  m. Required para
-00004b70: 6d65 7465 7273 2076 6172 6965 7320 7065  meters varies pe
-00004b80: 7220 616c 676f 7269 7468 6d2e 2906 726a  r algorithm.).rj
-00004b90: 0000 00da 0b70 6774 5f63 6f6e 7465 6e74  .....pgt_content
-00004ba0: 72a6 0000 0072 8d00 0000 da09 616c 676f  r....r......algo
-00004bb0: 7269 7468 6d72 b800 0000 6306 0000 0000  rithmr....c.....
-00004bc0: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
-00004bd0: 0000 0073 5800 0000 7400 7c01 7c00 8302  ...sX...t.|.|...
-00004be0: 7d06 6900 7d07 7c06 6401 1900 a001 6402  }.i.}.|.d.....d.
-00004bf0: a101 7324 7c06 a002 a100 7d07 7403 6a04  ..s$|.....}.t.j.
-00004c00: 6a05 a006 7c06 7c04 7c02 7c03 7c05 a007  j...|.|.|.|.|...
-00004c10: a100 a105 7d08 7c08 a008 7c07 a101 0100  ....}.|...|.....
-00004c20: 7409 7c08 8301 7d08 740a 7c08 8301 5300  t.|...}.t.|...S.
-00004c30: 2903 7ab3 0a20 2020 2055 7365 7320 7363  ).z..    Uses sc
-00004c40: 6865 6475 6c69 6e67 2061 6c67 6f72 6974  heduling algorit
-00004c50: 686d 7320 746f 2070 6172 7469 7469 6f6e  hms to partition
-00004c60: 2061 6e20 756e 726f 6c6c 6564 2070 6774   an unrolled pgt
-00004c70: 2061 6372 6f73 7320 7365 7665 7261 6c20   across several 
-00004c80: 7061 7274 6974 696f 6e73 2061 6e64 2064  partitions and d
-00004c90: 6174 6120 6973 6c61 6e64 732e 0a0a 2020  ata islands...  
-00004ca0: 2020 4f6e 6520 6f66 2070 6774 5f6e 616d    One of pgt_nam
-00004cb0: 6520 6f72 2070 6774 5f63 6f6e 7465 6e74  e or pgt_content
-00004cc0: 2c20 6275 7420 6e6f 7420 626f 7468 2c20  , but not both, 
-00004cd0: 6d75 7374 2062 6520 7370 6563 6966 6965  must be specifie
-00004ce0: 642e 0a20 2020 2072 c300 0000 da03 6f69  d..    r......oi
-00004cf0: 6429 0b72 0801 0000 da03 6765 74da 0370  d).r......get..p
-00004d00: 6f70 720b 0100 0072 0c01 0000 720d 0100  opr....r....r...
-00004d10: 00da 0970 6172 7469 7469 6f6e da04 6469  ...partition..di
-00004d20: 6374 72df 0000 0072 1d00 0000 720e 0000  ctr....r....r...
-00004d30: 0029 0972 6a00 0000 7217 0100 0072 a600  .).rj...r....r..
-00004d40: 0000 728d 0000 0072 1801 0000 72b8 0000  ..r....r....r...
-00004d50: 00da 0567 7261 7068 72db 0000 0072 6d00  ...graphr....rm.
-00004d60: 0000 725a 0000 0072 5a00 0000 725b 0000  ..rZ...rZ...r[..
-00004d70: 00da 0d70 6774 5f70 6172 7469 7469 6f6e  ...pgt_partition
-00004d80: b303 0000 731c 0000 0000 1e0a 0104 010e  ....s...........
-00004d90: 0108 0108 0102 0002 0002 0002 0006 ff04  ................
-00004da0: 030a 0108 0172 1f01 0000 7a15 2f75 6e72  .....r....z./unr
-00004db0: 6f6c 6c5f 616e 645f 7061 7274 6974 696f  oll_and_partitio
-00004dc0: 6e29 0972 4000 0000 7241 0000 0072 1201  n).r@...rA...r..
-00004dd0: 0000 7213 0100 0072 1401 0000 72a6 0000  ..r....r....r...
-00004de0: 0072 8d00 0000 7218 0100 0072 b800 0000  .r....r....r....
-00004df0: 6309 0000 0000 0000 0000 0000 000c 0000  c...............
-00004e00: 0008 0000 0043 0000 0073 6200 0000 7400  .....C...sb...t.
-00004e10: 7c01 7c00 8302 7d09 7401 6a02 6a03 a004  |.|...}.t.j.j...
-00004e20: 7c09 7c02 7c03 7c04 a104 7d0a 7405 7c0a  |.|.|.|...}.t.|.
-00004e30: 8301 7d0a 7c0a a006 a100 7d0b 7401 6a02  ..}.|.....}.t.j.
-00004e40: 6a03 a007 7c0a 7c07 7c05 7c06 7c08 a008  j...|.|.|.|.|...
-00004e50: a100 a105 7d0a 7c0a a009 7c0b a101 0100  ....}.|...|.....
-00004e60: 740a 7c0a 8301 7d0a 740b 7c0a 8301 5300  t.|...}.t.|...S.
-00004e70: 2901 7a9b 0a20 2020 2055 6e72 6f6c 6c73  ).z..    Unrolls
-00004e80: 2061 6e64 2070 6172 7469 7469 6f6e 7320   and partitions 
-00004e90: 6120 6c6f 6769 6361 6c20 6772 6170 6820  a logical graph 
-00004ea0: 7769 7468 2074 6865 2070 726f 7669 6465  with the provide
-00004eb0: 6420 7661 7269 6f75 7320 7061 7261 6d65  d various parame
-00004ec0: 7465 7273 2e0a 0a20 2020 204f 6e65 206f  ters...    One o
-00004ed0: 6620 6c67 5f6e 616d 6520 616e 6420 6c67  f lg_name and lg
-00004ee0: 5f63 6f6e 7465 6e74 2c20 6275 7420 6e6f  _content, but no
-00004ef0: 7420 626f 7468 2c20 6d75 7374 2062 6520  t both, must be 
-00004f00: 7370 6563 6966 6965 642e 0a20 2020 2029  specified..    )
-00004f10: 0c72 0801 0000 720b 0100 0072 0c01 0000  .r....r....r....
-00004f20: 720d 0100 0072 1501 0000 721e 0000 0072  r....r....r....r
-00004f30: 1b01 0000 721c 0100 0072 1d01 0000 72df  ....r....r....r.
-00004f40: 0000 0072 1d00 0000 720e 0000 0029 0c72  ...r....r....).r
-00004f50: 4000 0000 7241 0000 0072 1201 0000 7213  @...rA...r....r.
-00004f60: 0100 0072 1401 0000 72a6 0000 0072 8d00  ...r....r....r..
-00004f70: 0000 7218 0100 0072 b800 0000 720f 0100  ..r....r....r...
-00004f80: 0072 6d00 0000 72db 0000 0072 5a00 0000  .rm...r....rZ...
-00004f90: 725a 0000 0072 5b00 0000 da17 6c67 5f75  rZ...r[.....lg_u
-00004fa0: 6e72 6f6c 6c5f 616e 645f 7061 7274 6974  nroll_and_partit
-00004fb0: 696f 6edd 0300 0073 2600 0000 002b 0a01  ion....s&....+..
-00004fc0: 0801 0200 0200 0200 02ff 0403 0801 0801  ................
-00004fd0: 0801 0200 0200 0200 0200 06ff 0403 0a01  ................
-00004fe0: 0801 7220 0100 007a 042f 6d61 707a 4b49  ..r ...z./mapzKI
-00004ff0: 6620 7375 7070 6c69 6564 2c20 7468 6973  f supplied, this
-00005000: 2067 7261 7068 2077 696c 6c20 6174 7465   graph will atte
-00005010: 6d70 7465 6420 746f 2062 6520 6c6f 6164  mpted to be load
-00005020: 6564 2066 726f 6d20 6469 736b 206f 6e20  ed from disk on 
-00005030: 7468 6520 7365 7276 6572 7a26 4966 2073  the serverz&If s
-00005040: 7570 706c 6965 642c 2074 6869 7320 6973  upplied, this is
-00005050: 2074 6865 2067 7261 7068 2063 6f6e 7465   the graph conte
-00005060: 6e74 7a3c 436f 6d6d 6120 7365 7061 7261  ntz<Comma separa
-00005070: 7465 6420 6c69 7374 206f 6620 4950 2061  ted list of IP a
-00005080: 6464 7273 2065 2e67 2e20 276c 6f63 616c  ddrs e.g. 'local
-00005090: 686f 7374 2c20 3132 372e 302e 302e 3227  host, 127.0.0.2'
-000050a0: 7a24 5468 6520 6e75 6d62 6572 206f 6620  z$The number of 
-000050b0: 6461 7461 2069 736c 616e 6473 2074 6f20  data islands to 
-000050c0: 6c61 756e 6368 547a 4757 6865 7468 6572  launchTzGWhether
-000050d0: 2074 6f20 6c61 756e 6368 2064 6174 6120   to launch data 
-000050e0: 6973 6c61 6e64 206d 616e 6167 6572 2070  island manager p
-000050f0: 726f 6365 7373 6573 2061 6c6f 6e67 7369  rocesses alongsi
-00005100: 6465 206e 6f64 652d 6d61 6e61 6765 7273  de node-managers
-00005110: 7a40 4966 2070 7265 7365 6e74 2c20 7769  z@If present, wi
-00005120: 6c6c 2061 7474 656d 7074 2074 6f20 7175  ll attempt to qu
-00005130: 6572 7920 7468 6973 2061 6464 7265 7373  ery this address
-00005140: 2066 6f72 206e 6f64 652d 6d61 6e61 6765   for node-manage
-00005150: 7273 7a21 506f 7274 2075 7365 6420 6279  rsz!Port used by
-00005160: 2048 4f53 5420 6d61 6e61 6765 7220 7072   HOST manager pr
-00005170: 6f63 6573 7329 0772 6a00 0000 7217 0100  ocess).rj...r...
-00005180: 0072 e000 0000 728d 0000 00da 0b63 6f5f  .r....r......co_
-00005190: 686f 7374 5f64 696d 72cd 0000 0072 ce00  host_dimr....r..
-000051a0: 0000 6307 0000 0000 0000 0000 0000 000b  ..c.............
-000051b0: 0000 0006 0000 0043 0000 0073 aa00 0000  .......C...s....
-000051c0: 7c02 7320 7400 7c05 7c06 6401 6402 8d03  |.s t.|.|.d.d...
-000051d0: 7d07 7c05 6701 7c07 a001 a100 1700 7d02  }.|.g.|.......}.
-000051e0: 7402 7c02 8301 7c03 6b01 724e 7403 a004  t.|...|.k.rNt...
-000051f0: 6403 a101 0100 7405 6404 6405 7402 7c02  d.....t.d.d.t.|.
-00005200: 8301 7c03 6602 1600 6406 8d02 0100 7406  ..|.f...d.....t.
-00005210: 7c01 7c00 8302 7d08 6900 7d09 7c08 6407  |.|...}.i.}.|.d.
-00005220: 1900 a007 6408 a101 7372 7c08 a008 a100  ....d...sr|.....
-00005230: 7d09 7403 a009 7c02 a101 0100 740a 6a0b  }.t...|.....t.j.
-00005240: 6a0c a00d 7c08 7c02 7c03 7c04 a104 7d0a  j...|.|.|.|...}.
-00005250: 7c0a a00e 7c09 a101 0100 740f 7c0a 8301  |...|.....t.|...
-00005260: 7d0a 7410 7c0a 8301 5300 2909 7a3a 0a20  }.t.|...S.).z:. 
-00005270: 2020 204d 6170 7320 7068 7973 6963 616c     Maps physical
-00005280: 2067 7261 7068 2074 656d 706c 6174 6573   graph templates
-00005290: 2074 6f20 6e6f 6465 2072 6573 6f75 7263   to node resourc
-000052a0: 6573 2e0a 2020 2020 e90a 0000 0029 0172  es..    .....).r
-000052b0: cf00 0000 7a24 4e6f 7420 656e 6f75 6768  ....z$Not enough
-000052c0: 206e 6f64 6573 2074 6f20 6669 6c6c 2061   nodes to fill a
-000052d0: 6c6c 2069 736c 616e 6473 7248 0000 007a  ll islandsrH...z
-000052e0: 3c23 6e6f 6465 7320 2825 6429 2073 686f  <#nodes (%d) sho
-000052f0: 756c 6420 6265 206c 6172 6765 7220 7468  uld be larger th
-00005300: 616e 2074 6865 206e 756d 6265 7220 6f66  an the number of
-00005310: 2069 736c 616e 6473 2028 2564 2972 4400   islands (%d)rD.
-00005320: 0000 72c3 0000 0072 1901 0000 2911 7217  ..r....r....).r.
-00005330: 0000 0072 e000 0000 725f 0000 0072 4c00  ...r....r_...rL.
-00005340: 0000 7275 0000 0072 0a00 0000 7208 0100  ..ru...r....r...
-00005350: 0072 1a01 0000 721b 0100 0072 a300 0000  .r....r....r....
-00005360: 720b 0100 0072 0c01 0000 720d 0100 00da  r....r....r.....
-00005370: 0c72 6573 6f75 7263 655f 6d61 7072 df00  .resource_mapr..
-00005380: 0000 721f 0000 0072 0e00 0000 290b 726a  ..r....r....).rj
-00005390: 0000 0072 1701 0000 72e0 0000 0072 8d00  ...r....r....r..
-000053a0: 0000 7221 0100 0072 cd00 0000 72ce 0000  ..r!...r....r...
-000053b0: 00da 0663 6c69 656e 7472 6d00 0000 72db  ...clientrm...r.
-000053c0: 0000 00da 0270 6772 5a00 0000 725a 0000  .....pgrZ...rZ..
-000053d0: 0072 5b00 0000 da07 7067 745f 6d61 7016  .r[.....pgt_map.
-000053e0: 0400 0073 3200 0000 0020 0401 0e01 0e01  ...s2.... ......
-000053f0: 0c01 0a01 0201 0201 0201 0aff 02fe 0605  ................
-00005400: 0a01 0401 0e01 0801 0a01 0801 0200 0200  ................
-00005410: 0200 02ff 0403 0a01 0801 7226 0100 007a  ..........r&...z
-00005420: 162f 6170 692f 7375 626d 6973 7369 6f6e  ./api/submission
-00005430: 5f6d 6574 686f 647a 4549 6620 7072 6573  _methodzEIf pres
-00005440: 656e 742c 2074 7261 6e73 6c61 746f 7220  ent, translator 
-00005450: 7769 6c6c 2071 7565 7279 2074 6869 7320  will query this 
-00005460: 5552 4c20 666f 7220 6974 7320 6465 706c  URL for its depl
-00005470: 6f79 6d65 6e74 206f 7074 696f 6e73 7a47  oyment optionszG
-00005480: 4966 2070 7265 7365 6e74 2077 6974 6820  If present with 
-00005490: 6d70 6f72 7420 616e 6420 6d70 7265 6669  mport and mprefi
-000054a0: 782c 2077 696c 6c20 6265 2074 6865 2062  x, will be the b
-000054b0: 6173 6520 686f 7374 2066 6f72 2064 6570  ase host for dep
-000054c0: 6c6f 796d 656e 7472 9900 0000 2903 72bb  loymentr....).r.
-000054d0: 0000 0072 bc00 0000 72bd 0000 0063 0300  ...r....r....c..
-000054e0: 0000 0000 0000 0000 0000 0800 0000 0400  ................
-000054f0: 0000 4300 0000 737e 0000 0074 00a0 0164  ..C...s~...t...d
-00005500: 01a1 0101 007c 0072 1e74 027c 0083 015c  .....|.r.t.|...\
-00005510: 037d 037d 047d 056e 0c7c 017d 037c 027d  .}.}.}.n.|.}.|.}
-00005520: 0464 027d 0567 007d 0674 0383 0072 407c  .d.}.g.}.t...r@|
-00005530: 06a0 0474 056a 06a1 0101 007c 0364 006b  ...t.j.....|.d.k
-00005540: 0972 6a74 077c 037c 047c 0583 037d 0774  .rjt.|.|.|...}.t
-00005550: 056a 087c 076b 0672 6a7c 06a0 0474 056a  .j.|.k.rj|...t.j
-00005560: 09a1 0101 0074 00a0 0164 037c 06a1 0201  .....t...d.|....
-00005570: 0064 047c 0669 0153 0029 054e 7a22 5265  .d.|.i.S.).Nz"Re
-00005580: 6365 6976 6564 2073 7562 6d69 7373 696f  ceived submissio
-00005590: 6e5f 6d65 7468 6f64 2072 6571 7565 7374  n_method request
-000055a0: 7299 0000 007a 154d 6574 686f 6473 2061  r....z.Methods a
-000055b0: 7661 696c 6162 6c65 3a20 2573 da07 6d65  vailable: %s..me
-000055c0: 7468 6f64 7329 0a72 4c00 0000 72d8 0000  thods).rL...r...
-000055d0: 0072 3100 0000 7222 0000 0072 df00 0000  .r1...r"...r....
-000055e0: 7221 0000 005a 0448 454c 4d72 3000 0000  r!...Z.HELMr0...
-000055f0: 5a07 4252 4f57 5345 525a 0653 4552 5645  Z.BROWSERZ.SERVE
-00005600: 5229 0872 bb00 0000 72bc 0000 0072 bd00  R).r....r....r..
-00005610: 0000 72eb 0000 0072 ea00 0000 72e9 0000  ..r....r....r...
-00005620: 00da 1161 7661 696c 6162 6c65 5f6d 6574  ...available_met
-00005630: 686f 6473 5a16 686f 7374 5f61 7661 696c  hodsZ.host_avail
-00005640: 6162 6c65 5f6d 6574 686f 6473 725a 0000  able_methodsrZ..
-00005650: 0072 5a00 0000 725b 0000 00da 1567 6574  .rZ...r[.....get
-00005660: 5f73 7562 6d69 7373 696f 6e5f 6d65 7468  _submission_meth
-00005670: 6f64 4d04 0000 7326 0000 0000 0c0a 0104  odM...s&........
-00005680: 0110 0204 0104 0104 0104 0106 010c 0108  ................
-00005690: 0102 0102 0002 0002 ff04 030a 010c 010c  ................
-000056a0: 0172 2901 0000 725d 0000 007a 2554 6865  .r)...r]...z%The
-000056b0: 2070 6167 6520 7573 6564 2074 6f20 7669   page used to vi
-000056c0: 6577 2070 6879 7369 6361 6c20 6772 6170  ew physical grap
-000056d0: 6873 2902 7269 0000 0072 3300 0000 2901  hs).ri...r3...).
-000056e0: 726f 0000 0063 0100 0000 0000 0000 0000  ro...c..........
-000056f0: 0000 0200 0000 0900 0000 4300 0000 731c  ..........C...s.
-00005700: 0000 0074 00a0 0164 017c 0064 0064 0064  ...t...d.|.d.d.d
-00005710: 0264 0064 039c 05a1 027d 017c 0153 0029  .d.d.....}.|.S.)
-00005720: 044e 7271 0000 0072 7200 0000 7273 0000  .Nrq...rr...rs..
-00005730: 0072 7f00 0000 2902 726f 0000 0072 7a00  .r....).ro...rz.
-00005740: 0000 725a 0000 0072 5a00 0000 725b 0000  ..rZ...rZ...r[..
-00005750: 00da 0569 6e64 6578 6d04 0000 7314 0000  ...indexm...s...
-00005760: 0000 0604 0102 0202 0102 0102 0102 0102  ................
-00005770: fb04 fe04 0a72 2a01 0000 6300 0000 0000  .....r*...c.....
-00005780: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
-00005790: 0000 0073 0400 0000 6900 5300 a901 4e72  ...s....i.S...Nr
-000057a0: 5a00 0000 725a 0000 0072 5a00 0000 725a  Z...rZ...rZ...rZ
-000057b0: 0000 0072 5b00 0000 da0a 6c69 7665 6c69  ...r[.....liveli
-000057c0: 6e65 7373 8004 0000 7302 0000 0000 0272  ness....s......r
-000057d0: 2c01 0000 6302 0000 0000 0000 0000 0000  ,...c...........
-000057e0: 000a 0000 0009 0000 0043 0000 0073 1e02  .........C...s..
-000057f0: 0000 7400 a001 a100 7d02 7c02 6a02 6401  ..t.....}.|.j.d.
-00005800: 6402 6403 7403 6404 6405 6406 6407 8d07  d.d.t.d.d.d.d...
-00005810: 0100 7c02 6a02 6408 6409 6403 7403 640a  ..|.j.d.d.d.t.d.
-00005820: 6405 640b 6407 8d07 0100 7c02 6a02 640c  d.d.d.....|.j.d.
-00005830: 640d 6403 7403 640e 640f 6410 6407 8d07  d.d.t.d.d.d.d...
-00005840: 0100 7c02 6a02 6411 6412 6403 7404 6413  ..|.j.d.d.d.t.d.
-00005850: 6414 6415 6407 8d07 0100 7c02 6a02 6416  d.d.d.....|.j.d.
-00005860: 6417 6418 6419 641a 641b 641c 8d06 0100  d.d.d.d.d.d.....
-00005870: 7c02 6a02 641d 641e 6403 7403 641f 6420  |.j.d.d.d.t.d.d 
-00005880: 7405 a006 a100 6421 8d07 0100 7c02 a007  t.....d!....|...
-00005890: 7c01 a101 7d03 7c03 6a08 6422 6b08 73b8  |...}.|.j.d"k.s.
-000058a0: 7c03 6a09 6422 6b08 72c4 7c02 a00a 6423  |.j.d"k.r.|...d#
-000058b0: a101 0100 6e20 740b 6a0c a00d 7c03 6a08  ....n t.j...|.j.
-000058c0: a101 73e4 7c02 a00a 7c03 6a08 9b00 6424  ..s.|...|.j...d$
-000058d0: 9d02 a101 0100 7c03 6a0e 73f2 7c03 6a0f  ......|.j.s.|.j.
-000058e0: 9001 7282 7410 a011 6425 a101 7d04 7412  ..r.t...d%..}.t.
-000058f0: 6a13 7c04 5f14 7c03 6a0e 9001 723c 7410  j.|._.|.j...r<t.
-00005900: a015 7416 6a17 a101 7d05 7c05 a018 7c04  ..t.j...}.|...|.
-00005910: a101 0100 7410 6a19 a01a 7c05 a101 0100  ....t.j...|.....
-00005920: 7410 6a19 a01b 7410 6a1c a101 0100 7c03  t.j...t.j.....|.
-00005930: 6a0f 9001 7282 7c03 6a0f 7d06 7405 a01d  j...r.|.j.}.t...
-00005940: 7c06 a101 0100 740b 6a0c a01e 7c06 6426  |.....t.j...|.d&
-00005950: a102 7d07 7410 a01f 7c07 a101 7d08 7c08  ..}.t...|...}.|.
-00005960: a018 7c04 a101 0100 7410 6a19 a01a 7c08  ..|.....t.j...|.
-00005970: a101 0100 7a14 740b 6a20 7c03 6a09 6427  ....z.t.j |.j.d'
-00005980: 6428 8d02 0100 5700 6e24 0400 7421 6b0a  d(....W.n$..t!k.
-00005990: 9001 72ba 0100 0100 0100 7410 a022 6429  ..r.......t.."d)
-000059a0: 7c03 6a09 a102 0100 5900 6e02 5800 7c03  |.j.....Y.n.X.|.
-000059b0: 6a08 6123 7c03 6a09 6124 7425 7424 8301  j.a#|.j.a$t%t$..
-000059c0: 6126 642a 642b 8400 7d09 7427 a027 7427  a&d*d+..}.t'.'t'
-000059d0: 6a28 7c09 a102 0100 7427 a027 7427 6a29  j(|.....t'.'t'j)
-000059e0: 7c09 a102 0100 7410 a02a 642c 7c03 6a0e  |.....t..*d,|.j.
-000059f0: a102 0100 742b 6a2c 742d 7c03 6a2e 7c03  ....t+j,t-|.j.|.
-00005a00: 6a2f 7c03 6a0e 642d 8d04 0100 6422 5300  j/|.j.d-....d"S.
-00005a10: 292e 7a40 0a20 2020 2046 6173 7441 5049  ).z@.    FastAPI
-00005a20: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00005a30: 6f66 2064 616c 6975 6765 2074 7261 6e73  of daliuge trans
-00005a40: 6c61 746f 7220 696e 7465 7266 6163 650a  lator interface.
-00005a50: 2020 2020 7a02 2d64 7a07 2d2d 6c67 6469      z.-dz.--lgdi
-00005a60: 72da 0573 746f 7265 7228 0000 007a 042f  r..storer(...z./
-00005a70: 746d 707a 5341 2070 6174 6820 7468 6174  tmpzSA path that
-00005a80: 2063 6f6e 7461 696e 7320 6174 206c 6561   contains at lea
-00005a90: 7374 206f 6e65 2073 7562 2d64 6972 6563  st one sub-direc
-00005aa0: 746f 7279 2c20 7768 6963 6820 636f 6e74  tory, which cont
-00005ab0: 6169 6e73 206c 6f67 6963 616c 2067 7261  ains logical gra
-00005ac0: 7068 2066 696c 6573 2905 da06 6163 7469  ph files)...acti
-00005ad0: 6f6e da04 7479 7065 da04 6465 7374 723f  on..type..destr?
-00005ae0: 0000 00da 0468 656c 707a 022d 747a 082d  .....helpz.-tz.-
-00005af0: 2d70 6774 6469 7272 2b00 0000 7a25 7068  -pgtdirr+...z%ph
-00005b00: 7973 6963 616c 2067 7261 7068 2074 656d  ysical graph tem
-00005b10: 706c 6174 6520 7061 7468 2028 6f75 7470  plate path (outp
-00005b20: 7574 297a 022d 487a 062d 2d68 6f73 7472  ut)z.-Hz.--hostr
-00005b30: cd00 0000 7a07 302e 302e 302e 307a 2a6c  ....z.0.0.0.0z*l
-00005b40: 6f67 6963 616c 2067 7261 7068 2065 6469  ogical graph edi
-00005b50: 746f 7220 686f 7374 2028 616c 6c20 6279  tor host (all by
-00005b60: 2064 6566 6175 6c74 297a 022d 707a 062d   default)z.-pz.-
-00005b70: 2d70 6f72 7472 ce00 0000 6994 1f00 007a  -portr....i....z
-00005b80: 2b6c 6f67 6963 616c 2067 7261 7068 2065  +logical graph e
-00005b90: 6469 746f 7220 706f 7274 2028 3830 3834  ditor port (8084
-00005ba0: 2062 7920 6465 6661 756c 7429 7a02 2d76   by default)z.-v
-00005bb0: 7a09 2d2d 7665 7262 6f73 65da 0a73 746f  z.--verbose..sto
-00005bc0: 7265 5f74 7275 65da 0776 6572 626f 7365  re_true..verbose
-00005bd0: 467a 1345 6e61 626c 6520 6d6f 7265 206c  Fz.Enable more l
-00005be0: 6f67 6769 6e67 2904 722e 0100 0072 3001  ogging).r....r0.
-00005bf0: 0000 723f 0000 0072 3101 0000 7a02 2d6c  ..r?...r1...z.-l
-00005c00: 7a09 2d2d 6c6f 672d 6469 72da 066c 6f67  z.--log-dir..log
-00005c10: 6469 727a 3454 6865 2064 6972 6563 746f  dirz4The directo
-00005c20: 7279 2077 6865 7265 2074 6865 206c 6f67  ry where the log
-00005c30: 6769 6e67 2066 696c 6573 2077 696c 6c20  ging files will 
-00005c40: 6265 2073 746f 7265 6429 0572 2e01 0000  be stored).r....
-00005c50: 722f 0100 0072 3001 0000 7231 0100 0072  r/...r0...r1...r
-00005c60: 3f00 0000 4e7a 1b47 7261 7068 2070 6174  ?...Nz.Graph pat
-00005c70: 6873 206d 6973 7369 6e67 2028 2d64 2f2d  hs missing (-d/-
-00005c80: 7429 7a0f 2064 6f65 7320 6e6f 7420 6578  t)z. does not ex
-00005c90: 6973 747a 6425 2861 7363 7469 6d65 292d  istzd%(asctime)-
-00005ca0: 3135 7320 5b25 286c 6576 656c 6e61 6d65  15s [%(levelname
-00005cb0: 2935 2e35 735d 205b 2528 7468 7265 6164  )5.5s] [%(thread
-00005cc0: 4e61 6d65 2931 352e 3135 735d 2025 286e  Name)15.15s] %(n
-00005cd0: 616d 6529 7323 2528 6675 6e63 4e61 6d65  ame)s#%(funcName
-00005ce0: 2973 3a25 286c 696e 656e 6f29 7320 2528  )s:%(lineno)s %(
-00005cf0: 6d65 7373 6167 6529 737a 1164 6c67 5472  message)sz.dlgTr
-00005d00: 616e 736c 6174 6f72 2e6c 6f67 5429 01da  anslator.logT)..
-00005d10: 0865 7869 7374 5f6f 6b7a 1543 616e 6e6f  .exist_okz.Canno
-00005d20: 7420 6372 6561 7465 2070 6174 6820 2573  t create path %s
-00005d30: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00005d40: 0001 0000 0057 0000 0073 0800 0000 7400  .....W...s....t.
-00005d50: 8201 6400 5300 722b 0100 0029 01da 114b  ..d.S.r+...)...K
-00005d60: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-00005d70: 2901 da05 5f61 7267 7372 5a00 0000 725a  )..._argsrZ...rZ
-00005d80: 0000 0072 5b00 0000 da07 6861 6e64 6c65  ...r[.....handle
-00005d90: 72e8 0400 0073 0200 0000 0001 7a14 7275  r....s......z.ru
-00005da0: 6e2e 3c6c 6f63 616c 733e 2e68 616e 646c  n.<locals>.handl
-00005db0: 6572 7a1b 5374 6172 7469 6e67 2075 7669  erz.Starting uvi
-00005dc0: 636f 726e 2076 6572 626f 7365 2025 7329  corn verbose %s)
-00005dd0: 04da 0361 7070 72cd 0000 0072 ce00 0000  ...appr....r....
-00005de0: 72d8 0000 0029 30da 0861 7267 7061 7273  r....)0..argpars
-00005df0: 65da 0e41 7267 756d 656e 7450 6172 7365  e..ArgumentParse
-00005e00: 72da 0c61 6464 5f61 7267 756d 656e 7472  r..add_argumentr
-00005e10: 5800 0000 72d4 0000 0072 2000 0000 da0d  X...r....r .....
-00005e20: 6765 7444 6c67 4c6f 6773 4469 72da 0a70  getDlgLogsDir..p
-00005e30: 6172 7365 5f61 7267 7372 2800 0000 722b  arse_argsr(...r+
-00005e40: 0000 0072 7500 0000 7276 0000 0072 d600  ...ru...rv...r..
-00005e50: 0000 da06 6578 6973 7473 7233 0100 0072  ....existsr3...r
-00005e60: 3401 0000 da07 6c6f 6767 696e 67da 0946  4.....logging..F
-00005e70: 6f72 6d61 7474 6572 da04 7469 6d65 da06  ormatter..time..
-00005e80: 676d 7469 6d65 da09 636f 6e76 6572 7465  gmtime..converte
-00005e90: 72da 0d53 7472 6561 6d48 616e 646c 6572  r..StreamHandler
-00005ea0: da03 7379 73da 0673 7464 6f75 74da 0c73  ..sys..stdout..s
-00005eb0: 6574 466f 726d 6174 7465 72da 0472 6f6f  etFormatter..roo
-00005ec0: 74da 0a61 6464 4861 6e64 6c65 72da 0873  t..addHandler..s
-00005ed0: 6574 4c65 7665 6cda 0544 4542 5547 da12  etLevel..DEBUG..
-00005ee0: 6372 6561 7465 4469 7249 664d 6973 7369  createDirIfMissi
-00005ef0: 6e67 72a1 0000 00da 0b46 696c 6548 616e  ngr......FileHan
-00005f00: 646c 6572 da08 6d61 6b65 6469 7273 da07  dler..makedirs..
-00005f10: 4f53 4572 726f 7272 4d00 0000 7249 0000  OSErrorrM...rI..
-00005f20: 0072 6b00 0000 7224 0000 0072 8200 0000  .rk...r$...r....
-00005f30: da06 7369 676e 616c da07 5349 4754 4552  ..signal..SIGTER
-00005f40: 4dda 0653 4947 494e 5472 d800 0000 da07  M..SIGINTr......
-00005f50: 7576 6963 6f72 6eda 0372 756e 7239 0100  uvicorn..runr9..
-00005f60: 0072 cd00 0000 72ce 0000 0029 0ada 015f  .r....r....)..._
-00005f70: da04 6172 6773 da06 7061 7273 6572 da07  ..args..parser..
-00005f80: 6f70 7469 6f6e 73da 0366 6d74 5a0e 7374  options..fmtZ.st
-00005f90: 7265 616d 5f68 616e 646c 6572 7234 0100  ream_handlerr4..
-00005fa0: 00da 076c 6f67 6669 6c65 5a0b 6669 6c65  ...logfileZ.file
-00005fb0: 4861 6e64 6c65 7272 3801 0000 725a 0000  Handlerr8...rZ..
-00005fc0: 0072 5a00 0000 725b 0000 0072 5501 0000  .rZ...r[...rU...
-00005fd0: 8504 0000 73ba 0000 0000 0408 0104 0102  ....s...........
-00005fe0: 0102 0102 0102 0102 0102 0102 f906 0904  ................
-00005ff0: 0102 0102 0102 0102 0102 0102 0102 f906  ................
-00006000: 0904 0102 0102 0102 0102 0102 0102 0102  ................
-00006010: f906 0904 0102 0102 0102 0102 0102 0102  ................
-00006020: 0102 f906 0904 0102 0102 0102 0102 0102  ................
-00006030: 0102 fa06 0804 0102 0102 0102 0102 0102  ................
-00006040: 0102 0106 f906 0a0a 0214 010c 010e 0112  ................
-00006050: 020e 0104 0102 ff04 0408 0108 010c 010a  ................
-00006060: 010c 010e 0108 0206 010a 010e 010a 010a  ................
-00006070: 010c 0202 0114 0110 0114 0606 0106 0108  ................
-00006080: 0208 030e 010e 020e 0104 0102 0004 0004  ................
-00006090: 0004 ff72 5501 0000 da08 5f5f 6d61 696e  ...rU.....__main
-000060a0: 5f5f 298a 723a 0100 0072 e100 0000 724a  __).r:...r....rJ
-000060b0: 0000 0072 4001 0000 7276 0000 0072 4e00  ...r@...rv...rN.
-000060c0: 0000 7251 0100 0072 4601 0000 da09 7468  ..rQ...rF.....th
-000060d0: 7265 6164 696e 6772 4201 0000 72a4 0000  readingrB...r...
-000060e0: 0072 0901 0000 7202 0000 0072 0300 0000  .r....r....r....
-000060f0: da06 7479 7069 6e67 7204 0000 00da 0c75  ..typingr......u
-00006100: 726c 6c69 622e 7061 7273 6572 0500 0000  rllib.parser....
-00006110: 7254 0100 005a 0766 6173 7461 7069 7206  rT...Z.fastapir.
-00006120: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00006130: 0000 720a 0000 0072 0b00 0000 5a11 6661  ..r....r....Z.fa
-00006140: 7374 6170 692e 7265 7370 6f6e 7365 7372  stapi.responsesr
-00006150: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
-00006160: 0000 005a 1366 6173 7461 7069 2e73 7461  ...Z.fastapi.sta
-00006170: 7469 6366 696c 6573 7210 0000 005a 1266  ticfilesr....Z.f
-00006180: 6173 7461 7069 2e74 656d 706c 6174 696e  astapi.templatin
-00006190: 6772 1100 0000 5a0a 6a73 6f6e 7363 6865  gr....Z.jsonsche
-000061a0: 6d61 7212 0000 0072 1300 0000 5a08 7079  mar....r....Z.py
-000061b0: 6461 6e74 6963 7214 0000 00da 0d64 6c67  danticr......dlg
-000061c0: 2e63 6f6e 7374 616e 7473 720b 0100 005a  .constantsr....Z
-000061d0: 1964 6c67 2e64 726f 706d 616b 652e 7067  .dlg.dropmake.pg
-000061e0: 5f67 656e 6572 6174 6f72 7215 0000 0072  _generatorr....r
-000061f0: 1600 0000 da0b 646c 672e 636c 6965 6e74  ......dlg.client
-00006200: 7372 1700 0000 da24 646c 672e 636f 6d6d  sr.....$dlg.comm
-00006210: 6f6e 2e72 6570 726f 6475 6369 6269 6c69  on.reproducibili
-00006220: 7479 2e63 6f6e 7374 616e 7473 7218 0000  ty.constantsr...
-00006230: 0072 1900 0000 721a 0000 00da 2a64 6c67  .r....r.....*dlg
-00006240: 2e63 6f6d 6d6f 6e2e 7265 7072 6f64 7563  .common.reproduc
-00006250: 6962 696c 6974 792e 7265 7072 6f64 7563  ibility.reproduc
-00006260: 6962 696c 6974 7972 1b00 0000 721c 0000  ibilityr....r...
-00006270: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00006280: 7220 0000 005a 1d64 6c67 2e63 6f6d 6d6f  r ...Z.dlg.commo
-00006290: 6e2e 6465 706c 6f79 6d65 6e74 5f6d 6574  n.deployment_met
-000062a0: 686f 6473 7221 0000 005a 1464 6c67 2e63  hodsr!...Z.dlg.c
-000062b0: 6f6d 6d6f 6e2e 6b38 735f 7574 696c 7372  ommon.k8s_utilsr
-000062c0: 2200 0000 5a0f 646c 672e 6472 6f70 6d61  "...Z.dlg.dropma
-000062d0: 6b65 2e6c 6772 2300 0000 5a17 646c 672e  ke.lgr#...Z.dlg.
-000062e0: 6472 6f70 6d61 6b65 2e70 675f 6d61 6e61  dropmake.pg_mana
-000062f0: 6765 7272 2400 0000 5a16 646c 672e 6472  gerr$...Z.dlg.dr
-00006300: 6f70 6d61 6b65 2e73 6368 6564 756c 6572  opmake.scheduler
-00006310: 7225 0000 005a 2164 6c67 2e64 726f 706d  r%...Z!dlg.dropm
-00006320: 616b 652e 7765 622e 7472 616e 736c 6174  ake.web.translat
-00006330: 6f72 5f75 7469 6c73 7226 0000 0072 2700  or_utilsr&...r'.
-00006340: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00006350: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00006360: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00006370: 3100 0000 5a0f 4150 505f 4445 5343 5249  1...Z.APP_DESCRI
-00006380: 5054 494f 4e5a 1141 5050 5f54 4147 535f  PTIONZ.APP_TAGS_
-00006390: 4d45 5441 4441 5441 724f 0000 00da 085f  METADATArO....._
-000063a0: 5f66 696c 655f 5fda 0670 6172 656e 74da  _file__..parent.
-000063b0: 0861 6273 6f6c 7574 655a 0d66 696c 655f  .absoluteZ.file_
-000063c0: 6c6f 6361 7469 6f6e 7278 0000 0072 3900  locationrx...r9.
-000063d0: 0000 7239 0100 00da 056d 6f75 6e74 da09  ..r9.....mount..
-000063e0: 6765 744c 6f67 6765 7272 fd00 0000 724c  getLoggerr....rL
-000063f0: 0000 00da 0953 656d 6170 686f 7265 7250  .....SemaphorerP
-00006400: 0000 005a 0b67 656e 5f70 6774 5f73 656d  ...Z.gen_pgt_sem
-00006410: 724b 0000 0072 b500 0000 da04 706f 7374  rK...r......post
-00006420: 7258 0000 00da 0576 616c 7565 725c 0000  rX.....valuer\..
-00006430: 0072 1a01 0000 7268 0000 0072 6e00 0000  .r....rh...rn...
-00006440: 727b 0000 0072 8100 0000 7283 0000 0072  r{...r....r....r
-00006450: 8600 0000 7287 0000 0072 d400 0000 72aa  ....r....r....r.
-00006460: 0000 0072 b900 0000 72f3 0000 0072 dc00  ...r....r....r..
-00006470: 0000 72f8 0000 0072 fb00 0000 72fc 0000  ..r....r....r...
-00006480: 0072 0201 0000 7208 0100 0072 3200 0000  .r....r....r2...
-00006490: da07 4e4f 5448 494e 4772 1101 0000 da04  ..NOTHINGr......
-000064a0: 626f 6f6c 7216 0100 0072 1f01 0000 7220  boolr....r....r 
-000064b0: 0100 00da 0963 6f6e 7374 616e 7473 da18  .....constants..
-000064c0: 4953 4c41 4e44 5f44 4546 4155 4c54 5f52  ISLAND_DEFAULT_R
-000064d0: 4553 545f 504f 5254 7226 0100 0072 2901  EST_PORTr&...r).
-000064e0: 0000 722a 0100 00da 0468 6561 6472 2c01  ..r*.....headr,.
-000064f0: 0000 7255 0100 00da 0461 7267 7672 5a00  ..rU.....argvrZ.
-00006500: 0000 725a 0000 0072 5a00 0000 725b 0000  ..rZ...rZ...r[..
-00006510: 00da 083c 6d6f 6475 6c65 3e17 0000 0073  ...<module>....s
-00006520: d403 0000 0801 0801 0801 0801 0801 0801  ................
-00006530: 0801 0801 0801 0801 0801 0c01 0c01 0c01  ................
-00006540: 0c02 0801 2001 1806 0c01 0c01 1001 0c02  .... ...........
-00006550: 0801 0801 1001 0c01 1405 1c08 0c01 0c01  ................
-00006560: 0c01 0c01 0c01 0c01 380f 0413 0201 02fe  ........8.......
-00006570: 0405 0201 02fe 04fb 040b 1001 0a02 0201  ................
-00006580: 0201 0201 0201 0801 0602 0201 02fe 04fa  ................
-00006590: 060b 1601 0a02 0a01 0a05 0401 0aff 0405  ................
-000065a0: 0e02 0801 0201 02ff 0403 0efb 0201 0201  ................
-000065b0: 0203 02fb 0e24 0e02 0201 0200 02ff 04ff  .....$..........
-000065c0: 0201 02ff 0e1d 1002 08ff 0201 02ff 0e12  ................
-000065d0: 1003 0201 0200 02ff 04fe 0201 0201 02fe  ................
-000065e0: 0e25 1003 0201 02ff 04fe 0201 0201 02fe  .%..............
-000065f0: 0e14 0e02 0201 02ff 04ff 0201 02ff 0e14  ................
-00006600: 1003 0201 02ff 04fe 0201 0201 02fe 0e14  ................
-00006610: 0e02 0201 02ff 04ff 0201 02ff 0e17 0e03  ................
-00006620: 0201 02ff 0403 0201 0801 02fe 0404 0201  ................
-00006630: 0201 02fe 0404 0201 0200 02ff 0403 0201  ................
-00006640: 0201 02fe 0404 0201 0200 02ff 0403 0201  ................
-00006650: 0201 02fe 04e9 0201 0201 0203 0204 0204  ................
-00006660: 0203 0204 0203 02e9 0e59 1003 0201 02ff  .........Y......
-00006670: 0403 0201 02ff 0403 0201 0801 02fe 0404  ................
-00006680: 0201 0201 02fe 0404 0201 0201 02fe 0404  ................
-00006690: 0201 0200 02ff 0403 0201 0200 02ff 0403  ................
-000066a0: 0201 0201 02fe 0404 0801 0801 0801 0801  ................
-000066b0: 0801 0801 0801 0801 08da 0201 0201 0203  ................
-000066c0: 0203 0204 0204 0204 0203 0203 0204 0a01  ................
-000066d0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0ada  ................
-000066e0: 0e77 1003 0201 02ff 0403 0201 0201 02fe  .w..............
-000066f0: 0404 0201 0200 02ff 0403 0201 0201 02fe  ................
-00006700: 0404 0201 0201 02fe 0404 0201 0201 02fe  ................
-00006710: 04ec 0201 0201 0203 0a04 0a03 0a04 0a04  ................
-00006720: 02ec 0e7f 0004 0e02 0201 02ff 0403 0201  ................
-00006730: 0201 02fe 0404 0201 02ff 0403 0201 0201  ................
-00006740: 02fe 04f5 0201 0203 0204 0203 02f5 0e43  ...............C
-00006750: 0e02 0201 02ff 04ff 0201 02ff 0e29 1011  .............)..
-00006760: 120d 1021 1002 0201 0201 02fe 0404 0201  ...!............
-00006770: 0201 02fe 0404 0201 0200 02ff 0403 0201  ................
-00006780: 0401 0602 0afe 0404 02fa 04f4 0201 0204  ................
-00006790: 0204 0203 02f4 0e27 1002 0201 0201 02fe  .......'........
-000067a0: 0404 0201 0201 02fe 0404 0201 0200 02ff  ................
-000067b0: 0403 0201 0201 02fe 0404 0201 0201 02fe  ................
-000067c0: 04f0 0201 0204 0204 0203 0204 02f0 0e22  ..............."
-000067d0: 1002 0201 0201 02fe 0404 0201 0201 02fe  ................
-000067e0: 0404 0201 0201 02fe 0404 0201 0200 02ff  ................
-000067f0: 0403 0201 0200 02ff 0403 0201 0401 02fe  ................
-00006800: 04ed 0201 0204 0204 0204 0203 0203 02ed  ................
-00006810: 0e29 0401 0200 0200 04ff 0404 0201 0201  .)..............
-00006820: 02fe 0404 0201 0201 02fe 0404 0201 0200  ................
-00006830: 02ff 0403 0201 0201 02fe 0404 0201 0201  ................
-00006840: 02fe 0404 0201 0201 02fe 0404 0201 0200  ................
-00006850: 02ff 0403 0201 0200 02ff 0403 0201 0401  ................
-00006860: 02fe 04e2 0201 0204 0204 0203 0204 0204  ................
-00006870: 0204 0203 0203 02e2 0e36 1002 0201 0201  .........6......
-00006880: 02fe 0404 0201 0200 02ff 0403 0201 0201  ................
-00006890: 02fe 0404 0201 0200 02ff 0403 0201 0201  ................
-000068a0: 02fe 0404 0201 0201 02fe 0404 0201 0601  ................
-000068b0: 02fe 04e9 0201 0204 0203 0204 0203 0204  ................
-000068c0: 0204 02e9 0e36 0802 0201 0201 02fe 0404  .....6..........
-000068d0: 0201 0201 02fe 0404 0af7 0201 0204 0204  ................
-000068e0: 02f7 0e1f 0401 0201 0201 02fd 0405 100e  ................
-000068f0: 0801 0a04 086f 0a01                      .....o..
+00001410: 010e fe1c 0572 5c00 0000 7a24 5468 6520  .....r\...z$The 
+00001420: 6e61 6d65 206f 6620 7468 6520 6c67 2074  name of the lg t
+00001430: 6f20 6c6f 6164 2066 726f 6d20 6669 6c65  o load from file
+00001440: 2902 723f 0000 0072 3300 0000 2901 7240  ).r?...r3...).r@
+00001450: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001460: 0700 0000 0900 0000 4300 0000 73b6 0000  ........C...s...
+00001470: 007c 0064 016b 0873 1474 007c 0083 0164  .|.d.k.s.t.|...d
+00001480: 026b 0272 6474 0174 0283 017d 017a 2874  .k.rdt.t...}.z(t
+00001490: 0374 047c 0183 0183 017d 027c 0264 0317  .t.|.....}.|.d..
+000014a0: 007c 017c 0219 0064 0219 0017 007d 037c  .|.|...d.....}.|
+000014b0: 037d 0057 006e 1e04 0074 056b 0a72 6201  .}.W.n...t.k.rb.
+000014c0: 0001 0001 0064 04a0 0674 07a1 0106 0059  .....d...t.....Y
+000014d0: 0053 0058 0074 0874 027c 0083 0272 a074  .S.X.t.t.|...r.t
+000014e0: 0774 027c 0083 027d 0474 097c 0464 0583  .t.|...}.t.|.d..
+000014f0: 028f 107d 0574 0aa0 0b7c 05a1 017d 0657  ...}.t...|...}.W
+00001500: 0035 0051 0052 0058 0074 0c7c 0683 0153  .5.Q.R.X.t.|...S
+00001510: 0074 0d64 0664 07a0 067c 00a1 0164 088d  .t.d.d...|...d..
+00001520: 0282 0164 0153 0029 097a 3d0a 2020 2020  ...d.S.).z=.    
+00001530: 5265 7475 726e 7320 4a53 4f4e 2072 6570  Returns JSON rep
+00001540: 7265 7365 6e74 6174 696f 6e20 6f66 2073  resentation of s
+00001550: 6176 6564 206c 6f67 6963 616c 2067 7261  aved logical gra
+00001560: 7068 2e0a 2020 2020 4e72 0100 0000 fa01  ph..    Nr......
+00001570: 2f7a 184e 6f74 6869 6e67 2066 6f75 6e64  /z.Nothing found
+00001580: 2069 6e20 6469 7220 7b30 7dda 0172 7243   in dir {0}..rrC
+00001590: 0000 007a 194a 534f 4e20 6772 6170 6820  ...z.JSON graph 
+000015a0: 7b30 7d20 6e6f 7420 666f 756e 640a 7244  {0} not found.rD
+000015b0: 0000 0029 0eda 036c 656e 7227 0000 0072  ...)...lenr'...r
+000015c0: 4900 0000 da04 6e65 7874 da04 6974 6572  I.....next..iter
+000015d0: da0d 5374 6f70 4974 6572 6174 696f 6e72  ..StopIterationr
+000015e0: 5700 0000 7228 0000 0072 2900 0000 7253  W...r(...r)...rS
+000015f0: 0000 0072 4a00 0000 da04 6c6f 6164 720e  ...rJ.....loadr.
+00001600: 0000 0072 0a00 0000 2907 7240 0000 005a  ...r....).r@...Z
+00001610: 0761 6c6c 5f6c 6773 da09 6669 7273 745f  .all_lgs..first_
+00001620: 6469 725a 0866 6972 7374 5f6c 67da 036c  dirZ.first_lg..l
+00001630: 6770 da01 66da 0464 6174 6172 5a00 0000  gp..f..datarZ...
+00001640: 725a 0000 0072 5b00 0000 da0f 6a73 6f6e  rZ...r[.....json
+00001650: 626f 6479 5f67 6574 5f6c 67b1 0000 0073  body_get_lg....s
+00001660: 2200 0000 0009 1401 0801 0201 0c01 1401  "...............
+00001670: 0801 0e01 1001 0a02 0a01 0c01 1401 0802  ................
+00001680: 0201 0201 08fe 7268 0000 007a 0d2f 7067  ......rh...z./pg
+00001690: 745f 6a73 6f6e 626f 6479 2902 da0e 7265  t_jsonbody)...re
+000016a0: 7370 6f6e 7365 5f63 6c61 7373 723e 0000  sponse_classr>..
+000016b0: 007a 2554 6865 206e 616d 6520 6f66 2074  .z%The name of t
+000016c0: 6865 2070 6774 2074 6f20 6c6f 6164 2066  he pgt to load f
+000016d0: 726f 6d20 6669 6c65 2901 da08 7067 745f  rom file)...pgt_
+000016e0: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
+000016f0: 0004 0000 0009 0000 0043 0000 0073 5000  .........C...sP.
+00001700: 0000 7400 7401 7c00 8302 723a 7402 7401  ..t.t.|...r:t.t.
+00001710: 7c00 8302 7d01 7403 7c01 6401 8302 8f0e  |...}.t.|.d.....
+00001720: 7d02 7c02 a004 a100 7d03 5700 3500 5100  }.|.....}.W.5.Q.
+00001730: 5200 5800 7405 7c03 8301 5300 7406 6402  R.X.t.|...S.t.d.
+00001740: 6403 a007 7c00 a101 6404 8d02 8201 6405  d...|...d.....d.
+00001750: 5300 2906 7a41 0a20 2020 2052 6574 7572  S.).zA.    Retur
+00001760: 6e20 4a53 4f4e 2072 6570 7265 7365 6e74  n JSON represent
+00001770: 6174 696f 6e20 6f66 2061 2070 6879 7369  ation of a physi
+00001780: 6361 6c20 6772 6170 6820 7465 6d70 6c61  cal graph templa
+00001790: 7465 0a20 2020 2072 5e00 0000 7243 0000  te.    r^...rC..
+000017a0: 007a 184a 534f 4e20 6772 6170 6820 7b30  .z.JSON graph {0
+000017b0: 7d20 6e6f 7420 666f 756e 6472 4400 0000  } not foundrD...
+000017c0: 4e29 0872 2a00 0000 da07 7067 745f 6469  N).r*.....pgt_di
+000017d0: 7272 2b00 0000 7253 0000 00da 0472 6561  rr+...rS.....rea
+000017e0: 6472 0e00 0000 720a 0000 0072 5700 0000  dr....r....rW...
+000017f0: 2904 726a 0000 00da 0370 6774 7266 0000  ).rj.....pgtrf..
+00001800: 0072 6700 0000 725a 0000 0072 5a00 0000  .rg...rZ...rZ...
+00001810: 725b 0000 00da 106a 736f 6e62 6f64 795f  r[.....jsonbody_
+00001820: 6765 745f 7067 74cf 0000 0073 1200 0000  get_pgt....s....
+00001830: 0007 0a02 0a01 0c01 1201 0802 0201 0200  ................
+00001840: 08ff 726e 0000 007a 0a2f 7067 5f76 6965  ..rn...z./pg_vie
+00001850: 7765 727a 2954 6865 2073 7472 696e 6720  werz)The string 
+00001860: 6f66 2074 6865 2074 7970 6520 6f66 2076  of the type of v
+00001870: 6965 7720 746f 2070 726f 7669 6465 2902  iew to provide).
+00001880: da07 7265 7175 6573 74da 0d70 6774 5f76  ..request..pgt_v
+00001890: 6965 775f 6e61 6d65 6302 0000 0000 0000  iew_namec.......
+000018a0: 0000 0000 0005 0000 0009 0000 0043 0000  .............C..
+000018b0: 0073 9a00 0000 7c01 6401 6b08 7314 7400  .s....|.d.k.s.t.
+000018c0: 7c01 8301 6402 6b02 725c 7401 7402 8301  |...d.k.r\t.t...
+000018d0: 7d02 7a26 7403 7404 7c02 8301 8301 7d03  }.z&t.t.|.....}.
+000018e0: 7c03 7405 6a06 1700 7c02 7c03 1900 6402  |.t.j...|.|...d.
+000018f0: 1900 1700 7d01 5700 6e18 0400 7407 6b0a  ....}.W.n...t.k.
+00001900: 725a 0100 0100 0100 6401 7d01 5900 6e02  rZ......d.}.Y.n.
+00001910: 5800 7408 7402 7c01 8302 7282 7409 a00a  X.t.t.|...r.t...
+00001920: 6403 7c00 7c01 6401 6404 6401 6405 9c05  d.|.|.d.d.d.d...
+00001930: a102 7d04 7c04 5300 740b 6406 6407 a00c  ..}.|.S.t.d.d...
+00001940: 7c01 7402 a102 6408 8d02 8201 6401 5300  |.t...d.....d.S.
+00001950: 2909 7a29 0a20 2020 204c 6f61 6473 2074  ).z).    Loads t
+00001960: 6865 2070 6879 7369 6361 6c20 6772 6170  he physical grap
+00001970: 6820 7669 6577 6572 0a20 2020 204e 7201  h viewer.    Nr.
+00001980: 0000 00fa 0e70 675f 7669 6577 6572 2e68  .....pg_viewer.h
+00001990: 746d 6cfa 1750 6879 7369 6361 6c20 4772  tml..Physical Gr
+000019a0: 6170 6820 5465 6d70 6c61 7465 a905 726f  aph Template..ro
+000019b0: 0000 00da 1270 6774 5f76 6965 775f 6a73  .....pgt_view_js
+000019c0: 6f6e 5f6e 616d 655a 0e70 6172 7469 7469  on_nameZ.partiti
+000019d0: 6f6e 5f69 6e66 6f72 3700 0000 da05 6572  on_infor7.....er
+000019e0: 726f 7272 4300 0000 7a2e 5068 7973 6963  rorrC...z.Physic
+000019f0: 616c 2067 7261 7068 2074 656d 706c 6174  al graph templat
+00001a00: 6520 7669 6577 207b 307d 206e 6f74 2066  e view {0} not f
+00001a10: 6f75 6e64 207b 317d 7244 0000 0029 0d72  ound {1}rD...).r
+00001a20: 5f00 0000 722c 0000 0072 6b00 0000 7260  _...r,...rk...r`
+00001a30: 0000 0072 6100 0000 da02 6f73 da03 7365  ...ra.....os..se
+00001a40: 7072 6200 0000 722a 0000 00da 0974 656d  prb...r*.....tem
+00001a50: 706c 6174 6573 da10 5465 6d70 6c61 7465  plates..Template
+00001a60: 5265 7370 6f6e 7365 720a 0000 0072 5700  Responser....rW.
+00001a70: 0000 2905 726f 0000 0072 7000 0000 5a08  ..).ro...rp...Z.
+00001a80: 616c 6c5f 7067 7473 7264 0000 00da 0374  all_pgtsrd.....t
+00001a90: 706c 725a 0000 0072 5a00 0000 725b 0000  plrZ...rZ...r[..
+00001aa0: 00da 0e6c 6f61 645f 7067 5f76 6965 7765  ...load_pg_viewe
+00001ab0: 72e2 0000 0073 3200 0000 000a 1401 0801  r....s2.........
+00001ac0: 0201 0c01 1a01 0e01 0a01 0a01 0401 0202  ................
+00001ad0: 0201 0201 0201 0201 02fb 04fe 040a 0402  ................
+00001ae0: 0201 0201 0401 0200 02ff 02fe 727b 0000  ............r{..
+00001af0: 007a 112f 7368 6f77 5f67 616e 7474 5f63  .z./show_gantt_c
+00001b00: 6861 7274 7a32 5468 6520 7067 745f 6964  hartz2The pgt_id
+00001b10: 2075 7365 6420 746f 2069 6e74 6572 6e61   used to interna
+00001b20: 6c6c 7920 7265 6665 7265 6e63 6520 7468  lly reference th
+00001b30: 6973 2067 7261 7068 2902 726f 0000 00da  is graph).ro....
+00001b40: 0670 6774 5f69 6463 0200 0000 0000 0000  .pgt_idc........
+00001b50: 0000 0000 0300 0000 0700 0000 4300 0000  ............C...
+00001b60: 7318 0000 0074 00a0 0164 017c 007c 0164  s....t...d.|.|.d
+00001b70: 0264 039c 03a1 027d 027c 0253 0029 047a  .d.....}.|.S.).z
+00001b80: 2b0a 2020 2020 496e 7465 7266 6163 6520  +.    Interface 
+00001b90: 746f 2073 686f 7720 7468 6520 6761 6e74  to show the gant
+00001ba0: 7420 6368 6172 740a 2020 2020 fa0f 6d61  t chart.    ..ma
+00001bb0: 7472 6978 5f76 6973 2e68 746d 6c5a 0f70  trix_vis.htmlZ.p
+00001bc0: 6774 5f67 616e 7474 5f63 6861 7274 a903  gt_gantt_chart..
+00001bd0: 726f 0000 0072 7400 0000 5a0a 7669 735f  ro...rt...Z.vis_
+00001be0: 6163 7469 6f6e a902 7278 0000 0072 7900  action..rx...ry.
+00001bf0: 0000 a903 726f 0000 0072 7c00 0000 727a  ....ro...r|...rz
+00001c00: 0000 0072 5a00 0000 725a 0000 0072 5b00  ...rZ...rZ...r[.
+00001c10: 0000 da10 7368 6f77 5f67 616e 7474 5f63  ....show_gantt_c
+00001c20: 6861 7274 0801 0000 7310 0000 0000 0a04  hart....s.......
+00001c30: 0102 0202 0102 0102 fd04 fe04 0872 8100  .............r..
+00001c40: 0000 7a10 2f70 6774 5f67 616e 7474 5f63  ..z./pgt_gantt_c
+00001c50: 6861 7274 2901 727c 0000 0063 0100 0000  hart).r|...c....
+00001c60: 0000 0000 0000 0000 0300 0000 0a00 0000  ................
+00001c70: 4300 0000 734c 0000 007a 1074 00a0 017c  C...sL...z.t...|
+00001c80: 00a1 017d 017c 0157 0053 0004 0074 026b  ...}.|.W.S...t.k
+00001c90: 0a72 4601 007d 0201 007a 1874 0364 0164  .rF..}...z.t.d.d
+00001ca0: 02a0 047c 007c 02a1 0264 038d 0282 0157  ...|.|...d.....W
+00001cb0: 0035 0064 047d 027e 0258 0059 006e 0258  .5.d.}.~.X.Y.n.X
+00001cc0: 0064 0453 0029 057a 4a0a 2020 2020 496e  .d.S.).zJ.    In
+00001cd0: 7465 7266 6163 6520 746f 2072 6574 7269  terface to retri
+00001ce0: 6576 6520 6120 4761 6e74 7420 4368 6172  eve a Gantt Char
+00001cf0: 7420 6d61 7472 6978 2061 7373 6f63 6961  t matrix associa
+00001d00: 7465 6420 7769 7468 2061 2050 4754 0a20  ted with a PGT. 
+00001d10: 2020 2072 4800 0000 7a2b 4661 696c 6564     rH...z+Failed
+00001d20: 2074 6f20 6765 6e65 7261 7465 2047 616e   to generate Gan
+00001d30: 7474 2063 6861 7274 2066 6f72 207b 307d  tt chart for {0}
+00001d40: 3a20 7b31 7d72 4400 0000 4e29 05da 0670  : {1}rD...N)...p
+00001d50: 675f 6d67 72da 0f67 6574 5f67 616e 7474  g_mgr..get_gantt
+00001d60: 5f63 6861 7274 7223 0000 0072 0a00 0000  _chartr#...r....
+00001d70: 7257 0000 0029 0372 7c00 0000 da03 7265  rW...).r|.....re
+00001d80: 74da 0267 6572 5a00 0000 725a 0000 0072  t..gerZ...rZ...r
+00001d90: 5b00 0000 7283 0000 001d 0100 0073 1000  [...r........s..
+00001da0: 0000 0009 0201 0a01 0601 1001 0201 0201  ................
+00001db0: 0afe 7283 0000 007a 122f 7368 6f77 5f73  ..r....z./show_s
+00001dc0: 6368 6564 756c 655f 6d61 7463 0200 0000  chedule_matc....
+00001dd0: 0000 0000 0000 0000 0300 0000 0700 0000  ................
+00001de0: 4300 0000 7318 0000 0074 00a0 0164 017c  C...s....t...d.|
+00001df0: 007c 0164 0264 039c 03a1 027d 027c 0253  .|.d.d.....}.|.S
+00001e00: 0029 047a 2c0a 2020 2020 496e 7465 7266  .).z,.    Interf
+00001e10: 6163 6520 746f 2073 686f 7720 7468 6520  ace to show the 
+00001e20: 7363 6865 6475 6c65 206d 6174 0a20 2020  schedule mat.   
+00001e30: 2072 7d00 0000 5a10 7067 745f 7363 6865   r}...Z.pgt_sche
+00001e40: 6475 6c65 5f6d 6174 727e 0000 0072 7f00  dule_matr~...r..
+00001e50: 0000 7280 0000 0072 5a00 0000 725a 0000  ..r....rZ...rZ..
+00001e60: 0072 5b00 0000 da14 7368 6f77 5f73 6368  .r[.....show_sch
+00001e70: 6564 756c 655f 6d61 7472 6978 3001 0000  edule_matrix0...
+00001e80: 7310 0000 0000 0a04 0102 0202 0102 0102  s...............
+00001e90: fd04 fe04 0872 8600 0000 7a16 2f67 6574  .....r....z./get
+00001ea0: 5f73 6368 6564 756c 655f 6d61 7472 6963  _schedule_matric
+00001eb0: 6573 6301 0000 0000 0000 0000 0000 0003  esc.............
+00001ec0: 0000 000a 0000 0043 0000 0073 4c00 0000  .......C...sL...
+00001ed0: 7a10 7400 a001 7c00 a101 7d01 7c01 5700  z.t...|...}.|.W.
+00001ee0: 5300 0400 7402 6b0a 7246 0100 7d02 0100  S...t.k.rF..}...
+00001ef0: 7a18 7403 6401 6402 a004 7c00 7c02 a102  z.t.d.d...|.|...
+00001f00: 6403 8d02 8201 5700 3500 6404 7d02 7e02  d.....W.5.d.}.~.
+00001f10: 5800 5900 6e02 5800 6404 5300 2905 7a47  X.Y.n.X.d.S.).zG
+00001f20: 0a20 2020 2049 6e74 6572 6661 6365 2074  .    Interface t
+00001f30: 6f20 7265 7475 726e 2061 6c6c 2073 6368  o return all sch
+00001f40: 6564 756c 6520 6d61 7472 6963 6573 2066  edule matrices f
+00001f50: 6f72 2061 2073 696e 676c 6520 7067 745f  or a single pgt_
+00001f60: 6964 0a20 2020 2072 4800 0000 7a2c 4661  id.    rH...z,Fa
+00001f70: 696c 6564 2074 6f20 6765 7420 7363 6865  iled to get sche
+00001f80: 6475 6c65 206d 6174 7269 6365 7320 666f  dule matrices fo
+00001f90: 7220 7b30 7d3a 207b 317d 7244 0000 004e  r {0}: {1}rD...N
+00001fa0: 2905 7282 0000 00da 1567 6574 5f73 6368  ).r......get_sch
+00001fb0: 6564 756c 655f 6d61 7472 6963 6573 7256  edule_matricesrV
+00001fc0: 0000 0072 0a00 0000 7257 0000 0029 0372  ...r....rW...).r
+00001fd0: 7c00 0000 7284 0000 0072 5900 0000 725a  |...r....rY...rZ
+00001fe0: 0000 0072 5a00 0000 725b 0000 0072 8700  ...rZ...r[...r..
+00001ff0: 0000 4501 0000 7310 0000 0000 0902 010a  ..E...s.........
+00002000: 0106 0110 0102 0102 010a fe72 8700 0000  ...........r....
+00002010: 7a08 2f67 656e 5f70 6774 7a3d 4966 2070  z./gen_pgtz=If p
+00002020: 7265 7365 6e74 2c20 7472 616e 736c 6174  resent, translat
+00002030: 6f72 2077 696c 6c20 6174 7465 6d70 7420  or will attempt 
+00002040: 746f 206c 6f61 6420 7468 6973 206c 6720  to load this lg 
+00002050: 6672 6f6d 2066 696c 657a 6b52 6570 726f  from filezkRepro
+00002060: 6475 6369 6269 6c69 7479 206d 6f64 6520  ducibility mode 
+00002070: 7365 7474 696e 6720 6c65 7665 6c20 6f66  setting level of
+00002080: 2070 726f 7665 6e61 6e63 6520 7472 6163   provenance trac
+00002090: 6b69 6e67 2e20 5265 6665 7220 746f 206d  king. Refer to m
+000020a0: 6169 6e20 646f 6375 6d65 6e74 6174 696f  ain documentatio
+000020b0: 6e20 666f 7220 6d6f 7265 2069 6e66 6f72  n for more infor
+000020c0: 6d61 7469 6f6e da05 6661 6c73 657a 2c49  mation..falsez,I
+000020d0: 6620 2774 7275 6527 2c20 7769 6c6c 2072  f 'true', will r
+000020e0: 6570 6c61 6365 2061 6c6c 2061 7070 7320  eplace all apps 
+000020f0: 7769 7468 2073 6c65 6570 737a 2a54 6865  with sleepsz*The
+00002100: 206e 756d 6265 7220 6f66 2064 6174 6120   number of data 
+00002110: 7061 7274 6974 696f 6e73 2069 6e20 7468  partitions in th
+00002120: 6520 6772 6170 68da 056d 6574 6973 7a36  e graph..metisz6
+00002130: 5468 6520 7363 6865 6475 6c69 6e67 2061  The scheduling a
+00002140: 6c67 6f72 6974 686d 2075 7365 6420 7768  lgorithm used wh
+00002150: 656e 2075 6e72 6f6c 6c69 6e67 2074 6865  en unrolling the
+00002160: 2067 7261 7068 7a27 5468 6520 6e75 6d62   graphz'The numb
+00002170: 6572 206f 6620 6461 7461 2d69 736c 616e  er of data-islan
+00002180: 6473 2074 6f20 7061 7274 6974 696f 6e5a  ds to partitionZ
+00002190: 0950 6172 7469 7469 6f6e 7a2e 5468 6520  .Partitionz.The 
+000021a0: 6c61 6265 6c20 7072 6566 6978 6564 2074  label prefixed t
+000021b0: 6f20 6561 6368 2067 656e 6572 6174 6564  o each generated
+000021c0: 2070 6172 7469 7469 6f6e 2908 726f 0000   partition).ro..
+000021d0: 0072 4000 0000 7242 0000 00da 0474 6573  .r@...rB.....tes
+000021e0: 74da 076e 756d 5f70 6172 da04 616c 676f  t..num_par..algo
+000021f0: da0b 6e75 6d5f 6973 6c61 6e64 73da 0970  ..num_islands..p
+00002200: 6172 5f6c 6162 656c 6308 0000 0000 0000  ar_labelc.......
+00002210: 0000 0000 0011 0000 000a 0000 0043 0000  .............C..
+00002220: 0073 7401 0000 7400 7401 7c01 8302 731c  .st...t.t.|...s.
+00002230: 7402 6401 6402 a003 7c01 a101 6403 8d02  t.d.d...|...d...
+00002240: 8201 7a90 7404 7405 7401 7c01 8302 7c02  ..z.t.t.t.|...|.
+00002250: 8302 7d08 7c03 a006 a100 6404 6b02 7d03  ..}.|.....d.k.}.
+00002260: 7407 7c08 7c03 7c05 7c04 7c06 7c07 7c00  t.|.|.|.|.|.|.|.
+00002270: 6a08 a009 a100 8307 7d09 6405 7d0a 740a  j.......}.d.}.t.
+00002280: a00b 7c09 7c01 a102 7d0b 6406 a00c 6407  ..|.|...}.d...d.
+00002290: 6408 8400 7c09 a00d a100 a009 a100 4400  d...|.........D.
+000022a0: 8301 a101 7d0c 740e a00f 6409 7c00 7c0b  ....}.t...d.|.|.
+000022b0: 7c0c 640a 7c0a 6405 6b02 729a 640b 6e02  |.d.|.d.k.r.d.n.
+000022c0: 640c 1600 6400 640d 9c05 a102 7d0d 7c0d  d...d.d.....}.|.
+000022d0: 5700 5300 0400 7410 6b0a 72f0 0100 7d0e  W.S...t.k.r...}.
+000022e0: 0100 7a26 7411 a012 640e a101 0100 7402  ..z&t...d.....t.
+000022f0: 640f 6410 a003 7413 7c0e 8301 7c01 a102  d.d...t.|...|...
+00002300: 6403 8d02 8201 5700 3500 6400 7d0e 7e0e  d.....W.5.d.}.~.
+00002310: 5800 5900 6e80 0400 7414 6b0a 9001 7234  X.Y.n...t.k...r4
+00002320: 0100 7d0f 0100 7a26 7411 a012 6411 a101  ..}...z&t...d...
+00002330: 0100 7402 640f 6412 a003 7413 7c0f 8301  ..t.d.d...t.|...
+00002340: 7c01 a102 6403 8d02 8201 5700 3500 6400  |...d.....W.5.d.
+00002350: 7d0f 7e0f 5800 5900 6e3c 0400 7415 6b0a  }.~.X.Y.n<..t.k.
+00002360: 9001 726e 0100 0100 0100 7411 a012 6413  ..rn......t...d.
+00002370: a101 0100 7416 a017 a100 7d10 7402 640f  ....t.....}.t.d.
+00002380: 6414 a003 7c10 7c01 a102 6403 8d02 8201  d...|.|...d.....
+00002390: 5900 6e02 5800 6400 5300 2915 4e72 4300  Y.n.X.d.S.).NrC.
+000023a0: 0000 7a1d 4c6f 6769 6361 6c20 6772 6170  ..z.Logical grap
+000023b0: 6820 277b 307d 2720 6e6f 7420 666f 756e  h '{0}' not foun
+000023c0: 6472 4400 0000 da04 7472 7565 7201 0000  drD.....truer...
+000023d0: 00fa 0320 2d20 6301 0000 0000 0000 0000  ... - c.........
+000023e0: 0000 0003 0000 0006 0000 0053 0000 0073  ...........S...s
+000023f0: 1c00 0000 6700 7c00 5d14 5c02 7d01 7d02  ....g.|.].\.}.}.
+00002400: 6400 a000 7c01 7c02 a102 9102 7104 5300  d...|.|.....q.S.
+00002410: a901 7a07 7b30 7d3a 7b31 7da9 0172 5700  ..z.{0}:{1}..rW.
+00002420: 0000 a903 da02 2e30 da01 6bda 0176 725a  .......0..k..vrZ
+00002430: 0000 0072 5a00 0000 725b 0000 00da 0a3c  ...rZ...r[.....<
+00002440: 6c69 7374 636f 6d70 3e8e 0100 0073 0400  listcomp>....s..
+00002450: 0000 0600 0600 7a1b 6765 6e5f 7067 742e  ......z.gen_pgt.
+00002460: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00002470: 6d70 3e72 7100 0000 fa19 5068 7973 6963  mp>rq.....Physic
+00002480: 616c 2047 7261 7068 2054 656d 706c 6174  al Graph Templat
+00002490: 6525 73da 00da 0c50 6172 7469 7469 6f6e  e%s....Partition
+000024a0: 696e 6772 7300 0000 7a0f 4772 6170 6820  ingrs...z.Graph 
+000024b0: 4578 6365 7074 696f 6e72 4800 0000 fa1e  ExceptionrH.....
+000024c0: 496e 7661 6c69 6420 4c6f 6769 6361 6c20  Invalid Logical 
+000024d0: 4772 6170 6820 7b31 7d3a 207b 307d 7a12  Graph {1}: {0}z.
+000024e0: 5363 6865 6475 6c65 2045 7863 6570 7469  Schedule Excepti
+000024f0: 6f6e fa23 4772 6170 6820 7363 6865 6475  on.#Graph schedu
+00002500: 6c69 6e67 2065 7863 6570 7469 6f6e 207b  ling exception {
+00002510: 317d 3a20 7b30 7d7a 1b50 6172 7469 7469  1}: {0}z.Partiti
+00002520: 6f6e 202f 204f 7468 6572 2065 7863 6570  on / Other excep
+00002530: 7469 6f6e fa22 4772 6170 6820 7061 7274  tion."Graph part
+00002540: 6974 696f 6e20 6578 6365 7074 696f 6e20  ition exception 
+00002550: 7b31 7d3a 207b 307d 2918 7229 0000 0072  {1}: {0}).r)...r
+00002560: 4900 0000 720a 0000 0072 5700 0000 722d  I...r....rW...r-
+00002570: 0000 0072 2800 0000 da05 6c6f 7765 7272  ...r(.....lowerr
+00002580: 2e00 0000 5a0c 7175 6572 795f 7061 7261  ....Z.query_para
+00002590: 6d73 da05 6974 656d 7372 8200 0000 da07  ms..itemsr......
+000025a0: 6164 645f 7067 74da 046a 6f69 6eda 0672  add_pgt..join..r
+000025b0: 6573 756c 7472 7800 0000 7279 0000 0072  esultrx...ry...r
+000025c0: 2300 0000 724c 0000 00da 0469 6e66 6f72  #...rL.....infor
+000025d0: 5800 0000 7225 0000 0072 5600 0000 da09  X...r%...rV.....
+000025e0: 7472 6163 6562 6163 6bda 0a66 6f72 6d61  traceback..forma
+000025f0: 745f 6578 6329 1172 6f00 0000 7240 0000  t_exc).ro...r@..
+00002600: 0072 4200 0000 728a 0000 0072 8b00 0000  .rB...r....r....
+00002610: 728c 0000 0072 8d00 0000 728e 0000 005a  r....r....r....Z
+00002620: 036c 6774 726d 0000 00da 0e6e 756d 5f70  .lgtrm.....num_p
+00002630: 6172 7469 7469 6f6e 7372 7c00 0000 da09  artitionsr|.....
+00002640: 7061 7274 5f69 6e66 6f72 7a00 0000 7285  part_inforz...r.
+00002650: 0000 00da 0273 65da 0974 7261 6365 5f6d  .....se..trace_m
+00002660: 7367 725a 0000 0072 5a00 0000 725b 0000  sgrZ...rZ...r[..
+00002670: 00da 0767 656e 5f70 6774 5b01 0000 736a  ...gen_pgt[...sj
+00002680: 0000 0000 1d0a 0102 0102 0108 fe06 0402  ................
+00002690: 0110 010c 0102 0102 0102 0102 0102 0102  ................
+000026a0: 0102 0108 f904 0904 020c 0204 0114 ff04  ................
+000026b0: 0304 0102 0202 0102 0102 0102 010e ff02  ................
+000026c0: 0202 fa04 fe04 0b06 0110 010a 0102 0102  ................
+000026d0: 010e fe16 0412 010a 0102 0102 010e fe16  ................
+000026e0: 0410 010a 0108 0102 0102 010a fe72 aa00  .............r..
+000026f0: 0000 7a2c 5468 6520 6772 6170 6820 6461  ..z,The graph da
+00002700: 7461 2075 7365 6420 6173 2074 6865 2067  ta used as the g
+00002710: 7261 7068 2069 6620 7375 7070 6c69 6564  raph if supplied
+00002720: 2912 726f 0000 0072 4000 0000 da09 6a73  ).ro...r@.....js
+00002730: 6f6e 5f64 6174 6172 4200 0000 728a 0000  on_datarB...r...
+00002740: 0072 8c00 0000 728b 0000 0072 8d00 0000  .r....r....r....
+00002750: 728e 0000 00da 086d 696e 5f67 6f61 6cda  r......min_goal.
+00002760: 0570 7479 7065 da0c 6d61 785f 6c6f 6164  .ptype..max_load
+00002770: 5f69 6d62 da07 6d61 785f 6370 75da 0b74  _imb..max_cpu..t
+00002780: 696d 655f 6772 6565 6479 da08 6465 6164  ime_greedy..dead
+00002790: 6c69 6e65 da04 746f 706b da0a 7377 6172  line..topk..swar
+000027a0: 6d5f 7369 7a65 da07 6d61 785f 6d65 6d63  m_size..max_memc
+000027b0: 1200 0000 0000 0000 0000 0000 1d00 0000  ................
+000027c0: 0a00 0000 c300 0000 73b8 0100 007c 04a0  ........s....|..
+000027d0: 00a1 0064 016b 027d 047a e274 01a0 027c  ...d.k.}.z.t...|
+000027e0: 02a1 017d 127a 0e74 037c 1274 0483 0201  ...}.z.t.|.t....
+000027f0: 0057 006e 3c04 0074 056b 0a72 6201 007d  .W.n<..t.k.rb..}
+00002800: 1301 007a 1e64 02a0 0674 077c 1383 017c  ...z.d...t.|...|
+00002810: 01a1 027d 1474 08a0 097c 14a1 0101 0057  ...}.t...|.....W
+00002820: 0035 0064 037d 137e 1358 0059 006e 0258  .5.d.}.~.X.Y.n.X
+00002830: 0074 0a7c 127c 0383 027d 1274 0b7c 097c  .t.|.|...}.t.|.|
+00002840: 0a7c 0b7c 0c7c 0d7c 0e7c 0f7c 107c 1183  .|.|.|.|.|.|.|..
+00002850: 097d 1574 0c7c 127c 047c 057c 067c 077c  .}.t.|.|.|.|.|.|
+00002860: 087c 1583 077d 1674 0da0 0e7c 167c 01a1  .|...}.t...|.|..
+00002870: 027d 1764 04a0 0f64 0564 0684 007c 16a0  .}.d...d.d...|..
+00002880: 10a1 00a0 11a1 0044 0083 01a1 017d 1874  .......D.....}.t
+00002890: 12a0 1364 077c 007c 177c 1864 087c 0664  ...d.|.|.|.d.|.d
+000028a0: 096b 0272 dc64 0a6e 0264 0b16 0064 0364  .k.r.d.n.d...d.d
+000028b0: 0c9c 05a1 027d 197c 1957 0053 0004 0074  .....}.|.W.S...t
+000028c0: 146b 0a90 0172 3401 007d 1a01 007a 2674  .k...r4..}...z&t
+000028d0: 08a0 1564 0da1 0101 0074 1664 0e64 0fa0  ...d.....t.d.d..
+000028e0: 0674 077c 1a83 017c 01a1 0264 108d 0282  .t.|...|...d....
+000028f0: 0157 0035 0064 037d 1a7e 1a58 0059 006e  .W.5.d.}.~.X.Y.n
+00002900: 8004 0074 176b 0a90 0172 7801 007d 1b01  ...t.k...rx..}..
+00002910: 007a 2674 08a0 1564 11a1 0101 0074 1664  .z&t...d.....t.d
+00002920: 0e64 12a0 0674 077c 1b83 017c 01a1 0264  .d...t.|...|...d
+00002930: 108d 0282 0157 0035 0064 037d 1b7e 1b58  .....W.5.d.}.~.X
+00002940: 0059 006e 3c04 0074 186b 0a90 0172 b201  .Y.n<..t.k...r..
+00002950: 0001 0001 0074 08a0 1564 13a1 0101 0074  .....t...d.....t
+00002960: 19a0 1aa1 007d 1c74 1664 0e64 14a0 067c  .....}.t.d.d...|
+00002970: 1c7c 01a1 0264 108d 0282 0159 006e 0258  .|...d.....Y.n.X
+00002980: 0064 0353 0029 157a ee0a 2020 2020 5472  .d.S.).z..    Tr
+00002990: 616e 736c 6174 696e 6720 4c6f 6769 6361  anslating Logica
+000029a0: 6c20 4772 6170 6873 2074 6f20 5068 7973  l Graphs to Phys
+000029b0: 6963 616c 2047 7261 7068 732e 0a20 2020  ical Graphs..   
+000029c0: 2044 6966 6665 7273 2066 726f 6d20 6765   Differs from ge
+000029d0: 745f 7067 7420 6162 6f76 6520 6279 2074  t_pgt above by t
+000029e0: 6865 2066 6163 7420 7468 6174 2074 6865  he fact that the
+000029f0: 206c 6f67 6963 616c 2067 7261 7068 2064   logical graph d
+00002a00: 6174 6120 6973 2050 4f53 5465 640a 2020  ata is POSTed.  
+00002a10: 2020 746f 2074 6869 7320 726f 7574 6520    to this route 
+00002a20: 696e 2061 2048 5454 5020 666f 726d 2c20  in a HTTP form, 
+00002a30: 7768 6572 6561 7320 6765 6e5f 7067 7420  whereas gen_pgt 
+00002a40: 6c6f 6164 7320 7468 6520 6c6f 6769 6361  loads the logica
+00002a50: 6c20 6772 6170 6820 6461 7461 0a20 2020  l graph data.   
+00002a60: 2066 726f 6d20 6120 6c6f 6361 6c20 6669   from a local fi
+00002a70: 6c65 0a20 2020 2072 8f00 0000 7a19 5661  le.    r....z.Va
+00002a80: 6c69 6461 7469 6f6e 2045 7272 6f72 207b  lidation Error {
+00002a90: 317d 3a20 7b30 7d4e 7290 0000 0063 0100  1}: {0}Nr....c..
+00002aa0: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00002ab0: 0000 5300 0000 731c 0000 0067 007c 005d  ..S...s....g.|.]
+00002ac0: 145c 027d 017d 0264 00a0 007c 017c 02a1  .\.}.}.d...|.|..
+00002ad0: 0291 0271 0453 0072 9100 0000 7292 0000  ...q.S.r....r...
+00002ae0: 0072 9300 0000 725a 0000 0072 5a00 0000  .r....rZ...rZ...
+00002af0: 725b 0000 0072 9700 0000 0002 0000 7304  r[...r........s.
+00002b00: 0000 0006 0006 007a 2067 656e 5f70 6774  .......z gen_pgt
+00002b10: 5f70 6f73 742e 3c6c 6f63 616c 733e 2e3c  _post.<locals>.<
+00002b20: 6c69 7374 636f 6d70 3e72 7100 0000 7298  listcomp>rq...r.
+00002b30: 0000 0072 0100 0000 7299 0000 0072 9a00  ...r....r....r..
+00002b40: 0000 7273 0000 007a 0f47 5241 5048 2045  ..rs...z.GRAPH E
+00002b50: 5843 4550 5449 4f4e 7248 0000 0072 9b00  XCEPTIONrH...r..
+00002b60: 0000 7244 0000 007a 1253 4348 4544 554c  ..rD...z.SCHEDUL
+00002b70: 4520 4558 4345 5054 494f 4e72 9c00 0000  E EXCEPTIONr....
+00002b80: 7a0f 4f54 4845 5220 4558 4345 5054 494f  z.OTHER EXCEPTIO
+00002b90: 4e72 9d00 0000 291b 729e 0000 0072 4a00  Nr....).r....rJ.
+00002ba0: 0000 724b 0000 0072 1200 0000 da09 4c47  ..rK...r......LG
+00002bb0: 5f53 4348 454d 4172 1300 0000 7257 0000  _SCHEMAr....rW..
+00002bc0: 0072 5800 0000 724c 0000 0072 7500 0000  .rX...rL...ru...
+00002bd0: 722d 0000 0072 2f00 0000 722e 0000 0072  r-...r/...r....r
+00002be0: 8200 0000 72a0 0000 0072 a100 0000 72a2  ....r....r....r.
+00002bf0: 0000 0072 9f00 0000 7278 0000 0072 7900  ...r....rx...ry.
+00002c00: 0000 7223 0000 0072 a300 0000 720a 0000  ..r#...r....r...
+00002c10: 0072 2500 0000 7256 0000 0072 a400 0000  .r%...rV...r....
+00002c20: 72a5 0000 0029 1d72 6f00 0000 7240 0000  r....).ro...r@..
+00002c30: 0072 ab00 0000 7242 0000 0072 8a00 0000  .r....rB...r....
+00002c40: 728c 0000 0072 8b00 0000 728d 0000 0072  r....r....r....r
+00002c50: 8e00 0000 72ac 0000 0072 ad00 0000 72ae  ....r....r....r.
+00002c60: 0000 0072 af00 0000 72b0 0000 0072 b100  ...r....r....r..
+00002c70: 0000 72b2 0000 0072 b300 0000 72b4 0000  ..r....r....r...
+00002c80: 00da 0d6c 6f67 6963 616c 5f67 7261 7068  ...logical_graph
+00002c90: da02 7665 7275 0000 00da 0b61 6c67 6f5f  ..veru.....algo_
+00002ca0: 7061 7261 6d73 726d 0000 0072 7c00 0000  paramsrm...r|...
+00002cb0: 72a7 0000 0072 7a00 0000 7285 0000 0072  r....rz...r....r
+00002cc0: a800 0000 72a9 0000 0072 5a00 0000 725a  ....r....rZ...rZ
+00002cd0: 0000 0072 5b00 0000 da0c 6765 6e5f 7067  ...r[.....gen_pg
+00002ce0: 745f 706f 7374 b101 0000 7380 0000 0000  t_post....s.....
+00002cf0: 2d0c 0102 010a 0102 010e 0110 0110 011c  -...............
+00002d00: 020a 0302 0102 0102 0102 0102 0102 0102  ................
+00002d10: 0102 0102 0102 f704 0b02 0102 0102 0102  ................
+00002d20: 0102 0102 0102 0102 f904 090c 0104 0114  ................
+00002d30: ff04 0304 0102 0202 0102 0102 0102 010e  ................
+00002d40: ff02 0202 fa04 fe04 0b06 0112 010a 0102  ................
+00002d50: 0102 010e fe16 0412 010a 0102 0102 010e  ................
+00002d60: fe16 0410 010a 0108 0102 0102 010a fe72  ...............r
+00002d70: b900 0000 7a07 2f67 656e 5f70 677a 6c49  ....z./gen_pgzlI
+00002d80: 6620 7375 7070 6c69 6564 2c20 7468 6973  f supplied, this
+00002d90: 2065 6e64 706f 696e 7420 7769 6c6c 2061   endpoint will a
+00002da0: 7474 656d 7074 2074 6f20 6465 706c 6f79  ttempt to deploy
+00002db0: 2074 6865 2067 7261 7068 2069 7320 7468   the graph is th
+00002dc0: 6520 646c 675f 7067 745f 7572 6c20 6f72  e dlg_pgt_url or
+00002dd0: 2064 6c67 5f6d 6772 5f68 6f73 742f 706f   dlg_mgr_host/po
+00002de0: 7274 2065 6e64 706f 696e 747a 2a54 6865  rt endpointz*The
+00002df0: 2044 414c 6975 4745 206d 616e 6167 6572   DALiuGE manager
+00002e00: 2074 6f20 6465 706c 6f79 2074 6865 2067   to deploy the g
+00002e10: 7261 7068 2074 6f7a 3254 6865 2044 414c  raph toz2The DAL
+00002e20: 6975 4745 206d 616e 6167 6572 2062 6173  iuGE manager bas
+00002e30: 6520 4950 2074 6f20 6465 706c 6f79 2074  e IP to deploy t
+00002e40: 6865 2067 7261 7068 2074 6f7a 2f54 6865  he graph toz/The
+00002e50: 2044 414c 6975 4745 206d 616e 6167 6572   DALiuGE manager
+00002e60: 2070 6f72 7420 746f 2064 6570 6c6f 7920   port to deploy 
+00002e70: 7468 6520 6772 6170 6820 746f 7a35 5468  the graph toz5Th
+00002e80: 6520 6e75 6d62 6572 206f 6620 6e6f 6465  e number of node
+00002e90: 7320 746f 2075 6e72 6f6c 6c20 7468 6520  s to unroll the 
+00002ea0: 6772 6170 6820 7061 7274 6974 696f 6e20  graph partition 
+00002eb0: 666f 7229 0772 6f00 0000 727c 0000 00da  for).ro...r|....
+00002ec0: 0e64 6c67 5f6d 6772 5f64 6570 6c6f 79da  .dlg_mgr_deploy.
+00002ed0: 0b64 6c67 5f6d 6772 5f75 726c da0c 646c  .dlg_mgr_url..dl
+00002ee0: 675f 6d67 725f 686f 7374 da0c 646c 675f  g_mgr_host..dlg_
+00002ef0: 6d67 725f 706f 7274 da0d 7470 6c5f 6e6f  mgr_port..tpl_no
+00002f00: 6465 735f 6c65 6e63 0700 0000 0000 0000  des_lenc........
+00002f10: 0000 0000 1900 0000 0a00 0000 4300 0000  ............C...
+00002f20: 739a 0200 0064 017d 0764 027d 087c 0364  s....d.}.d.}.|.d
+00002f30: 036b 0972 8474 007c 0383 017d 097a 1c7c  .k.r.t.|...}.z.|
+00002f40: 096a 01a0 0264 04a1 015c 027d 0a7d 0874  .j...d...\.}.}.t
+00002f50: 037c 0883 017d 0857 006e 3001 0001 0001  .|...}.W.n0.....
+00002f60: 007c 096a 017d 0a7c 096a 0464 056b 0272  .|.j.}.|.j.d.k.r
+00002f70: 5264 067d 086e 0e7c 096a 0464 076b 0272  Rd.}.n.|.j.d.k.r
+00002f80: 6064 027d 0859 006e 0258 007c 096a 057d  `d.}.Y.n.X.|.j.}
+00002f90: 077c 07a0 0664 08a1 0172 9a7c 0764 0364  .|...d...r.|.d.d
+00002fa0: 0985 0219 007d 076e 167c 047d 0a7c 0564  .....}.n.|.}.|.d
+00002fb0: 036b 0972 967c 057d 086e 0464 027d 0874  .k.r.|.}.n.d.}.t
+00002fc0: 07a0 0864 0a7c 0aa1 0201 0074 07a0 0864  ...d.|.....t...d
+00002fd0: 0b7c 08a1 0201 0074 07a0 0864 0c7c 07a1  .|.....t...d.|..
+00002fe0: 0201 007c 0264 036b 097d 0b74 09a0 0a7c  ...|.d.k.}.t...|
+00002ff0: 01a1 017d 0c7c 0c64 036b 0872 ea74 0b64  ...}.|.d.k.r.t.d
+00003000: 0d64 0ea0 0c7c 01a1 0164 0f8d 0282 017c  .d...|...d.....|
+00003010: 0c6a 0d7d 0d7c 0c6a 0e7d 0e74 0f74 1074  .j.}.|.j.}.t.t.t
+00003020: 1164 1064 1184 007c 0d64 1219 0083 0283  .d.d...|.d......
+00003030: 0183 017d 0f7c 0a64 036b 0890 0172 587c  ...}.|.d.k...rX|
+00003040: 0664 136b 0490 0172 2a7c 0f7d 106e 0c74  .d.k...r*|.}.n.t
+00003050: 0b64 1464 1564 0f8d 0282 017c 0c6a 1267  .d.d.d.....|.j.g
+00003060: 0064 167c 1064 178d 037d 117c 11a0 137c  .d.|.d...}.|...|
+00003070: 0ea1 0101 0074 147c 1183 0153 007a c274  .....t.|...S.z.t
+00003080: 157c 0a7c 087c 0764 1864 198d 047d 127c  .|.|.|.d.d...}.|
+00003090: 12a0 16a1 007d 137c 0c6a 127c 1364 1664  .....}.|.j.|.d.d
+000030a0: 1a8d 027d 117c 0b90 0272 0e74 176a 17a0  ...}.|...r.t.j..
+000030b0: 18a1 00a0 1964 1ba1 017d 1464 1ca0 0c7c  .....d...}.d...|
+000030c0: 01a0 0264 1da1 0164 1319 00a0 0264 1ea1  ...d...d.....d..
+000030d0: 0164 1319 00a0 0264 08a1 0164 0919 007c  .d.....d...d...|
+000030e0: 14a1 027d 157c 12a0 1a7c 15a1 0101 0074  ...}.|...|.....t
+000030f0: 1ba0 1c7c 11a1 017d 167c 11a0 137c 0ea1  ...|...}.|...|..
+00003100: 0101 007c 12a0 1d7c 157c 11a1 0201 007c  ...|...|.|.....|
+00003110: 126a 1e7c 157c 1664 1f8d 0201 0074 1f64  .j.|.|.d.....t.d
+00003120: 20a0 0c7c 0a7c 087c 077c 15a1 0483 0157   ..|.|.|.|.....W
+00003130: 0053 0074 147c 1183 0157 0053 0057 006e  .S.t.|...W.S.W.n
+00003140: 7a04 0074 206a 216b 0a90 0272 5201 007d  z..t j!k...rR..}
+00003150: 1701 007a 1674 0b64 1464 21a0 0c7c 17a1  ...z.t.d.d!..|..
+00003160: 0164 0f8d 0282 0157 0035 0064 037d 177e  .d.....W.5.d.}.~
+00003170: 1758 0059 006e 4404 0074 226b 0a90 0272  .X.Y.nD..t"k...r
+00003180: 9401 007d 1801 007a 2474 07a0 2374 24a0  ...}...z$t..#t$.
+00003190: 25a1 00a1 0101 0074 0b64 1464 22a0 0c7c  %......t.d.d"..|
+000031a0: 18a1 0164 0f8d 0282 0157 0035 0064 037d  ...d.....W.5.d.}
+000031b0: 187e 1858 0059 006e 0258 0064 0353 0029  .~.X.Y.n.X.d.S.)
+000031c0: 237a 750a 2020 2020 5245 5354 6675 6c20  #zu.    RESTful 
+000031d0: 696e 7465 7266 6163 6520 746f 2063 6f6e  interface to con
+000031e0: 7665 7274 2061 2050 4754 2850 2920 696e  vert a PGT(P) in
+000031f0: 746f 2050 4720 6279 206d 6170 7069 6e67  to PG by mapping
+00003200: 0a20 2020 2050 4754 2850 2920 6f6e 746f  .    PGT(P) onto
+00003210: 2061 2067 6976 656e 2073 6574 206f 6620   a given set of 
+00003220: 6176 6169 6c61 626c 6520 7265 736f 7572  available resour
+00003230: 6365 730a 2020 2020 7299 0000 0069 bb01  ces.    r....i..
+00003240: 0000 4efa 013a da04 6874 7470 e950 0000  ..N..:..http.P..
+00003250: 00da 0568 7474 7073 725d 0000 00e9 ffff  ...httpsr]......
+00003260: ffff 7a10 4d61 6e61 6765 7220 686f 7374  ..z.Manager host
+00003270: 3a20 2573 7a10 4d61 6e61 6765 7220 706f  : %sz.Manager po
+00003280: 7274 3a20 2573 7a12 4d61 6e61 6765 7220  rt: %sz.Manager 
+00003290: 7072 6566 6978 3a20 2573 7243 0000 00fa  prefix: %srC....
+000032a0: 3a50 4754 2850 2920 7769 7468 2069 6420  :PGT(P) with id 
+000032b0: 7b30 7d20 6e6f 7420 666f 756e 6420 696e  {0} not found in
+000032c0: 2074 6865 2050 6879 7369 6361 6c20 4772   the Physical Gr
+000032d0: 6170 6820 4d61 6e61 6765 7272 4400 0000  aph ManagerrD...
+000032e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000032f0: 0002 0000 0053 0000 0073 0800 0000 6401  .....S...s....d.
+00003300: 7c00 6b06 5300 a902 4e5a 0769 7347 726f  |.k.S...NZ.isGro
+00003310: 7570 725a 0000 00a9 01da 016e 725a 0000  uprZ.......nrZ..
+00003320: 0072 5a00 0000 725b 0000 00da 083c 6c61  .rZ...r[.....<la
+00003330: 6d62 6461 3e69 0200 00f3 0000 0000 7a18  mbda>i........z.
+00003340: 6765 6e5f 7067 2e3c 6c6f 6361 6c73 3e2e  gen_pg.<locals>.
+00003350: 3c6c 616d 6264 613e da0d 6e6f 6465 4461  <lambda>..nodeDa
+00003360: 7461 4172 7261 7972 0100 0000 7248 0000  taArrayr....rH..
+00003370: 007a 324d 7573 7420 7370 6563 6966 7920  .z2Must specify 
+00003380: 4441 4c69 7547 4520 6d61 6e61 6765 7220  DALiuGE manager 
+00003390: 686f 7374 206f 7220 7470 6c5f 6e6f 6465  host or tpl_node
+000033a0: 735f 6c65 6e46 2902 da07 7265 745f 7374  s_lenF)...ret_st
+000033b0: 7272 be00 0000 e91e 0000 0029 04da 0468  rr.........)...h
+000033c0: 6f73 74da 0470 6f72 745a 0a75 726c 5f70  ost..portZ.url_p
+000033d0: 7265 6669 78da 0774 696d 656f 7574 2901  refix..timeout).
+000033e0: 72cb 0000 007a 1425 592d 256d 2d25 6454  r....z.%Y-%m-%dT
+000033f0: 2548 2d25 4d2d 2553 2e25 667a 077b 307d  %H-%M-%S.%fz.{0}
+00003400: 5f7b 317d 7a06 2e67 7261 7068 5a04 5f70  _{1}z..graphZ._p
+00003410: 6774 2901 da0e 636f 6d70 6c65 7465 645f  gt)...completed_
+00003420: 7569 6473 7a27 6874 7470 3a2f 2f7b 307d  uidsz'http://{0}
+00003430: 3a7b 317d 7b32 7d2f 7365 7373 696f 6e3f  :{1}{2}/session?
+00003440: 7365 7373 696f 6e49 643d 7b33 7d7a 3146  sessionId={3}z1F
+00003450: 6169 6c65 6420 746f 2069 6e74 6572 6163  ailed to interac
+00003460: 7420 7769 7468 2044 414c 6955 4745 2044  t with DALiUGE D
+00003470: 726f 7020 4d61 6e61 6765 723a 207b 307d  rop Manager: {0}
+00003480: fa24 4661 696c 6564 2074 6f20 6465 706c  .$Failed to depl
+00003490: 6f79 2070 6879 7369 6361 6c20 6772 6170  oy physical grap
+000034a0: 683a 207b 307d 2926 7205 0000 00da 066e  h: {0})&r......n
+000034b0: 6574 6c6f 63da 0573 706c 6974 da03 696e  etloc..split..in
+000034c0: 74da 0673 6368 656d 65da 0470 6174 68da  t..scheme..path.
+000034d0: 0865 6e64 7377 6974 6872 4c00 0000 da05  .endswithrL.....
+000034e0: 6465 6275 6772 8200 0000 da07 6765 745f  debugr......get_
+000034f0: 7067 7472 0a00 0000 7257 0000 00da 0e5f  pgtr....rW....._
+00003500: 676f 6a73 5f6a 736f 6e5f 6f62 6ada 0972  gojs_json_obj..r
+00003510: 6570 726f 6461 7461 725f 0000 00da 046c  eprodatar_.....l
+00003520: 6973 74da 0666 696c 7465 72da 0a74 6f5f  ist..filter..to_
+00003530: 7067 5f73 7065 63da 0661 7070 656e 6472  pg_spec..appendr
+00003540: 0e00 0000 7217 0000 00da 056e 6f64 6573  ....r......nodes
+00003550: da08 6461 7465 7469 6d65 da03 6e6f 77da  ..datetime..now.
+00003560: 0873 7472 6674 696d 65da 0e63 7265 6174  .strftime..creat
+00003570: 655f 7365 7373 696f 6e72 1600 0000 da09  e_sessionr......
+00003580: 6765 745f 726f 6f74 73da 0c61 7070 656e  get_roots..appen
+00003590: 645f 6772 6170 68da 0e64 6570 6c6f 795f  d_graph..deploy_
+000035a0: 7365 7373 696f 6e72 0f00 0000 7215 0000  sessionr....r...
+000035b0: 00da 1352 6573 7443 6c69 656e 7445 7863  ...RestClientExc
+000035c0: 6570 7469 6f6e 7256 0000 0072 7500 0000  eptionrV...ru...
+000035d0: 72a4 0000 0072 a500 0000 2919 726f 0000  r....r....).ro..
+000035e0: 0072 7c00 0000 72ba 0000 0072 bb00 0000  .r|...r....r....
+000035f0: 72bc 0000 0072 bd00 0000 72be 0000 00da  r....r....r.....
+00003600: 076d 7072 6566 6978 da05 6d70 6f72 745a  .mprefix..mportZ
+00003610: 066d 7061 7273 65da 056d 686f 7374 5a06  .mparse..mhostZ.
+00003620: 6465 706c 6f79 da04 7067 7470 da05 7067  deploy..pgtp..pg
+00003630: 7470 6a72 db00 0000 72a6 0000 005a 066e  tpjr....r....Z.n
+00003640: 6e6f 6465 73da 0770 675f 7370 6563 5a0a  nodes..pg_specZ.
+00003650: 6d67 725f 636c 6965 6e74 da09 6e6f 6465  mgr_client..node
+00003660: 5f6c 6973 74da 0264 745a 0473 7369 6472  _list..dtZ.ssidr
+00003670: d000 0000 da02 7265 da02 6578 725a 0000  ......re..exrZ..
+00003680: 0072 5a00 0000 725b 0000 00da 0667 656e  .rZ...r[.....gen
+00003690: 5f70 6723 0200 0073 aa00 0000 001e 0401  _pg#...s........
+000036a0: 0401 0801 0801 0201 1001 0c01 0601 0601  ................
+000036b0: 0a01 0601 0a01 0a01 0601 0a01 0e02 0401  ................
+000036c0: 0801 0602 0402 0c01 0c01 0c03 0801 0a01  ................
+000036d0: 0801 0201 0201 0401 02ff 02fe 0607 0601  ................
+000036e0: 0601 1a02 0a01 0a01 0602 0201 0201 02fe  ................
+000036f0: 0605 1001 0a01 0801 0201 0201 0200 0200  ................
+00003700: 0200 02ff 0604 0802 0e02 0601 1001 0401  ................
+00003710: 2000 02ff 0403 0a02 0a01 0a01 0c02 0e04   ...............
+00003720: 0201 0401 0200 0200 0200 02ff 02ff 0606  ................
+00003730: 0e01 1401 0201 0201 08fe 1604 1201 0e01  ................
+00003740: 0201 0201 08fe 72f3 0000 007a 0c2f 6765  ......r....z./ge
+00003750: 6e5f 7067 5f73 7065 637a 3054 6865 206c  n_pg_specz0The l
+00003760: 6973 7420 6f66 2064 616c 6975 6765 206e  ist of daliuge n
+00003770: 6f64 6573 2074 6f20 7375 626d 6974 2074  odes to submit t
+00003780: 6865 2067 7261 7068 2074 6f7a 4454 6865  he graph tozDThe
+00003790: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
+000037a0: 6d61 6e61 6765 7220 686f 7374 2077 6865  manager host whe
+000037b0: 7265 2074 6865 2067 7261 7068 2077 696c  re the graph wil
+000037c0: 6c20 6265 2064 6570 6c6f 7965 6420 746f  l be deployed to
+000037d0: 2e7a 2a54 6865 206e 756d 6265 7220 6f66  .z*The number of
+000037e0: 206e 6f64 6573 2072 6571 7565 7374 6564   nodes requested
+000037f0: 2062 7920 7468 6520 6772 6170 6829 0472   by the graph).r
+00003800: 7c00 0000 72ef 0000 00da 0c6d 616e 6167  |...r......manag
+00003810: 6572 5f68 6f73 7472 be00 0000 6304 0000  er_hostr....c...
+00003820: 0000 0000 0000 0000 0009 0000 000a 0000  ................
+00003830: 0043 0000 0073 3801 0000 7a20 7c02 6401  .C...s8...z |.d.
+00003840: 6b02 720e 6401 7d02 7400 a001 6402 7402  k.r.d.}.t...d.t.
+00003850: 7c00 8301 a102 0100 5700 6e44 0400 7403  |.......W.nD..t.
+00003860: 6b0a 7264 0100 7d04 0100 7a26 7400 a004  k.rd..}...z&t...
+00003870: 6403 7405 a006 a100 a102 0100 7407 6404  d.t.........t.d.
+00003880: 6405 a008 7c04 a101 6406 8d02 8201 5700  d...|...d.....W.
+00003890: 3500 6407 7d04 7e04 5800 5900 6e02 5800  5.d.}.~.X.Y.n.X.
+000038a0: 7409 a00a 7c00 a101 7d05 7c05 6407 6b08  t...|...}.|.d.k.
+000038b0: 728a 7407 6408 6409 a008 7c00 a101 6406  r.t.d.d...|...d.
+000038c0: 8d02 8201 7c01 6407 6b08 729e 7407 6404  ....|.d.k.r.t.d.
+000038d0: 640a 6406 8d02 8201 7a4e 7c05 6a0b 7c02  d.d.....zN|.j.|.
+000038e0: 6701 7c01 1700 7c03 640b 640c 8d03 7d06  g.|...|.d.d...}.
+000038f0: 740c a00d 7c06 a101 7d07 7400 a001 640d  t...|...}.t...d.
+00003900: 740e 7c07 8301 a102 0100 740f 7410 a011  t.|.......t.t...
+00003910: 7c06 740e 7c07 8301 640e 9c02 a101 8301  |.t.|...d.......
+00003920: 7d08 7c08 5700 5300 0400 7403 6b0a 9001  }.|.W.S...t.k...
+00003930: 7232 0100 7d04 0100 7a26 7400 a004 6403  r2..}...z&t...d.
+00003940: 7405 a006 a100 a102 0100 7407 6404 640f  t.........t.d.d.
+00003950: a008 7c04 a101 6406 8d02 8201 5700 3500  ..|...d.....W.5.
+00003960: 6407 7d04 7e04 5800 5900 6e02 5800 6407  d.}.~.X.Y.n.X.d.
+00003970: 5300 2910 7a34 0a20 2020 2049 6e74 6572  S.).z4.    Inter
+00003980: 6661 6365 2074 6f20 636f 6e76 6572 7420  face to convert 
+00003990: 6120 5047 5428 5029 2069 6e74 6f20 7067  a PGT(P) into pg
+000039a0: 5f73 7065 630a 2020 2020 da09 6c6f 6361  _spec.    ..loca
+000039b0: 6c68 6f73 747a 0a70 6774 5f69 643a 2025  lhostz.pgt_id: %
+000039c0: 737a 0225 7372 4800 0000 7a35 556e 6162  sz.%srH...z5Unab
+000039d0: 6c65 2074 6f20 7061 7273 6520 6a73 6f6e  le to parse json
+000039e0: 2062 6f64 7920 6f66 2072 6571 7565 7374   body of request
+000039f0: 2066 6f72 2070 675f 7370 6563 3a20 7b30   for pg_spec: {0
+00003a00: 7d72 4400 0000 4e72 4300 0000 72c4 0000  }rD...NrC...r...
+00003a10: 007a 1f4d 7573 7420 7370 6563 6966 7920  .z.Must specify 
+00003a20: 4441 4c69 7547 4520 6e6f 6465 7320 6c69  DALiuGE nodes li
+00003a30: 7374 4629 0272 be00 0000 72cb 0000 007a  stF).r....r....z
+00003a40: 0d52 6f6f 7420 5549 4473 3a20 2573 2902  .Root UIDs: %s).
+00003a50: 72ee 0000 00da 0972 6f6f 745f 7569 6473  r......root_uids
+00003a60: 7a1f 4661 696c 6564 2074 6f20 6765 6e65  z.Failed to gene
+00003a70: 7261 7465 2070 675f 7370 6563 3a20 7b30  rate pg_spec: {0
+00003a80: 7d29 1272 4c00 0000 72d8 0000 0072 5800  }).rL...r....rX.
+00003a90: 0000 7256 0000 0072 7500 0000 72a4 0000  ..rV...ru...r...
+00003aa0: 0072 a500 0000 720a 0000 0072 5700 0000  .r....r....rW...
+00003ab0: 7282 0000 0072 d900 0000 72de 0000 0072  r....r....r....r
+00003ac0: 1600 0000 72e5 0000 0072 dc00 0000 720e  ....r....r....r.
+00003ad0: 0000 0072 4a00 0000 7255 0000 0029 0972  ...rJ...rU...).r
+00003ae0: 7c00 0000 72ef 0000 0072 f400 0000 72be  |...r....r....r.
+00003af0: 0000 0072 f200 0000 72ec 0000 0072 ee00  ...r....r....r..
+00003b00: 0000 72f6 0000 00da 0872 6573 706f 6e73  ..r......respons
+00003b10: 6572 5a00 0000 725a 0000 0072 5b00 0000  erZ...rZ...r[...
+00003b20: da0b 6765 6e5f 7067 5f73 7065 63a3 0200  ..gen_pg_spec...
+00003b30: 0073 5000 0000 0014 0201 0801 0401 1402  .sP.............
+00003b40: 1001 1001 0201 0201 08fe 1804 0a01 0801  ................
+00003b50: 0201 0201 0401 02ff 02fe 0606 0801 0c02  ................
+00003b60: 0201 0401 0801 0201 02fd 0605 0a01 1001  ................
+00003b70: 0201 0401 0cff 02ff 0405 0601 1201 1001  ................
+00003b80: 0201 0201 08fe 72f8 0000 007a 0c2f 6765  ......r....z./ge
+00003b90: 6e5f 7067 5f68 656c 6d63 0100 0000 0000  n_pg_helmc......
+00003ba0: 0000 0000 0000 0600 0000 0a00 0000 4300  ..............C.
+00003bb0: 0000 73b6 0000 0064 0164 026c 006d 017d  ..s....d.d.l.m.}
+00003bc0: 0101 0074 02a0 037c 00a1 017d 027c 0264  ...t...|...}.|.d
+00003bd0: 036b 0872 3074 0464 0464 05a0 057c 00a1  .k.r0t.d.d...|..
+00003be0: 0164 068d 0282 017c 026a 067d 0374 07a0  .d.....|.j.}.t..
+00003bf0: 0864 077c 03a1 0201 0074 0974 0a74 0b64  .d.|.....t.t.t.d
+00003c00: 0864 0984 007c 0364 0a19 0083 0283 0183  .d...|.d........
+00003c10: 017d 047a 107c 017c 027c 0474 0c83 0301  .}.z.|.|.|.t....
+00003c20: 0057 006e 4404 0074 0d6a 0e6b 0a72 b001  .W.nD..t.j.k.r..
+00003c30: 007d 0501 007a 2474 07a0 0f74 10a0 11a1  .}...z$t...t....
+00003c40: 00a1 0101 0074 0464 0b64 0ca0 057c 05a1  .....t.d.d...|..
+00003c50: 0164 068d 0282 0157 0035 0064 037d 057e  .d.....W.5.d.}.~
+00003c60: 0558 0059 006e 0258 0064 0d53 0029 0e7a  .X.Y.n.X.d.S.).z
+00003c70: 2c0a 2020 2020 4465 706c 6f79 7320 6120  ,.    Deploys a 
+00003c80: 5047 5420 6173 2061 204b 3873 2068 656c  PGT as a K8s hel
+00003c90: 6d20 6368 6172 742e 0a20 2020 20e9 0300  m chart..    ...
+00003ca0: 0000 2901 da0a 7374 6172 745f 6865 6c6d  ..)...start_helm
+00003cb0: 4e72 4300 0000 72c4 0000 0072 4400 0000  NrC...r....rD...
+00003cc0: 7a08 5047 5450 3a20 2573 6301 0000 0000  z.PGTP: %sc.....
+00003cd0: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00003ce0: 0000 0073 0800 0000 6401 7c00 6b06 5300  ...s....d.|.k.S.
+00003cf0: 72c5 0000 0072 5a00 0000 72c6 0000 0072  r....rZ...r....r
+00003d00: 5a00 0000 725a 0000 0072 5b00 0000 72c8  Z...rZ...r[...r.
+00003d10: 0000 00fa 0200 0072 c900 0000 7a1d 6765  .......r....z.ge
+00003d20: 6e5f 7067 5f68 656c 6d2e 3c6c 6f63 616c  n_pg_helm.<local
+00003d30: 733e 2e3c 6c61 6d62 6461 3e72 ca00 0000  s>.<lambda>r....
+00003d40: 7248 0000 0072 d100 0000 7a30 496e 7370  rH...r....z0Insp
+00003d50: 6563 7420 796f 7572 206b 3873 2064 6173  ect your k8s das
+00003d60: 6862 6f61 7264 2066 6f72 2064 6570 6c6f  hboard for deplo
+00003d70: 796d 656e 7420 7374 6174 7573 2912 5a19  yment status).Z.
+00003d80: 6465 706c 6f79 2e73 7461 7274 5f68 656c  deploy.start_hel
+00003d90: 6d5f 636c 7573 7465 7272 fa00 0000 7282  m_clusterr....r.
+00003da0: 0000 0072 d900 0000 720a 0000 0072 5700  ...r....r....rW.
+00003db0: 0000 72da 0000 0072 4c00 0000 72a3 0000  ..r....rL...r...
+00003dc0: 0072 5f00 0000 72dc 0000 0072 dd00 0000  .r_...r....r....
+00003dd0: 726b 0000 0072 1500 0000 72e8 0000 0072  rk...r....r....r
+00003de0: 7500 0000 72a4 0000 0072 a500 0000 2906  u...r....r....).
+00003df0: 727c 0000 0072 fa00 0000 72ec 0000 0072  r|...r....r....r
+00003e00: ed00 0000 72a6 0000 0072 f200 0000 725a  ....r....r....rZ
+00003e10: 0000 0072 5a00 0000 725b 0000 00da 0b67  ...rZ...r[.....g
+00003e20: 656e 5f70 675f 6865 6c6d e302 0000 732a  en_pg_helm....s*
+00003e30: 0000 0000 0a0c 020a 0108 0102 0102 0104  ................
+00003e40: 0102 ff02 fe06 0706 010c 011a 0202 0110  ................
+00003e50: 0112 010e 0102 0102 0108 fe18 0572 fb00  .............r..
+00003e60: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003e70: 0000 0003 0000 0040 0000 0073 c600 0000  .......@...s....
+00003e80: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
+00003e90: 5a04 6505 6506 6402 6602 1900 6507 6403  Z.e.e.d.f...e.d.
+00003ea0: 3c00 6402 5a08 6505 6506 6402 6602 1900  <.d.Z.e.e.d.f...
+00003eb0: 6507 6404 3c00 6402 5a09 6505 6506 6402  e.d.<.d.Z.e.e.d.
+00003ec0: 6602 1900 6507 6405 3c00 6402 5a0a 6505  f...e.d.<.d.Z.e.
+00003ed0: 6506 6402 6602 1900 6507 6406 3c00 6402  e.d.f...e.d.<.d.
+00003ee0: 5a0b 6505 6506 6402 6602 1900 6507 6407  Z.e.e.d.f...e.d.
+00003ef0: 3c00 6402 5a0c 6505 6506 6402 6602 1900  <.d.Z.e.e.d.f...
+00003f00: 6507 6408 3c00 6402 5a0d 6505 6506 6402  e.d.<.d.Z.e.e.d.
+00003f10: 6602 1900 6507 6409 3c00 6402 5a0e 6505  f...e.d.<.d.Z.e.
+00003f20: 6506 6402 6602 1900 6507 640a 3c00 6402  e.d.f...e.d.<.d.
+00003f30: 5a0f 6505 6506 6402 6602 1900 6507 640b  Z.e.e.d.f...e.d.
+00003f40: 3c00 6402 5300 290c da0a 416c 676f 5061  <.d.S.)...AlgoPa
+00003f50: 7261 6d73 7a88 0a20 2020 2053 6574 206f  ramsz..    Set o
+00003f60: 6620 7363 6865 6475 6c69 6e67 2061 6c67  f scheduling alg
+00003f70: 6f72 6974 686d 2070 6172 616d 6574 6572  orithm parameter
+00003f80: 732c 206e 6f74 2061 6c6c 2061 7070 6c79  s, not all apply
+00003f90: 2074 6f20 616c 6c20 616c 676f 7269 7468   to all algorith
+00003fa0: 6d73 2e0a 2020 2020 5265 6665 7220 746f  ms..    Refer to
+00003fb0: 206d 6169 6e20 646f 6375 6d65 6e74 6174   main documentat
+00003fc0: 696f 6e20 666f 7220 6d6f 7265 2069 6e66  ion for more inf
+00003fd0: 6f72 6d61 7469 6f6e 2e0a 2020 2020 4e72  ormation..    Nr
+00003fe0: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
+00003ff0: 0000 0072 b000 0000 72b1 0000 0072 b200  ...r....r....r..
+00004000: 0000 72b3 0000 0072 b400 0000 2910 da08  ..r....r....)...
+00004010: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00004020: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00004030: 5f5f da07 5f5f 646f 635f 5f72 ac00 0000  __..__doc__r....
+00004040: 7204 0000 0072 d400 0000 da0f 5f5f 616e  r....r......__an
+00004050: 6e6f 7461 7469 6f6e 735f 5f72 ad00 0000  notations__r....
+00004060: 72ae 0000 0072 af00 0000 72b0 0000 0072  r....r....r....r
+00004070: b100 0000 72b2 0000 0072 b300 0000 72b4  ....r....r....r.
+00004080: 0000 0072 5a00 0000 725a 0000 0072 5a00  ...rZ...rZ...rZ.
+00004090: 0000 725b 0000 0072 fc00 0000 0b03 0000  ..r[...r........
+000040a0: 7314 0000 000a 0104 0514 0114 0114 0114  s...............
+000040b0: 0114 0114 0114 0114 0172 fc00 0000 6300  .........r....c.
+000040c0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000040d0: 0000 0040 0000 0073 2400 0000 6500 5a01  ...@...s$...e.Z.
+000040e0: 6400 5a02 6401 5a03 6402 5a04 6403 5a05  d.Z.d.Z.d.Z.d.Z.
+000040f0: 6404 5a06 6405 5a07 6406 5a08 6407 5300  d.Z.d.Z.d.Z.d.S.
+00004100: 2908 da0f 4b6e 6f77 6e41 6c67 6f72 6974  )...KnownAlgorit
+00004110: 686d 737a 540a 2020 2020 4c69 7374 206f  hmszT.    List o
+00004120: 6620 6b6e 6f77 6e20 7363 6865 6475 6c69  f known scheduli
+00004130: 6e67 2061 6c67 6f72 6974 686d 732e 0a20  ng algorithms.. 
+00004140: 2020 2057 696c 6c20 6e65 6564 2074 6f20     Will need to 
+00004150: 6265 2075 7064 6174 6564 206d 616e 7561  be updated manua
+00004160: 6c6c 792e 0a20 2020 2029 01da 046e 6f6e  lly..    )...non
+00004170: 6529 0172 8900 0000 2901 5a08 6d79 7361  e).r....).Z.mysa
+00004180: 726b 6172 2901 5a0d 6d69 6e5f 6e75 6d5f  rkar).Z.min_num_
+00004190: 7061 7274 735a 0370 736f 4e29 0972 fd00  partsZ.psoN).r..
+000041a0: 0000 72fe 0000 0072 ff00 0000 7200 0100  ..r....r....r...
+000041b0: 005a 0941 4c47 4f5f 4e4f 4e45 5a0a 414c  .Z.ALGO_NONEZ.AL
+000041c0: 474f 5f4d 4554 4953 5a0e 414c 474f 5f4d  GO_METISZ.ALGO_M
+000041d0: 595f 5341 524b 4152 5a12 414c 474f 5f4d  Y_SARKARZ.ALGO_M
+000041e0: 494e 5f4e 554d 5f50 4152 5453 5a08 414c  IN_NUM_PARTSZ.AL
+000041f0: 474f 5f50 534f 725a 0000 0072 5a00 0000  GO_PSOrZ...rZ...
+00004200: 725a 0000 0072 5b00 0000 7202 0100 001c  rZ...r[...r.....
+00004210: 0300 0073 0c00 0000 0801 0405 0401 0401  ...s............
+00004220: 0401 0401 7202 0100 0029 02da 0d67 7261  ....r....)...gra
+00004230: 7068 5f63 6f6e 7465 6e74 da0a 6772 6170  ph_content..grap
+00004240: 685f 6e61 6d65 6302 0000 0000 0000 0000  h_namec.........
+00004250: 0000 0006 0000 000b 0000 0043 0000 0073  ...........C...s
+00004260: f200 0000 6900 7d02 7c00 6400 6b09 7220  ....i.}.|.d.k.r 
+00004270: 7c01 6400 6b09 7220 7400 6401 6402 6403  |.d.k.r t.d.d.d.
+00004280: 8d02 8201 7401 7402 7c01 8302 7386 7c00  ....t.t.|...s.|.
+00004290: 733c 7400 6401 6404 6403 8d02 8201 71ee  s<t.d.d.d.....q.
+000042a0: 7a0e 7403 a004 7c00 a101 7d02 5700 71ee  z.t...|...}.W.q.
+000042b0: 0400 7405 6b0a 7282 0100 7d03 0100 7a1a  ..t.k.r...}...z.
+000042c0: 7406 a007 7c03 a101 0100 7400 6401 6405  t...|.....t.d.d.
+000042d0: 6403 8d02 8201 5700 3500 6400 7d03 7e03  d.....W.5.d.}.~.
+000042e0: 5800 5900 71ee 5800 6e68 7408 7402 7c01  X.Y.q.X.nht.t.|.
+000042f0: 8302 7d04 7409 7c04 6406 8302 8f4e 7d05  ..}.t.|.d....N}.
+00004300: 7a0e 7403 a00a 7c05 a101 7d02 5700 6e38  z.t...|...}.W.n8
+00004310: 0400 7405 6b0a 72e2 0100 7d03 0100 7a1a  ..t.k.r...}...z.
+00004320: 7406 a007 7c03 a101 0100 7400 6407 6408  t...|.....t.d.d.
+00004330: 6403 8d02 8201 5700 3500 6400 7d03 7e03  d.....W.5.d.}.~.
+00004340: 5800 5900 6e02 5800 5700 3500 5100 5200  X.Y.n.X.W.5.Q.R.
+00004350: 5800 7c02 5300 2909 4ee9 9001 0000 7a35  X.|.S.).N.....z5
+00004360: 4e65 6564 2074 6f20 7375 7070 6c79 2065  Need to supply e
+00004370: 6974 6865 7220 616e 206e 616d 6520 6f72  ither an name or
+00004380: 2063 6f6e 7465 6e74 2062 7574 206e 6f74   content but not
+00004390: 2062 6f74 6872 4400 0000 7a19 4c47 2063   bothrD...z.LG c
+000043a0: 6f6e 7465 6e74 2069 7320 6e6f 6e65 7869  ontent is nonexi
+000043b0: 7374 656e 747a 174c 4720 636f 6e74 656e  stentz.LG conten
+000043c0: 7420 6973 206d 616c 666f 726d 6564 725e  t is malformedr^
+000043d0: 0000 0072 4800 0000 7a21 4c47 2067 7261  ...rH...z!LG gra
+000043e0: 7068 206f 6e20 6669 6c65 2063 616e 6e6f  ph on file canno
+000043f0: 7420 6265 206c 6f61 6465 6429 0b72 0a00  t be loaded).r..
+00004400: 0000 7229 0000 0072 4900 0000 724a 0000  ..r)...rI...rJ..
+00004410: 0072 4b00 0000 7203 0000 0072 4c00 0000  .rK...r....rL...
+00004420: 7275 0000 0072 2800 0000 7253 0000 0072  ru...r(...rS...r
+00004430: 6300 0000 2906 7204 0100 0072 0501 0000  c...).r....r....
+00004440: 5a09 6f75 745f 6772 6170 68da 066a 6572  Z.out_graph..jer
+00004450: 726f 7272 6500 0000 7266 0000 0072 5a00  rorre...rf...rZ.
+00004460: 0000 725a 0000 0072 5b00 0000 da0a 6c6f  ..rZ...r[.....lo
+00004470: 6164 5f67 7261 7068 2903 0000 7332 0000  ad_graph)...s2..
+00004480: 0000 0104 0110 0102 0102 0102 fe06 040a  ................
+00004490: 0104 010e 0202 010e 0110 010a 0120 020a  ............. ..
+000044a0: 010c 0102 010e 0110 010a 0102 0102 0002  ................
+000044b0: ff22 0372 0801 0000 7a08 2f6c 675f 6669  .".r....z./lg_fi
+000044c0: 6c6c 7a40 4966 2070 7265 7365 6e74 2c20  llz@If present, 
+000044d0: 7472 616e 736c 6174 6f72 2077 696c 6c20  translator will 
+000044e0: 7573 6520 7468 6973 2073 7472 696e 6720  use this string 
+000044f0: 6173 2074 6865 2067 7261 7068 2063 6f6e  as the graph con
+00004500: 7465 6e74 7a02 7b7d 7a27 4a53 4f4e 206b  tentz.{}z'JSON k
+00004510: 6579 3a20 7661 6c75 6520 7374 6f72 6520  ey: value store 
+00004520: 6f66 2067 7261 7068 2070 6172 616d 7465  of graph paramte
+00004530: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
+00004540: 0000 0300 0000 4300 0000 7312 0000 0067  ......C...s....g
+00004550: 007c 005d 0a7d 017c 016a 0091 0271 0453  .|.].}.|.j...q.S
+00004560: 0072 5a00 0000 723b 0000 0029 0272 9400  .rZ...r;...).r..
+00004570: 0000 5a07 726f 7074 696f 6e72 5a00 0000  ..Z.roptionrZ...
+00004580: 725a 0000 0072 5b00 0000 7297 0000 0055  rZ...r[...r....U
+00004590: 0300 0073 0400 0000 0600 0200 7297 0000  ...s........r...
+000045a0: 0029 02da 0465 6e75 6d72 3300 0000 2904  .)...enumr3...).
+000045b0: 7240 0000 0072 4100 0000 da0a 7061 7261  r@...rA.....para
+000045c0: 6d65 7465 7273 7242 0000 0063 0400 0000  metersrB...c....
+000045d0: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
+000045e0: 4300 0000 7378 0000 0074 007c 017c 0083  C...sx...t.|.|..
+000045f0: 027d 047a 0e74 01a0 027c 02a1 017d 0557  .}.z.t...|...}.W
+00004600: 006e 3804 0074 036b 0a72 5001 007d 0601  .n8..t.k.rP..}..
+00004610: 007a 1a74 04a0 057c 06a1 0101 0074 0664  .z.t...|.....t.d
+00004620: 0164 0264 038d 0282 0157 0035 0064 047d  .d.d.....W.5.d.}
+00004630: 067e 0658 0059 006e 0258 0074 076a 086a  .~.X.Y.n.X.t.j.j
+00004640: 09a0 0a7c 047c 05a1 027d 0774 0b74 0c7c  ...|.|...}.t.t.|
+00004650: 077c 0383 0283 017d 0774 0d7c 0783 0153  .|.....}.t.|...S
+00004660: 0029 057a 950a 2020 2020 5769 6c6c 2066  .).z..    Will f
+00004670: 696c 6c20 6120 6c6f 6769 6361 6c20 6772  ill a logical gr
+00004680: 6170 6820 6279 2072 6570 6c61 6369 6e67  aph by replacing
+00004690: 2066 6965 6c64 7320 7769 7468 2073 7570   fields with sup
+000046a0: 706c 6965 6420 7061 7261 6d65 7465 7273  plied parameters
+000046b0: 2e0a 0a20 2020 204f 6e65 206f 6620 6c67  ...    One of lg
+000046c0: 5f6e 616d 6520 6f72 206c 675f 636f 6e74  _name or lg_cont
+000046d0: 656e 742c 2062 7574 206e 6f74 2062 6f74  ent, but not bot
+000046e0: 682c 206d 7573 7420 6265 2073 7065 6369  h, must be speci
+000046f0: 6669 6564 2e0a 2020 2020 7206 0100 007a  fied..    r....z
+00004700: 1b50 6172 616d 6574 6572 2073 7472 696e  .Parameter strin
+00004710: 6720 6973 2069 6e76 616c 6964 7244 0000  g is invalidrD..
+00004720: 004e 290e 7208 0100 0072 4a00 0000 724b  .N).r....rJ...rK
+00004730: 0000 0072 0300 0000 724c 0000 0072 7500  ...r....rL...ru.
+00004740: 0000 720a 0000 00da 0364 6c67 da08 6472  ..r......dlg..dr
+00004750: 6f70 6d61 6b65 da0c 7067 5f67 656e 6572  opmake..pg_gener
+00004760: 6174 6f72 da04 6669 6c6c 721c 0000 0072  ator..fillr....r
+00004770: 1b00 0000 720e 0000 0029 0872 4000 0000  ....r....).r@...
+00004780: 7241 0000 0072 0a01 0000 7242 0000 00da  rA...r....rB....
+00004790: 086c 675f 6772 6170 68da 0670 6172 616d  .lg_graph..param
+000047a0: 7372 0701 0000 5a0c 6f75 7470 7574 5f67  sr....Z.output_g
+000047b0: 7261 7068 725a 0000 0072 5a00 0000 725b  raphrZ...rZ...r[
+000047c0: 0000 00da 076c 675f 6669 6c6c 4603 0000  .....lg_fillF...
+000047d0: 7312 0000 0000 180a 0102 010e 0110 010a  s...............
+000047e0: 011e 0110 010e 0172 1101 0000 7a07 2f75  .......r....z./u
+000047f0: 6e72 6f6c 6c7a 2449 4420 7072 6566 6978  nrollz$ID prefix
+00004800: 2061 7070 656e 6465 6420 746f 2075 6e72   appended to unr
+00004810: 6f6c 6c65 6420 6e6f 6465 737a 2e49 6620  olled nodesz.If 
+00004820: 7472 7565 2c20 6170 7073 2077 696c 6c20  true, apps will 
+00004830: 6265 2072 6570 6c61 6365 6420 7769 7468  be replaced with
+00004840: 2073 6c65 6570 2061 7070 737a 2e49 6620   sleep appsz.If 
+00004850: 7365 742c 2077 696c 6c20 6368 616e 6765  set, will change
+00004860: 2061 6c6c 2061 7070 7320 746f 2074 6869   all apps to thi
+00004870: 7320 6170 7020 636c 6173 7329 0572 4000  s app class).r@.
+00004880: 0000 7241 0000 00da 0a6f 6964 5f70 7265  ..rA.....oid_pre
+00004890: 6669 78da 087a 6572 6f5f 7275 6eda 0b64  fix..zero_run..d
+000048a0: 6566 6175 6c74 5f61 7070 6305 0000 0000  efault_appc.....
+000048b0: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
+000048c0: 0000 0073 2e00 0000 7400 7c01 7c00 8302  ...s....t.|.|...
+000048d0: 7d05 7401 6a02 6a03 a004 7c05 7c02 7c03  }.t.j.j...|.|.|.
+000048e0: 7c04 a104 7d06 7405 7c06 8301 7d06 7406  |...}.t.|...}.t.
+000048f0: 7c06 8301 5300 2901 7a8d 0a20 2020 2057  |...S.).z..    W
+00004900: 696c 6c20 756e 726f 6c6c 2061 206c 6f67  ill unroll a log
+00004910: 6963 616c 2067 7261 7068 2069 6e74 6f20  ical graph into 
+00004920: 6120 7068 7973 6963 616c 2067 7261 7068  a physical graph
+00004930: 2074 656d 706c 6174 652e 0a0a 2020 2020   template...    
+00004940: 4f6e 6520 6f66 206c 675f 6e61 6d65 206f  One of lg_name o
+00004950: 7220 6c67 5f63 6f6e 7465 6e74 2c20 6275  r lg_content, bu
+00004960: 7420 6e6f 7420 626f 7468 2c20 6e65 6564  t not both, need
+00004970: 7320 746f 2062 6520 7370 6563 6966 6965  s to be specifie
+00004980: 642e 0a20 2020 2029 0772 0801 0000 720b  d..    ).r....r.
+00004990: 0100 0072 0c01 0000 720d 0100 00da 0675  ...r....r......u
+000049a0: 6e72 6f6c 6c72 1e00 0000 720e 0000 0029  nrollr....r....)
+000049b0: 0772 4000 0000 7241 0000 0072 1201 0000  .r@...rA...r....
+000049c0: 7213 0100 0072 1401 0000 720f 0100 0072  r....r....r....r
+000049d0: 6d00 0000 725a 0000 0072 5a00 0000 725b  m...rZ...rZ...r[
+000049e0: 0000 00da 096c 675f 756e 726f 6c6c 6903  .....lg_unrolli.
+000049f0: 0000 7308 0000 0000 1b0a 0114 0108 0172  ..s............r
+00004a00: 1601 0000 7a0a 2f70 6172 7469 7469 6f6e  ....z./partition
+00004a10: 7a3d 4966 2073 7065 6369 6669 6564 2c20  z=If specified, 
+00004a20: 7472 616e 736c 6174 6f72 2077 696c 6c20  translator will 
+00004a30: 6174 7465 6d70 7420 746f 206c 6f61 6420  attempt to load 
+00004a40: 6772 6170 6820 6672 6f6d 2066 696c 657a  graph from filez
+00004a50: 2f4e 756d 6265 7220 6f66 2070 6172 7469  /Number of parti
+00004a60: 7469 6f6e 7320 746f 2075 6e72 6f6c 6c20  tions to unroll 
+00004a70: 7468 6520 6772 6170 6820 6163 726f 7373  the graph across
+00004a80: 7a27 4e75 6d62 6572 206f 6620 6461 7461  z'Number of data
+00004a90: 2069 736c 616e 6473 2074 6f20 7061 7274   islands to part
+00004aa0: 6974 696f 6e20 666f 727a 2154 6865 2073  ition forz!The s
+00004ab0: 656c 6563 7465 6420 7363 6865 6475 6c69  elected scheduli
+00004ac0: 6e67 2061 6c67 6f72 6974 686d 7a62 5468  ng algorithmzbTh
+00004ad0: 6520 7061 7261 6d65 7465 7220 7661 6c75  e parameter valu
+00004ae0: 6573 2070 6173 7365 6420 746f 2074 6865  es passed to the
+00004af0: 2073 6368 6564 756c 696e 6720 616c 676f   scheduling algo
+00004b00: 7269 7468 6d2e 2052 6571 7569 7265 6420  rithm. Required 
+00004b10: 7061 7261 6d65 7465 7273 2076 6172 6965  parameters varie
+00004b20: 7320 7065 7220 616c 676f 7269 7468 6d2e  s per algorithm.
+00004b30: 2906 726a 0000 00da 0b70 6774 5f63 6f6e  ).rj.....pgt_con
+00004b40: 7465 6e74 72a6 0000 0072 8d00 0000 da09  tentr....r......
+00004b50: 616c 676f 7269 7468 6d72 b800 0000 6306  algorithmr....c.
+00004b60: 0000 0000 0000 0000 0000 0009 0000 0008  ................
+00004b70: 0000 0043 0000 0073 5800 0000 7400 7c01  ...C...sX...t.|.
+00004b80: 7c00 8302 7d06 6900 7d07 7c06 6401 1900  |...}.i.}.|.d...
+00004b90: a001 6402 a101 7324 7c06 a002 a100 7d07  ..d...s$|.....}.
+00004ba0: 7403 6a04 6a05 a006 7c06 7c04 7c02 7c03  t.j.j...|.|.|.|.
+00004bb0: 7c05 a007 a100 a105 7d08 7c08 a008 7c07  |.......}.|...|.
+00004bc0: a101 0100 7409 7c08 8301 7d08 740a 7c08  ....t.|...}.t.|.
+00004bd0: 8301 5300 2903 7ab3 0a20 2020 2055 7365  ..S.).z..    Use
+00004be0: 7320 7363 6865 6475 6c69 6e67 2061 6c67  s scheduling alg
+00004bf0: 6f72 6974 686d 7320 746f 2070 6172 7469  orithms to parti
+00004c00: 7469 6f6e 2061 6e20 756e 726f 6c6c 6564  tion an unrolled
+00004c10: 2070 6774 2061 6372 6f73 7320 7365 7665   pgt across seve
+00004c20: 7261 6c20 7061 7274 6974 696f 6e73 2061  ral partitions a
+00004c30: 6e64 2064 6174 6120 6973 6c61 6e64 732e  nd data islands.
+00004c40: 0a0a 2020 2020 4f6e 6520 6f66 2070 6774  ..    One of pgt
+00004c50: 5f6e 616d 6520 6f72 2070 6774 5f63 6f6e  _name or pgt_con
+00004c60: 7465 6e74 2c20 6275 7420 6e6f 7420 626f  tent, but not bo
+00004c70: 7468 2c20 6d75 7374 2062 6520 7370 6563  th, must be spec
+00004c80: 6966 6965 642e 0a20 2020 2072 c300 0000  ified..    r....
+00004c90: da03 6f69 6429 0b72 0801 0000 da03 6765  ..oid).r......ge
+00004ca0: 74da 0370 6f70 720b 0100 0072 0c01 0000  t..popr....r....
+00004cb0: 720d 0100 00da 0970 6172 7469 7469 6f6e  r......partition
+00004cc0: da04 6469 6374 72df 0000 0072 1d00 0000  ..dictr....r....
+00004cd0: 720e 0000 0029 0972 6a00 0000 7217 0100  r....).rj...r...
+00004ce0: 0072 a600 0000 728d 0000 0072 1801 0000  .r....r....r....
+00004cf0: 72b8 0000 00da 0567 7261 7068 72db 0000  r......graphr...
+00004d00: 0072 6d00 0000 725a 0000 0072 5a00 0000  .rm...rZ...rZ...
+00004d10: 725b 0000 00da 0d70 6774 5f70 6172 7469  r[.....pgt_parti
+00004d20: 7469 6f6e 8a03 0000 731c 0000 0000 1e0a  tion....s.......
+00004d30: 0104 010e 0108 0108 0102 0002 0002 0002  ................
+00004d40: 0006 ff04 030a 0108 0172 1f01 0000 7a15  .........r....z.
+00004d50: 2f75 6e72 6f6c 6c5f 616e 645f 7061 7274  /unroll_and_part
+00004d60: 6974 696f 6e29 0972 4000 0000 7241 0000  ition).r@...rA..
+00004d70: 0072 1201 0000 7213 0100 0072 1401 0000  .r....r....r....
+00004d80: 72a6 0000 0072 8d00 0000 7218 0100 0072  r....r....r....r
+00004d90: b800 0000 6309 0000 0000 0000 0000 0000  ....c...........
+00004da0: 000c 0000 0008 0000 0043 0000 0073 6200  .........C...sb.
+00004db0: 0000 7400 7c01 7c00 8302 7d09 7401 6a02  ..t.|.|...}.t.j.
+00004dc0: 6a03 a004 7c09 7c02 7c03 7c04 a104 7d0a  j...|.|.|.|...}.
+00004dd0: 7405 7c0a 8301 7d0a 7c0a a006 a100 7d0b  t.|...}.|.....}.
+00004de0: 7401 6a02 6a03 a007 7c0a 7c07 7c05 7c06  t.j.j...|.|.|.|.
+00004df0: 7c08 a008 a100 a105 7d0a 7c0a a009 7c0b  |.......}.|...|.
+00004e00: a101 0100 740a 7c0a 8301 7d0a 740b 7c0a  ....t.|...}.t.|.
+00004e10: 8301 5300 2901 7a9b 0a20 2020 2055 6e72  ..S.).z..    Unr
+00004e20: 6f6c 6c73 2061 6e64 2070 6172 7469 7469  olls and partiti
+00004e30: 6f6e 7320 6120 6c6f 6769 6361 6c20 6772  ons a logical gr
+00004e40: 6170 6820 7769 7468 2074 6865 2070 726f  aph with the pro
+00004e50: 7669 6465 6420 7661 7269 6f75 7320 7061  vided various pa
+00004e60: 7261 6d65 7465 7273 2e0a 0a20 2020 204f  rameters...    O
+00004e70: 6e65 206f 6620 6c67 5f6e 616d 6520 616e  ne of lg_name an
+00004e80: 6420 6c67 5f63 6f6e 7465 6e74 2c20 6275  d lg_content, bu
+00004e90: 7420 6e6f 7420 626f 7468 2c20 6d75 7374  t not both, must
+00004ea0: 2062 6520 7370 6563 6966 6965 642e 0a20   be specified.. 
+00004eb0: 2020 2029 0c72 0801 0000 720b 0100 0072     ).r....r....r
+00004ec0: 0c01 0000 720d 0100 0072 1501 0000 721e  ....r....r....r.
+00004ed0: 0000 0072 1b01 0000 721c 0100 0072 1d01  ...r....r....r..
+00004ee0: 0000 72df 0000 0072 1d00 0000 720e 0000  ..r....r....r...
+00004ef0: 0029 0c72 4000 0000 7241 0000 0072 1201  .).r@...rA...r..
+00004f00: 0000 7213 0100 0072 1401 0000 72a6 0000  ..r....r....r...
+00004f10: 0072 8d00 0000 7218 0100 0072 b800 0000  .r....r....r....
+00004f20: 720f 0100 0072 6d00 0000 72db 0000 0072  r....rm...r....r
+00004f30: 5a00 0000 725a 0000 0072 5b00 0000 da17  Z...rZ...r[.....
+00004f40: 6c67 5f75 6e72 6f6c 6c5f 616e 645f 7061  lg_unroll_and_pa
+00004f50: 7274 6974 696f 6eb4 0300 0073 1c00 0000  rtition....s....
+00004f60: 0029 0a01 1401 0801 0801 0801 0200 0200  .)..............
+00004f70: 0200 0200 06ff 0403 0a01 0801 7220 0100  ............r ..
+00004f80: 007a 042f 6d61 707a 4b49 6620 7375 7070  .z./mapzKIf supp
+00004f90: 6c69 6564 2c20 7468 6973 2067 7261 7068  lied, this graph
+00004fa0: 2077 696c 6c20 6174 7465 6d70 7465 6420   will attempted 
+00004fb0: 746f 2062 6520 6c6f 6164 6564 2066 726f  to be loaded fro
+00004fc0: 6d20 6469 736b 206f 6e20 7468 6520 7365  m disk on the se
+00004fd0: 7276 6572 7a26 4966 2073 7570 706c 6965  rverz&If supplie
+00004fe0: 642c 2074 6869 7320 6973 2074 6865 2067  d, this is the g
+00004ff0: 7261 7068 2063 6f6e 7465 6e74 7a3c 436f  raph contentz<Co
+00005000: 6d6d 6120 7365 7061 7261 7465 6420 6c69  mma separated li
+00005010: 7374 206f 6620 4950 2061 6464 7273 2065  st of IP addrs e
+00005020: 2e67 2e20 276c 6f63 616c 686f 7374 2c20  .g. 'localhost, 
+00005030: 3132 372e 302e 302e 3227 7a24 5468 6520  127.0.0.2'z$The 
+00005040: 6e75 6d62 6572 206f 6620 6461 7461 2069  number of data i
+00005050: 736c 616e 6473 2074 6f20 6c61 756e 6368  slands to launch
+00005060: 547a 4757 6865 7468 6572 2074 6f20 6c61  TzGWhether to la
+00005070: 756e 6368 2064 6174 6120 6973 6c61 6e64  unch data island
+00005080: 206d 616e 6167 6572 2070 726f 6365 7373   manager process
+00005090: 6573 2061 6c6f 6e67 7369 6465 206e 6f64  es alongside nod
+000050a0: 652d 6d61 6e61 6765 7273 7a40 4966 2070  e-managersz@If p
+000050b0: 7265 7365 6e74 2c20 7769 6c6c 2061 7474  resent, will att
+000050c0: 656d 7074 2074 6f20 7175 6572 7920 7468  empt to query th
+000050d0: 6973 2061 6464 7265 7373 2066 6f72 206e  is address for n
+000050e0: 6f64 652d 6d61 6e61 6765 7273 7a21 506f  ode-managersz!Po
+000050f0: 7274 2075 7365 6420 6279 2048 4f53 5420  rt used by HOST 
+00005100: 6d61 6e61 6765 7220 7072 6f63 6573 7329  manager process)
+00005110: 0772 6a00 0000 7217 0100 0072 e000 0000  .rj...r....r....
+00005120: 728d 0000 00da 0b63 6f5f 686f 7374 5f64  r......co_host_d
+00005130: 696d 72cd 0000 0072 ce00 0000 6307 0000  imr....r....c...
+00005140: 0000 0000 0000 0000 000b 0000 0006 0000  ................
+00005150: 0043 0000 0073 aa00 0000 7c02 7320 7400  .C...s....|.s t.
+00005160: 7c05 7c06 6401 6402 8d03 7d07 7c05 6701  |.|.d.d...}.|.g.
+00005170: 7c07 a001 a100 1700 7d02 7402 7c02 8301  |.......}.t.|...
+00005180: 7c03 6b01 724e 7403 a004 6403 a101 0100  |.k.rNt...d.....
+00005190: 7405 6404 6405 7402 7c02 8301 7c03 6602  t.d.d.t.|...|.f.
+000051a0: 1600 6406 8d02 0100 7406 7c01 7c00 8302  ..d.....t.|.|...
+000051b0: 7d08 6900 7d09 7c08 6407 1900 a007 6408  }.i.}.|.d.....d.
+000051c0: a101 7372 7c08 a008 a100 7d09 7403 a009  ..sr|.....}.t...
+000051d0: 7c02 a101 0100 740a 6a0b 6a0c a00d 7c08  |.....t.j.j...|.
+000051e0: 7c02 7c03 7c04 a104 7d0a 7c0a a00e 7c09  |.|.|...}.|...|.
+000051f0: a101 0100 740f 7c0a 8301 7d0a 7410 7c0a  ....t.|...}.t.|.
+00005200: 8301 5300 2909 7a3a 0a20 2020 204d 6170  ..S.).z:.    Map
+00005210: 7320 7068 7973 6963 616c 2067 7261 7068  s physical graph
+00005220: 2074 656d 706c 6174 6573 2074 6f20 6e6f   templates to no
+00005230: 6465 2072 6573 6f75 7263 6573 2e0a 2020  de resources..  
+00005240: 2020 e90a 0000 0029 0172 cf00 0000 7a24    .....).r....z$
+00005250: 4e6f 7420 656e 6f75 6768 206e 6f64 6573  Not enough nodes
+00005260: 2074 6f20 6669 6c6c 2061 6c6c 2069 736c   to fill all isl
+00005270: 616e 6473 7248 0000 007a 3c23 6e6f 6465  andsrH...z<#node
+00005280: 7320 2825 6429 2073 686f 756c 6420 6265  s (%d) should be
+00005290: 206c 6172 6765 7220 7468 616e 2074 6865   larger than the
+000052a0: 206e 756d 6265 7220 6f66 2069 736c 616e   number of islan
+000052b0: 6473 2028 2564 2972 4400 0000 72c3 0000  ds (%d)rD...r...
+000052c0: 0072 1901 0000 2911 7217 0000 0072 e000  .r....).r....r..
+000052d0: 0000 725f 0000 0072 4c00 0000 7275 0000  ..r_...rL...ru..
+000052e0: 0072 0a00 0000 7208 0100 0072 1a01 0000  .r....r....r....
+000052f0: 721b 0100 0072 a300 0000 720b 0100 0072  r....r....r....r
+00005300: 0c01 0000 720d 0100 00da 0c72 6573 6f75  ....r......resou
+00005310: 7263 655f 6d61 7072 df00 0000 721f 0000  rce_mapr....r...
+00005320: 0072 0e00 0000 290b 726a 0000 0072 1701  .r....).rj...r..
+00005330: 0000 72e0 0000 0072 8d00 0000 7221 0100  ..r....r....r!..
+00005340: 0072 cd00 0000 72ce 0000 00da 0663 6c69  .r....r......cli
+00005350: 656e 7472 6d00 0000 72db 0000 00da 0270  entrm...r......p
+00005360: 6772 5a00 0000 725a 0000 0072 5b00 0000  grZ...rZ...r[...
+00005370: da07 7067 745f 6d61 70e9 0300 0073 2800  ..pgt_map....s(.
+00005380: 0000 0020 0401 0e01 0e01 0c01 0a01 0201  ... ............
+00005390: 0201 0201 0aff 02fe 0605 0a01 0401 0e01  ................
+000053a0: 0801 0a01 1401 0a01 0801 7226 0100 007a  ..........r&...z
+000053b0: 162f 6170 692f 7375 626d 6973 7369 6f6e  ./api/submission
+000053c0: 5f6d 6574 686f 647a 4549 6620 7072 6573  _methodzEIf pres
+000053d0: 656e 742c 2074 7261 6e73 6c61 746f 7220  ent, translator 
+000053e0: 7769 6c6c 2071 7565 7279 2074 6869 7320  will query this 
+000053f0: 5552 4c20 666f 7220 6974 7320 6465 706c  URL for its depl
+00005400: 6f79 6d65 6e74 206f 7074 696f 6e73 7a47  oyment optionszG
+00005410: 4966 2070 7265 7365 6e74 2077 6974 6820  If present with 
+00005420: 6d70 6f72 7420 616e 6420 6d70 7265 6669  mport and mprefi
+00005430: 782c 2077 696c 6c20 6265 2074 6865 2062  x, will be the b
+00005440: 6173 6520 686f 7374 2066 6f72 2064 6570  ase host for dep
+00005450: 6c6f 796d 656e 7472 9900 0000 2903 72bb  loymentr....).r.
+00005460: 0000 0072 bc00 0000 72bd 0000 0063 0300  ...r....r....c..
+00005470: 0000 0000 0000 0000 0000 0700 0000 0400  ................
+00005480: 0000 4300 0000 7368 0000 0074 00a0 0164  ..C...sh...t...d
+00005490: 01a1 0101 007c 0072 1e74 027c 0083 015c  .....|.r.t.|...\
+000054a0: 037d 037d 047d 056e 0c7c 017d 037c 027d  .}.}.}.n.|.}.|.}
+000054b0: 0464 027d 0567 007d 0674 0383 0072 407c  .d.}.g.}.t...r@|
+000054c0: 06a0 0474 056a 06a1 0101 007c 0364 006b  ...t.j.....|.d.k
+000054d0: 0972 5474 077c 037c 047c 0583 037d 0674  .rTt.|.|.|...}.t
+000054e0: 00a0 0164 037c 06a1 0201 0064 047c 0669  ...d.|.....d.|.i
+000054f0: 0153 0029 054e 7a22 5265 6365 6976 6564  .S.).Nz"Received
+00005500: 2073 7562 6d69 7373 696f 6e5f 6d65 7468   submission_meth
+00005510: 6f64 2072 6571 7565 7374 7299 0000 007a  od requestr....z
+00005520: 154d 6574 686f 6473 2061 7661 696c 6162  .Methods availab
+00005530: 6c65 3a20 2573 da07 6d65 7468 6f64 7329  le: %s..methods)
+00005540: 0872 4c00 0000 72d8 0000 0072 3100 0000  .rL...r....r1...
+00005550: 7222 0000 0072 df00 0000 7221 0000 005a  r"...r....r!...Z
+00005560: 0448 454c 4d72 3000 0000 2907 72bb 0000  .HELMr0...).r...
+00005570: 0072 bc00 0000 72bd 0000 0072 eb00 0000  .r....r....r....
+00005580: 72ea 0000 0072 e900 0000 da11 6176 6169  r....r......avai
+00005590: 6c61 626c 655f 6d65 7468 6f64 7372 5a00  lable_methodsrZ.
+000055a0: 0000 725a 0000 0072 5b00 0000 da15 6765  ..rZ...r[.....ge
+000055b0: 745f 7375 626d 6973 7369 6f6e 5f6d 6574  t_submission_met
+000055c0: 686f 641e 0400 0073 1a00 0000 000c 0a01  hod....s........
+000055d0: 0401 1002 0401 0401 0401 0401 0601 0c01  ................
+000055e0: 0801 0c01 0c01 7229 0100 0072 5d00 0000  ......r)...r]...
+000055f0: 7a25 5468 6520 7061 6765 2075 7365 6420  z%The page used 
+00005600: 746f 2076 6965 7720 7068 7973 6963 616c  to view physical
+00005610: 2067 7261 7068 7329 0272 6900 0000 7233   graphs).ri...r3
+00005620: 0000 0029 0172 6f00 0000 6301 0000 0000  ...).ro...c.....
+00005630: 0000 0000 0000 0002 0000 0009 0000 0043  ...............C
+00005640: 0000 0073 1c00 0000 7400 a001 6401 7c00  ...s....t...d.|.
+00005650: 6400 6400 6402 6400 6403 9c05 a102 7d01  d.d.d.d.d.....}.
+00005660: 7c01 5300 2904 4e72 7100 0000 7272 0000  |.S.).Nrq...rr..
+00005670: 0072 7300 0000 727f 0000 0029 0272 6f00  .rs...r....).ro.
+00005680: 0000 727a 0000 0072 5a00 0000 725a 0000  ..rz...rZ...rZ..
+00005690: 0072 5b00 0000 da05 696e 6465 783a 0400  .r[.....index:..
+000056a0: 0073 1400 0000 0006 0401 0202 0201 0201  .s..............
+000056b0: 0201 0201 02fb 04fe 040a 722a 0100 0063  ..........r*...c
+000056c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000056d0: 0100 0000 4300 0000 7304 0000 0069 0053  ....C...s....i.S
+000056e0: 00a9 014e 725a 0000 0072 5a00 0000 725a  ...NrZ...rZ...rZ
+000056f0: 0000 0072 5a00 0000 725b 0000 00da 0a6c  ...rZ...r[.....l
+00005700: 6976 656c 696e 6573 734d 0400 0073 0200  ivelinessM...s..
+00005710: 0000 0002 722c 0100 0063 0200 0000 0000  ....r,...c......
+00005720: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
+00005730: 0000 731e 0200 0074 00a0 01a1 007d 027c  ..s....t.....}.|
+00005740: 026a 0264 0164 0264 0374 0364 0464 0564  .j.d.d.d.t.d.d.d
+00005750: 0664 078d 0701 007c 026a 0264 0864 0964  .d.....|.j.d.d.d
+00005760: 0374 0364 0a64 0564 0b64 078d 0701 007c  .t.d.d.d.d.....|
+00005770: 026a 0264 0c64 0d64 0374 0364 0e64 0f64  .j.d.d.d.t.d.d.d
+00005780: 1064 078d 0701 007c 026a 0264 1164 1264  .d.....|.j.d.d.d
+00005790: 0374 0464 1364 1464 1564 078d 0701 007c  .t.d.d.d.d.....|
+000057a0: 026a 0264 1664 1764 1864 1964 1a64 1b64  .j.d.d.d.d.d.d.d
+000057b0: 1c8d 0601 007c 026a 0264 1d64 1e64 0374  .....|.j.d.d.d.t
+000057c0: 0364 1f64 2074 05a0 06a1 0064 218d 0701  .d.d t.....d!...
+000057d0: 007c 02a0 077c 01a1 017d 037c 036a 0864  .|...|...}.|.j.d
+000057e0: 226b 0873 b87c 036a 0964 226b 0872 c47c  "k.s.|.j.d"k.r.|
+000057f0: 02a0 0a64 23a1 0101 006e 2074 0b6a 0ca0  ...d#....n t.j..
+00005800: 0d7c 036a 08a1 0173 e47c 02a0 0a7c 036a  .|.j...s.|...|.j
+00005810: 089b 0064 249d 02a1 0101 007c 036a 0e73  ...d$......|.j.s
+00005820: f27c 036a 0f90 0172 8274 10a0 1164 25a1  .|.j...r.t...d%.
+00005830: 017d 0474 126a 137c 045f 147c 036a 0e90  .}.t.j.|._.|.j..
+00005840: 0172 3c74 10a0 1574 166a 17a1 017d 057c  .r<t...t.j...}.|
+00005850: 05a0 187c 04a1 0101 0074 106a 19a0 1a7c  ...|.....t.j...|
+00005860: 05a1 0101 0074 106a 19a0 1b74 106a 1ca1  .....t.j...t.j..
+00005870: 0101 007c 036a 0f90 0172 827c 036a 0f7d  ...|.j...r.|.j.}
+00005880: 0674 05a0 1d7c 06a1 0101 0074 0b6a 0ca0  .t...|.....t.j..
+00005890: 1e7c 0664 26a1 027d 0774 10a0 1f7c 07a1  .|.d&..}.t...|..
+000058a0: 017d 087c 08a0 187c 04a1 0101 0074 106a  .}.|...|.....t.j
+000058b0: 19a0 1a7c 08a1 0101 007a 1474 0b6a 207c  ...|.....z.t.j |
+000058c0: 036a 0964 2764 288d 0201 0057 006e 2404  .j.d'd(....W.n$.
+000058d0: 0074 216b 0a90 0172 ba01 0001 0001 0074  .t!k...r.......t
+000058e0: 10a0 2264 297c 036a 09a1 0201 0059 006e  .."d)|.j.....Y.n
+000058f0: 0258 007c 036a 0861 237c 036a 0961 2474  .X.|.j.a#|.j.a$t
+00005900: 2574 2483 0161 2664 2a64 2b84 007d 0974  %t$..a&d*d+..}.t
+00005910: 27a0 2774 276a 287c 09a1 0201 0074 27a0  '.'t'j(|.....t'.
+00005920: 2774 276a 297c 09a1 0201 0074 10a0 2a64  't'j)|.....t..*d
+00005930: 2c7c 036a 0ea1 0201 0074 2b6a 2c74 2d7c  ,|.j.....t+j,t-|
+00005940: 036a 2e7c 036a 2f7c 036a 0e64 2d8d 0401  .j.|.j/|.j.d-...
+00005950: 0064 2253 0029 2e7a 400a 2020 2020 4661  .d"S.).z@.    Fa
+00005960: 7374 4150 4920 696d 706c 656d 656e 7461  stAPI implementa
+00005970: 7469 6f6e 206f 6620 6461 6c69 7567 6520  tion of daliuge 
+00005980: 7472 616e 736c 6174 6f72 2069 6e74 6572  translator inter
+00005990: 6661 6365 0a20 2020 207a 022d 647a 072d  face.    z.-dz.-
+000059a0: 2d6c 6764 6972 da05 7374 6f72 6572 2800  -lgdir..storer(.
+000059b0: 0000 7a04 2f74 6d70 7a53 4120 7061 7468  ..z./tmpzSA path
+000059c0: 2074 6861 7420 636f 6e74 6169 6e73 2061   that contains a
+000059d0: 7420 6c65 6173 7420 6f6e 6520 7375 622d  t least one sub-
+000059e0: 6469 7265 6374 6f72 792c 2077 6869 6368  directory, which
+000059f0: 2063 6f6e 7461 696e 7320 6c6f 6769 6361   contains logica
+00005a00: 6c20 6772 6170 6820 6669 6c65 7329 05da  l graph files)..
+00005a10: 0661 6374 696f 6eda 0474 7970 65da 0464  .action..type..d
+00005a20: 6573 7472 3f00 0000 da04 6865 6c70 7a02  estr?.....helpz.
+00005a30: 2d74 7a08 2d2d 7067 7464 6972 722b 0000  -tz.--pgtdirr+..
+00005a40: 007a 2570 6879 7369 6361 6c20 6772 6170  .z%physical grap
+00005a50: 6820 7465 6d70 6c61 7465 2070 6174 6820  h template path 
+00005a60: 286f 7574 7075 7429 7a02 2d48 7a06 2d2d  (output)z.-Hz.--
+00005a70: 686f 7374 72cd 0000 007a 0730 2e30 2e30  hostr....z.0.0.0
+00005a80: 2e30 7a2a 6c6f 6769 6361 6c20 6772 6170  .0z*logical grap
+00005a90: 6820 6564 6974 6f72 2068 6f73 7420 2861  h editor host (a
+00005aa0: 6c6c 2062 7920 6465 6661 756c 7429 7a02  ll by default)z.
+00005ab0: 2d70 7a06 2d2d 706f 7274 72ce 0000 0069  -pz.--portr....i
+00005ac0: 941f 0000 7a2b 6c6f 6769 6361 6c20 6772  ....z+logical gr
+00005ad0: 6170 6820 6564 6974 6f72 2070 6f72 7420  aph editor port 
+00005ae0: 2838 3038 3420 6279 2064 6566 6175 6c74  (8084 by default
+00005af0: 297a 022d 767a 092d 2d76 6572 626f 7365  )z.-vz.--verbose
+00005b00: da0a 7374 6f72 655f 7472 7565 da07 7665  ..store_true..ve
+00005b10: 7262 6f73 6546 7a13 456e 6162 6c65 206d  rboseFz.Enable m
+00005b20: 6f72 6520 6c6f 6767 696e 6729 0472 2e01  ore logging).r..
+00005b30: 0000 7230 0100 0072 3f00 0000 7231 0100  ..r0...r?...r1..
+00005b40: 007a 022d 6c7a 092d 2d6c 6f67 2d64 6972  .z.-lz.--log-dir
+00005b50: da06 6c6f 6764 6972 7a34 5468 6520 6469  ..logdirz4The di
+00005b60: 7265 6374 6f72 7920 7768 6572 6520 7468  rectory where th
+00005b70: 6520 6c6f 6767 696e 6720 6669 6c65 7320  e logging files 
+00005b80: 7769 6c6c 2062 6520 7374 6f72 6564 2905  will be stored).
+00005b90: 722e 0100 0072 2f01 0000 7230 0100 0072  r....r/...r0...r
+00005ba0: 3101 0000 723f 0000 004e 7a1b 4772 6170  1...r?...Nz.Grap
+00005bb0: 6820 7061 7468 7320 6d69 7373 696e 6720  h paths missing 
+00005bc0: 282d 642f 2d74 297a 0f20 646f 6573 206e  (-d/-t)z. does n
+00005bd0: 6f74 2065 7869 7374 7a64 2528 6173 6374  ot existzd%(asct
+00005be0: 696d 6529 2d31 3573 205b 2528 6c65 7665  ime)-15s [%(leve
+00005bf0: 6c6e 616d 6529 352e 3573 5d20 5b25 2874  lname)5.5s] [%(t
+00005c00: 6872 6561 644e 616d 6529 3135 2e31 3573  hreadName)15.15s
+00005c10: 5d20 2528 6e61 6d65 2973 2325 2866 756e  ] %(name)s#%(fun
+00005c20: 634e 616d 6529 733a 2528 6c69 6e65 6e6f  cName)s:%(lineno
+00005c30: 2973 2025 286d 6573 7361 6765 2973 7a11  )s %(message)sz.
+00005c40: 646c 6754 7261 6e73 6c61 746f 722e 6c6f  dlgTranslator.lo
+00005c50: 6754 2901 da08 6578 6973 745f 6f6b 7a15  gT)...exist_okz.
+00005c60: 4361 6e6e 6f74 2063 7265 6174 6520 7061  Cannot create pa
+00005c70: 7468 2025 7363 0000 0000 0000 0000 0000  th %sc..........
+00005c80: 0000 0100 0000 0100 0000 5700 0000 7308  ..........W...s.
+00005c90: 0000 0074 0082 0164 0053 0072 2b01 0000  ...t...d.S.r+...
+00005ca0: 2901 da11 4b65 7962 6f61 7264 496e 7465  )...KeyboardInte
+00005cb0: 7272 7570 7429 01da 055f 6172 6773 725a  rrupt)..._argsrZ
+00005cc0: 0000 0072 5a00 0000 725b 0000 00da 0768  ...rZ...r[.....h
+00005cd0: 616e 646c 6572 b504 0000 7302 0000 0000  andler....s.....
+00005ce0: 017a 1472 756e 2e3c 6c6f 6361 6c73 3e2e  .z.run.<locals>.
+00005cf0: 6861 6e64 6c65 727a 1b53 7461 7274 696e  handlerz.Startin
+00005d00: 6720 7576 6963 6f72 6e20 7665 7262 6f73  g uvicorn verbos
+00005d10: 6520 2573 2904 da03 6170 7072 cd00 0000  e %s)...appr....
+00005d20: 72ce 0000 0072 d800 0000 2930 da08 6172  r....r....)0..ar
+00005d30: 6770 6172 7365 da0e 4172 6775 6d65 6e74  gparse..Argument
+00005d40: 5061 7273 6572 da0c 6164 645f 6172 6775  Parser..add_argu
+00005d50: 6d65 6e74 7258 0000 0072 d400 0000 7220  mentrX...r....r 
+00005d60: 0000 00da 0d67 6574 446c 674c 6f67 7344  .....getDlgLogsD
+00005d70: 6972 da0a 7061 7273 655f 6172 6773 7228  ir..parse_argsr(
+00005d80: 0000 0072 2b00 0000 7275 0000 0072 7600  ...r+...ru...rv.
+00005d90: 0000 72d6 0000 00da 0665 7869 7374 7372  ..r......existsr
+00005da0: 3301 0000 7234 0100 00da 076c 6f67 6769  3...r4.....loggi
+00005db0: 6e67 da09 466f 726d 6174 7465 72da 0474  ng..Formatter..t
+00005dc0: 696d 65da 0667 6d74 696d 65da 0963 6f6e  ime..gmtime..con
+00005dd0: 7665 7274 6572 da0d 5374 7265 616d 4861  verter..StreamHa
+00005de0: 6e64 6c65 72da 0373 7973 da06 7374 646f  ndler..sys..stdo
+00005df0: 7574 da0c 7365 7446 6f72 6d61 7474 6572  ut..setFormatter
+00005e00: da04 726f 6f74 da0a 6164 6448 616e 646c  ..root..addHandl
+00005e10: 6572 da08 7365 744c 6576 656c da05 4445  er..setLevel..DE
+00005e20: 4255 47da 1263 7265 6174 6544 6972 4966  BUG..createDirIf
+00005e30: 4d69 7373 696e 6772 a100 0000 da0b 4669  Missingr......Fi
+00005e40: 6c65 4861 6e64 6c65 72da 086d 616b 6564  leHandler..maked
+00005e50: 6972 73da 074f 5345 7272 6f72 724d 0000  irs..OSErrorrM..
+00005e60: 0072 4900 0000 726b 0000 0072 2400 0000  .rI...rk...r$...
+00005e70: 7282 0000 00da 0673 6967 6e61 6cda 0753  r......signal..S
+00005e80: 4947 5445 524d da06 5349 4749 4e54 72d8  IGTERM..SIGINTr.
+00005e90: 0000 00da 0775 7669 636f 726e da03 7275  .....uvicorn..ru
+00005ea0: 6e72 3901 0000 72cd 0000 0072 ce00 0000  nr9...r....r....
+00005eb0: 290a da01 5fda 0461 7267 73da 0670 6172  )..._..args..par
+00005ec0: 7365 72da 076f 7074 696f 6e73 da03 666d  ser..options..fm
+00005ed0: 745a 0e73 7472 6561 6d5f 6861 6e64 6c65  tZ.stream_handle
+00005ee0: 7272 3401 0000 da07 6c6f 6766 696c 655a  rr4.....logfileZ
+00005ef0: 0b66 696c 6548 616e 646c 6572 7238 0100  .fileHandlerr8..
+00005f00: 0072 5a00 0000 725a 0000 0072 5b00 0000  .rZ...rZ...r[...
+00005f10: 7255 0100 0052 0400 0073 b000 0000 0004  rU...R...s......
+00005f20: 0801 0401 0201 0201 0201 0201 0201 0201  ................
+00005f30: 02f9 0609 0401 0201 0201 0201 0201 0201  ................
+00005f40: 0201 02f9 0609 0401 0201 0201 0201 0201  ................
+00005f50: 0201 0201 02f9 0609 0401 0201 0201 0201  ................
+00005f60: 0201 0201 0201 02f9 0609 0401 0201 0201  ................
+00005f70: 0201 0201 0201 02fa 0608 0401 0201 0201  ................
+00005f80: 0201 0201 0201 0201 06f9 060a 0a02 1401  ................
+00005f90: 0c01 0e01 1202 0e01 0401 02ff 0404 0801  ................
+00005fa0: 0801 0c01 0a01 0c01 0e01 0802 0601 0a01  ................
+00005fb0: 0e01 0a01 0a01 0c02 0201 1401 1001 1406  ................
+00005fc0: 0601 0601 0802 0803 0e01 0e02 0e01 7255  ..............rU
+00005fd0: 0100 00da 085f 5f6d 6169 6e5f 5f29 8a72  .....__main__).r
+00005fe0: 3a01 0000 72e1 0000 0072 4a00 0000 7240  :...r....rJ...r@
+00005ff0: 0100 0072 7600 0000 724e 0000 0072 5101  ...rv...rN...rQ.
+00006000: 0000 7246 0100 00da 0974 6872 6561 6469  ..rF.....threadi
+00006010: 6e67 7242 0100 0072 a400 0000 7209 0100  ngrB...r....r...
+00006020: 0072 0200 0000 7203 0000 00da 0674 7970  .r....r......typ
+00006030: 696e 6772 0400 0000 da0c 7572 6c6c 6962  ingr......urllib
+00006040: 2e70 6172 7365 7205 0000 0072 5401 0000  .parser....rT...
+00006050: 5a07 6661 7374 6170 6972 0600 0000 7207  Z.fastapir....r.
+00006060: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00006070: 0000 720b 0000 005a 1166 6173 7461 7069  ..r....Z.fastapi
+00006080: 2e72 6573 706f 6e73 6573 720c 0000 0072  .responsesr....r
+00006090: 0d00 0000 720e 0000 0072 0f00 0000 5a13  ....r....r....Z.
+000060a0: 6661 7374 6170 692e 7374 6174 6963 6669  fastapi.staticfi
+000060b0: 6c65 7372 1000 0000 5a12 6661 7374 6170  lesr....Z.fastap
+000060c0: 692e 7465 6d70 6c61 7469 6e67 7211 0000  i.templatingr...
+000060d0: 005a 0a6a 736f 6e73 6368 656d 6172 1200  .Z.jsonschemar..
+000060e0: 0000 7213 0000 005a 0870 7964 616e 7469  ..r....Z.pydanti
+000060f0: 6372 1400 0000 da0d 646c 672e 636f 6e73  cr......dlg.cons
+00006100: 7461 6e74 7372 0b01 0000 5a19 646c 672e  tantsr....Z.dlg.
+00006110: 6472 6f70 6d61 6b65 2e70 675f 6765 6e65  dropmake.pg_gene
+00006120: 7261 746f 7272 1500 0000 7216 0000 00da  ratorr....r.....
+00006130: 0b64 6c67 2e63 6c69 656e 7473 7217 0000  .dlg.clientsr...
+00006140: 00da 2464 6c67 2e63 6f6d 6d6f 6e2e 7265  ..$dlg.common.re
+00006150: 7072 6f64 7563 6962 696c 6974 792e 636f  producibility.co
+00006160: 6e73 7461 6e74 7372 1800 0000 7219 0000  nstantsr....r...
+00006170: 0072 1a00 0000 da2a 646c 672e 636f 6d6d  .r.....*dlg.comm
+00006180: 6f6e 2e72 6570 726f 6475 6369 6269 6c69  on.reproducibili
+00006190: 7479 2e72 6570 726f 6475 6369 6269 6c69  ty.reproducibili
+000061a0: 7479 721b 0000 0072 1c00 0000 721d 0000  tyr....r....r...
+000061b0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+000061c0: 5a1d 646c 672e 636f 6d6d 6f6e 2e64 6570  Z.dlg.common.dep
+000061d0: 6c6f 796d 656e 745f 6d65 7468 6f64 7372  loyment_methodsr
+000061e0: 2100 0000 5a14 646c 672e 636f 6d6d 6f6e  !...Z.dlg.common
+000061f0: 2e6b 3873 5f75 7469 6c73 7222 0000 005a  .k8s_utilsr"...Z
+00006200: 0f64 6c67 2e64 726f 706d 616b 652e 6c67  .dlg.dropmake.lg
+00006210: 7223 0000 005a 1764 6c67 2e64 726f 706d  r#...Z.dlg.dropm
+00006220: 616b 652e 7067 5f6d 616e 6167 6572 7224  ake.pg_managerr$
+00006230: 0000 005a 1664 6c67 2e64 726f 706d 616b  ...Z.dlg.dropmak
+00006240: 652e 7363 6865 6475 6c65 7272 2500 0000  e.schedulerr%...
+00006250: 5a21 646c 672e 6472 6f70 6d61 6b65 2e77  Z!dlg.dropmake.w
+00006260: 6562 2e74 7261 6e73 6c61 746f 725f 7574  eb.translator_ut
+00006270: 696c 7372 2600 0000 7227 0000 0072 2800  ilsr&...r'...r(.
+00006280: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
+00006290: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
+000062a0: 722f 0000 0072 3000 0000 7231 0000 005a  r/...r0...r1...Z
+000062b0: 0f41 5050 5f44 4553 4352 4950 5449 4f4e  .APP_DESCRIPTION
+000062c0: 5a11 4150 505f 5441 4753 5f4d 4554 4144  Z.APP_TAGS_METAD
+000062d0: 4154 4172 4f00 0000 da08 5f5f 6669 6c65  ATArO.....__file
+000062e0: 5f5f da06 7061 7265 6e74 da08 6162 736f  __..parent..abso
+000062f0: 6c75 7465 5a0d 6669 6c65 5f6c 6f63 6174  luteZ.file_locat
+00006300: 696f 6e72 7800 0000 7239 0000 0072 3901  ionrx...r9...r9.
+00006310: 0000 da05 6d6f 756e 74da 0967 6574 4c6f  ....mount..getLo
+00006320: 6767 6572 72fd 0000 0072 4c00 0000 da09  ggerr....rL.....
+00006330: 5365 6d61 7068 6f72 6572 5000 0000 5a0b  SemaphorerP...Z.
+00006340: 6765 6e5f 7067 745f 7365 6d72 4b00 0000  gen_pgt_semrK...
+00006350: 72b5 0000 00da 0470 6f73 7472 5800 0000  r......postrX...
+00006360: da05 7661 6c75 6572 5c00 0000 721a 0100  ..valuer\...r...
+00006370: 0072 6800 0000 726e 0000 0072 7b00 0000  .rh...rn...r{...
+00006380: 7281 0000 0072 8300 0000 7286 0000 0072  r....r....r....r
+00006390: 8700 0000 72d4 0000 0072 aa00 0000 72b9  ....r....r....r.
+000063a0: 0000 0072 f300 0000 72dc 0000 0072 f800  ...r....r....r..
+000063b0: 0000 72fb 0000 0072 fc00 0000 7202 0100  ..r....r....r...
+000063c0: 0072 0801 0000 7232 0000 00da 074e 4f54  .r....r2.....NOT
+000063d0: 4849 4e47 7211 0100 00da 0462 6f6f 6c72  HINGr......boolr
+000063e0: 1601 0000 721f 0100 0072 2001 0000 da09  ....r....r .....
+000063f0: 636f 6e73 7461 6e74 73da 1849 534c 414e  constants..ISLAN
+00006400: 445f 4445 4641 554c 545f 5245 5354 5f50  D_DEFAULT_REST_P
+00006410: 4f52 5472 2601 0000 7229 0100 0072 2a01  ORTr&...r)...r*.
+00006420: 0000 da04 6865 6164 722c 0100 0072 5501  ....headr,...rU.
+00006430: 0000 da04 6172 6776 725a 0000 0072 5a00  ....argvrZ...rZ.
+00006440: 0000 725a 0000 0072 5b00 0000 da08 3c6d  ..rZ...r[.....<m
+00006450: 6f64 756c 653e 1700 0000 73ba 0300 0008  odule>....s.....
+00006460: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00006470: 0108 0108 010c 010c 010c 010c 0208 0120  ............... 
+00006480: 0118 060c 010c 0110 010c 0208 0108 0110  ................
+00006490: 010c 0114 051c 080c 010c 010c 010c 010c  ................
+000064a0: 010c 0138 0f04 1302 0102 fe04 0502 0102  ...8............
+000064b0: fe04 fb04 0b10 010a 0202 0102 0102 0102  ................
+000064c0: 0108 0106 0202 0102 fe04 fa06 0b16 010a  ................
+000064d0: 020a 010a 0512 030e 0208 0108 010e fd02  ................
+000064e0: 0102 0102 0102 fd0e 200e 0202 0102 0002  ........ .......
+000064f0: ff04 ff02 0102 ff0e 1d10 0208 ff02 0102  ................
+00006500: ff0e 1210 0302 0102 0002 ff04 fe02 0102  ................
+00006510: 0102 fe0e 2510 0302 0102 ff04 fe02 0102  ....%...........
+00006520: 0102 fe0e 140e 0202 0102 ff04 ff02 0102  ................
+00006530: ff0e 1210 0302 0102 ff04 fe02 0102 0102  ................
+00006540: fe0e 140e 0202 0102 ff04 ff02 0102 ff0e  ................
+00006550: 150e 0302 0102 ff04 0302 0108 0102 fe04  ................
+00006560: 0402 0102 0102 fe04 0402 0102 0002 ff04  ................
+00006570: 0302 0102 0102 fe04 0402 0102 0002 ff04  ................
+00006580: 0302 0102 0102 fe04 e902 0102 0102 0302  ................
+00006590: 0402 0402 0302 0402 0302 e90e 5510 0302  ............U...
+000065a0: 0102 ff04 0308 0102 0108 0102 fe04 0402  ................
+000065b0: 0102 0102 fe04 0402 0102 0102 fe04 0402  ................
+000065c0: 0102 0002 ff04 0302 0102 0002 ff04 0302  ................
+000065d0: 0102 0102 fe04 0408 0108 0108 0108 0108  ................
+000065e0: 0108 0108 0108 0108 dc02 0102 0102 0302  ................
+000065f0: 0102 0402 0402 0402 0302 0302 040a 010a  ................
+00006600: 010a 010a 010a 010a 010a 010a 010a dc0e  ................
+00006610: 7110 0302 0102 ff04 0302 0102 0102 fe04  q...............
+00006620: 0402 0102 0002 ff04 0302 0102 0102 fe04  ................
+00006630: 0402 0102 0102 fe04 0402 0102 0102 fe04  ................
+00006640: ec02 0102 0102 030a 040a 030a 040a 0402  ................
+00006650: ec0e 7f0e 0202 0102 ff04 0302 0102 0102  ................
+00006660: fe04 0402 0102 ff04 0302 0102 0102 fe04  ................
+00006670: f502 0102 0302 0402 0302 f50e 3f0e 0202  ............?...
+00006680: 0102 ff04 ff02 0102 ff0e 2710 1112 0d10  ..........'.....
+00006690: 1d10 0202 0102 0102 fe04 0402 0102 0102  ................
+000066a0: fe04 0402 0102 0002 ff04 0302 0104 0114  ................
+000066b0: 0102 fd04 f402 0102 0402 0402 0302 f40e  ................
+000066c0: 2210 0202 0102 0102 fe04 0402 0102 0102  "...............
+000066d0: fe04 0402 0102 0002 ff04 0302 0102 0102  ................
+000066e0: fe04 0402 0102 0102 fe04 f002 0102 0402  ................
+000066f0: 0402 0302 0402 f00e 2010 0202 0102 0102  ........ .......
+00006700: fe04 0402 0102 0102 fe04 0402 0102 0102  ................
+00006710: fe04 0402 0102 0002 ff04 0302 0102 0002  ................
+00006720: ff04 0302 0104 0102 fe04 ed02 0102 0402  ................
+00006730: 0402 0402 0302 0302 ed0e 2910 0202 0102  ..........).....
+00006740: 0102 fe04 0402 0102 0102 fe04 0402 0102  ................
+00006750: 0002 ff04 0302 0102 0102 fe04 0402 0102  ................
+00006760: 0102 fe04 0402 0102 0102 fe04 0402 0102  ................
+00006770: 0002 ff04 0302 0102 0002 ff04 0302 0104  ................
+00006780: 0102 fe04 e202 0102 0402 0402 0302 0402  ................
+00006790: 0402 0402 0302 0302 e20e 3410 0202 0102  ..........4.....
+000067a0: 0102 fe04 0402 0102 0002 ff04 0302 0102  ................
+000067b0: 0102 fe04 0402 0102 0002 ff04 0302 0102  ................
+000067c0: 0102 fe04 0402 0102 0102 fe04 0402 0106  ................
+000067d0: 0102 fe04 e902 0102 0402 0302 0402 0302  ................
+000067e0: 0402 0402 e90e 3408 0202 0102 0102 fe04  ......4.........
+000067f0: 0402 0102 0102 fe04 040a f702 0102 0402  ................
+00006800: 0402 f70e 1b04 0102 0102 0102 fd04 0510  ................
+00006810: 0e08 010a 0408 6d0a 01                   ......m..
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_rest.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-37.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May  9 13:46:34 2023 UTC, .py size: 4718 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ba4e 5a64 6e12 0000  U........NZdn...
+00000000: 550d 0d0a 0000 0000 735d 1966 7a12 0000  U.......s].fz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
@@ -48,52 +48,52 @@
 000002f0: 6f72 6d61 74a9 02da 066c 675f 6469 72da  ormat....lg_dir.
 00000300: 076c 675f 6e61 6d65 a900 721c 0000 00fa  .lg_name..r.....
 00000310: 522f 686f 6d65 2f61 7769 6365 6e65 632f  R/home/awicenec/
 00000320: 6769 742f 6461 6c69 7567 652f 6461 6c69  git/daliuge/dali
 00000330: 7567 652d 7472 616e 736c 6174 6f72 2f64  uge-translator/d
 00000340: 6c67 2f64 726f 706d 616b 652f 7765 622f  lg/dropmake/web/
 00000350: 7472 616e 736c 6174 6f72 5f75 7469 6c73  translator_utils
-00000360: 2e70 79da 076c 675f 7061 7468 1d00 0000  .py..lg_path....
+00000360: 2e70 79da 076c 675f 7061 7468 2100 0000  .py..lg_path!...
 00000370: 7302 0000 0000 0172 1e00 0000 6302 0000  s......r....c...
 00000380: 0000 0000 0000 0000 0002 0000 0005 0000  ................
 00000390: 0043 0000 0073 1200 0000 7400 6a01 a002  .C...s....t.j...
 000003a0: 7403 7c00 7c01 8302 a101 5300 a901 4e29  t.|.|.....S...N)
 000003b0: 04da 026f 73da 0470 6174 68da 0665 7869  ...os..path..exi
 000003c0: 7374 7372 1e00 0000 7219 0000 0072 1c00  stsr....r....r..
 000003d0: 0000 721c 0000 0072 1d00 0000 da09 6c67  ..r....r......lg
-000003e0: 5f65 7869 7374 7321 0000 0073 0200 0000  _exists!...s....
+000003e0: 5f65 7869 7374 7325 0000 0073 0200 0000  _exists%...s....
 000003f0: 0001 7223 0000 0063 0200 0000 0000 0000  ..r#...c........
 00000400: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
 00000410: 730c 0000 0064 01a0 007c 007c 01a1 0253  s....d...|.|...S
 00000420: 0072 1600 0000 7217 0000 00a9 02da 0770  .r....r........p
-00000430: 6774 5f64 6972 5a08 7067 745f 6e61 6d65  gt_dirZ.pgt_name
+00000430: 6774 5f64 6972 da08 7067 745f 6e61 6d65  gt_dir..pgt_name
 00000440: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00000450: 0870 6774 5f70 6174 6825 0000 0073 0200  .pgt_path%...s..
-00000460: 0000 0001 7226 0000 0063 0200 0000 0000  ....r&...c......
+00000450: 0870 6774 5f70 6174 6829 0000 0073 0200  .pgt_path)...s..
+00000460: 0000 0001 7227 0000 0063 0200 0000 0000  ....r'...c......
 00000470: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
 00000480: 0000 7312 0000 0074 006a 01a0 0274 037c  ..s....t.j...t.|
 00000490: 007c 0183 02a1 0153 0072 1f00 0000 2904  .|.....S.r....).
 000004a0: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-000004b0: 2600 0000 7224 0000 0072 1c00 0000 721c  &...r$...r....r.
+000004b0: 2700 0000 7224 0000 0072 1c00 0000 721c  '...r$...r....r.
 000004c0: 0000 0072 1d00 0000 da0a 7067 745f 6578  ...r......pgt_ex
-000004d0: 6973 7473 2900 0000 7302 0000 0000 0172  ists)...s......r
-000004e0: 2700 0000 6301 0000 0000 0000 0000 0000  '...c...........
+000004d0: 6973 7473 2d00 0000 7302 0000 0000 0172  ists-...s......r
+000004e0: 2800 0000 6301 0000 0000 0000 0000 0000  (...c...........
 000004f0: 0001 0000 0002 0000 0043 0000 0073 0800  .........C...s..
 00000500: 0000 7400 7c00 8301 5300 721f 0000 00a9  ..t.|...S.r.....
 00000510: 01da 0e5f 7265 706f 5f63 6f6e 7465 6e74  ..._repo_content
 00000520: 7329 0172 1a00 0000 721c 0000 0072 1c00  s).r....r....r..
 00000530: 0000 721d 0000 00da 106c 675f 7265 706f  ..r......lg_repo
-00000540: 5f63 6f6e 7465 6e74 732d 0000 0073 0200  _contents-...s..
-00000550: 0000 0001 722a 0000 0063 0100 0000 0000  ....r*...c......
+00000540: 5f63 6f6e 7465 6e74 7331 0000 0073 0200  _contents1...s..
+00000550: 0000 0001 722b 0000 0063 0100 0000 0000  ....r+...c......
 00000560: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
 00000570: 0000 7308 0000 0074 007c 0083 0153 0072  ..s....t.|...S.r
-00000580: 1f00 0000 7228 0000 0029 0172 2500 0000  ....r(...).r%...
+00000580: 1f00 0000 7229 0000 0029 0172 2500 0000  ....r)...).r%...
 00000590: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
 000005a0: 1170 6774 5f72 6570 6f5f 636f 6e74 656e  .pgt_repo_conten
-000005b0: 7473 3100 0000 7302 0000 0000 0172 2b00  ts1...s......r+.
+000005b0: 7473 3500 0000 7302 0000 0000 0172 2c00  ts5...s......r,.
 000005c0: 0000 6301 0000 0000 0000 0000 0000 0007  ..c.............
 000005d0: 0000 0005 0000 0043 0000 0073 6000 0000  .......C...s`...
 000005e0: 7400 6a01 6a02 7d01 6900 7d02 7400 a003  t.j.j.}.i.}.t...
 000005f0: 7c00 a101 4400 5d44 5c03 7d03 7d04 7d05  |...D.]D\.}.}.}.
 00000600: 6401 7c04 6b06 7232 7c04 a004 6401 a101  d.|.k.r2|...d...
 00000610: 0100 7c03 7c00 6b02 723c 7116 6402 6403  ..|.|.k.r<q.d.d.
 00000620: 8400 7c05 4400 8301 7d06 7c06 7216 7c06  ..|.D...}.|.r.|.
@@ -101,121 +101,121 @@
 00000640: 2904 4e7a 042e 6769 7463 0100 0000 0000  ).Nz..gitc......
 00000650: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
 00000660: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
 00000670: 01a0 0064 00a1 0172 047c 0191 0271 0453  ...d...r.|...q.S
 00000680: 0029 017a 062e 6772 6170 6829 01da 0865  .).z..graph)...e
 00000690: 6e64 7377 6974 6829 02da 022e 30da 0166  ndswith)....0..f
 000006a0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-000006b0: 0a3c 6c69 7374 636f 6d70 3e41 0000 0073  .<listcomp>A...s
+000006b0: 0a3c 6c69 7374 636f 6d70 3e45 0000 0073  .<listcomp>E...s
 000006c0: 0600 0000 0600 0200 0a00 7a22 5f72 6570  ..........z"_rep
 000006d0: 6f5f 636f 6e74 656e 7473 2e3c 6c6f 6361  o_contents.<loca
 000006e0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2905  ls>.<listcomp>).
 000006f0: 7220 0000 0072 2100 0000 da08 6261 7365  r ...r!.....base
 00000700: 6e61 6d65 da04 7761 6c6b da06 7265 6d6f  name..walk..remo
 00000710: 7665 2907 da08 726f 6f74 5f64 6972 da01  ve)...root_dir..
 00000720: 62da 0863 6f6e 7465 6e74 73da 0764 6972  b..contents..dir
 00000730: 7061 7468 da08 6469 726e 616d 6573 da06  path..dirnames..
 00000740: 666e 616d 6573 da05 6669 6c65 7372 1c00  fnames..filesr..
-00000750: 0000 721c 0000 0072 1d00 0000 7229 0000  ..r....r....r)..
-00000760: 0035 0000 0073 1600 0000 0002 0801 0401  .5...s..........
+00000750: 0000 721c 0000 0072 1d00 0000 722a 0000  ..r....r....r*..
+00000760: 0039 0000 0073 1600 0000 0002 0801 0401  .9...s..........
 00000770: 1401 0801 0a01 0801 0204 0e01 0401 0e02  ................
-00000780: 7229 0000 00da 0475 7466 3863 0300 0000  r).....utf8c....
+00000780: 722a 0000 00da 0475 7466 3863 0300 0000  r*.....utf8c....
 00000790: 0000 0000 0000 0000 0400 0000 0400 0000  ................
 000007a0: 4300 0000 7318 0000 0074 00a0 017c 017c  C...s....t...|.|
 000007b0: 00a1 027d 0374 02a0 037c 037c 02a1 0253  ...}.t...|.|...S
 000007c0: 0072 1f00 0000 2904 da0d 706b 675f 7265  .r....)...pkg_re
 000007d0: 736f 7572 6365 73da 0f72 6573 6f75 7263  sources..resourc
 000007e0: 655f 7374 7269 6e67 7203 0000 00da 0362  e_stringr......b
 000007f0: 3273 2904 da05 666e 616d 65da 0770 6163  2s)...fname..pac
-00000800: 6b61 6765 da03 656e 6372 3400 0000 721c  kage..encr4...r.
+00000800: 6b61 6765 da03 656e 6372 3500 0000 721c  kage..encr5...r.
 00000810: 0000 0072 1c00 0000 721d 0000 00da 0e66  ...r....r......f
-00000820: 696c 655f 6173 5f73 7472 696e 6748 0000  ile_as_stringH..
-00000830: 0073 0400 0000 0001 0c01 7241 0000 0029  .s........rA...)
+00000820: 696c 655f 6173 5f73 7472 696e 674c 0000  ile_as_stringL..
+00000830: 0073 0400 0000 0001 0c01 7242 0000 0029  .s........rB...)
 00000840: 01da 0572 6d6f 6465 6302 0000 0000 0000  ...rmodec.......
 00000850: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
 00000860: 0073 1200 0000 7400 7401 7402 7c00 8301  .s....t.t.t.|...
 00000870: 7c01 8302 8301 5300 721f 0000 0029 0372  |.....S.r....).r
 00000880: 0500 0000 7206 0000 0072 0900 0000 2902  ....r....r....).
-00000890: da08 6669 6c65 6e61 6d65 7242 0000 0072  ..filenamerB...r
+00000890: da08 6669 6c65 6e61 6d65 7243 0000 0072  ..filenamerC...r
 000008a0: 1c00 0000 721c 0000 0072 1d00 0000 da0b  ....r....r......
-000008b0: 7072 6570 6172 655f 6c67 744d 0000 0073  prepare_lgtM...s
-000008c0: 0200 0000 0001 7244 0000 0029 01da 0a69  ......rD...)...i
+000008b0: 7072 6570 6172 655f 6c67 7451 0000 0073  prepare_lgtQ...s
+000008c0: 0200 0000 0001 7245 0000 0029 01da 0a69  ......rE...)...i
 000008d0: 6e70 7574 5f64 6963 7463 0100 0000 0000  nput_dictc......
 000008e0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
 000008f0: 0000 732c 0000 0069 007d 0174 0044 005d  ..s,...i.}.t.D.]
 00000900: 1e5c 027d 027d 037c 027c 006b 0672 087c  .\.}.}.|.|.k.r.|
 00000910: 00a0 017c 02a1 017c 017c 023c 0071 087c  ...|...|.|.<.q.|
 00000920: 0153 0072 1f00 0000 2902 da0b 414c 474f  .S.r....)...ALGO
-00000930: 5f50 4152 414d 53da 0367 6574 2904 7245  _PARAMS..get).rE
+00000930: 5f50 4152 414d 53da 0367 6574 2904 7246  _PARAMS..get).rF
 00000940: 0000 00da 0b61 6c67 6f5f 7061 7261 6d73  .....algo_params
 00000950: da04 6e61 6d65 da03 7479 7072 1c00 0000  ..name..typr....
 00000960: 721c 0000 0072 1d00 0000 da1a 6669 6c74  r....r......filt
 00000970: 6572 5f64 6963 745f 746f 5f61 6c67 6f5f  er_dict_to_algo_
-00000980: 7061 7261 6d73 5100 0000 730a 0000 0000  paramsQ...s.....
-00000990: 0104 010c 0108 0110 0172 4b00 0000 6303  .........rK...c.
+00000980: 7061 7261 6d73 5500 0000 730a 0000 0000  paramsU...s.....
+00000990: 0104 010c 0108 0110 0172 4c00 0000 6303  .........rL...c.
 000009a0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
 000009b0: 0000 0043 0000 0073 5400 0000 7a28 7400  ...C...sT...z(t.
 000009c0: 7c00 7c01 7c02 6401 6402 8d04 7d03 7c03  |.|.|.d.d...}.|.
 000009d0: a001 a100 7d04 7c04 a002 6403 6700 a102  ....}.|...d.g...
 000009e0: 7d04 5700 6e26 0400 7403 6b0a 724e 0100  }.W.n&..t.k.rN..
 000009f0: 0100 0100 7404 a005 6404 7c00 7c01 a103  ....t...d.|.|...
 00000a00: 0100 6700 7d04 5900 6e02 5800 7c04 5300  ..g.}.Y.n.X.|.S.
 00000a10: 2905 4ee9 0f00 0000 2904 da04 686f 7374  ).N.....)...host
-00000a20: da04 706f 7274 5a0a 7572 6c5f 7072 6566  ..portZ.url_pref
+00000a20: da04 706f 7274 da0a 7572 6c5f 7072 6566  ..port..url_pref
 00000a30: 6978 da07 7469 6d65 6f75 74da 076d 6574  ix..timeout..met
 00000a40: 686f 6473 7a32 4361 6e6e 6f74 2063 6f6e  hodsz2Cannot con
 00000a50: 6e65 6374 2074 6f20 6d61 6e61 6765 7220  nect to manager 
 00000a60: 6f62 6a65 6374 2061 7420 656e 6470 6f69  object at endpoi
-00000a70: 6e74 2025 733a 2564 2906 7204 0000 005a  nt %s:%d).r....Z
+00000a70: 6e74 2025 733a 2564 2906 7204 0000 00da  nt %s:%d).r.....
 00000a80: 1567 6574 5f73 7562 6d69 7373 696f 6e5f  .get_submission_
-00000a90: 6d65 7468 6f64 7247 0000 0072 0c00 0000  methodrG...r....
+00000a90: 6d65 7468 6f64 7248 0000 0072 0c00 0000  methodrH...r....
 00000aa0: da06 6c6f 6767 6572 da05 6465 6275 6729  ..logger..debug)
-00000ab0: 055a 056d 686f 7374 da05 6d70 6f72 74da  .Z.mhost..mport.
-00000ac0: 076d 7072 6566 6978 5a0a 6d67 725f 636c  .mprefixZ.mgr_cl
+00000ab0: 05da 056d 686f 7374 da05 6d70 6f72 74da  ...mhost..mport.
+00000ac0: 076d 7072 6566 6978 da0a 6d67 725f 636c  .mprefix..mgr_cl
 00000ad0: 6965 6e74 da08 7265 7370 6f6e 7365 721c  ient..responser.
 00000ae0: 0000 0072 1c00 0000 721d 0000 00da 1a67  ...r....r......g
 00000af0: 6574 5f6d 6772 5f64 6570 6c6f 796d 656e  et_mgr_deploymen
-00000b00: 745f 6d65 7468 6f64 7359 0000 0073 1a00  t_methodsY...s..
+00000b00: 745f 6d65 7468 6f64 735d 0000 0073 1a00  t_methods]...s..
 00000b10: 0000 0001 0201 0201 0200 0200 0200 02ff  ................
-00000b20: 0603 0801 1001 0e01 0e01 0a01 7256 0000  ............rV..
+00000b20: 0603 0801 1001 0e01 0e01 0a01 725b 0000  ............r[..
 00000b30: 0063 0100 0000 0000 0000 0000 0000 0400  .c..............
 00000b40: 0000 0300 0000 4300 0000 7370 0000 0064  ......C...sp...d
 00000b50: 017d 0174 007c 0083 017d 027c 026a 0164  .}.t.|...}.|.j.d
 00000b60: 026b 0272 1c64 037d 016e 0e7c 026a 0164  .k.r.d.}.n.|.j.d
 00000b70: 046b 0272 2a64 057d 017c 026a 0264 006b  .k.r*d.}.|.j.d.k
 00000b80: 0972 3a7c 026a 027d 017c 026a 037d 037c  .r:|.j.}.|.j.}.|
 00000b90: 0364 006b 0972 607c 03a0 0464 06a1 0172  .d.k.r`|...d...r
 00000ba0: 647c 0364 0064 0185 0219 007d 036e 0464  d|.d.d.....}.n.d
 00000bb0: 077d 037c 026a 057c 017c 0366 0353 0029  .}.|.j.|.|.f.S.)
 00000bc0: 084e e9ff ffff ffda 0468 7474 70e9 5000  .N.......http.P.
 00000bd0: 0000 da05 6874 7470 7369 bb01 0000 fa01  ....httpsi......
 00000be0: 2fda 0029 0672 0200 0000 da06 7363 6865  /..).r......sche
-00000bf0: 6d65 724e 0000 0072 2100 0000 722c 0000  merN...r!...r,..
+00000bf0: 6d65 724f 0000 0072 2100 0000 722d 0000  merO...r!...r-..
 00000c00: 00da 0868 6f73 746e 616d 6529 045a 076d  ...hostname).Z.m
-00000c10: 6772 5f75 726c 7253 0000 005a 066d 7061  gr_urlrS...Z.mpa
-00000c20: 7273 6572 5400 0000 721c 0000 0072 1c00  rserT...r....r..
+00000c10: 6772 5f75 726c 7257 0000 00da 066d 7061  gr_urlrW.....mpa
+00000c20: 7273 6572 5800 0000 721c 0000 0072 1c00  rserX...r....r..
 00000c30: 0000 721d 0000 00da 0d70 6172 7365 5f6d  ..r......parse_m
-00000c40: 6772 5f75 726c 6600 0000 731c 0000 0000  gr_urlf...s.....
+00000c40: 6772 5f75 726c 6a00 0000 731c 0000 0000  gr_urlj...s.....
 00000c50: 0104 0108 010a 0106 010a 0104 010a 0106  ................
-00000c60: 0106 0108 010a 010e 0204 0172 5f00 0000  ...........r_...
+00000c60: 0106 0108 010a 010e 0204 0172 6500 0000  ...........re...
 00000c70: 6309 0000 0000 0000 0000 0000 0009 0000  c...............
 00000c80: 000a 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
 00000c90: 7c01 7c02 7c03 7c04 7c05 7c06 7c07 7c08  |.|.|.|.|.|.|.|.
 00000ca0: 6401 9c09 5300 2902 4e29 0972 0d00 0000  d...S.).N).r....
 00000cb0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
 00000cc0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
 00000cd0: 0000 0072 1500 0000 721c 0000 0029 0972  ...r....r....).r
 00000ce0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
 00000cf0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
 00000d00: 0000 5a09 7377 616d 5f73 697a 6572 1500  ..Z.swam_sizer..
 00000d10: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
 00000d20: 00da 146d 616b 655f 616c 676f 5f70 6172  ...make_algo_par
-00000d30: 616d 5f64 6963 7478 0000 0073 1400 0000  am_dictx...s....
-00000d40: 0002 0201 0201 0201 0201 0201 0201 0201  ................
-00000d50: 0201 02f7 7260 0000 00da 046e 6f6e 65e9  ....r`.....none.
+00000d30: 616d 5f64 6963 747c 0000 0073 1400 0000  am_dict|...s....
+00000d40: 000c 0201 0201 0201 0201 0201 0201 0201  ................
+00000d50: 0201 02f7 7266 0000 00da 046e 6f6e 65e9  ....rf.....none.
 00000d60: 0100 0000 da09 5061 7274 6974 696f 6e29  ......Partition)
 00000d70: 06da 036c 6774 da04 7465 7374 da09 616c  ...lgt..test..al
 00000d80: 676f 7269 7468 6dda 0e6e 756d 5f70 6172  gorithm..num_par
 00000d90: 7469 7469 6f6e 73da 0b6e 756d 5f69 736c  titions..num_isl
 00000da0: 616e 6473 da09 7061 725f 6c61 6265 6c63  ands..par_labelc
 00000db0: 0700 0000 0000 0000 0000 0000 0c00 0000  ................
 00000dc0: 0800 0000 4300 0000 7398 0000 007c 0664  ....C...s....|.d
@@ -227,60 +227,60 @@
 00000e20: 087c 086a 0567 0064 057c 047c 037c 0417  .|.j.g.d.|.|.|..
 00000e30: 0064 068d 047d 0b7c 0ba0 067c 0aa1 0101  .d...}.|...|....
 00000e40: 0074 077c 0b83 0101 007c 0ba0 03a1 007d  .t.|.....|.....}
 00000e50: 0a7c 0a7c 085f 0874 09a0 0a7c 0aa1 0101  .|.|._.t...|....
 00000e60: 007c 0853 0029 074e 7a18 646c 672e 6170  .|.S.).Nz.dlg.ap
 00000e70: 7073 2e73 696d 706c 652e 536c 6565 7041  ps.simple.SleepA
 00000e80: 7070 2901 da03 6170 7054 2905 da04 616c  pp)...appT)...al
-00000e90: 676f 7267 0000 0072 6800 0000 da0f 7061  gorg...rh.....pa
+00000e90: 676f 726d 0000 0072 6e00 0000 da0f 7061  gorm...rn.....pa
 00000ea0: 7274 6974 696f 6e5f 6c61 6265 6cda 0973  rtition_label..s
 00000eb0: 686f 775f 676f 6a73 4629 03da 0772 6574  how_gojsF)...ret
-00000ec0: 5f73 7472 7268 0000 00da 0d74 706c 5f6e  _strrh.....tpl_n
+00000ec0: 5f73 7472 726e 0000 00da 0d74 706c 5f6e  _strrn.....tpl_n
 00000ed0: 6f64 6573 5f6c 656e 290b 7207 0000 0072  odes_len).r....r
-00000ee0: 0a00 0000 724b 0000 00da 0370 6f70 720b  ....rK.....popr.
+00000ee0: 0a00 0000 724c 0000 00da 0370 6f70 720b  ....rL.....popr.
 00000ef0: 0000 00da 0a74 6f5f 7067 5f73 7065 63da  .....to_pg_spec.
 00000f00: 0661 7070 656e 6472 0800 0000 da09 7265  .appendr......re
-00000f10: 7072 6f64 6174 6172 5100 0000 da04 696e  prodatarQ.....in
-00000f20: 666f 290c 7264 0000 0072 6500 0000 7266  fo).rd...re...rf
-00000f30: 0000 0072 6700 0000 7268 0000 0072 6900  ...rg...rh...ri.
+00000f10: 7072 6f64 6174 6172 5400 0000 da04 696e  prodatarT.....in
+00000f20: 666f 290c 726a 0000 0072 6b00 0000 726c  fo).rj...rk...rl
+00000f30: 0000 0072 6d00 0000 726e 0000 0072 6f00  ...rm...rn...ro.
 00000f40: 0000 5a14 616c 676f 7269 7468 6d5f 7061  ..Z.algorithm_pa
-00000f50: 7261 6d65 7465 7273 726a 0000 00da 0370  rametersrj.....p
-00000f60: 6774 7248 0000 0072 7300 0000 5a08 7067  gtrH...rs...Z.pg
+00000f50: 7261 6d65 7465 7273 7270 0000 00da 0370  rametersrp.....p
+00000f60: 6774 7249 0000 0072 7900 0000 5a08 7067  gtrI...ry...Z.pg
 00000f70: 745f 7370 6563 721c 0000 0072 1c00 0000  t_specr....r....
 00000f80: 721d 0000 00da 2075 6e72 6f6c 6c5f 616e  r..... unroll_an
 00000f90: 645f 7061 7274 6974 696f 6e5f 7769 7468  d_partition_with
-00000fa0: 5f70 6172 616d 7386 0000 0073 3a00 0000  _params....s:...
-00000fb0: 0003 0801 0401 0c01 1001 0801 0802 0201  ................
+00000fa0: 5f70 6172 616d 7394 0000 0073 3a00 0000  _params....s:...
+00000fb0: 0009 0801 0401 0c01 1001 0801 0802 0201  ................
 00000fc0: 02ff 0202 0201 0201 0201 0201 02fa 0407  ................
 00000fd0: 02f9 060a 0401 0201 0201 0201 06fc 0606  ................
-00000fe0: 0a01 0801 0801 0601 0a01 7276 0000 0029  ..........rv...)
-00000ff0: 0572 6100 0000 7262 0000 0072 0100 0000  .ra...rb...r....
-00001000: 7263 0000 004e 292c 7220 0000 00da 076c  rc...N),r .....l
-00001010: 6f67 6769 6e67 723b 0000 00da 0c75 726c  oggingr;.....url
+00000fe0: 0a01 0801 0801 0601 0a01 727c 0000 0029  ..........r|...)
+00000ff0: 0572 6700 0000 7268 0000 0072 0100 0000  .rg...rh...r....
+00001000: 7269 0000 004e 292c 7220 0000 00da 076c  ri...N),r .....l
+00001010: 6f67 6769 6e67 723c 0000 00da 0c75 726c  oggingr<.....url
 00001020: 6c69 622e 7061 7273 6572 0200 0000 da03  lib.parser......
-00001030: 646c 6772 0300 0000 5a0b 646c 672e 636c  dlgr....Z.dlg.cl
-00001040: 6965 6e74 7372 0400 0000 5a2a 646c 672e  ientsr....Z*dlg.
+00001030: 646c 6772 0300 0000 da0b 646c 672e 636c  dlgr......dlg.cl
+00001040: 6965 6e74 7372 0400 0000 da2a 646c 672e  ientsr.....*dlg.
 00001050: 636f 6d6d 6f6e 2e72 6570 726f 6475 6369  common.reproduci
 00001060: 6269 6c69 7479 2e72 6570 726f 6475 6369  bility.reproduci
 00001070: 6269 6c69 7479 7205 0000 0072 0600 0000  bilityr....r....
 00001080: 7207 0000 0072 0800 0000 da0f 646c 672e  r....r......dlg.
 00001090: 6472 6f70 6d61 6b65 2e6c 6772 0900 0000  dropmake.lgr....
-000010a0: 5a19 646c 672e 6472 6f70 6d61 6b65 2e70  Z.dlg.dropmake.p
+000010a0: da19 646c 672e 6472 6f70 6d61 6b65 2e70  ..dlg.dropmake.p
 000010b0: 675f 6765 6e65 7261 746f 7272 0a00 0000  g_generatorr....
-000010c0: 720b 0000 00da 0d64 6c67 2e72 6573 7475  r......dlg.restu
+000010c0: 720b 0000 005a 0d64 6c67 2e72 6573 7475  r....Z.dlg.restu
 000010d0: 7469 6c73 720c 0000 00da 0967 6574 4c6f  tilsr......getLo
-000010e0: 6767 6572 da08 5f5f 6e61 6d65 5f5f 7251  gger..__name__rQ
+000010e0: 6767 6572 da08 5f5f 6e61 6d65 5f5f 7254  gger..__name__rT
 000010f0: 0000 00da 0369 6e74 da05 666c 6f61 7472  .....int..floatr
-00001100: 4600 0000 721e 0000 0072 2300 0000 7226  F...r....r#...r&
-00001110: 0000 0072 2700 0000 722a 0000 0072 2b00  ...r'...r*...r+.
-00001120: 0000 7229 0000 0072 4100 0000 da03 7374  ..r)...rA.....st
-00001130: 7272 4400 0000 da04 6469 6374 724b 0000  rrD.....dictrK..
-00001140: 0072 5600 0000 725f 0000 0072 6000 0000  .rV...r_...r`...
-00001150: da04 626f 6f6c 7276 0000 0072 1c00 0000  ..boolrv...r....
+00001100: 4700 0000 721e 0000 0072 2300 0000 7227  G...r....r#...r'
+00001110: 0000 0072 2800 0000 722b 0000 0072 2c00  ...r(...r+...r,.
+00001120: 0000 722a 0000 0072 4200 0000 da03 7374  ..r*...rB.....st
+00001130: 7272 4500 0000 da04 6469 6374 724c 0000  rrE.....dictrL..
+00001140: 0072 5b00 0000 7265 0000 0072 6600 0000  .r[...re...rf...
+00001150: da04 626f 6f6c 727c 0000 0072 1c00 0000  ..boolr|...r....
 00001160: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00001170: 083c 6d6f 6475 6c65 3e01 0000 0073 5600  .<module>....sV.
-00001180: 0000 0801 0801 0801 0c02 0c01 0c01 1802  ................
+00001170: 083c 6d6f 6475 6c65 3e01 0000 0073 5c00  .<module>....s\.
+00001180: 0000 0801 0801 0801 0c02 0c01 0c01 1806  ................
 00001190: 0c01 1001 0c02 0a03 0601 0601 0601 0601  ................
 000011a0: 0601 0601 0601 0601 06f7 040d 0804 0804  ................
 000011b0: 0804 0804 0804 0804 0813 0e05 0e04 0e08  ................
-000011c0: 080d 0812 080e 0001 0000 0001 0000 00fe  ................
-000011d0: 0801 0200 0201 02fe                      ........
+000011c0: 080d 0812 081b 0001 0001 0001 0001 00f9  ................
+000011d0: 0201 0201 0201 0201 0201 0201 02fa       ..............
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/dropmake/web/__pycache__/translator_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/d3.v3.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/graph_init.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/graph_init.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/img/jsoneditor-icons.png` & `daliuge-translator-4.0.1/dlg/dropmake/web/img/jsoneditor-icons.png`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/license.html` & `daliuge-translator-4.0.1/dlg/dropmake/web/license.html`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/main.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/main.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/matrix_vis.html` & `daliuge-translator-4.0.1/dlg/dropmake/web/matrix_vis.html`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/pg_viewer.html` & `daliuge-translator-4.0.1/dlg/dropmake/web/pg_viewer.html`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/pure-min.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/pure-min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/FileSaver.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/FileSaver.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/d3.v5.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/dagre-d3.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/dagre-d3.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/d3/dagre-d3.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/data_prep.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/data_prep.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/echarts-dagre.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/echarts-dagre.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/html2canvas.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/liu.svg` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/liu.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/liuFavIcon.svg` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/liuFavIcon.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/settings_white_24dp.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/icons/translate_green.png` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/icons/translate_green.png`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/jquery-ui.min.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/jquery.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/jquery.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/canteen.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/canteen.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/caseFrame.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/caseFrame.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/caseFrame.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/caseFrame.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/config.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/config.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/countup.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/countup.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/dat.gui.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/dat.gui.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/draggable.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/draggable.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecSimpleTransform.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/ecStat.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/ecStat.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/echarts-dagre.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/echarts.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/echarts.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/esl.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/esl.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/facePrint.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/facePrint.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/fflate/index.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/fflate/index.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/frameInsight.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/frameInsight.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/jquery.min.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/perlin.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/perlin.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/rearrange.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/rearrange.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/require.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/require.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/requireES.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/requireES.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/reset.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/reset.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/rollup.browser.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/rollup.browser.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/lib/testHelper.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/lib/testHelper.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/main.css` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/main.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/src/require.js` & `daliuge-translator-4.0.1/dlg/dropmake/web/src/require.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/translator_rest.py` & `daliuge-translator-4.0.1/dlg/dropmake/web/translator_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,25 +134,21 @@
 
 post_sem = threading.Semaphore(1)
 gen_pgt_sem = threading.Semaphore(1)
 
 global lg_dir
 global pgt_dir
 global pg_mgr
-LG_SCHEMA = json.loads(
-    file_as_string("lg.graph.schema", package="dlg.dropmake")
-)
+LG_SCHEMA = json.loads(file_as_string("lg.graph.schema", package="dlg.dropmake"))
 
 
 @app.post("/jsonbody", tags=["Original"])
 def jsonbody_post_lg(
     lg_name: str = Form(description="The name of the lg to use"),
-    lg_content: str = Form(
-        description="The content of the lg to save to file"
-    ),
+    lg_content: str = Form(description="The content of the lg to save to file"),
     rmode: str = Form(default=str(REPRO_DEFAULT.value)),
 ):
     """
     Post a logical graph JSON.
     """
     if not lg_exists(lg_dir, lg_name):
         raise HTTPException(
@@ -168,17 +164,15 @@
     post_sem.acquire()
     try:
         with open(lg_path, "w") as lg_file:
             lg_file.write(json.dumps(lg_content))
     except Exception as e:
         raise HTTPException(
             status_code=500,
-            detail="Failed to save logical graph {0}:{1}".format(
-                lg_name, str(e)
-            ),
+            detail="Failed to save logical graph {0}:{1}".format(lg_name, str(e)),
         )
     finally:
         post_sem.release()
 
 
 @app.get("/jsonbody", tags=["Original"])
 def jsonbody_get_lg(
@@ -299,17 +293,15 @@
     """
     try:
         ret = pg_mgr.get_gantt_chart(pgt_id)
         return ret
     except GraphException as ge:
         raise HTTPException(
             status_code=500,
-            detail="Failed to generate Gantt chart for {0}: {1}".format(
-                pgt_id, ge
-            ),
+            detail="Failed to generate Gantt chart for {0}: {1}".format(pgt_id, ge),
         )
 
 
 @app.get("/show_schedule_mat", response_class=HTMLResponse, tags=["Original"])
 def show_schedule_matrix(
     request: Request,
     pgt_id: str = Query(
@@ -341,17 +333,15 @@
     """
     try:
         ret = pg_mgr.get_schedule_matrices(pgt_id)
         return ret
     except Exception as e:
         raise HTTPException(
             status_code=500,
-            detail="Failed to get schedule matrices for {0}: {1}".format(
-                pgt_id, e
-            ),
+            detail="Failed to get schedule matrices for {0}: {1}".format(pgt_id, e),
         )
 
 
 # ------ Graph deployment methods ------ #
 
 
 @app.get("/gen_pgt", tags=["Original"])
@@ -425,38 +415,32 @@
             status_code=500,
             detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name),
         )
     except SchedulerException as se:
         logger.info("Schedule Exception")
         raise HTTPException(
             status_code=500,
-            detail="Graph scheduling exception {1}: {0}".format(
-                str(se), lg_name
-            ),
+            detail="Graph scheduling exception {1}: {0}".format(str(se), lg_name),
         )
     except Exception:
         logger.info("Partition / Other exception")
         trace_msg = traceback.format_exc()
         raise HTTPException(
             status_code=500,
-            detail="Graph partition exception {1}: {0}".format(
-                trace_msg, lg_name
-            ),
+            detail="Graph partition exception {1}: {0}".format(trace_msg, lg_name),
         )
 
 
 @app.post("/gen_pgt", response_class=HTMLResponse, tags=["Original"])
 async def gen_pgt_post(
     request: Request,
     lg_name: str = Form(
         description="If present, translator will attempt to load this lg from file"
     ),
-    json_data: str = Form(
-        description="The graph data used as the graph if supplied"
-    ),
+    json_data: str = Form(description="The graph data used as the graph if supplied"),
     rmode: str = Form(
         str(REPRO_DEFAULT.value),
         description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information",
     ),
     test: str = Form(
         default="false",
         description="If 'true', will replace all apps with sleeps",
@@ -545,26 +529,22 @@
             status_code=500,
             detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name),
         )
     except SchedulerException as se:
         logger.info("SCHEDULE EXCEPTION")
         raise HTTPException(
             status_code=500,
-            detail="Graph scheduling exception {1}: {0}".format(
-                str(se), lg_name
-            ),
+            detail="Graph scheduling exception {1}: {0}".format(str(se), lg_name),
         )
     except Exception:
         logger.info("OTHER EXCEPTION")
         trace_msg = traceback.format_exc()
         raise HTTPException(
             status_code=500,
-            detail="Graph partition exception {1}: {0}".format(
-                trace_msg, lg_name
-            ),
+            detail="Graph partition exception {1}: {0}".format(trace_msg, lg_name),
         )
 
 
 @app.get("/gen_pg", response_class=JSONResponse, tags=["Original"])
 def gen_pg(
     request: Request,
     pgt_id: str = Query(
@@ -630,17 +610,15 @@
             detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
                 pgt_id
             ),
         )
 
     pgtpj = pgtp._gojs_json_obj
     reprodata = pgtp.reprodata
-    num_partitions = len(
-        list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"]))
-    )
+    num_partitions = len(list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"])))
 
     if mhost is None:
         if tpl_nodes_len > 0:
             nnodes = num_partitions
         else:
             raise HTTPException(
                 status_code=500,
@@ -680,17 +658,15 @@
                 )
             )
         else:
             return JSONResponse(pg_spec)
     except restutils.RestClientException as re:
         raise HTTPException(
             status_code=500,
-            detail="Failed to interact with DALiUGE Drop Manager: {0}".format(
-                re
-            ),
+            detail="Failed to interact with DALiUGE Drop Manager: {0}".format(re),
         )
     except Exception as ex:
         logger.error(traceback.format_exc())
         raise HTTPException(
             status_code=500,
             detail="Failed to deploy physical graph: {0}".format(ex),
         )
@@ -721,30 +697,26 @@
             manager_host = "localhost"
         logger.debug("pgt_id: %s", str(pgt_id))
         # logger.debug("node_list: %s", str(node_list))
     except Exception as ex:
         logger.error("%s", traceback.format_exc())
         raise HTTPException(
             status_code=500,
-            detail="Unable to parse json body of request for pg_spec: {0}".format(
-                ex
-            ),
+            detail="Unable to parse json body of request for pg_spec: {0}".format(ex),
         )
     pgtp = pg_mgr.get_pgt(pgt_id)
     if pgtp is None:
         raise HTTPException(
             status_code=404,
             detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
                 pgt_id
             ),
         )
     if node_list is None:
-        raise HTTPException(
-            status_code=500, detail="Must specify DALiuGE nodes list"
-        )
+        raise HTTPException(status_code=500, detail="Must specify DALiuGE nodes list")
 
     try:
         pg_spec = pgtp.to_pg_spec(
             [manager_host] + node_list,
             tpl_nodes_len=tpl_nodes_len,
             ret_str=False,
         )
@@ -783,17 +755,15 @@
             detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
                 pgt_id
             ),
         )
 
     pgtpj = pgtp._gojs_json_obj
     logger.info("PGTP: %s", pgtpj)
-    num_partitions = len(
-        list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"]))
-    )
+    num_partitions = len(list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"])))
     # Send pgt_data to helm_start
     try:
         start_helm(pgtp, num_partitions, pgt_dir)
     except restutils.RestClientException as ex:
         logger.error(traceback.format_exc())
         raise HTTPException(
             status_code=500,
@@ -841,25 +811,21 @@
     if graph_content is not None and graph_name is not None:
         raise HTTPException(
             status_code=400,
             detail="Need to supply either an name or content but not both",
         )
     if not lg_exists(lg_dir, graph_name):
         if not graph_content:
-            raise HTTPException(
-                status_code=400, detail="LG content is nonexistent"
-            )
+            raise HTTPException(status_code=400, detail="LG content is nonexistent")
         else:
             try:
                 out_graph = json.loads(graph_content)
             except JSONDecodeError as jerror:
                 logger.error(jerror)
-                raise HTTPException(
-                    status_code=400, detail="LG content is malformed"
-                )
+                raise HTTPException(status_code=400, detail="LG content is malformed")
     else:
         lgp = lg_path(lg_dir, graph_name)
         with open(lgp, "r") as f:
             try:
                 out_graph = json.load(f)
             except JSONDecodeError as jerror:
                 logger.error(jerror)
@@ -880,34 +846,29 @@
         description="If present, translator will use this string as the graph content",
     ),
     parameters: str = Form(
         default="{}", description="JSON key: value store of graph paramter"
     ),
     rmode: str = Form(
         REPRO_DEFAULT.name,
-        enum=[
-            roption.name
-            for roption in [ReproducibilityFlags.NOTHING] + ALL_RMODES
-        ],
+        enum=[roption.name for roption in [ReproducibilityFlags.NOTHING] + ALL_RMODES],
         description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information",
     ),
 ):
     """
     Will fill a logical graph by replacing fields with supplied parameters.
 
     One of lg_name or lg_content, but not both, must be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
     try:
         params = json.loads(parameters)
     except JSONDecodeError as jerror:
         logger.error(jerror)
-        raise HTTPException(
-            status_code=400, detail="Parameter string is invalid"
-        )
+        raise HTTPException(status_code=400, detail="Parameter string is invalid")
     output_graph = dlg.dropmake.pg_generator.fill(lg_graph, params)
     output_graph = init_lg_repro_data(init_lgt_repro_data(output_graph, rmode))
     return JSONResponse(output_graph)
 
 
 @app.post("/unroll", response_class=JSONResponse, tags=["Updated"])
 def lg_unroll(
@@ -933,17 +894,15 @@
 ):
     """
     Will unroll a logical graph into a physical graph template.
 
     One of lg_name or lg_content, but not both, needs to be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
-    pgt = dlg.dropmake.pg_generator.unroll(
-        lg_graph, oid_prefix, zero_run, default_app
-    )
+    pgt = dlg.dropmake.pg_generator.unroll(lg_graph, oid_prefix, zero_run, default_app)
     pgt = init_pgt_unroll_repro_data(pgt)
     return JSONResponse(pgt)
 
 
 @app.post("/partition", response_class=JSONResponse, tags=["Updated"])
 def pgt_partition(
     pgt_name: str = Form(
@@ -982,17 +941,15 @@
         graph, algorithm, num_partitions, num_islands, algo_params.dict()
     )
     pgt.append(reprodata)
     pgt = init_pgt_partition_repro_data(pgt)
     return JSONResponse(pgt)
 
 
-@app.post(
-    "/unroll_and_partition", response_class=JSONResponse, tags=["Updated"]
-)
+@app.post("/unroll_and_partition", response_class=JSONResponse, tags=["Updated"])
 def lg_unroll_and_partition(
     lg_name: str = Form(
         default=None,
         description="If present, translator will attempt to load this lg from file",
     ),
     lg_content: str = Form(
         default=None,
@@ -1026,17 +983,15 @@
 ):
     """
     Unrolls and partitions a logical graph with the provided various parameters.
 
     One of lg_name and lg_content, but not both, must be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
-    pgt = dlg.dropmake.pg_generator.unroll(
-        lg_graph, oid_prefix, zero_run, default_app
-    )
+    pgt = dlg.dropmake.pg_generator.unroll(lg_graph, oid_prefix, zero_run, default_app)
     pgt = init_pgt_unroll_repro_data(pgt)
     reprodata = pgt.pop()
     pgt = dlg.dropmake.pg_generator.partition(
         pgt, algorithm, num_partitions, num_islands, algo_params.dict()
     )
     pgt.append(reprodata)
     pgt = init_pgt_partition_repro_data(pgt)
@@ -1086,17 +1041,15 @@
             % (len(nodes), num_islands),
         )
     pgt = load_graph(pgt_content, pgt_name)
     reprodata = {}
     if not pgt[-1].get("oid"):
         reprodata = pgt.pop()
     logger.info(nodes)
-    pg = dlg.dropmake.pg_generator.resource_map(
-        pgt, nodes, num_islands, co_host_dim
-    )
+    pg = dlg.dropmake.pg_generator.resource_map(pgt, nodes, num_islands, co_host_dim)
     pg.append(reprodata)
     pg = init_pg_repro_data(pg)
     return JSONResponse(pg)
 
 
 @app.get("/api/submission_method")
 def get_submission_method(
@@ -1117,19 +1070,15 @@
         mhost = dlg_mgr_host
         mport = dlg_mgr_port
         mprefix = ""
     available_methods = []
     if check_k8s_env():
         available_methods.append(DeploymentMethods.HELM)
     if mhost is not None:
-        host_available_methods = get_mgr_deployment_methods(
-            mhost, mport, mprefix
-        )
-        if DeploymentMethods.BROWSER in host_available_methods:
-            available_methods.append(DeploymentMethods.SERVER)
+        available_methods = get_mgr_deployment_methods(mhost, mport, mprefix)
     logger.debug("Methods available: %s", available_methods)
     return {"methods": available_methods}
 
 
 @app.get(
     "/",
     response_class=HTMLResponse,
@@ -1256,14 +1205,12 @@
     def handler(*_args):
         raise KeyboardInterrupt
 
     signal.signal(signal.SIGTERM, handler)
     signal.signal(signal.SIGINT, handler)
 
     logging.debug("Starting uvicorn verbose %s", options.verbose)
-    uvicorn.run(
-        app=app, host=options.host, port=options.port, debug=options.verbose
-    )
+    uvicorn.run(app=app, host=options.host, port=options.port, debug=options.verbose)
 
 
 if __name__ == "__main__":
     run(None, sys.argv[1:])
```

### Comparing `daliuge-translator-4.0.0/dlg/dropmake/web/translator_utils.py` & `daliuge-translator-4.0.1/dlg/dropmake/web/translator_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
 import logging
 import pkg_resources
 from urllib.parse import urlparse
 
 from dlg import common
 from dlg.clients import CompositeManagerClient
-from dlg.common.reproducibility.reproducibility import init_lg_repro_data, init_lgt_repro_data, \
-    init_pgt_unroll_repro_data, init_pgt_partition_repro_data
+from dlg.common.reproducibility.reproducibility import (
+    init_lg_repro_data,
+    init_lgt_repro_data,
+    init_pgt_unroll_repro_data,
+    init_pgt_partition_repro_data,
+)
 from dlg.dropmake.lg import load_lg
 from dlg.dropmake.pg_generator import unroll, partition
 from dlg.restutils import RestClientException
 
 logger = logging.getLogger(__name__)
 
 ALGO_PARAMS = [
@@ -113,31 +117,47 @@
         if mprefix.endswith("/"):
             mprefix = mprefix[:-1]
     else:
         mprefix = ""
     return mparse.hostname, mport, mprefix
 
 
-def make_algo_param_dict(min_goal, ptype, max_load_imb, max_cpu, time_greedy, deadline, topk, swam_size, max_mem):
+def make_algo_param_dict(
+    min_goal,
+    ptype,
+    max_load_imb,
+    max_cpu,
+    time_greedy,
+    deadline,
+    topk,
+    swam_size,
+    max_mem,
+):
     return {
         "min_goal": min_goal,
         "ptype": ptype,
         "max_load_imb": max_load_imb,
         "max_cpu": max_cpu,
         "time_greedy": time_greedy,
         "deadline": deadline,
         "topk": topk,
         "swarm_size": swam_size,
-        "max_mem": max_mem
+        "max_mem": max_mem,
     }
 
 
-def unroll_and_partition_with_params(lgt: dict, test: bool, algorithm: str = "none",
-                                     num_partitions: int = 1, num_islands: int = 0,
-                                     par_label: str = "Partition", algorithm_parameters=None):
+def unroll_and_partition_with_params(
+    lgt: dict,
+    test: bool,
+    algorithm: str = "none",
+    num_partitions: int = 1,
+    num_islands: int = 0,
+    par_label: str = "Partition",
+    algorithm_parameters=None,
+):
     if algorithm_parameters is None:
         algorithm_parameters = {}
     app = "dlg.apps.simple.SleepApp" if test else None
     pgt = init_pgt_unroll_repro_data(unroll(lgt, app=app))
     algo_params = filter_dict_to_algo_params(algorithm_parameters)
     reprodata = pgt.pop()
     # Partition the PGT
```

### Comparing `daliuge-translator-4.0.0/dlg/translator/__init__.py` & `daliuge-translator-4.0.1/dlg/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-310.pyc` & `daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-38.pyc` & `daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/translator/__pycache__/tool_commands.cpython-39.pyc` & `daliuge-translator-4.0.1/dlg/translator/__pycache__/tool_commands.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg/translator/tool_commands.py` & `daliuge-translator-4.0.1/dlg/translator/tool_commands.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/dlg.spec` & `daliuge-translator-4.0.1/dlg.spec`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/docker/Dockerfile` & `daliuge-translator-4.0.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/docker/Dockerfile.dev` & `daliuge-translator-4.0.1/docker/Dockerfile.dev`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 # First stage build based on daliuge-common and cleanup
 ARG VCS_TAG
 ARG BUILD_ID
 FROM icrar/daliuge-common:${VCS_TAG:-latest}
 LABEL stage=builder
 LABEL build=$BUILD_ID
-# all dependencies are already installed in daliuge-common
-# RUN apt-get update && \
-#     apt-get clean && \
-#     apt install -y gcc python3-venv python3-distutils
 
+RUN service avahi-daemon stop && \
+    service dbus start && \
+    service avahi-daemon start && \
+    avahi-set-host-name dlg-trans
 COPY / /daliuge
 RUN . /dlg/bin/activate && \
     cd /daliuge && \
     pip3 install wheel && \
     pip3 install . 
 
 # Second stage build taking what's required from first stage
```

### Comparing `daliuge-translator-4.0.0/docker/Dockerfile.ray` & `daliuge-translator-4.0.1/docker/Dockerfile.ray`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/docker/README.md` & `daliuge-translator-4.0.1/docker/README.md`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/run_translator.sh` & `daliuge-translator-4.0.1/run_translator.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env bash
 case "$1" in
     "dep")
         VCS_TAG=`git describe --tags --abbrev=0|sed s/v//`
         echo "Running Translator deployment version in background..."
-        docker run --name daliuge-translator --rm -td -p 8084:8084 icrar/daliuge-translator:${VCS_TAG}
-        echo "Translator URL: http://"`docker exec daliuge-translator sh -c "hostname --ip-address"`:8084
-        exit 0;;
+        docker run -h dlg-trans --name daliuge-translator --rm -td -p 8084:8084 icrar/daliuge-translator:${VCS_TAG};;
     "dev")
         export VCS_TAG=`git rev-parse --abbrev-ref HEAD| tr '[:upper:]' '[:lower:]'`
-        echo "Running Translator development version in foreground..."
-        docker run --volume $PWD/dlg/dropmake:/dlg/lib/python3.8/site-packages/dlg/dropmake --name daliuge-translator --rm -t -p 8084:8084 icrar/daliuge-translator:${VCS_TAG}
-        echo "Translator URL: http://"`docker exec daliuge-translator sh -c "hostname --ip-address"`:8084
-        exit 0;;
+        echo "Running Translator development version in background..."
+        docker run -d -h dlg-trans --volume $PWD/dlg/dropmake:/dlg/lib/python3.8/site-packages/dlg/dropmake --name daliuge-translator --rm -t -p 8084:8084 icrar/daliuge-translator:${VCS_TAG}
+        sleep 3
+        docker exec -u root daliuge-translator bash -c "service avahi-daemon stop > /dev/null 2>&1 && service dbus restart > /dev/null 2>&1 && service avahi-daemon start > /dev/null 2>&1";;
     "casa")
         export VCS_TAG=`git rev-parse --abbrev-ref HEAD| tr '[:upper:]' '[:lower:]'`-casa
         echo "Running Translator development version in foreground..."
-        docker run --volume $PWD/dlg/dropmake:/dlg/lib/python3.8/site-packages/dlg/dropmake --name daliuge-translator --rm -t -p 8084:8084 icrar/daliuge-translator:${VCS_TAG}
-        echo "Translator URL: http://"`docker exec daliuge-translator sh -c "hostname --ip-address"`:8084
-        exit 0;;
+        docker run -h dlg-trans --volume $PWD/dlg/dropmake:/dlg/lib/python3.8/site-packages/dlg/dropmake --name daliuge-translator --rm -t -p 8084:8084 icrar/daliuge-translator:${VCS_TAG};;
     *)
         echo "Usage run_translator.sh <dep|dev|casa>"
         exit 0;;
 esac
+sleep 3
+TRANS_NAME=`docker exec daliuge-translator sh -c "hostname"`
+TRANS_IP=`docker exec daliuge-translator sh -c "hostname --ip-address"`
+echo "Translator URL: http://${TRANS_NAME}.local:8084"
```

### Comparing `daliuge-translator-4.0.0/setup.py` & `daliuge-translator-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
 MAJOR = 4
 MINOR = 0
-PATCH = 0
+PATCH = 1
 RELEASE = True
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/translator/version.py"
 
 
 def get_git_version():
     out = subprocess.check_output(["git", "rev-parse", "HEAD"])
```

### Comparing `daliuge-translator-4.0.0/test/__init__.py` & `daliuge-translator-4.0.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/__init__.py` & `daliuge-translator-4.0.1/test/dropmake/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/ArrayLoop.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/ArrayLoop.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/HelloWorld_simple.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/HelloWorld_simple.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/Plasma_test.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/Plasma_test.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/SharedMemoryTest.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/SharedMemoryTest.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/chiles_simple.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/chiles_simple.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/cont_img_mvp.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/cont_img_mvp.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.graph.schema` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.graph.schema`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.json.schema` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.json.schema`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/dlg-lg.schema` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/dlg-lg.schema`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather_empty.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather_empty.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/eagle_gather_simple.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/eagle_gather_simple.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/lofar_std.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/lofar_std.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/nagsIo.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/nagsIo.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/simpleMKN.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/simpleMKN.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/test-20190830-110556.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/test-20190830-110556.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/testLoop.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/testLoop.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/testScatter.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/testScatter.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/logical_graphs/test_grpby_gather.graph` & `daliuge-translator-4.0.1/test/dropmake/logical_graphs/test_grpby_gather.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/test_lg_fill.py` & `daliuge-translator-4.0.1/test/dropmake/test_lg_fill.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/test_lgweb.py` & `daliuge-translator-4.0.1/test/dropmake/test_lgweb.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/test_pg_gen.py` & `daliuge-translator-4.0.1/test/dropmake/test_pg_gen.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/dropmake/test_scheduler.py` & `daliuge-translator-4.0.1/test/dropmake/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/__init__.py` & `daliuge-translator-4.0.1/test/reproducibility/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSBash.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSBash.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSPython.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSPython.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloSPython2.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloSPython2.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldBash.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldBash.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldBashSplit.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldBashSplit.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/HelloWorldFile.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/HelloWorldFile.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/apps.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/apps.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/files.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/files.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/groupUse.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/groupUse.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/groups.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/groups.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/misc.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/misc.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/simpleNoScatter.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/simpleNoScatter.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/reproGraphs/simpleScatter.graph` & `daliuge-translator-4.0.1/test/reproducibility/reproGraphs/simpleScatter.graph`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_accumulatedata.py` & `daliuge-translator-4.0.1/test/reproducibility/test_accumulatedata.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_integration.py` & `daliuge-translator-4.0.1/test/reproducibility/test_integration.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_json_output.py` & `daliuge-translator-4.0.1/test/reproducibility/test_json_output.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_repro_inits.py` & `daliuge-translator-4.0.1/test/reproducibility/test_repro_inits.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_reprodata_compare.py` & `daliuge-translator-4.0.1/test/reproducibility/test_reprodata_compare.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/reproducibility/test_scatter_blockdag.py` & `daliuge-translator-4.0.1/test/reproducibility/test_scatter_blockdag.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-4.0.0/test/test_tool_trans.py` & `daliuge-translator-4.0.1/test/test_tool_trans.py`

 * *Files identical despite different names*

