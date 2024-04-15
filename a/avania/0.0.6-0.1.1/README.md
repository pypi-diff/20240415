# Comparing `tmp/avania-0.0.6.tar.gz` & `tmp/avania-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.0.6.tar", last modified: Thu Apr 11 06:21:05 2024, max compression
+gzip compressed data, was "avania-0.1.1.tar", last modified: Mon Apr 15 04:46:45 2024, max compression
```

## Comparing `avania-0.0.6.tar` & `avania-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:21:05.125361 avania-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-11 06:20:49.000000 avania-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 06:21:05.125361 avania-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 06:20:49.000000 avania-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:21:05.121361 avania-0.0.6/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 06:20:49.000000 avania-0.0.6/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:21:05.121361 avania-0.0.6/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 06:20:49.000000 avania-0.0.6/avania/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 06:20:49.000000 avania-0.0.6/avania/orm/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:21:05.125361 avania-0.0.6/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 06:21:05.000000 avania-0.0.6/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-11 06:21:05.000000 avania-0.0.6/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:21:05.000000 avania-0.0.6/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 06:21:05.000000 avania-0.0.6/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 06:21:05.000000 avania-0.0.6/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:21:05.125361 avania-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 06:20:49.000000 avania-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.395943 avania-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 04:46:35.000000 avania-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 04:46:45.395943 avania-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 04:46:35.000000 avania-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 04:46:35.000000 avania-0.1.1/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:46:45.395943 avania-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 04:46:35.000000 avania-0.1.1/setup.py
```

### Comparing `avania-0.0.6/LICENSE` & `avania-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.0.6/PKG-INFO` & `avania-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.0.6
+Version: 0.1.1
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: numpy
+Requires-Dist: mysql-connector-python
+Requires-Dist: flask
 
 # Avania Framework
 
 ## Development Team
 
 ### Founder
```

### Comparing `avania-0.0.6/README.md` & `avania-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.0.6/avania.egg-info/PKG-INFO` & `avania-0.1.1/avania.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.0.6
+Version: 0.1.1
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: numpy
+Requires-Dist: mysql-connector-python
+Requires-Dist: flask
 
 # Avania Framework
 
 ## Development Team
 
 ### Founder
```

