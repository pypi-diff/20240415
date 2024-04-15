# Comparing `tmp/pluginlib-0.9.1.tar.gz` & `tmp/pluginlib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginlib-0.9.1.tar", last modified: Tue Jun 13 01:08:07 2023, max compression
+gzip compressed data, was "pluginlib-0.9.2.tar", last modified: Mon Apr 15 15:44:58 2024, max compression
```

## Comparing `pluginlib-0.9.1.tar` & `pluginlib-0.9.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/
--rw-rw-r--   0 avram     (1000) avram     (1000)    16726 2017-10-10 15:55:09.000000 pluginlib-0.9.1/LICENSE
--rw-rw-r--   0 avram     (1000) avram     (1000)       97 2022-02-13 15:53:51.000000 pluginlib-0.9.1/MANIFEST.in
--rw-r--r--   0 avram     (1000) avram     (1000)     9642 2023-06-13 01:08:07.519497 pluginlib-0.9.1/PKG-INFO
--rw-rw-r--   0 avram     (1000) avram     (1000)     8286 2022-12-30 13:57:46.000000 pluginlib-0.9.1/README.rst
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.517497 pluginlib-0.9.1/doc/
--rw-rw-r--   0 avram     (1000) avram     (1000)     1575 2020-06-03 01:12:58.000000 pluginlib-0.9.1/doc/api.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     8896 2018-08-28 12:21:53.000000 pluginlib-0.9.1/doc/concepts.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     3648 2022-06-02 12:47:07.000000 pluginlib-0.9.1/doc/conf.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2707 2018-07-17 02:26:58.000000 pluginlib-0.9.1/doc/error_handling.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)     4661 2020-05-02 19:07:31.000000 pluginlib-0.9.1/doc/faq.rst
--rw-r--r--   0 avram     (1000) avram     (1000)     3915 2022-06-02 12:45:02.000000 pluginlib-0.9.1/doc/index.rst
--rw-rw-r--   0 avram     (1000) avram     (1000)       87 2018-07-30 14:56:06.000000 pluginlib-0.9.1/doc/spelling_wordlist.txt
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/pluginlib/
--rw-r--r--   0 avram     (1000) avram     (1000)     1006 2023-06-12 23:57:19.000000 pluginlib-0.9.1/pluginlib/__init__.py
--rw-r--r--   0 avram     (1000) avram     (1000)    16942 2023-06-12 23:57:06.000000 pluginlib-0.9.1/pluginlib/_loader.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     8939 2023-06-12 23:44:40.000000 pluginlib-0.9.1/pluginlib/_objects.py
--rw-r--r--   0 avram     (1000) avram     (1000)    16642 2023-06-12 23:44:42.000000 pluginlib-0.9.1/pluginlib/_parent.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     6520 2023-06-12 23:44:45.000000 pluginlib-0.9.1/pluginlib/_util.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     1688 2023-06-12 23:44:47.000000 pluginlib-0.9.1/pluginlib/exceptions.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/pluginlib.egg-info/
--rw-rw-r--   0 avram     (1000) avram     (1000)     9642 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/PKG-INFO
--rw-rw-r--   0 avram     (1000) avram     (1000)     1375 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/SOURCES.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)        1 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/dependency_links.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)        1 2018-08-06 20:52:27.000000 pluginlib-0.9.1/pluginlib.egg-info/not-zip-safe
--rw-rw-r--   0 avram     (1000) avram     (1000)       11 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/requires.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)       10 2023-06-13 01:08:07.000000 pluginlib-0.9.1/pluginlib.egg-info/top_level.txt
--rw-rw-r--   0 avram     (1000) avram     (1000)      571 2023-06-13 01:08:07.520497 pluginlib-0.9.1/setup.cfg
--rw-r--r--   0 avram     (1000) avram     (1000)     2215 2023-06-12 23:57:12.000000 pluginlib-0.9.1/setup.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2508 2020-08-16 11:52:05.000000 pluginlib-0.9.1/setup_helpers.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/
--rw-rw-r--   0 avram     (1000) avram     (1000)     1743 2023-06-12 23:45:31.000000 pluginlib-0.9.1/tests/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     2588 2023-06-12 23:45:33.000000 pluginlib-0.9.1/tests/test_exceptions.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    20686 2023-06-12 23:45:35.000000 pluginlib-0.9.1/tests/test_loader.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    16120 2023-06-12 23:45:37.000000 pluginlib-0.9.1/tests/test_objects.py
--rw-rw-r--   0 avram     (1000) avram     (1000)    25795 2023-06-12 23:45:39.000000 pluginlib-0.9.1/tests/test_parent.py
--rw-rw-r--   0 avram     (1000) avram     (1000)     7473 2023-06-12 23:45:40.000000 pluginlib-0.9.1/tests/test_util.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:03:46.000000 pluginlib-0.9.1/tests/testdata/__init__.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bad/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-01 15:23:47.000000 pluginlib-0.9.1/tests/testdata/bad/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      408 2020-06-02 13:34:23.000000 pluginlib-0.9.1/tests/testdata/bad/syntax.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      533 2020-06-01 15:26:37.000000 pluginlib-0.9.1/tests/testdata/bad2.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.516497 pluginlib-0.9.1/tests/testdata/bare/
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bare/engines/
--rw-rw-r--   0 avram     (1000) avram     (1000)      524 2020-06-02 05:00:57.000000 pluginlib-0.9.1/tests/testdata/bare/engines/electric.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.518497 pluginlib-0.9.1/tests/testdata/bare/hooks/
--rw-rw-r--   0 avram     (1000) avram     (1000)      553 2022-02-13 14:41:50.000000 pluginlib-0.9.1/tests/testdata/bare/hooks/fish.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      550 2020-06-02 05:04:18.000000 pluginlib-0.9.1/tests/testdata/bare/hooks/grappling.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/bare/package/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:13.000000 pluginlib-0.9.1/tests/testdata/bare/package/__init__.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/bare/package/parsers/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:24.000000 pluginlib-0.9.1/tests/testdata/bare/package/parsers/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      535 2020-06-02 05:02:36.000000 pluginlib-0.9.1/tests/testdata/bare/package/parsers/silly_walks.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/importer/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-15 02:39:55.000000 pluginlib-0.9.1/tests/testdata/importer/__init__.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:04.000000 pluginlib-0.9.1/tests/testdata/lib/__init__.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/engines/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-08 01:55:41.000000 pluginlib-0.9.1/tests/testdata/lib/engines/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      512 2020-06-02 05:03:03.000000 pluginlib-0.9.1/tests/testdata/lib/engines/steam.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/hooks/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      530 2020-06-02 05:03:14.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/left.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      534 2020-06-02 05:03:22.000000 pluginlib-0.9.1/tests/testdata/lib/hooks/right.py
-drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2023-06-13 01:08:07.519497 pluginlib-0.9.1/tests/testdata/lib/parsers/
--rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/__init__.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      669 2020-06-02 05:04:01.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/json.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      503 2020-06-02 05:03:52.000000 pluginlib-0.9.1/tests/testdata/lib/parsers/xml.py
--rw-rw-r--   0 avram     (1000) avram     (1000)      760 2018-07-09 01:05:42.000000 pluginlib-0.9.1/tests/testdata/parents.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/
+-rw-rw-r--   0 avram     (1000) avram     (1000)    16726 2017-10-10 15:55:09.000000 pluginlib-0.9.2/LICENSE
+-rw-rw-r--   0 avram     (1000) avram     (1000)       97 2022-02-13 15:53:51.000000 pluginlib-0.9.2/MANIFEST.in
+-rw-r--r--   0 avram     (1000) avram     (1000)     9668 2024-04-15 15:44:58.057404 pluginlib-0.9.2/PKG-INFO
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8286 2022-12-30 13:57:46.000000 pluginlib-0.9.2/README.rst
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.055404 pluginlib-0.9.2/doc/
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1575 2023-08-25 22:33:02.000000 pluginlib-0.9.2/doc/api.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8896 2018-08-28 12:21:53.000000 pluginlib-0.9.2/doc/concepts.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     3639 2023-08-25 22:41:43.000000 pluginlib-0.9.2/doc/conf.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     2707 2018-07-17 02:26:58.000000 pluginlib-0.9.2/doc/error_handling.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)     4661 2020-05-02 19:07:31.000000 pluginlib-0.9.2/doc/faq.rst
+-rw-r--r--   0 avram     (1000) avram     (1000)     3915 2022-06-02 12:45:02.000000 pluginlib-0.9.2/doc/index.rst
+-rw-rw-r--   0 avram     (1000) avram     (1000)       87 2018-07-30 14:56:06.000000 pluginlib-0.9.2/doc/spelling_wordlist.txt
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.055404 pluginlib-0.9.2/pluginlib/
+-rw-r--r--   0 avram     (1000) avram     (1000)     1006 2024-04-15 15:39:27.000000 pluginlib-0.9.2/pluginlib/__init__.py
+-rw-r--r--   0 avram     (1000) avram     (1000)    16999 2024-04-14 17:19:03.000000 pluginlib-0.9.2/pluginlib/_loader.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     8939 2023-08-25 22:33:26.000000 pluginlib-0.9.2/pluginlib/_objects.py
+-rw-r--r--   0 avram     (1000) avram     (1000)    16642 2023-08-25 22:33:34.000000 pluginlib-0.9.2/pluginlib/_parent.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     6520 2023-08-25 22:33:39.000000 pluginlib-0.9.2/pluginlib/_util.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1688 2023-06-12 23:44:47.000000 pluginlib-0.9.2/pluginlib/exceptions.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/pluginlib.egg-info/
+-rw-r--r--   0 avram     (1000) avram     (1000)     9668 2024-04-15 15:44:58.000000 pluginlib-0.9.2/pluginlib.egg-info/PKG-INFO
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1375 2024-04-15 15:44:58.000000 pluginlib-0.9.2/pluginlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)        1 2024-04-15 15:44:58.000000 pluginlib-0.9.2/pluginlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)        1 2018-08-06 20:52:27.000000 pluginlib-0.9.2/pluginlib.egg-info/not-zip-safe
+-rw-rw-r--   0 avram     (1000) avram     (1000)       11 2024-04-15 15:44:58.000000 pluginlib-0.9.2/pluginlib.egg-info/requires.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)       10 2024-04-15 15:44:58.000000 pluginlib-0.9.2/pluginlib.egg-info/top_level.txt
+-rw-rw-r--   0 avram     (1000) avram     (1000)      572 2024-04-15 15:44:58.058404 pluginlib-0.9.2/setup.cfg
+-rw-r--r--   0 avram     (1000) avram     (1000)     2215 2023-08-25 22:33:48.000000 pluginlib-0.9.2/setup.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     6993 2023-08-25 22:14:47.000000 pluginlib-0.9.2/setup_helpers.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/
+-rw-rw-r--   0 avram     (1000) avram     (1000)     1743 2023-08-25 22:33:55.000000 pluginlib-0.9.2/tests/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     2588 2023-06-12 23:45:33.000000 pluginlib-0.9.2/tests/test_exceptions.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    20686 2023-08-25 22:34:01.000000 pluginlib-0.9.2/tests/test_loader.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    16120 2023-08-25 22:34:14.000000 pluginlib-0.9.2/tests/test_objects.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)    25795 2023-08-25 22:34:20.000000 pluginlib-0.9.2/tests/test_parent.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)     7473 2023-08-25 22:34:56.000000 pluginlib-0.9.2/tests/test_util.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:03:46.000000 pluginlib-0.9.2/tests/testdata/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/bad/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-01 15:23:47.000000 pluginlib-0.9.2/tests/testdata/bad/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      408 2020-06-02 13:34:23.000000 pluginlib-0.9.2/tests/testdata/bad/syntax.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      533 2020-06-01 15:26:37.000000 pluginlib-0.9.2/tests/testdata/bad2.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.053404 pluginlib-0.9.2/tests/testdata/bare/
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/bare/engines/
+-rw-rw-r--   0 avram     (1000) avram     (1000)      524 2020-06-02 05:00:57.000000 pluginlib-0.9.2/tests/testdata/bare/engines/electric.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/bare/hooks/
+-rw-rw-r--   0 avram     (1000) avram     (1000)      553 2023-08-25 22:34:47.000000 pluginlib-0.9.2/tests/testdata/bare/hooks/fish.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      550 2020-06-02 05:04:18.000000 pluginlib-0.9.2/tests/testdata/bare/hooks/grappling.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/bare/package/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:13.000000 pluginlib-0.9.2/tests/testdata/bare/package/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/bare/package/parsers/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2020-06-02 04:46:24.000000 pluginlib-0.9.2/tests/testdata/bare/package/parsers/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      535 2020-06-02 05:02:36.000000 pluginlib-0.9.2/tests/testdata/bare/package/parsers/silly_walks.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.056404 pluginlib-0.9.2/tests/testdata/importer/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-15 02:39:55.000000 pluginlib-0.9.2/tests/testdata/importer/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/tests/testdata/lib/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:04.000000 pluginlib-0.9.2/tests/testdata/lib/__init__.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/tests/testdata/lib/engines/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-08 01:55:41.000000 pluginlib-0.9.2/tests/testdata/lib/engines/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      512 2020-06-02 05:03:03.000000 pluginlib-0.9.2/tests/testdata/lib/engines/steam.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/tests/testdata/lib/hooks/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.2/tests/testdata/lib/hooks/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      530 2020-06-02 05:03:14.000000 pluginlib-0.9.2/tests/testdata/lib/hooks/left.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      534 2020-06-02 05:03:22.000000 pluginlib-0.9.2/tests/testdata/lib/hooks/right.py
+drwxr-xr-x   0 avram     (1000) avram     (1000)        0 2024-04-15 15:44:58.057404 pluginlib-0.9.2/tests/testdata/lib/parsers/
+-rw-rw-r--   0 avram     (1000) avram     (1000)        0 2018-07-07 21:04:38.000000 pluginlib-0.9.2/tests/testdata/lib/parsers/__init__.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      669 2020-06-02 05:04:01.000000 pluginlib-0.9.2/tests/testdata/lib/parsers/json.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      503 2020-06-02 05:03:52.000000 pluginlib-0.9.2/tests/testdata/lib/parsers/xml.py
+-rw-rw-r--   0 avram     (1000) avram     (1000)      760 2018-07-09 01:05:42.000000 pluginlib-0.9.2/tests/testdata/parents.py
```

### Comparing `pluginlib-0.9.1/LICENSE` & `pluginlib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/PKG-INFO` & `pluginlib-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluginlib
-Version: 0.9.1
+Version: 0.9.2
 Summary: A framework for creating and importing plugins
 Home-page: https://github.com/Rockhopper-Technologies/pluginlib
 Author: Avram Lubkin
 Author-email: avylove@rockhopper.net
 License: MPLv2.0
 Keywords: plugin,plugins,pluginlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: setuptools
 
 .. start-badges
 
 | |docs| |gh_actions| |codecov|
 | |pypi| |supported-versions| |supported-implementations|
 | |fedora| |EPEL|
