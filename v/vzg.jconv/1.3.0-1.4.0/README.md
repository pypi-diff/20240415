# Comparing `tmp/vzg.jconv-1.3.0.tar.gz` & `tmp/vzg.jconv-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.3.0.tar", last modified: Mon Aug  7 14:51:18 2023, max compression
+gzip compressed data, was "vzg.jconv-1.4.0.tar", last modified: Mon Apr 15 11:12:22 2024, max compression
```

## Comparing `vzg.jconv-1.3.0.tar` & `vzg.jconv-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.3.0/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.3.0/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.3.0/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-07 14:50:50.000000 vzg.jconv-1.3.0/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1868 2023-08-02 11:54:02.000000 vzg.jconv-1.3.0/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.890899 vzg.jconv-1.3.0/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.3.0/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.3.0/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/archives/
--rw-rw-r--   0 teg       (1000) teg       (1000)      361 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/archives/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2323 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/archives/springer.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.3.0/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    15363 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4136 2023-08-01 08:59:23.000000 vzg.jconv-1.3.0/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1285 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/journal/
--rw-rw-r--   0 teg       (1000) teg       (1000)     6629 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/journal/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.3.0/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.3.0/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.3.0/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.3.0/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.3.0/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/conftest.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1819 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_archives.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_degruyter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-01 09:54:23.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jatsdate.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_journal.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.3.0/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6200 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.3.0/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-01 09:44:49.000000 vzg.jconv-1.3.0/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1422 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.4.0/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.4.0/MANIFEST.in
+-rw-r--r--   0 teg       (1000) teg       (1000)     1493 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2024-04-15 11:10:31.000000 vzg.jconv-1.4.0/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2035 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.4.0/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/archives/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      361 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/archives/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4247 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/archives/oai.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2323 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/archives/springer.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.4.0/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    15358 2023-10-13 08:10:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     8434 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/converter/oai.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.4.0/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5745 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1285 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/journal/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6629 2023-10-13 08:10:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/journal/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.4.0/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.4.0/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.4.0/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.776120 vzg.jconv-1.4.0/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.4.0/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2552 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_archives.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     7269 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_jatsdate.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3980 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_journal.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6269 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_oai_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1086 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_oai_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.4.0/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.4.0/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     9002 2024-04-15 11:09:26.000000 vzg.jconv-1.4.0/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-25 10:32:02.000000 vzg.jconv-1.4.0/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2024-04-15 11:12:22.780120 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/
+-rw-r--r--   0 teg       (1000) teg       (1000)     1493 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1543 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       64 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2024-01-23 13:48:55.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2024-04-15 11:12:22.000000 vzg.jconv-1.4.0/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.3.0/LICENSE.txt` & `vzg.jconv-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/PKG-INFO` & `vzg.jconv-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: jsonschema
+Requires-Dist: lxml
+Requires-Dist: setuptools
+Requires-Dist: wheel
+Requires-Dist: zope.interface
 
 # VZG Schema Converter Library
 
 This library converts specific metadata files to [JSON VZG Schema](https://github.com/gbv/articleformat).
 
 ## Metadata sources
 
@@ -35,9 +40,7 @@
 foo@bar:~$ python3 -m venv vzg.jconv
 foo@bar:~$ cd vzg.jconv
 foo@bar:~$ source bin/activate
 (vzg.jconv) foo@bar:~$ pip install --upgrade pip
 (vzg.jconv) foo@bar:~$ pip install vzg.jconv
 (vzg.jconv) foo@bar:~$ simple-conv -h
 ```
-
-
```

### Comparing `vzg.jconv-1.3.0/setup.py` & `vzg.jconv-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 
 def gc(fname):
@@ -32,26 +32,32 @@
     long_description_content_type="text/markdown",
     keywords="VZG Python JSON XML JAST",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU Affero General Public License v3",
     ],
     url="https://github.com/gbv/vzg.jconv",
     project_urls={
         "PyPI": "https://pypi.python.org/pypi/vzg.jconv",
         "Source": "https://github.com/gbv/vzg.jconv",
         "Tracker": "https://github.com/gbv/vzg.jconv/issues",
     },
