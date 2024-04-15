# Comparing `tmp/pyfilename-0.4.0.tar.gz` & `tmp/pyfilename-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilename-0.4.0.tar", last modified: Fri Sep 29 14:07:57 2023, max compression
+gzip compressed data, was "pyfilename-0.5.0.tar", max compression
```

## Comparing `pyfilename-0.4.0.tar` & `pyfilename-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-09-29 14:07:57.831117 pyfilename-0.4.0/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 pyfilename-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 pyfilename-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2000 2023-09-29 14:07:57.829666 pyfilename-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1291 2023-09-10 13:09:04.000000 pyfilename-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-09-29 14:07:57.822831 pyfilename-0.4.0/pyfilename/
--rw-rw-rw-   0        0        0     1119 2023-09-29 14:07:51.000000 pyfilename-0.4.0/pyfilename/__init__.py
--rw-rw-rw-   0        0        0    21441 2023-09-29 14:04:58.000000 pyfilename-0.4.0/pyfilename/pyfilename.py
-drwxrwxrwx   0        0        0        0 2023-09-29 14:07:57.826965 pyfilename-0.4.0/pyfilename.egg-info/
--rw-rw-rw-   0        0        0     2000 2023-09-29 14:07:57.000000 pyfilename-0.4.0/pyfilename.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-09-29 14:07:57.000000 pyfilename-0.4.0/pyfilename.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-29 14:07:57.000000 pyfilename-0.4.0/pyfilename.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 20:38:56.000000 pyfilename-0.4.0/pyfilename.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-09-29 14:07:57.000000 pyfilename-0.4.0/pyfilename.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-29 14:07:57.831117 pyfilename-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1385 2023-09-23 13:31:00.000000 pyfilename-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-29 14:07:57.829666 pyfilename-0.4.0/test/
--rw-rw-rw-   0        0        0      151 2023-07-13 09:44:26.000000 pyfilename-0.4.0/test/__init__.py
--rw-rw-rw-   0        0        0      284 2023-07-13 20:36:56.000000 pyfilename-0.4.0/test/test.py
+-rw-r--r--   0        0        0     1089 2023-05-15 00:16:47.868006 pyfilename-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-14 14:47:01.937320 pyfilename-0.5.0/pyfilename/__init__.py
+-rw-r--r--   0        0        0    14412 2024-04-14 15:01:00.290187 pyfilename-0.5.0/pyfilename/main.py
+-rw-r--r--   0        0        0     1073 2024-04-15 07:44:38.290877 pyfilename-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2640 2024-04-14 15:13:28.503121 pyfilename-0.5.0/README.md
+-rw-r--r--   0        0        0     3481 1970-01-01 00:00:00.000000 pyfilename-0.5.0/PKG-INFO
```

### Comparing `pyfilename-0.4.0/LICENSE` & `pyfilename-0.5.0/LICENSE`

 * *Files identical despite different names*