```

### Comparing `pluginlib-0.9.1/README.rst` & `pluginlib-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/doc/api.rst` & `pluginlib-0.9.2/doc/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-  Copyright 2018 Avram Lubkin, All Rights Reserved
+  Copyright 2020 Avram Lubkin, All Rights Reserved
 
   This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 :github_url: https://github.com/Rockhopper-Technologies/pluginlib
```

### Comparing `pluginlib-0.9.1/doc/concepts.rst` & `pluginlib-0.9.2/doc/concepts.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/doc/conf.py` & `pluginlib-0.9.2/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = []
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = '%sdoc' % project
```

### Comparing `pluginlib-0.9.1/doc/error_handling.rst` & `pluginlib-0.9.2/doc/error_handling.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/doc/faq.rst` & `pluginlib-0.9.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/doc/index.rst` & `pluginlib-0.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/pluginlib/__init__.py` & `pluginlib-0.9.2/pluginlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2014 - 2018 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib Package**
 
 A framework for creating and importing plugins
 """
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 __all__ = ['abstractmethod', 'abstractproperty', 'abstractstaticmethod', 'abstractclassmethod',
            'abstractattribute', 'BlacklistEntry', 'EntryPointWarning', 'Parent', 'Plugin',
            'PluginlibError', 'PluginImportError', 'PluginLoader', 'PluginWarning']
 
 from abc import abstractmethod, abstractproperty
```

### Comparing `pluginlib-0.9.1/pluginlib/_loader.py` & `pluginlib-0.9.2/pluginlib/_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     if isinstance(name, EntryPoint):
         epoint = name
         name = epoint.module_name
 
     if path is None:
         try:
             if PY2:
+                # pylint: disable-next=deprecated-method
                 loader = pkgutil.get_loader(name)  # pragma: no cover
             else:
                 loader = getattr(importlib.util.find_spec(name), 'loader', None)
         except ImportError:
             pass
         else:
             if loader:
```

### Comparing `pluginlib-0.9.1/pluginlib/_objects.py` & `pluginlib-0.9.2/pluginlib/_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib Object Module**
```

### Comparing `pluginlib-0.9.1/pluginlib/_parent.py` & `pluginlib-0.9.2/pluginlib/_parent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib Parent Submodule**
```

### Comparing `pluginlib-0.9.1/pluginlib/_util.py` & `pluginlib-0.9.2/pluginlib/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib Utility Module**
```

### Comparing `pluginlib-0.9.1/pluginlib/exceptions.py` & `pluginlib-0.9.2/pluginlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/pluginlib.egg-info/PKG-INFO` & `pluginlib-0.9.2/pluginlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluginlib
-Version: 0.9.1
+Version: 0.9.2
 Summary: A framework for creating and importing plugins
 Home-page: https://github.com/Rockhopper-Technologies/pluginlib
 Author: Avram Lubkin
 Author-email: avylove@rockhopper.net
 License: MPLv2.0
 Keywords: plugin,plugins,pluginlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: setuptools
 
 .. start-badges
 
 | |docs| |gh_actions| |codecov|
 | |pypi| |supported-versions| |supported-implementations|
 | |fedora| |EPEL|
```

### Comparing `pluginlib-0.9.1/pluginlib.egg-info/SOURCES.txt` & `pluginlib-0.9.2/pluginlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/setup.cfg` & `pluginlib-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 description_file = README.rst
-license_file = LICENSE
+license_files = LICENSE
 
 [flake8]
 builtins = __path__
 max-line-length = 100
 
 [pycodestyle]
 max-line-length = 100
```

### Comparing `pluginlib-0.9.1/setup.py` & `pluginlib-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2018 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Pluginlib setup file**
```

### Comparing `pluginlib-0.9.1/tests/__init__.py` & `pluginlib-0.9.2/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2018 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Test module for pluginlib**
```

### Comparing `pluginlib-0.9.1/tests/test_exceptions.py` & `pluginlib-0.9.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/test_loader.py` & `pluginlib-0.9.2/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Test module for pluginlib._loader**
```

### Comparing `pluginlib-0.9.1/tests/test_objects.py` & `pluginlib-0.9.2/tests/test_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Test module for pluginlib._objects**
```

### Comparing `pluginlib-0.9.1/tests/test_parent.py` & `pluginlib-0.9.2/tests/test_parent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2023 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Test module for pluginlib._parent**
```

### Comparing `pluginlib-0.9.1/tests/test_util.py` & `pluginlib-0.9.2/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2018 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Test module for pluginlib._util**
```

### Comparing `pluginlib-0.9.1/tests/testdata/bad2.py` & `pluginlib-0.9.2/tests/testdata/bad2.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/bare/engines/electric.py` & `pluginlib-0.9.2/tests/testdata/bare/engines/electric.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/bare/hooks/fish.py` & `pluginlib-0.9.2/tests/testdata/bare/hooks/fish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 - 2020 Avram Lubkin, All Rights Reserved
+# Copyright 2014 - 2022 Avram Lubkin, All Rights Reserved
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 **Fish hook**
```

### Comparing `pluginlib-0.9.1/tests/testdata/bare/hooks/grappling.py` & `pluginlib-0.9.2/tests/testdata/bare/hooks/grappling.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/bare/package/parsers/silly_walks.py` & `pluginlib-0.9.2/tests/testdata/bare/package/parsers/silly_walks.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/lib/engines/steam.py` & `pluginlib-0.9.2/tests/testdata/lib/engines/steam.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/lib/hooks/left.py` & `pluginlib-0.9.2/tests/testdata/lib/hooks/left.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/lib/hooks/right.py` & `pluginlib-0.9.2/tests/testdata/lib/hooks/right.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/lib/parsers/json.py` & `pluginlib-0.9.2/tests/testdata/lib/parsers/json.py`

 * *Files identical despite different names*

### Comparing `pluginlib-0.9.1/tests/testdata/parents.py` & `pluginlib-0.9.2/tests/testdata/parents.py`

 * *Files identical despite different names*

