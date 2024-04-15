# Comparing `tmp/ParendumLib-0.1.8.tar.gz` & `tmp/ParendumLib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParendumLib-0.1.8.tar", last modified: Thu Dec 28 22:19:16 2023, max compression
+gzip compressed data, was "ParendumLib-0.1.9.tar", last modified: Mon Apr 15 12:35:18 2024, max compression
```

## Comparing `ParendumLib-0.1.8.tar` & `ParendumLib-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-12-28 22:19:16.110631 ParendumLib-0.1.8/
--rw-rw-rw-   0        0        0      163 2023-12-28 22:19:16.109211 ParendumLib-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-28 22:19:16.104263 ParendumLib-0.1.8/ParendumLib.egg-info/
--rw-rw-rw-   0        0        0      163 2023-12-28 22:19:15.000000 ParendumLib-0.1.8/ParendumLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-12-28 22:19:16.000000 ParendumLib-0.1.8/ParendumLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-28 22:19:15.000000 ParendumLib-0.1.8/ParendumLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-12-28 22:19:15.000000 ParendumLib-0.1.8/ParendumLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-12-28 22:19:15.000000 ParendumLib-0.1.8/ParendumLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1253 2023-12-17 23:21:59.000000 ParendumLib-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-28 22:19:16.108030 ParendumLib-0.1.8/parendumlib/
--rw-rw-rw-   0        0        0      222 2023-12-27 22:30:57.000000 ParendumLib-0.1.8/parendumlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-28 22:19:16.108030 ParendumLib-0.1.8/parendumlib/database/
--rw-rw-rw-   0        0        0        0 2023-12-27 20:05:10.000000 ParendumLib-0.1.8/parendumlib/database/__init__.py
--rw-rw-rw-   0        0        0     3458 2023-12-27 20:21:09.000000 ParendumLib-0.1.8/parendumlib/database/mongodb.py
--rw-rw-rw-   0        0        0       55 2023-10-10 13:03:24.000000 ParendumLib-0.1.8/parendumlib/exceptions.py
--rw-rw-rw-   0        0        0     5318 2023-12-21 01:19:55.000000 ParendumLib-0.1.8/parendumlib/logger.py
--rw-rw-rw-   0        0        0     3821 2023-12-26 07:28:58.000000 ParendumLib-0.1.8/parendumlib/mailer.py
-drwxrwxrwx   0        0        0        0 2023-12-28 22:19:16.109211 ParendumLib-0.1.8/parendumlib/permissions/
--rw-rw-rw-   0        0        0        0 2023-12-27 22:27:26.000000 ParendumLib-0.1.8/parendumlib/permissions/__init__.py
--rw-rw-rw-   0        0        0     3273 2023-12-27 22:35:03.000000 ParendumLib-0.1.8/parendumlib/permissions/mongodb.py
--rw-rw-rw-   0        0        0     1483 2023-12-27 22:31:06.000000 ParendumLib-0.1.8/parendumlib/responses.py
--rw-rw-rw-   0        0        0     2089 2023-12-28 22:19:08.000000 ParendumLib-0.1.8/parendumlib/utils.py
--rw-rw-rw-   0        0        0       42 2023-12-28 22:19:16.110631 ParendumLib-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      386 2023-12-28 22:19:12.000000 ParendumLib-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/
+-rw-rw-rw-   0        0        0      233 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.141933 ParendumLib-0.1.9/ParendumLib.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 12:35:18.000000 ParendumLib-0.1.9/ParendumLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1253 2023-12-17 23:21:59.000000 ParendumLib-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.146577 ParendumLib-0.1.9/parendumlib/
+-rw-rw-rw-   0        0        0      222 2023-12-27 22:30:57.000000 ParendumLib-0.1.9/parendumlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/parendumlib/database/
+-rw-rw-rw-   0        0        0        0 2023-12-27 20:05:10.000000 ParendumLib-0.1.9/parendumlib/database/__init__.py
+-rw-rw-rw-   0        0        0     3458 2023-12-27 20:21:09.000000 ParendumLib-0.1.9/parendumlib/database/mongodb.py
+-rw-rw-rw-   0        0        0       55 2023-10-10 13:03:24.000000 ParendumLib-0.1.9/parendumlib/exceptions.py
+-rw-rw-rw-   0        0        0     5318 2023-12-21 01:19:55.000000 ParendumLib-0.1.9/parendumlib/logger.py
+-rw-rw-rw-   0        0        0     4996 2024-04-15 12:30:24.000000 ParendumLib-0.1.9/parendumlib/mailer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/parendumlib/permissions/
+-rw-rw-rw-   0        0        0        0 2023-12-27 22:27:26.000000 ParendumLib-0.1.9/parendumlib/permissions/__init__.py
+-rw-rw-rw-   0        0        0     3273 2023-12-27 22:35:03.000000 ParendumLib-0.1.9/parendumlib/permissions/mongodb.py
+-rw-rw-rw-   0        0        0     1483 2023-12-27 22:31:06.000000 ParendumLib-0.1.9/parendumlib/responses.py
+-rw-rw-rw-   0        0        0     2089 2023-12-28 22:19:08.000000 ParendumLib-0.1.9/parendumlib/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:35:18.148513 ParendumLib-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-04-15 12:30:32.000000 ParendumLib-0.1.9/setup.py
```

### Comparing `ParendumLib-0.1.8/README.md` & `ParendumLib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.8/parendumlib/database/mongodb.py` & `ParendumLib-0.1.9/parendumlib/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.8/parendumlib/logger.py` & `ParendumLib-0.1.9/parendumlib/logger.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.8/parendumlib/permissions/mongodb.py` & `ParendumLib-0.1.9/parendumlib/permissions/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.8/parendumlib/responses.py` & `ParendumLib-0.1.9/parendumlib/responses.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.1.8/parendumlib/utils.py` & `ParendumLib-0.1.9/parendumlib/utils.py`

 * *Files identical despite different names*

