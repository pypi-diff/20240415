# Comparing `tmp/pisces-0.4.3.tar.gz` & `tmp/pisces-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisces-0.4.3.tar", last modified: Tue Feb 27 18:30:02 2024, max compression
+gzip compressed data, was "pisces-0.4.4.tar", last modified: Mon Apr 15 19:36:41 2024, max compression
```

## Comparing `pisces-0.4.3.tar` & `pisces-0.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.988975 pisces-0.4.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-02-27 18:29:50.000000 pisces-0.4.3/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-02-27 18:29:50.000000 pisces-0.4.3/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-02-27 18:29:50.000000 pisces-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-27 18:30:02.988975 pisces-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-27 18:29:50.000000 pisces-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.980975 pisces-0.4.3/pisces/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1055 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5004 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.984975 pisces-0.4.3/pisces/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/db2db.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/drop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7742 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/mseed2db.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6052 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/sac2db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/commands/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.984975 pisces-0.4.3/pisces/io/
--rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2062 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/mseed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/readwaveform.py
--rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/response.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28825 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/sac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/trace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/io/util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29502 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.988975 pisces-0.4.3/pisces/schema/
--rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/schema/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28343 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/schema/antelope.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30373 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/schema/css3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35759 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/schema/kbcore.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15671 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/schema/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.988975 pisces-0.4.3/pisces/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/tables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/tables/antelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/tables/css3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/tables/kbcore.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32016 2024-02-27 18:29:50.000000 pisces-0.4.3/pisces/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.988975 pisces-0.4.3/pisces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-27 18:30:02.000000 pisces-0.4.3/pisces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 18:30:02.988975 pisces-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1860 2024-02-27 18:29:50.000000 pisces-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:30:02.988975 pisces-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-02-27 18:29:50.000000 pisces-0.4.3/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-27 18:29:50.000000 pisces-0.4.3/tests/test_readwaveform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5330 2024-02-27 18:29:50.000000 pisces-0.4.3/tests/test_schema_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-02-27 18:29:50.000000 pisces-0.4.3/tests/test_stations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-02-27 18:29:50.000000 pisces-0.4.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.040062 pisces-0.4.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-04-15 19:36:31.000000 pisces-0.4.4/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-04-15 19:36:31.000000 pisces-0.4.4/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-04-15 19:36:31.000000 pisces-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-15 19:36:41.040062 pisces-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-15 19:36:31.000000 pisces-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.032062 pisces-0.4.4/pisces/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1055 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5004 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.036062 pisces-0.4.4/pisces/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/db2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/drop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7742 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/mseed2db.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6052 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/sac2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/commands/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.036062 pisces-0.4.4/pisces/io/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2062 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/mseed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/readwaveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/response.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28826 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/sac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/io/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29504 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.036062 pisces-0.4.4/pisces/schema/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/schema/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28343 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/schema/antelope.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30373 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/schema/css3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35759 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/schema/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15671 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/schema/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.036062 pisces-0.4.4/pisces/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/tables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/tables/antelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/tables/css3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/tables/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32016 2024-04-15 19:36:31.000000 pisces-0.4.4/pisces/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.040062 pisces-0.4.4/pisces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:36:41.000000 pisces-0.4.4/pisces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:36:41.040062 pisces-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1860 2024-04-15 19:36:31.000000 pisces-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:36:41.040062 pisces-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-04-15 19:36:31.000000 pisces-0.4.4/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-15 19:36:31.000000 pisces-0.4.4/tests/test_readwaveform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5330 2024-04-15 19:36:31.000000 pisces-0.4.4/tests/test_schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-15 19:36:31.000000 pisces-0.4.4/tests/test_stations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-15 19:36:31.000000 pisces-0.4.4/tests/test_util.py
```

### Comparing `pisces-0.4.3/LICENSE.txt` & `pisces-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/MANIFEST.in` & `pisces-0.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/PKG-INFO` & `pisces-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
 Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.4.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
 Keywords: seismology,geophysics,database
