# Comparing `tmp/radical_repex-1.47.1.tar.gz` & `tmp/radical_repex-1.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_repex-1.47.1.tar", last modified: Mon Apr 15 06:14:50 2024, max compression
+gzip compressed data, was "radical_repex-1.50.0.tar", last modified: Mon Apr 15 07:50:23 2024, max compression
```

## Comparing `radical_repex-1.47.1.tar` & `radical_repex-1.50.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2753 2024-02-08 22:00:18.000000 radical_repex-1.47.1/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical_repex-1.47.1/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical_repex-1.47.1/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 06:14:50.606056 radical_repex-1.47.1/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical_repex-1.47.1/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 06:14:14.000000 radical_repex-1.47.1/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical_repex-1.47.1/bin/radical-repex
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical_repex-1.47.1/bin/radical-repex-version
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-04-15 06:14:50.606056 radical_repex-1.47.1/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10332 2024-04-15 06:14:46.000000 radical_repex-1.47.1/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/src/radical/repex/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical/repex/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical/repex/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical_repex-1.47.1/src/radical/repex/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/algorithms.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/exchange.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/replica.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/utils.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/src/radical.repex.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      556 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2875 2024-04-15 07:50:15.000000 radical_repex-1.50.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical_repex-1.50.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical_repex-1.50.0/MANIFEST.in
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 07:50:23.942277 radical_repex-1.50.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical_repex-1.50.0/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 07:49:54.000000 radical_repex-1.50.0/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical_repex-1.50.0/bin/radical-repex
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical_repex-1.50.0/bin/radical-repex-version
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-04-15 07:50:23.942277 radical_repex-1.50.0/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    10332 2024-04-15 07:40:43.000000 radical_repex-1.50.0/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/src/radical/repex/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical/repex/SDIST
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical/repex/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical_repex-1.50.0/src/radical/repex/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical_repex-1.50.0/src/radical/repex/algorithms.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical_repex-1.50.0/src/radical/repex/exchange.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical_repex-1.50.0/src/radical/repex/replica.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical_repex-1.50.0/src/radical/repex/utils.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:50:23.942277 radical_repex-1.50.0/src/radical.repex.egg-info/
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      556 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 07:50:23.000000 radical_repex-1.50.0/src/radical.repex.egg-info/top_level.txt
```

### Comparing `radical_repex-1.47.1/CHANGES.md` & `radical_repex-1.50.0/CHANGES.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,20 @@
     https://github.com/radical-cybertools/radical.repex/ \
             issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
   - For a list of open issues and known problems, see
     https://github.com/radical-cybertools/radical.repex/ \
             issues?q=is%3Aissue+is%3Aopen+
 
 
+1.50.0 Release                                                        2024-04-15
+--------------------------------------------------------------------------------
+
+  - fix for setuptools upgrade
+
+
 1.47.0 Release                                                        2024-02-08
 --------------------------------------------------------------------------------
 
   - maintenance
 
 
 1.46.0 Release                                                        2024-01-11
@@ -75,8 +81,7 @@
 --------------------------------------------------------------------------------
 
   -  initial commit for radical project 'repex'
 
 
 --------------------------------------------------------------------------------
 
-  - (HEAD -> master, origin/devel, origin/HEAD, devel) devel version bump
```

### Comparing `radical_repex-1.47.1/LICENSE.md` & `radical_repex-1.50.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/PKG-INFO` & `radical_repex-1.50.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.47.1
+Version: 1.50.0
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical_repex-1.47.1/README.md` & `radical_repex-1.50.0/README.md`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/bin/radical-repex` & `radical_repex-1.50.0/bin/radical-repex`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/setup.py` & `radical_repex-1.50.0/setup.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical/repex/__init__.py` & `radical_repex-1.50.0/src/radical/repex/__init__.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical/repex/algorithms.py` & `radical_repex-1.50.0/src/radical/repex/algorithms.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical/repex/exchange.py` & `radical_repex-1.50.0/src/radical/repex/exchange.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical/repex/replica.py` & `radical_repex-1.50.0/src/radical/repex/replica.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical/repex/utils.py` & `radical_repex-1.50.0/src/radical/repex/utils.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.47.1/src/radical.repex.egg-info/PKG-INFO` & `radical_repex-1.50.0/src/radical.repex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.47.1
+Version: 1.50.0
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical_repex-1.47.1/src/radical.repex.egg-info/SOURCES.txt` & `radical_repex-1.50.0/src/radical.repex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