-    packages=find_packages("src"),
+    packages=find_namespace_packages("src"),
     include_package_data=True,
     license="GNU Affero General Public License v3",
     package_dir={"": "src"},
     namespace_packages=["vzg"],
-    install_requires=["jsonschema", "lxml", "setuptools", "wheel", "zope.interface"],
+    install_requires=["jsonschema",
+                      "lxml",
+                      "setuptools",
+                      "wheel",
+                      "zope.interface"],
     zip_safe=False,
     python_requires=">=3.10",
-    entry_points={"console_scripts": ["simple-conv = vzg.jconv.tools.simple_conv:run"]},
+    entry_points={"console_scripts": [
+        "simple-conv = vzg.jconv.tools.simple_conv:run"]},
 )
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/archives/springer.py` & `vzg.jconv-1.4.0/src/vzg/jconv/archives/springer.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/converter/jats.py` & `vzg.jconv-1.4.0/src/vzg/jconv/converter/jats.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,17 +353,16 @@
                 "lang_code": lang_code,
             }
 
             for node in groupnode.xpath(subjext_exp):
                 subject["terms"].append(node)
 
             if (
-                len(subject["lang_code"]) > 0
-                and len(subject["scheme"]) > 0
-                and len(subject["terms"]) > 0
+                (len(subject["lang_code"]) > 0) and (
+                    len(subject["scheme"]) > 0) and (len(subject["terms"]) > 0)
             ):
                 subjects.append(subject)
 
         return subjects
 
     @property
     def title(self):
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.4.0/src/vzg/jconv/interfaces.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/journal/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.4.0/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.4.0/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/conftest.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/conftest.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_archives.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_archives.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 #
 # Copyright (c) 2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
+import datetime
 import unittest
 import zipfile
 from pathlib import Path
 from zope.interface import providedBy
+from vzg.jconv.archives.oai import ArchiveOAIDC
 from vzg.jconv.archives.springer import ArchiveSpringer
 from vzg.jconv.converter.jats import JatsConverter
+from vzg.jconv.converter.oai import OAIDCConverter
 from vzg.jconv.interfaces import IConverter
 
 
 __author__ = """Marc-J. Tegethoff <tegethoff@gbv.de>"""
 __docformat__ = 'plaintext'
 
 
@@ -59,7 +62,28 @@
         """"""
         archive = ArchiveSpringer(self.archive)
 
         for conv in archive.converters:
             self.assertIn(IConverter, providedBy(conv), "IConverter")
             self.assertIsInstance(conv, JatsConverter, "Konverter")
             self.assertEqual(conv.name, self.fpath, "Name")
+
+
+class TestOAIDC(unittest.TestCase):
+
+    def setUp(self) -> None:
+        self.baseurl = Path(
+            "data/tests/oai/2024-01-23_10-59-52-001.zip").absolute().as_posix()
+
+    def test_num(self):
+        """"""
+        archive = ArchiveOAIDC(self.baseurl)
+
+        self.assertEqual(archive.num_files, 19, "Anzahl der Dateien")
+
+    def test_converter(self):
+        """"""
+        archive = ArchiveOAIDC(self.baseurl)
+
+        for i, conv in enumerate(archive.converters):
+            self.assertIn(IConverter, providedBy(conv), "IConverter")
+            self.assertIsInstance(conv, OAIDCConverter, "Konverter")
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_article.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_converter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_degruyter.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_jats_degruyter.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         """primary_id"""
         self.assertEqual(
             self.jobj.primary_id, self.testdata["primary_id"], "primary_id"
         )
 
     def test04(self):
         """journal"""
-        print(self.jobj.journal)
         self.assertEqual(self.jobj.journal, self.testdata["journal"], "journal")
 
     def test05(self):
         """other_ids"""
         self.assertEqual(self.jobj.other_ids, self.testdata["other_ids"], "other_ids")
 
     def test06(self):
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jatsdate.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_jatsdate.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_journal.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_journal.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,14 @@
         self.assertEqual(
             journal.date.year, int(self.testdata["journal"]["year"]), "year"
         )
 
     def test06_journal_ids(self):
         journal = JatsJournal(self.article)
 
