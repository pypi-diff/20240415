# Comparing `tmp/krypper_tgstat-0.1.6.tar.gz` & `tmp/krypper_tgstat-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krypper_tgstat-0.1.6.tar", last modified: Sun Apr 14 20:56:04 2024, max compression
+gzip compressed data, was "krypper_tgstat-0.1.6.1.tar", last modified: Sun Apr 14 21:00:38 2024, max compression
```

## Comparing `krypper_tgstat-0.1.6.tar` & `krypper_tgstat-0.1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-13 08:38:04.000000 krypper_tgstat-0.1.6/LICENSE
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      908 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-13 08:55:13.000000 krypper_tgstat-0.1.6/README.md
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.028566 krypper_tgstat-0.1.6/krypper_tgstat/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      238 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.6/krypper_tgstat/__init__.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     9194 2024-04-14 20:50:02.000000 krypper_tgstat-0.1.6/krypper_tgstat/classes.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.6/krypper_tgstat/enums.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      661 2024-04-14 19:01:40.000000 krypper_tgstat-0.1.6/krypper_tgstat/exceptions.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     7611 2024-04-14 20:50:23.000000 krypper_tgstat-0.1.6/krypper_tgstat/tg_stat.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.028566 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      908 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/SOURCES.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/dependency_links.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/requires.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/top_level.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/setup.cfg
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1287 2024-04-14 20:55:52.000000 krypper_tgstat-0.1.6/setup.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/tests/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    36813 2024-04-14 20:46:26.000000 krypper_tgstat-0.1.6/tests/test_TGStatSync.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 21:00:38.016609 krypper_tgstat-0.1.6.1/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-13 08:38:04.000000 krypper_tgstat-0.1.6.1/LICENSE
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      910 2024-04-14 21:00:38.016609 krypper_tgstat-0.1.6.1/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-13 08:55:13.000000 krypper_tgstat-0.1.6.1/README.md
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 21:00:38.015609 krypper_tgstat-0.1.6.1/krypper_tgstat/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      244 2024-04-14 21:00:01.000000 krypper_tgstat-0.1.6.1/krypper_tgstat/__init__.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     9194 2024-04-14 20:50:02.000000 krypper_tgstat-0.1.6.1/krypper_tgstat/classes.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.6.1/krypper_tgstat/enums.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      661 2024-04-14 19:01:40.000000 krypper_tgstat-0.1.6.1/krypper_tgstat/exceptions.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     7611 2024-04-14 20:50:23.000000 krypper_tgstat-0.1.6.1/krypper_tgstat/tg_stat.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 21:00:38.016609 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      910 2024-04-14 21:00:37.000000 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-14 21:00:37.000000 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/SOURCES.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-14 21:00:37.000000 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/dependency_links.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-14 21:00:37.000000 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/requires.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-14 21:00:37.000000 krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/top_level.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-14 21:00:38.017609 krypper_tgstat-0.1.6.1/setup.cfg
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1289 2024-04-14 21:00:08.000000 krypper_tgstat-0.1.6.1/setup.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 21:00:38.016609 krypper_tgstat-0.1.6.1/tests/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    36810 2024-04-14 20:59:49.000000 krypper_tgstat-0.1.6.1/tests/test_TGStatSync.py
```

### Comparing `krypper_tgstat-0.1.6/LICENSE` & `krypper_tgstat-0.1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.6/PKG-INFO` & `krypper_tgstat-0.1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.6/krypper_tgstat/classes.py` & `krypper_tgstat-0.1.6.1/krypper_tgstat/classes.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.6/krypper_tgstat/enums.py` & `krypper_tgstat-0.1.6.1/krypper_tgstat/enums.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.6/krypper_tgstat/exceptions.py` & `krypper_tgstat-0.1.6.1/krypper_tgstat/exceptions.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.6/krypper_tgstat/tg_stat.py` & `krypper_tgstat-0.1.6.1/krypper_tgstat/tg_stat.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.6/krypper_tgstat.egg-info/PKG-INFO` & `krypper_tgstat-0.1.6.1/krypper_tgstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper-tgstat
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.6/setup.py` & `krypper_tgstat-0.1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 :authors: Evgeny Momotov (KrymmyEM)
 :license: MIT License
 Copyright: (c) 2024 Evgeny
 """
 
-version = "0.1.6"
+version = "0.1.6.1"
 
 long_description = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
```

### Comparing `krypper_tgstat-0.1.6/tests/test_TGStatSync.py` & `krypper_tgstat-0.1.6.1/tests/test_TGStatSync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import environ
 import unittest
 
 from dotenv import load_dotenv
-from PyrapperTGStatAPI import classes, enums, exceptions, tg_stat
+from krypper_tgstat import classes, enums, exceptions, tg_stat
 
 load_dotenv()
 
 class TGStatSyncTest(unittest.TestCase):
 
     def test_token_exeptions(self):
         self.assertRaises(exceptions.TGStatAuthError, tg_stat.TGStatSync, "")
```

