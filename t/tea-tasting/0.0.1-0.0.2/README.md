# Comparing `tmp/tea_tasting-0.0.1.tar.gz` & `tmp/tea_tasting-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tea_tasting-0.0.1.tar", last modified: Sun Dec 10 21:34:09 2023, max compression
+gzip compressed data, was "tea_tasting-0.0.2.tar", last modified: Mon Apr 15 20:14:15 2024, max compression
```

## Comparing `tea_tasting-0.0.1.tar` & `tea_tasting-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-12-10 21:33:50.714310 tea_tasting-0.0.1/LICENSE
--rw-r--r--   0        0        0    25722 2023-12-10 21:33:50.714310 tea_tasting-0.0.1/README.md
--rw-r--r--   0        0        0     1027 2023-12-10 21:34:09.422181 tea_tasting-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-12-10 21:33:50.714310 tea_tasting-0.0.1/src/tea_tasting/__init__.py
--rw-r--r--   0        0        0        0 2023-12-10 21:33:50.714310 tea_tasting-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    26654 1970-01-01 00:00:00.000000 tea_tasting-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-15 20:13:54.794706 tea_tasting-0.0.2/LICENSE
+-rw-r--r--   0        0        0    13369 2024-04-15 20:13:54.794706 tea_tasting-0.0.2/README.md
+-rw-r--r--   0        0        0     3015 2024-04-15 20:14:15.554745 tea_tasting-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      379 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/__init__.py
+-rw-r--r--   0        0        0        6 2024-04-15 20:14:15.550745 tea_tasting-0.0.2/src/tea_tasting/_version.txt
+-rw-r--r--   0        0        0    11873 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/aggr.py
+-rw-r--r--   0        0        0     2926 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/config.py
+-rw-r--r--   0        0        0    13048 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/datasets.py
+-rw-r--r--   0        0        0     6842 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/experiment.py
+-rw-r--r--   0        0        0      307 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/__init__.py
+-rw-r--r--   0        0        0     8882 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/base.py
+-rw-r--r--   0        0        0    11922 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/mean.py
+-rw-r--r--   0        0        0     3164 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/utils.py
+-rw-r--r--   0        0        0      390 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/version.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/test_base.py
+-rw-r--r--   0        0        0     8565 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/test_mean.py
+-rw-r--r--   0        0        0     6811 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_aggr.py
+-rw-r--r--   0        0        0     1504 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     3538 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_datasets.py
+-rw-r--r--   0        0        0    10574 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_experiment.py
+-rw-r--r--   0        0        0     3089 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0      779 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_version.py
+-rw-r--r--   0        0        0    14583 1970-01-01 00:00:00.000000 tea_tasting-0.0.2/PKG-INFO
```

### Comparing `tea_tasting-0.0.1/LICENSE` & `tea_tasting-0.0.2/LICENSE`

 * *Files identical despite different names*

