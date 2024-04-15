# Comparing `tmp/python-timeout-5.5.tar.gz` & `tmp/python-timeout-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-timeout-5.5.tar", last modified: Tue Oct 10 21:51:58 2023, max compression
+gzip compressed data, was "python-timeout-5.6.tar", last modified: Mon Apr 15 12:44:06 2024, max compression
```

## Comparing `python-timeout-5.5.tar` & `python-timeout-5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-10-10 21:51:58.033422 python-timeout-5.5/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.5/.gitignore
--rw-rw-rw-   0        0        0     1148 2023-10-10 21:51:58.033422 python-timeout-5.5/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-07-09 11:48:09.000000 python-timeout-5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-10-10 21:51:58.029432 python-timeout-5.5/python_timeout.egg-info/
--rw-rw-rw-   0        0        0     1148 2023-10-10 21:51:57.000000 python-timeout-5.5/python_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-10-10 21:51:57.000000 python-timeout-5.5/python_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-10 21:51:57.000000 python-timeout-5.5/python_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-10-10 21:51:57.000000 python-timeout-5.5/python_timeout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-10 21:51:57.000000 python-timeout-5.5/python_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-10-10 21:51:58.033422 python-timeout-5.5/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-10-10 21:51:54.000000 python-timeout-5.5/setup.py
--rw-rw-rw-   0        0        0      574 2023-06-16 10:18:33.000000 python-timeout-5.5/test.py
-drwxrwxrwx   0        0        0        0 2023-10-10 21:51:58.030429 python-timeout-5.5/timeout/
--rw-rw-rw-   0        0        0     9668 2023-10-10 21:51:37.000000 python-timeout-5.5/timeout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-10 21:51:58.031428 python-timeout-5.5/timeout/__pycache__/
--rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.5/timeout/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-04-15 12:44:06.758130 python-timeout-5.6/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.6/.gitignore
+-rw-rw-rw-   0        0        0     1210 2024-04-15 12:44:06.757133 python-timeout-5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2023-07-09 11:48:09.000000 python-timeout-5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 12:44:06.756135 python-timeout-5.6/python_timeout.egg-info/
+-rw-rw-rw-   0        0        0     1210 2024-04-15 12:44:06.000000 python-timeout-5.6/python_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-15 12:44:06.000000 python-timeout-5.6/python_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:44:06.000000 python-timeout-5.6/python_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-15 12:44:06.000000 python-timeout-5.6/python_timeout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 12:44:06.000000 python-timeout-5.6/python_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-15 12:44:06.759127 python-timeout-5.6/setup.cfg
+-rw-rw-rw-   0        0        0      413 2024-04-15 12:38:33.000000 python-timeout-5.6/setup.py
+-rw-rw-rw-   0        0        0      574 2023-06-16 10:18:33.000000 python-timeout-5.6/test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:44:06.751149 python-timeout-5.6/timeout/
+-rw-rw-rw-   0        0        0     9864 2024-04-15 12:38:27.000000 python-timeout-5.6/timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:44:06.755138 python-timeout-5.6/timeout/__pycache__/
+-rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.6/timeout/__pycache__/__init__.cpython-39.pyc
```

### Comparing `python-timeout-5.5/PKG-INFO` & `python-timeout-5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.5
+Version: 5.6
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
+Requires-Dist: python-dateutil
+Requires-Dist: python-printr
 
 ### Timeout
 Random timeout between minimum and maximum values
 
 Installation:
 `pip install python-timeout`
```

### Comparing `python-timeout-5.5/README.md` & `python-timeout-5.6/README.md`

 * *Files identical despite different names*

### Comparing `python-timeout-5.5/python_timeout.egg-info/PKG-INFO` & `python-timeout-5.6/python_timeout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.5
+Version: 5.6
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
+Requires-Dist: python-dateutil
+Requires-Dist: python-printr
 
 ### Timeout
 Random timeout between minimum and maximum values
 
 Installation:
 `pip install python-timeout`
```

### Comparing `python-timeout-5.5/test.py` & `python-timeout-5.6/test.py`

 * *Files identical despite different names*

### Comparing `python-timeout-5.5/timeout/__init__.py` & `python-timeout-5.6/timeout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from time import sleep
 from random import random, uniform, randrange
 from datetime import datetime, timedelta, time
 from dateutil.parser import parse
 from printr import print
 
 class sleep_timer:
-    def __init__(self, hour_to_start_at, hour_to_stop_at, sleeping_message='Sleeping'):
-        if type(hour_to_start_at) == int:
+    def __init__(self, hour_to_start_at=True, hour_to_stop_at=None, sleeping_message='Sleeping'):
+        if type(hour_to_start_at) != str:
             self.hour_to_start_at = hour_to_start_at
             self.hour_to_stop_at = hour_to_stop_at
         else:
             self.hour_to_start_at = parse(hour_to_start_at).hour
             self.hour_to_stop_at = parse(hour_to_stop_at).hour
 
         self.sleeping_message = sleeping_message
@@ -33,15 +33,19 @@
         return False
     
     def during_active_time(self):
         now = datetime.now()
         current_hour = now.hour
         current_minute = now.minute
 
-        if self.current_hour_within_active_hours(current_hour):
+        if self.hour_to_start_at == True: # Permanently active
+            return True
+        elif self.hour_to_start_at == False: # Permanently inactive
+            return False
+        elif self.current_hour_within_active_hours(current_hour):
             self.is_active = True
             if self.random_minute_to_start_at != 0:
                 self.random_minute_to_start_at = 0
 
             # Check after start time with randomised minute to start at
         elif current_hour == self.hour_to_start_at and current_minute >= self.random_minute_to_start_at:
             self.is_active = True
```

### Comparing `python-timeout-5.5/timeout/__pycache__/__init__.cpython-39.pyc` & `python-timeout-5.6/timeout/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

