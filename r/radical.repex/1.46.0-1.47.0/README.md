# Comparing `tmp/radical.repex-1.46.0.tar.gz` & `tmp/radical.repex-1.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical.repex-1.46.0.tar", last modified: Thu Jan 11 08:26:28 2024, max compression
+gzip compressed data, was "radical.repex-1.47.0.tar", last modified: Thu Feb  8 22:00:15 2024, max compression
```

## Comparing `radical.repex-1.46.0.tar` & `radical.repex-1.47.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2498 2024-01-11 08:26:23.000000 radical.repex-1.46.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical.repex-1.46.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical.repex-1.46.0/MANIFEST.in
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-01-11 08:26:28.693610 radical.repex-1.46.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical.repex-1.46.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-01-11 08:25:53.000000 radical.repex-1.46.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical.repex-1.46.0/bin/radical-repex
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical.repex-1.46.0/bin/radical-repex-version
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-01-11 08:26:28.693610 radical.repex-1.46.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10450 2022-08-15 10:38:30.000000 radical.repex-1.46.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/src/radical/repex/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical/repex/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical/repex/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical.repex-1.46.0/src/radical/repex/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical.repex-1.46.0/src/radical/repex/algorithms.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical.repex-1.46.0/src/radical/repex/exchange.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical.repex-1.46.0/src/radical/repex/replica.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical.repex-1.46.0/src/radical/repex/utils.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-01-11 08:26:28.693610 radical.repex-1.46.0/src/radical.repex.egg-info/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      606 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-01-11 08:26:28.000000 radical.repex-1.46.0/src/radical.repex.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2753 2024-02-08 22:00:09.000000 radical.repex-1.47.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical.repex-1.47.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical.repex-1.47.0/MANIFEST.in
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-02-08 22:00:15.297839 radical.repex-1.47.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical.repex-1.47.0/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-02-08 21:59:57.000000 radical.repex-1.47.0/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical.repex-1.47.0/bin/radical-repex
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical.repex-1.47.0/bin/radical-repex-version
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-02-08 22:00:15.297839 radical.repex-1.47.0/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    10450 2022-08-15 10:38:30.000000 radical.repex-1.47.0/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical/repex/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical/repex/SDIST
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical/repex/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical.repex-1.47.0/src/radical/repex/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/algorithms.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/exchange.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/replica.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/utils.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical.repex.egg-info/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      606 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/top_level.txt
```

### Comparing `radical.repex-1.46.0/CHANGES.md` & `radical.repex-1.47.0/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,20 @@
     https://github.com/radical-cybertools/radical.repex/ \
             issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
   - For a list of open issues and known problems, see
     https://github.com/radical-cybertools/radical.repex/ \
             issues?q=is%3Aissue+is%3Aopen+
 
 
+1.47.0 Release                                                        2024-02-08
+--------------------------------------------------------------------------------
+
+  - maintenance
+
+
 1.46.0 Release                                                        2024-01-11
 --------------------------------------------------------------------------------
 
   - pypi fix
 
 
 1.44.0 Release                                                        2024-01-10
@@ -69,7 +75,8 @@
 --------------------------------------------------------------------------------
 
   -  initial commit for radical project 'repex'
 
 
 --------------------------------------------------------------------------------
 
+  - (HEAD -> master, origin/devel, origin/HEAD, devel) devel version bump
```

### Comparing `radical.repex-1.46.0/LICENSE.md` & `radical.repex-1.47.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/PKG-INFO` & `radical.repex-1.47.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.46.0
+Version: 1.47.0
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.repex-1.46.0/README.md` & `radical.repex-1.47.0/README.md`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/bin/radical-repex` & `radical.repex-1.47.0/bin/radical-repex`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/setup.py` & `radical.repex-1.47.0/setup.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical/repex/__init__.py` & `radical.repex-1.47.0/src/radical/repex/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical/repex/algorithms.py` & `radical.repex-1.47.0/src/radical/repex/algorithms.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical/repex/exchange.py` & `radical.repex-1.47.0/src/radical/repex/exchange.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical/repex/replica.py` & `radical.repex-1.47.0/src/radical/repex/replica.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical/repex/utils.py` & `radical.repex-1.47.0/src/radical/repex/utils.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.46.0/src/radical.repex.egg-info/PKG-INFO` & `radical.repex-1.47.0/src/radical.repex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.46.0
+Version: 1.47.0
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.repex-1.46.0/src/radical.repex.egg-info/SOURCES.txt` & `radical.repex-1.47.0/src/radical.repex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

