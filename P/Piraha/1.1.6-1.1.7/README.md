# Comparing `tmp/Piraha-1.1.6.tar.gz` & `tmp/Piraha-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Piraha-1.1.6.tar", last modified: Fri Feb  3 22:20:25 2023, max compression
+gzip compressed data, was "Piraha-1.1.7.tar", last modified: Mon Apr 15 21:02:01 2024, max compression
```

## Comparing `Piraha-1.1.6.tar` & `Piraha-1.1.7.tar`

### file list

```diff
@@ -1,26 +1,18 @@
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:24.215167 Piraha-1.1.6/
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)     1062 2022-10-12 18:21:11.000000 Piraha-1.1.6/LICENSE
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      295 2023-02-03 22:20:24.207169 Piraha-1.1.6/PKG-INFO
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:23.940950 Piraha-1.1.6/Piraha.egg-info/
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      295 2023-02-03 22:20:20.000000 Piraha-1.1.6/Piraha.egg-info/PKG-INFO
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      362 2023-02-03 22:20:22.000000 Piraha-1.1.6/Piraha.egg-info/SOURCES.txt
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)        1 2023-02-03 22:20:20.000000 Piraha-1.1.6/Piraha.egg-info/dependency_links.txt
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)        7 2023-02-03 22:20:20.000000 Piraha-1.1.6/Piraha.egg-info/top_level.txt
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      211 2021-03-10 22:31:41.000000 Piraha-1.1.6/README.md
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:23.771556 Piraha-1.1.6/examples/
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:24.004470 Piraha-1.1.6/examples/calc/
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      382 2021-03-10 22:31:41.000000 Piraha-1.1.6/examples/calc/calc.peg
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)     1531 2022-10-14 20:08:32.000000 Piraha-1.1.6/examples/calc/calc.py
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:24.097159 Piraha-1.1.6/examples/calc2/
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)       67 2021-03-10 22:31:41.000000 Piraha-1.1.6/examples/calc2/calc.in
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      481 2021-03-10 22:31:41.000000 Piraha-1.1.6/examples/calc2/calc.peg
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)     1981 2022-10-14 20:08:32.000000 Piraha-1.1.6/examples/calc2/calc.py
-drwxr-xr-x   0 sbrandt   (1000) sbrandt   (1000)        0 2023-02-03 22:20:24.187076 Piraha-1.1.6/piraha/
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)    38377 2023-02-03 22:18:42.000000 Piraha-1.1.6/piraha/__init__.py
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      795 2023-02-03 21:20:20.000000 Piraha-1.1.6/piraha/colored.py
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      486 2023-02-03 22:17:24.000000 Piraha-1.1.6/piraha/here.py
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)        0 2023-01-20 15:04:17.000000 Piraha-1.1.6/piraha/py.typed
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)       22 2023-02-03 22:18:54.000000 Piraha-1.1.6/piraha/version.py
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)       96 2022-10-12 18:21:16.000000 Piraha-1.1.6/pyproject.toml
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)       38 2023-02-03 22:20:24.216165 Piraha-1.1.6/setup.cfg
--rw-r--r--   0 sbrandt   (1000) sbrandt   (1000)      694 2023-01-20 03:58:39.000000 Piraha-1.1.6/setup.py
+drwxr-xr-x   0 sbrandt   (1000) docker    (1001)        0 2024-04-15 21:02:01.312655 Piraha-1.1.7/
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)     1062 2023-04-18 18:06:01.000000 Piraha-1.1.7/LICENSE
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      314 2024-04-15 21:02:01.312655 Piraha-1.1.7/PKG-INFO
+drwxr-xr-x   0 sbrandt   (1000) docker    (1001)        0 2024-04-15 21:02:01.171630 Piraha-1.1.7/Piraha.egg-info/
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      314 2024-04-15 21:02:00.000000 Piraha-1.1.7/Piraha.egg-info/PKG-INFO
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      247 2024-04-15 21:02:00.000000 Piraha-1.1.7/Piraha.egg-info/SOURCES.txt
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)        1 2024-04-15 21:02:00.000000 Piraha-1.1.7/Piraha.egg-info/dependency_links.txt
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)        7 2024-04-15 21:02:00.000000 Piraha-1.1.7/Piraha.egg-info/top_level.txt
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      211 2023-04-18 18:06:01.000000 Piraha-1.1.7/README.md
+drwxr-xr-x   0 sbrandt   (1000) docker    (1001)        0 2024-04-15 21:02:01.281402 Piraha-1.1.7/piraha/
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)    38377 2023-04-18 18:06:01.000000 Piraha-1.1.7/piraha/__init__.py
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      794 2024-04-15 20:39:57.000000 Piraha-1.1.7/piraha/colored.py
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      486 2023-04-18 18:06:01.000000 Piraha-1.1.7/piraha/here.py
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)        0 2023-04-18 18:06:01.000000 Piraha-1.1.7/piraha/py.typed
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)       22 2024-04-15 20:40:34.000000 Piraha-1.1.7/piraha/version.py
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)       96 2023-04-18 18:06:01.000000 Piraha-1.1.7/pyproject.toml
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)       38 2024-04-15 21:02:01.312655 Piraha-1.1.7/setup.cfg
+-rw-r--r--   0 sbrandt   (1000) docker    (1001)      694 2023-04-18 18:06:01.000000 Piraha-1.1.7/setup.py
```

### Comparing `Piraha-1.1.6/LICENSE` & `Piraha-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Piraha-1.1.6/piraha/__init__.py` & `Piraha-1.1.7/piraha/__init__.py`

 * *Files identical despite different names*

### Comparing `Piraha-1.1.6/piraha/colored.py` & `Piraha-1.1.7/piraha/colored.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 import sys
 
 def not_colored(a,_):
-    return repr(a)
+    return str(a)
 
 colors = {
   "red":"\033[31m",
   "green":"\033[32m",
   "yellow":"\033[33m",
   "blue":"\033[34m",
   "magenta":"\033[35m",
```

### Comparing `Piraha-1.1.6/setup.py` & `Piraha-1.1.7/setup.py`

 * *Files identical despite different names*