-        print(journal.ids)
-
         self.assertEqual(
             journal.ids,
             self.testdata["journal"]["journal_ids"],
             "ids",
         )
 
     def test07_journal_publisher(self):
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.4.0/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.4.0/src/vzg/jconv/tools/simple_conv.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 # Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
+import datetime
 import logging
+import uuid
 from pathlib import Path
 import zipfile
 import tempfile
 from vzg.jconv.archives.springer import ArchiveSpringer
+from vzg.jconv.archives.oai import ArchiveOAIDC
 from vzg.jconv.converter.jats import JatsConverter
+from vzg.jconv.converter.oai import OAIDCConverter
+from vzg.jconv.gapi import OAI_ARTICLES_TYPES
+
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 
 def fromarchive(options):
     """Uses a ZIP Archive as source"""
@@ -71,16 +77,14 @@
                         msg = "Validation problem"
                         logger.info(msg)
                         break
 
 
 def jats(options):
     """Use a ZIP Archive as source."""
-    import uuid
-
     logger = logging.getLogger(__name__)
 
     jpath = Path(options.jfiles[0]).absolute()
     opath = Path(options.outdir).absolute()
     dst = opath / jpath.name
     deliverysignature = uuid.uuid4()
 
@@ -115,25 +119,131 @@
                     )
 
             if options.stop and jconv.validation_failed:
                 msg = "Validation problem"
                 logger.info(msg)
                 break
 
+            del jconv
+
+
+def oai(options):
+    """Use a OAI responses as source"""
+    logger = logging.getLogger(__name__)
+
+    deliverysignature = uuid.uuid4()
+    opath = Path(options.outdir).absolute()
+
+    atype = getattr(OAI_ARTICLES_TYPES,
+                    options.publisher,
+                    OAI_ARTICLES_TYPES.unknown)
+
+    archive = ArchiveOAIDC(options.zippath[0],
+                           converter_kwargs={"article_type": atype,
+                                             "validate": options.validate})
+    num_res = float(archive.num_files)
+
+    for i, conv in enumerate(archive.converters):
+        xpercent = i / num_res * 100
+        msg = f"{conv.header.identifier} ({xpercent:.2f}%)"
+        logger.info(msg)
+
+        conv.run()
+
+        anum = len(conv.articles)
+        msg = f"\t{anum} article(s)"
+        logger.info(msg)
+
+        if options.dry_run is False:
+            for j, article in enumerate(conv.articles):
+                aname = f"{deliverysignature}-{i}-{j}.json"
+                logger.info(aname)
+                jpath = opath / aname
+
+                with jpath.open("w") as jfh:
+                    jfh.write(article.json)
+
+        if options.stop and conv.validation_failed:
+            msg = "Validation problem"
+            logger.info(msg)
+            break
+
+        del conv
+
 
 def run():
     """Start the application"""
     from argparse import ArgumentParser
 
     description = "Simple conversion tool."
 
     parser = ArgumentParser(description=description)
 
     subparsers = parser.add_subparsers()
 
