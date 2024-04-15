# Comparing `tmp/hypickle-1.1.3.tar.gz` & `tmp/hypickle-1.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypickle-1.1.3.tar", last modified: Mon Apr 15 00:37:53 2024, max compression
+gzip compressed data, was "hypickle-1.1.33.tar", last modified: Mon Apr 15 01:15:17 2024, max compression
```

## Comparing `hypickle-1.1.3.tar` & `hypickle-1.1.33.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.063571 hypickle-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 00:37:45.000000 hypickle-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 00:37:53.059571 hypickle-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 00:37:45.000000 hypickle-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.059571 hypickle-1.1.3/hypickle/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Colours.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Graphing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/MyClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Player.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/ProcessingResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/additional_friends.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/bedwars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/hypixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/leveling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.059571 hypickle-1.1.3/hypickle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-15 00:37:45.000000 hypickle-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:37:53.063571 hypickle-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:15:17.649110 hypickle-1.1.33/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 01:15:13.000000 hypickle-1.1.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-15 01:15:17.649110 hypickle-1.1.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 01:15:13.000000 hypickle-1.1.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:15:17.649110 hypickle-1.1.33/hypickle/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Graphing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/MyClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/ProcessingResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/additional_friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/bedwars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/hypixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/leveling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-15 01:15:13.000000 hypickle-1.1.33/hypickle/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:15:17.649110 hypickle-1.1.33/hypickle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 01:15:17.000000 hypickle-1.1.33/hypickle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 01:15:13.000000 hypickle-1.1.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:15:17.649110 hypickle-1.1.33/setup.cfg
```

### Comparing `hypickle-1.1.3/LICENSE` & `hypickle-1.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/PKG-INFO` & `hypickle-1.1.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.3
+Version: 1.1.33
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `hypickle-1.1.3/README.md` & `hypickle-1.1.33/README.md`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Args.py` & `hypickle-1.1.33/hypickle/Args.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Colours.py` & `hypickle-1.1.33/hypickle/Colours.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Files.py` & `hypickle-1.1.33/hypickle/Files.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Graphing.py` & `hypickle-1.1.33/hypickle/Graphing.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/MyClasses.py` & `hypickle-1.1.33/hypickle/MyClasses.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Pit.py` & `hypickle-1.1.33/hypickle/Pit.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Player.py` & `hypickle-1.1.33/hypickle/Player.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/ProcessingResults.py` & `hypickle-1.1.33/hypickle/ProcessingResults.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Rank.py` & `hypickle-1.1.33/hypickle/Rank.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/Utils.py` & `hypickle-1.1.33/hypickle/Utils.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/additional_friends.py` & `hypickle-1.1.33/hypickle/additional_friends.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/bedwars.py` & `hypickle-1.1.33/hypickle/bedwars.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/hypixel.py` & `hypickle-1.1.33/hypickle/hypixel.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/leveling.py` & `hypickle-1.1.33/hypickle/leveling.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/hypickle/main.py` & `hypickle-1.1.33/hypickle/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 from itertools import permutations
 from copy import deepcopy
 
 from . import hypixel
 from . import MyClasses
 from .MyClasses import Specs, UUID_Plus_Time, args
 from . import Files
@@ -213,18 +213,19 @@
             print(f"Keyword matches for '{substr}':\n" + '\n'.join(keyword_matches))
             ign_matches = sorted([ign for ign in ProcessingResults.ign_uuid_pairs_in_results()
                                   if substr in ign.lower()])
             print(f"\nPlayer name matches for '{substr}':\n" + '\n'.join(ign_matches) + '\n')
     else:
         assert False
 
-def main(argv: List[str]) -> None:
-    """When called as a script, `argv` is passed `sys.argv` from the if statement at the end of this file.
-       If called as a module (e.g., as a dev from the parent dir), argv is whatever the caller passes."""
-    MyClasses.set_args(argv)
+def main(argv: Optional[List[str]] = None) -> None:
+    """When called as a script, `argv` is left as None and `sys.argv` is used.
+       If calling main() programatically from another python file though, pass the args
+       you want via `argv`."""
+    MyClasses.set_args(argv if argv is not None else sys.argv)
 
     if args().do_mini_program():
         do_mini_program()
         sys.exit(0)
 
     newest_n_friends, oldest_n_friends = None, None
     if args().get_newest_friends():
@@ -257,8 +258,8 @@
     if args().do_file_output():
         filename = ("Friends of " +
                     ("friends of " if args().find_friends_of_friends() else "") +
                     player.name_for_file_output())
         Files.write_data_as_json_to_file(report, filename)
 
 if __name__ == '__main__':
-    main(sys.argv)
+    main()
```

### Comparing `hypickle-1.1.3/hypickle.egg-info/PKG-INFO` & `hypickle-1.1.33/hypickle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.3
+Version: 1.1.33
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `hypickle-1.1.3/hypickle.egg-info/SOURCES.txt` & `hypickle-1.1.33/hypickle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.3/pyproject.toml` & `hypickle-1.1.33/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">= 3.0"
 name = "hypickle"
-version = "1.1.3"
+version = "1.1.33"
 authors = [
   { name="John Doknjas", email="jdoknjas@sfu.ca" },
 ]
 description = "A script that outputs realtime stats for custom lists of friends you create."
 keywords = ["hypickle", "hypixel", "pit", "bedwars", "friends", "stats", "api"]
 dependencies = [
   "requests",
```

