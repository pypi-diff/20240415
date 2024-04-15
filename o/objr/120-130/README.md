# Comparing `tmp/objr-120.tar.gz` & `tmp/objr-130.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objr-120.tar", last modified: Fri Apr 12 14:51:32 2024, max compression
+gzip compressed data, was "objr-130.tar", last modified: Mon Apr 15 12:30:39 2024, max compression
```

## Comparing `objr-120.tar` & `objr-130.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.988106 objr-120/
--rw-r--r--   0 bart      (1000) bart      (1000)     3989 2024-04-12 14:51:32.988106 objr-120/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3462 2024-04-12 14:00:10.000000 objr-120/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.984106 objr-120/objr/
--rw-r--r--   0 bart      (1000) bart      (1000)      560 2024-04-12 13:30:26.000000 objr-120/objr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3871 2024-04-12 12:29:51.000000 objr-120/objr/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1888 2024-04-12 12:29:51.000000 objr-120/objr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      941 2024-04-12 12:29:51.000000 objr-120/objr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      762 2024-04-12 12:29:51.000000 objr-120/objr/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1361 2024-04-12 12:29:51.000000 objr-120/objr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-12 12:29:51.000000 objr-120/objr/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-12 12:29:51.000000 objr-120/objr/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-12 12:29:51.000000 objr-120/objr/timer.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.988106 objr-120/objr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3989 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      335 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      907 2024-04-12 14:04:57.000000 objr-120/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 14:51:32.988106 objr-120/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-09 11:10:16.000000 objr-120/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:30:39.670737 objr-130/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1617 2024-04-15 12:30:39.670737 objr-130/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-15 12:26:59.000000 objr-130/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:30:39.670737 objr-130/objr/
+-rw-r--r--   0 bart      (1000) bart      (1000)      852 2024-04-15 12:23:40.000000 objr-130/objr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-15 12:23:40.000000 objr-130/objr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1919 2024-04-15 12:23:40.000000 objr-130/objr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      227 2024-04-15 12:23:40.000000 objr-130/objr/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      941 2024-04-15 12:23:40.000000 objr-130/objr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-15 12:23:40.000000 objr-130/objr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1361 2024-04-15 12:23:40.000000 objr-130/objr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3260 2024-04-15 12:23:40.000000 objr-130/objr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-15 12:23:40.000000 objr-130/objr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-15 12:23:40.000000 objr-130/objr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-15 12:23:40.000000 objr-130/objr/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      728 2024-04-15 12:23:40.000000 objr-130/objr/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:30:39.670737 objr-130/objr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1617 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      383 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-15 12:30:39.000000 objr-130/objr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      906 2024-04-15 12:25:40.000000 objr-130/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-15 12:30:39.670737 objr-130/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-15 12:17:59.000000 objr-130/setup.py
```

### Comparing `objr-120/objr/__init__.py` & `objr-130/objr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,35 +3,50 @@
 # pylint: disable=C,R,W0105
 
 
 "runtime"
 
 
 from .client   import *
+from .command  import *
+from .default  import *
 from .errors   import *
 from .event    import *
 from .handler  import *
+from .persist  import *
 from .repeater import *
 from .thread   import *
 from .timer    import *
+from .workdir  import *
 
 
 def __dir__():
     return (
+        'Client',
+        'Command',
+        'Default',
         'Event',
         'Handler',
-        'Client',
+        'Persist',
         'Repeater',
         'Thread',
         'Timer',
+        'Workdir',
         'cmnd',
         'command',
-        'debug',
-        'parse_cmd',
-        'launch',
+        'fetch',
+        'fntime',
+        'find',
         'laps',
+        'last',
+        'launch',
         'name',
-        'spl'
+        'long',
+        'ident',
+        'parse_cmd',
+        'spl',
+        'sync',
+        'whitelist'
     )
 
 
 __all__ = __dir__()
```

### Comparing `objr-120/objr/client.py` & `objr-130/objr/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 #
 # pylint: disable=C,R,W0105,W0718
 
 
 "client"
 
 
-from objx import Default
-
-
 from .command import Command
+from .default import Default
 from .errors  import later
 from .event   import Event
 from .handler import Handler
 
 
 class Client(Handler):
```

### Comparing `objr-120/objr/command.py` & `objr-130/objr/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 "command"
 
 
 from objx import Object
 
 
+from .default import Default
+
+
 class Command:
 
     "Command"
 
     cmds = Object()
 
     @staticmethod
```

### Comparing `objr-120/objr/errors.py` & `objr-130/objr/errors.py`

 * *Files identical despite different names*

### Comparing `objr-120/objr/event.py` & `objr-130/objr/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 "event"
 
 
 import threading
 
 
-from objx import Default
+from .default import Default
 
 
 class Event(Default):
 
     "Event"
 
     def __init__(self):
```

### Comparing `objr-120/objr/handler.py` & `objr-130/objr/handler.py`

 * *Files identical despite different names*

### Comparing `objr-120/objr/thread.py` & `objr-130/objr/thread.py`

 * *Files identical despite different names*

### Comparing `objr-120/objr/timer.py` & `objr-130/objr/timer.py`

 * *Files identical despite different names*

### Comparing `objr-120/pyproject.toml` & `objr-130/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "objr"
-description = "objects runtime"
-version = "120"
+description = "object runtime"
+version = "130"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 dependencies = [
     'objx',
```