```

### Comparing `pisces-0.4.3/README.md` & `pisces-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/__init__.py` & `pisces-0.4.4/pisces/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 The ultimate goal of Pisces is to allow the user to write code that will not 
 eventually have to be abandoned due to different project scales, system 
 architectures, or licensing concerns.  
 
 """
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 from pisces.util import db_connect, get_tables, travel_times, make_table
 from pisces.schema.util import string_formatter
 from pisces.io.trace import wfdisc2trace
 from pisces.schema import kbcore
 from pisces.io.readwaveform import read_waveform
 from pisces import request
```

### Comparing `pisces-0.4.3/pisces/client.py` & `pisces-0.4.4/pisces/client.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/commands/main.py` & `pisces-0.4.4/pisces/commands/main.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/commands/mseed2db.py` & `pisces-0.4.4/pisces/commands/mseed2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/commands/sac2db.py` & `pisces-0.4.4/pisces/commands/sac2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/commands/util.py` & `pisces-0.4.4/pisces/commands/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/crud.py` & `pisces-0.4.4/pisces/crud.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/events.py` & `pisces-0.4.4/pisces/events.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/io/mseed.py` & `pisces-0.4.4/pisces/io/mseed.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/io/readwaveform.py` & `pisces-0.4.4/pisces/io/readwaveform.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/io/response.py` & `pisces-0.4.4/pisces/io/response.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/io/sac.py` & `pisces-0.4.4/pisces/io/sac.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         assocdict[col] = val if val != SACDEFAULT[hdr] else None
 
     # overwrite if any are None
     if not assocdict:
         try:
             delta = geod.locations2degrees(header['stla'], header['stlo'],
                                            header['evla'], header['evlo'])
-            m, seaz, esaz = geod.gps2DistAzimuth(header['stla'], header['stlo'],
+            m, seaz, esaz = geod.gps2dist_azimuth(header['stla'], header['stlo'],
                                                  header['evla'], header['evlo'])
             assocdict['esaz'] = esaz
             assocdict['seaz'] = seaz
             assocdict['delta'] = delta
         except (ValueError, TypeError):
             # some sac header values are None
             pass
```

### Comparing `pisces-0.4.3/pisces/io/trace.py` & `pisces-0.4.4/pisces/io/trace.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/io/util.py` & `pisces-0.4.4/pisces/io/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/request.py` & `pisces-0.4.4/pisces/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         if deg[3] is not None:
             mask0 = np.logical_and(mask0, deg[3] >= degrees)
 
         #mask0 = np.logical_and(mask0, mask)
 
     if km:
         #???: this may be backwards
-        mgen = (geod.gps2DistAzimuth(irec.lat, irec.lon, km[0], km[1])[0] \
+        mgen = (geod.gps2dist_azimuth(irec.lat, irec.lon, km[0], km[1])[0] \
                   for irec in records)
         kilometers = np.fromiter(mgen, dtype=float)/1e3
         #meters, azs, bazs = zip(*valgen)
         #kilometers = np.array(meters)/1e3
         if km[2] is not None:
             mask0 = np.logical_and(mask0, km[2] <= kilometers)
         if km[3] is not None:
@@ -129,15 +129,15 @@
 
         #mask0 = np.logical_and(mask0, mask)
 
     if swath is not None:
         minaz = swath[2] - swath[3]
         maxaz = swath[2] + swath[3]
         #???: this may be backwards
-        azgen = (geod.gps2DistAzimuth(irec.lat, irec.lon, km[0], km[1])[1] \
+        azgen = (geod.gps2dist_azimuth(irec.lat, irec.lon, km[0], km[1])[1] \
                  for irec in records)
         azimuths = np.fromiter(azgen, dtype=float)
         mask0 = np.logical_and(mask0, azimuths >= minaz)
         mask0 = np.logical_and(mask0, azimuths <= maxaz)
 
     #idx = np.nonzero(np.atleast_1d(mask0))[0] ???
     idx = np.nonzero(mask0)[0]
```

### Comparing `pisces-0.4.3/pisces/schema/antelope.py` & `pisces-0.4.4/pisces/schema/antelope.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/schema/css3.py` & `pisces-0.4.4/pisces/schema/css3.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/schema/kbcore.py` & `pisces-0.4.4/pisces/schema/kbcore.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/schema/util.py` & `pisces-0.4.4/pisces/schema/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/stations.py` & `pisces-0.4.4/pisces/stations.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/tables/antelope.py` & `pisces-0.4.4/pisces/tables/antelope.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/tables/css3.py` & `pisces-0.4.4/pisces/tables/css3.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/tables/kbcore.py` & `pisces-0.4.4/pisces/tables/kbcore.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces/util.py` & `pisces-0.4.4/pisces/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/pisces.egg-info/PKG-INFO` & `pisces-0.4.4/pisces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
 Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.4.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
 Keywords: seismology,geophysics,database
```

### Comparing `pisces-0.4.3/pisces.egg-info/SOURCES.txt` & `pisces-0.4.4/pisces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/setup.py` & `pisces-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open('README.md') as readme:
     # https://dustingram.com/articles/2018/03/16/markdown-descriptions-on-pypi
     long_description = readme.read()
 
 doclines = __doc__.split("\n")
 
 setup(name='pisces',
-      version='0.4.3',
+      version='0.4.4',
       description='A Practical Seismological Database Library in Python.',
       long_description=long_description,
       long_description_content_type="text/markdown", # setuptools >= 38.6.0
       author='Jonathan MacCarthy',
       author_email='jkmacc@lanl.gov',
       packages=['pisces','pisces.schema','pisces.io','pisces.tables',
                 'pisces.commands'],
```

### Comparing `pisces-0.4.3/tests/test_events.py` & `pisces-0.4.4/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/tests/test_readwaveform.py` & `pisces-0.4.4/tests/test_readwaveform.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/tests/test_schema_util.py` & `pisces-0.4.4/tests/test_schema_util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/tests/test_stations.py` & `pisces-0.4.4/tests/test_stations.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.3/tests/test_util.py` & `pisces-0.4.4/tests/test_util.py`

 * *Files identical despite different names*