+    parser_oai = subparsers.add_parser(
+        "oai", help="Convert OAI responses"
+    )
+
+    parser_oai.add_argument(
+        "-n",
+        "--dry-run",
+        dest="dry_run",
+        action="store_true",
+        default=False,
+        help="Do nothing",
+    )
+
+    parser_oai.add_argument(
+        "-p",
+        "--publisher",
+        dest="publisher",
+        metavar="Publisher",
+        type=str,
+        required=False,
+        default="unknown",
+        help="""The name of the publisher. Values: [openedition|cairn]""",
+    )
+
+    parser_oai.add_argument(
+        "-o",
+        "--output-directory",
+        dest="outdir",
+        metavar="Output directory",
+        type=str,
+        default="output",
+        help="Directory of JSON files",
+    )
+
+    parser_oai.add_argument(
+        "--stop",
+        dest="stop",
+        action="store_true",
+        default=False,
+        help="Stop if JSON Schema Validation fails",
+    )
+
+    parser_oai.add_argument(
+        "--validate",
+        dest="validate",
+        action="store_true",
+        default=False,
+        help="JSON Schema Validation",
+    )
+
+    parser_oai.add_argument(
+        dest="zippath",
+        metavar="Zipfile",
+        type=str,
+        nargs=1,
+        help="Zipfile with OAI records",
+    )
+
+    parser_oai.set_defaults(func=oai)
+
     parser_springer = subparsers.add_parser(
         "jats", help="Convert JATS files from ZIP files"
     )
 
     parser_springer.add_argument(
         "-n",
         "--dry-run",
```

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.4.0/src/vzg/jconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.4.0/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.3.0/src/vzg.jconv.egg-info/PKG-INFO` & `vzg.jconv-1.4.0/src/vzg.jconv.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: jsonschema
+Requires-Dist: lxml
+Requires-Dist: setuptools
+Requires-Dist: wheel
+Requires-Dist: zope.interface
 
 # VZG Schema Converter Library
 
 This library converts specific metadata files to [JSON VZG Schema](https://github.com/gbv/articleformat).
 
 ## Metadata sources
 
@@ -35,9 +40,7 @@
 foo@bar:~$ python3 -m venv vzg.jconv
 foo@bar:~$ cd vzg.jconv
 foo@bar:~$ source bin/activate
 (vzg.jconv) foo@bar:~$ pip install --upgrade pip
 (vzg.jconv) foo@bar:~$ pip install vzg.jconv
 (vzg.jconv) foo@bar:~$ simple-conv -h
 ```
-
-
```

### Comparing `vzg.jconv-1.3.0/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.4.0/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 VERSION.txt
 setup.cfg
 setup.py
-src/vzg/__init__.py
 src/vzg.jconv.egg-info/PKG-INFO
 src/vzg.jconv.egg-info/SOURCES.txt
 src/vzg.jconv.egg-info/dependency_links.txt
 src/vzg.jconv.egg-info/entry_points.txt
 src/vzg.jconv.egg-info/namespace_packages.txt
 src/vzg.jconv.egg-info/not-zip-safe
 src/vzg.jconv.egg-info/requires.txt
 src/vzg.jconv.egg-info/top_level.txt
 src/vzg/jconv/__init__.py
 src/vzg/jconv/errors.py
 src/vzg/jconv/gapi.py
 src/vzg/jconv/interfaces.py
 src/vzg/jconv/archives/__init__.py
+src/vzg/jconv/archives/oai.py
 src/vzg/jconv/archives/springer.py
 src/vzg/jconv/converter/__init__.py
 src/vzg/jconv/converter/jats.py
+src/vzg/jconv/converter/oai.py
 src/vzg/jconv/journal/__init__.py
 src/vzg/jconv/langcode/__init__.py
 src/vzg/jconv/langcode/language-codes.json
 src/vzg/jconv/person/__init__.py
 src/vzg/jconv/publisher/__init__.py
 src/vzg/jconv/publisher/publisher-codes.json
 src/vzg/jconv/schema/article_schema.json
@@ -33,13 +34,15 @@
 src/vzg/jconv/test/test_archives.py
 src/vzg/jconv/test/test_jats_article.py
 src/vzg/jconv/test/test_jats_converter.py
 src/vzg/jconv/test/test_jats_degruyter.py
 src/vzg/jconv/test/test_jatsdate.py
 src/vzg/jconv/test/test_journal.py
 src/vzg/jconv/test/test_langcode.py
+src/vzg/jconv/test/test_oai_article.py
+src/vzg/jconv/test/test_oai_converter.py
 src/vzg/jconv/test/test_person.py
 src/vzg/jconv/test/test_publisher.py
 src/vzg/jconv/tools/__init__.py
 src/vzg/jconv/tools/simple_conv.py
 src/vzg/jconv/utils/__init__.py
 src/vzg/jconv/utils/date.py
```

