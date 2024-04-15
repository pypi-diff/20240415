# Comparing `tmp/hypickle-1.1.2.tar.gz` & `tmp/hypickle-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypickle-1.1.2.tar", last modified: Tue Mar 26 04:00:25 2024, max compression
+gzip compressed data, was "hypickle-1.1.3.tar", last modified: Mon Apr 15 00:37:53 2024, max compression
```

## Comparing `hypickle-1.1.2.tar` & `hypickle-1.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:00:25.354308 hypickle-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-26 04:00:21.000000 hypickle-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 04:00:25.354308 hypickle-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-26 04:00:21.000000 hypickle-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:00:25.350308 hypickle-1.1.2/hypickle/
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Colours.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Graphing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/MyClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    20897 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Player.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/ProcessingResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/additional_friends.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/bedwars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/hypixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/leveling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-03-26 04:00:21.000000 hypickle-1.1.2/hypickle/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:00:25.354308 hypickle-1.1.2/hypickle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 04:00:25.000000 hypickle-1.1.2/hypickle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-26 04:00:21.000000 hypickle-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 04:00:25.354308 hypickle-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.063571 hypickle-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 00:37:45.000000 hypickle-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 00:37:53.059571 hypickle-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 00:37:45.000000 hypickle-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.059571 hypickle-1.1.3/hypickle/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Graphing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/MyClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/ProcessingResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/additional_friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/bedwars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/hypixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/leveling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-15 00:37:45.000000 hypickle-1.1.3/hypickle/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:37:53.059571 hypickle-1.1.3/hypickle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 00:37:53.000000 hypickle-1.1.3/hypickle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-15 00:37:45.000000 hypickle-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:37:53.063571 hypickle-1.1.3/setup.cfg
```

### Comparing `hypickle-1.1.2/LICENSE` & `hypickle-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/PKG-INFO` & `hypickle-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.2
+Version: 1.1.3
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,15 +40,15 @@
 with the `hypickle` script (explained below).
 
 ### Main features:
 
 - Basic usage is to run with `hypickle *username/uuid*`
   - This will output stats for the specified player, and then output any friends for them.
   - Since the `friends` endpoint of hypixel's API was deprecated, you must manually add any friends for them you want.
-    To do this, run `hypickle addadditionalfriends *username/uuid*`
+    To do this, run `hypickle addfriends *username/uuid*`
 - If there's a player you run the program on often, consider making an alias for their uuid:
   - Run `hypickle updateuuidaliases *username*`
   - Then when running `hypickle *username*`, the program will automatically substitute the username for the uuid.
     This is useful when running the program in quick succession for the same player, since the hypixel api forces a cooldown
     when sending in a username instead of a uuid.
 - You can also add an optional argument called 'all', if you'd like to output all friends (not just those currently online).
   - E.g., `hypickle *username/uuid* all`
@@ -56,15 +56,15 @@
 ### Developer commands:
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
-  - `pydeps main.py` will output a dependency graph of the project's modules.
+  - `pydeps hypickle` will output a dependency graph of the project's modules.
   - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
   - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.2/README.md` & `hypickle-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 with the `hypickle` script (explained below).
 
 ### Main features:
 
 - Basic usage is to run with `hypickle *username/uuid*`
   - This will output stats for the specified player, and then output any friends for them.
   - Since the `friends` endpoint of hypixel's API was deprecated, you must manually add any friends for them you want.
-    To do this, run `hypickle addadditionalfriends *username/uuid*`
+    To do this, run `hypickle addfriends *username/uuid*`
 - If there's a player you run the program on often, consider making an alias for their uuid:
   - Run `hypickle updateuuidaliases *username*`
   - Then when running `hypickle *username*`, the program will automatically substitute the username for the uuid.
     This is useful when running the program in quick succession for the same player, since the hypixel api forces a cooldown
     when sending in a username instead of a uuid.
 - You can also add an optional argument called 'all', if you'd like to output all friends (not just those currently online).
   - E.g., `hypickle *username/uuid* all`
@@ -37,15 +37,15 @@
 ### Developer commands:
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
-  - `pydeps main.py` will output a dependency graph of the project's modules.
+  - `pydeps hypickle` will output a dependency graph of the project's modules.
   - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
   - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.2/hypickle/Args.py` & `hypickle-1.1.3/hypickle/Args.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         assert re.split(r'/|\\', args[0])[-1] in ('main.py', 'hypickle')
         args = [arg if arg.endswith('.txt') else arg.lower() for arg in args[1:]]
         self._ARGS = Files.apply_aliases(args)
         self._ARG_KEYWORDS = ('all', 'friendsoffriends', 'justuuids', 'checkresults',
                               'diff', 'starsort', 'pitsort',
                               'fileoutput', 'updateuuids', 'matchingignsuuids',
                               'includemultiplayerfiles', 'keepfirstdictmultifiles',
-                              'addadditionalfriends', 'addadditionals',
+                              'addadditionalfriends', 'addadditionals', 'addfriends',
                               'noadditionalfriends', 'noadditionals',
                               'addaliases', 'updatealiases', 'adduuidaliases', 'updateuuidaliases',
                               'showaliases', 'printaliases',
                               'getplayerjson', 'playerjson', 'noverify', 'dontverify', 'nover',
                               'pitpercent', 'pit%', 'pitplot', 'nwplot', 'bwplot', 'contains',
                               'trackargs', 'argsonline', 'newest', 'oldest',
                               'debugapi', 'showjsondiff', 'showjsonupdates')
@@ -76,15 +76,15 @@
 
     def skip_first_dict_in_multi_player_files(self) -> bool:
         assert self.include_multi_player_files()
         # Only makes sense to call this function if the above is true.
         return 'keepfirstdictmultifiles' not in self._ARGS
 
     def add_additional_friends(self) -> bool:
-        return any(x in self._ARGS for x in ('addadditionalfriends', 'addadditionals'))
+        return any(x in self._ARGS for x in ('addadditionalfriends', 'addadditionals', 'addfriends'))
 
     def get_additional_friends(self) -> bool:
         return all(x not in self._ARGS for x in ('noadditionalfriends', 'noadditionals'))
 
     def update_aliases(self) -> bool:
         return 'addaliases' in self._ARGS or 'updatealiases' in self._ARGS
 
@@ -143,15 +143,16 @@
         assert all(arg.endswith('.txt') or arg.lower() == arg
                    for arg in self.get_args(False))
         assert set(self.get_keywords()).isdisjoint(Files.get_aliases().keys())
         if self.do_file_output():
             assert self.date_cutoff() is None and not self.just_online_friends()
             assert not self.get_newest_friends() and not self.get_oldest_friends()
         assert not (self.sort_by_pit_rank() and self.sort_by_star())
-        if any((self.update_aliases(), self.print_aliases(), self.pit_plot(), self.network_plot(), self.bedwars_plot())):
+        if any((self.update_aliases(), self.print_aliases(), self.pit_plot(), self.network_plot(),
+                self.bedwars_plot())):
             assert len(self.get_args(False)) == 1 and not self.get_args(True)
         if self.add_additional_friends():
             assert len(self.get_args(True)) == 1 and len(self.get_args(False)) == 2
         if self.get_player_json() or self.pit_percent() or self.add_uuid_aliases():
             assert len(self.get_args(True)) >= 1
         if self.contains_substr() or self.add_uuid_aliases():
             assert len(self.get_args(False)) >= 2
```

### Comparing `hypickle-1.1.2/hypickle/Colours.py` & `hypickle-1.1.3/hypickle/Colours.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/hypickle/Files.py` & `hypickle-1.1.3/hypickle/Files.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,28 +77,34 @@
 def assertions_for_aliases(alias: str, meaning: str, keywords: Iterable[str]) -> None:
     assert alias not in keywords and not Utils.contains_whitespace(alias)
     assert '.txt' not in meaning and '.txt' not in alias
 
 def get_new_aliases_from_user(aliases: Dict[str, str], keywords: Iterable[str]) -> None:
     """Asks the user for new aliases, and updates the `aliases` parameter accordingly."""
     while True:
-        curr_alias = input("Enter alias (or 'done'/'stop' to quit): ").lower()
-        if curr_alias in ('done', 'stop', 'quit'):
+        alias = input("Enter alias (or 'done'/'stop' to quit): ").lower()
+        if alias in ('done', 'stop', 'quit'):
             return
-        curr_meaning = input("Enter the text this alias stands for: ").lower()
-        assertions_for_aliases(curr_alias, curr_meaning, keywords)
-        if curr_meaning in ('del', 'delete', 'remove'):
-            if input(f"Confirm you want to delete the {curr_alias} alias by entering y: ") in ('y', 'Y'):
-                del aliases[curr_alias]
+        meaning = input("Enter the text this alias stands for: ").lower()
+        if meaning in ('del', 'delete', 'remove'):
+            if input(f"Confirm you want to delete the {alias} alias by entering y: ") in ('y', 'Y'):
+                del aliases[alias]
             continue
-        if curr_alias in aliases:
-            print(f"'{curr_alias}' is already an alias that stands for '{aliases[curr_alias]}'. ", end='')
-            if input(f"To confirm replacing its meaning to be '{curr_meaning}', enter y: ") not in ('y', 'Y'):
+        elif meaning == 'append':
+            new_words = input(f"Enter the new word(s) to append to this alias' meaning: ").lower().split()
+            meaning = ' '.join(aliases[alias].split() + new_words)
+        elif meaning in ('shorten', 'trim'):
+            remove_words = input(f"Enter the word(s) to remove from this alias' meaning: ").lower().split()
+            meaning = ' '.join(x for x in aliases[alias].split() if x not in remove_words)
+        if alias in aliases:
+            print(f"'{alias}' is already an alias that stands for '{aliases[alias]}'. ", end='')
+            if input(f"To confirm replacing its meaning to be '{meaning}', enter y: ") not in ('y', 'Y'):
                 continue
-        aliases[curr_alias] = curr_meaning
+        assertions_for_aliases(alias, meaning, keywords)
+        aliases[alias] = meaning
         print()
 
 def add_new_ign_uuid_aliases(
         aliases: Dict[str, str], ign_uuid_pairs: Iterable[Tuple[str, str]], keywords: Iterable[str]
     ) -> None:
     """Makes each ign an alias for its uuid, and adds it to `aliases` (if the ign is not
        already an existing alias)."""
```

### Comparing `hypickle-1.1.2/hypickle/Graphing.py` & `hypickle-1.1.3/hypickle/Graphing.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/hypickle/MyClasses.py` & `hypickle-1.1.3/hypickle/MyClasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-"""This file should only depend on Utils.py."""
-
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Optional, Union
+from typing import Optional, Union, List
+import urllib3
 
 from . import Utils
-from . import Args
+from .Args import Args
+
+_args: Optional[Args] = None
+
+def set_args(args: List[str]) -> None:
+    global _args
+    assert not _args
+    _args = Args(args)
+    if not _args.verify_requests():
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+def args() -> Args:
+    assert _args
+    return _args
 
 class UUID_Plus_Time:
     """This class encapsulates a UUID and a time (unix epoch), likely representing when
     the player was friended to the parent player."""
 
     def __init__(self, uuid: str, time_val: Union[str, float, int, None]):
         """time_val must be either a date string, or the unix epoch time in either seconds or milliseconds"""
@@ -66,18 +78,18 @@
 
     @classmethod
     def _get_value_for_key(cls, key: str) -> bool:
         assert cls._common_specs[key] is not None and cls._common_specs['set flag']
         return cls._common_specs[key]
 
     @classmethod
-    def make_specs_object_and_initialize_common_specs(cls, args: Args.Args) -> Specs:
-        Specs.set_common_specs(not args.find_friends_of_friends())
-        friendsfriendsSpecs = Specs(True, False, None, 2) if args.find_friends_of_friends() else None
-        friendsSpecs = Specs(args.just_uuids(), args.just_online_friends(), friendsfriendsSpecs, 1)
+    def make_specs_object_and_initialize_common_specs(cls) -> Specs:
+        Specs.set_common_specs(not args().find_friends_of_friends())
+        friendsfriendsSpecs = Specs(True, False, None, 2) if args().find_friends_of_friends() else None
+        friendsSpecs = Specs(args().just_uuids(), args().just_online_friends(), friendsfriendsSpecs, 1)
         playerSpecs = Specs(False, False, friendsSpecs, 0)
         return playerSpecs
 
     def __init__(self, just_uuids: bool, player_must_be_online: bool,
                  friends_specs: Optional[Specs], degrees_from_original_player: int):
         assert Specs._common_specs['set flag']
         self._just_uuids = just_uuids
```

### Comparing `hypickle-1.1.2/hypickle/Pit.py` & `hypickle-1.1.3/hypickle/Pit.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 # Got a lot of guidance from brooke-gill's pit repo.
 
 LVL_GROUP_MULTIPLIER = (15, 30, 50, 75, 125, 300, 600, 800, 900, 1000, 1200, 1500, 0)
 PRESTIGE_MULTIPLIER = (100, 110, 120, 130, 140, 150, 175, 200, 250, 300, 400, 500, 600, 700, 800, 900, 1000,
              1200, 1400, 1600, 1800, 2000, 2400, 2800, 3200, 3600, 4000, 4500, 5000, 7500, 10000, 10100,
              10100, 10100, 10100, 10100, 20000, 30000, 40000, 50000, 75000, 100000, 125000, 150000,
-             175000, 200000, 300000, 500000, 1000000, 5000000, 10000000)
+             175000, 200000, 300000, 500000, 1_000_000, 5_000_000, 10_000_000)
 PRESTIGE_XP = (65950, 138510, 217680, 303430, 395760, 494700, 610140, 742040, 906930, 1104780, 1368580,
                1698330, 2094030, 2555680, 3083280, 3676830, 4336330, 5127730, 6051030, 7106230, 8293330,
                9612330, 11195130, 13041730, 15152130, 17526330, 20164330, 23132080, 26429580, 31375830,
                37970830, 44631780, 51292730, 57953680, 64614630, 71275580, 84465580, 104250580, 130630580,
                163605580, 213068080, 279018080, 361455580, 460380580,575793080, 707693080, 905543080,
                1235293080, 1894793080, 5192293080,11787293080)
 # https://github.com/brooke-gill/pit/blob/307c126be78a5615b437205966dba13cbab3b787/xp2level.html#L93
@@ -80,30 +80,41 @@
             if self.xp() >= xp_reqs_levels[i]:
                 return i+1
         assert False
 
     def xp_gained_during_curr_pres(self) -> int:
         return self.xp() - total_xp_req_for_pres(self.prestige())
 
+    def xp_delta_req_for_curr_pres(self) -> int:
+        """Returns the xp requirements for the curr prestige (not including past prestiges)."""
+        return total_xp_req_for_pres(self.prestige()+1) - total_xp_req_for_pres(self.prestige())
+
     def percent_through_curr_pres(self) -> float:
-        return self.xp_gained_during_curr_pres() / (total_xp_req_for_pres(self.prestige()+1) -
-                                                    total_xp_req_for_pres(self.prestige()))
+        return self.xp_gained_during_curr_pres() / self.xp_delta_req_for_curr_pres()
 
     def percent_overall_to_given_pres(self, prestige: int) -> float:
         return self.xp() / total_xp_req_for_pres(prestige)
 
     def print_info(self) -> None:
         print(f"pit rank: {self.rank_string()}, pit xp: {self.xp()}")
         print(f"percent through current prestige: {Utils.percentify(self.percent_through_curr_pres())}")
         for i in range(1, 6):
             future_pres = self.prestige() + i
             if future_pres > 51:
                 break
             print(f"Overall way through to prestige {future_pres}: ", end="")
             print(Utils.percentify(self.percent_overall_to_given_pres(future_pres)), end=", ")
+        total_xp_for_120 = total_xp_reqs_for_levels(self.prestige())[-1]
+        xp_after_kings = round(min(total_xp_for_120, self.xp() + 0.30326 * self.xp_delta_req_for_curr_pres()))
+        # 30.326% figure from https://pit.wiki/Kings_Quest
+        print(f"King's quest would bring the rank to {PitStats(xp_after_kings).rank_string()}")
+        xp_after_overdrive = min(total_xp_for_120, self.xp() + 4000)
+        print(f"Overdrive would cover {round(4000 / self.xp_delta_req_for_curr_pres() * 100, 2)}% " +
+              f"of the current prestige's xp requirements. It would bring the rank to " +
+              f"{PitStats(xp_after_overdrive).rank_string()}")
         if not self._playtime_kills_deaths:
             print("\n")
             return
         playtime_mins, kills, deaths = self._playtime_kills_deaths
         playtime_hrs = playtime_mins / 60
         print(f"\npit playtime hours: {round(playtime_hrs, 3)}, ", end='')
         print(f"total kills: {kills}, KDR: {round(Utils.kdr_division(kills, deaths), 3)}, ", end='')
```

### Comparing `hypickle-1.1.2/hypickle/Player.py` & `hypickle-1.1.3/hypickle/Player.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional, List, Union, Dict
 from copy import deepcopy
 from datetime import datetime
+import time
 
 from . import Utils
 from . import hypixel
 from .MyClasses import UUID_Plus_Time, Specs
 from . import Files
 from .Pit import PitStats
 from . import ProcessingResults
@@ -133,14 +134,17 @@
 
     def percent_way_to_next_network_level(self) -> float:
         return leveling.getPercentageToNextLevel(self.get_network_xp())
 
     def percent_way_overall_to_given_network_level(self, target_level: int) -> float:
         return self.get_network_xp() / leveling.getTotalExpToLevelFloor(target_level)
 
+    def recent_games(self) -> List[Dict]:
+        return self.hypixel_object().getRecentGames()
+
     def specs_for_friends(self) -> Optional[Specs]:
         return self.specs().specs_for_friends()
 
     def represents_same_person(self, other: Player) -> bool:
         return self.uuid() == other.uuid()
 
     def set_specs(self, specs: Specs) -> None:
@@ -239,18 +243,23 @@
                 'star': self.get_bw_star(), 'pit_rank': self.pit_rank_string()}
 
     def print_dict_report(self, report: Dict, extra_text: str = '') -> None:
         report = deepcopy(report)
         assert all(isinstance(v, (str,float,int)) for v in report.values())
         possible_keys = ('name', 'fkdr', 'star', 'pit_rank', 'uuid', 'time')
         assert {'uuid'} <= set(report.keys()) <= set(possible_keys)
-        name, fkdr, star, pit_rank, uuid, time = [report.get(k) for k in possible_keys]
+        name, fkdr, star, pit_rank, uuid, time_friended = [report.get(k) for k in possible_keys]
         assert isinstance(uuid, str) # for mypy
-        rank = None if self.specs().just_uuids() else self.network_rank()
+        rank = None if (just_uuids := self.specs().just_uuids()) else self.network_rank()
 
+        recent_game_msg = ''
+        if not just_uuids and (recent_game := next(iter(self.recent_games()), None)):
+            ms_passed = time.time_ns() // 1_000_000 - (recent_game.get('ended') or recent_game['date'])
+            recent_game_msg = (('Exited' if 'ended' in recent_game else 'Entered') +
+                               f" {recent_game['gameType']} {round(ms_passed/60000, 2)} mins ago.\n")
         if name is not None:
             assert isinstance(name, str)
             if old_name := ProcessingResults.uuid_ign_pairs_in_results().get(uuid, ''):
                 old_name = '' if old_name.lower() == name.lower() else f' ({old_name})'
             if not self.root_player():
                 print_length = (len(rank.rank(True)) if rank else 0) + len(name) + len(old_name)
                 print(' ' * max(0, 38 - print_length), end='')
@@ -265,22 +274,25 @@
             magnitude = len(str(int(fkdr := round(fkdr, 3))))
             print(f" {fkdr:.3f}".ljust(6) + " fkdr".ljust(7-magnitude), end='')
         if star is not None:
             Colours.print_bw_star(star)
         if pit_rank is not None:
             Colours.print_pit_rank(pit_rank)
         if not self.root_player():
-            print(f" uuid {uuid[:(show := 5)]}...{uuid[-show:]}".ljust(10+show*2), end='')
-        if time is not None:
-            if Utils.is_date_string(time):
-                date_obj = datetime.strptime(time, '%Y-%m-%d')
-                time = date_obj.strftime('%b ') + date_obj.strftime('%d/%y').lstrip('0')
-            print(f" friended {time}", end='')
+            uuid_display = (f"{uuid[:(show := 5)]}...{uuid[-show:]}".ljust(4+show*2)
+                            if not just_uuids else f"{uuid} ")
+            print(f" uuid {uuid_display}", end='')
+        if time_friended is not None:
+            if Utils.is_date_string(time_friended):
+                date_obj = datetime.strptime(time_friended, '%Y-%m-%d')
+                time_friended = date_obj.strftime('%b ') + date_obj.strftime('%d/%y').lstrip('0')
+            print(f" friended {time_friended}".ljust(20), end='')
+        print(recent_game_msg, end='')
         print(extra_text, end='')
-        if (updated_json := self.hypixel_object().updated_json) is not None:
+        if not just_uuids and (updated_json := self.hypixel_object().updated_json) is not None:
             print(f" (updated player json obtained {updated_json[1].strftime('%I:%M:%S %p')})", end='')
         print()
 
     def print_player_info(self) -> None:
         print(f"{len(self.friends())} unique friends total\n")
         nw_level = self.get_network_level()
         closest_multiple_50 = Utils.round_up_to_closest_multiple(nw_level, 50)
@@ -298,15 +310,15 @@
         self.pit_stats_object().print_info()
         print(f"{'-'*150}\n\n")
 
     def create_dictionary_report(self, sort_key: str = "fkdr", should_terminate: bool = True,
                                  on_first_pass: Optional[bool] = None) -> dict:
         assert not (self.root_player() and self.time_friended_parent_player('date'))
         if (self.specs().required_online() and
-            not self.hypixel_object().isOnline((False, on_first_pass is False))):
+            not self.hypixel_object().isOnline((False, on_first_pass is False, False))):
             return {}
 
         report = self.get_stats_dict() if not self.specs().just_uuids() else {'uuid': self.uuid()}
         if time := self.time_friended_parent_player('date'):
             report['time'] = time
         if self.specs().print_player_data_exclude_friends():
             self.print_dict_report(report)
@@ -319,15 +331,15 @@
         self, report: dict, do_additional_passes: bool, sort_key: str,
         on_perpetual_pass: bool, on_first_pass: bool, end_index: Optional[int] = None
     ) -> None:
         """Will modify `report`, which is passed by reference."""
         if self._players_used_to_combine:
             assert self.root_player()
             for player in self._players_used_to_combine:
-                online_status = 'online' if player.hypixel_object().isOnline((True, True)) else 'offline'
+                online_status = 'online' if player.hypixel_object().isOnline((True,)*3) else 'offline'
                 player.print_dict_report(player.get_stats_dict(), f"this arg player is {online_status}")
             print()
 
         report.setdefault('friends', [])
         assert not on_first_pass or not on_perpetual_pass
         if do_additional_passes:
             assert on_first_pass and self.root_player()
```

### Comparing `hypickle-1.1.2/hypickle/ProcessingResults.py` & `hypickle-1.1.3/hypickle/ProcessingResults.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,24 @@
 from typing import Optional, List, Dict
 from copy import deepcopy
 
 from . import Utils
 from . import Files
 from .MyClasses import UUID_Plus_Time
 from . import hypixel
-from .Args import Args
+from .MyClasses import args
 
-_args: Optional[Args] = None
 _all_dicts_standard_files: Optional[List[dict]] = None
 _all_dicts_additional_friends_files: Optional[List[dict]] = None
 _all_dicts_unique_uuids: Optional[List[dict]] = None
 _ign_uuid_pairs_in_results: Optional[Dict[str, str]] = None
 _uuid_ign_pairs_in_results: Optional[Dict[str, str]] = None
 
 _NON_TRIVIAL_KEYS = ('friends', 'name', 'fkdr', 'star', 'pit_rank')
 
-def set_args(args: Args) -> None:
-    global _args
-    assert not _args
-    _args = deepcopy(args)
-
 def ign_uuid_pairs_in_results(get_deepcopy: bool = False) -> Dict[str, str]:
     global _ign_uuid_pairs_in_results
 
     if not _ign_uuid_pairs_in_results:
         _ign_uuid_pairs_in_results = {}
         for d in (get_all_dicts_in_results(False, True) + get_all_dicts_in_results(False, False)):
             _ign_uuid_pairs_in_results.update(Utils.get_all_ign_uuid_pairs_in_dict(d))
@@ -148,32 +142,30 @@
 def _get_all_jsons_in_results(get_additional_friends: bool = False) -> List[dict]:
     """Returns a list of dicts, where each dict represents the json each textfile stores."""
     if not os.path.isdir('results'):
         return []
     all_jsons: List[dict] = []
     all_paths = sorted(Path('results').iterdir(), key=os.path.getmtime, reverse=True)
     all_files = [f.name for f in all_paths if _does_filename_meet_reqs(f.name, get_additional_friends)]
-    assert _args
     for f in all_files:
         filename = os.path.join('results', f)
         is_multi_player_file = any(x in f for x in [' plus ', ' minus ', ' intersect '])
-        if is_multi_player_file and not _args.include_multi_player_files():
+        if is_multi_player_file and not args().include_multi_player_files():
             continue
         json_in_file = Files.read_json_textfile(filename)
         json_in_file['filename'] = filename
-        if is_multi_player_file and _args.skip_first_dict_in_multi_player_files():
+        if is_multi_player_file and args().skip_first_dict_in_multi_player_files():
             json_in_file['exclude'] = '' # Adding this key as a signal to exclude this
                                          # outermost dict of the file, when unnesting.
         all_jsons.append(json_in_file)
     return all_jsons
 
 def _does_filename_meet_reqs(f: str, for_additional_friends: bool = False) -> bool:
-    if for_additional_friends:
-        return f.startswith('Additional friends of') and f.endswith('.txt')
-    return f.startswith('Friends of') and f.endswith('.txt')
+    required_start = 'Additional friends of' if for_additional_friends else 'Friends of'
+    return f.startswith(required_start) and f.endswith('.txt')
 
 def _get_only_non_trivial_keys_in_dict(dicts: List[dict]) -> List[dict]:
     return [d for d in dicts if any(k in d for k in _NON_TRIVIAL_KEYS)]
 
 def _get_all_unique_uuids_in_results() -> List[str]:
     """Returns all uuids written at some point in the results folder - most will be friends of friends."""
     all_dicts = []
```

### Comparing `hypickle-1.1.2/hypickle/Rank.py` & `hypickle-1.1.3/hypickle/Rank.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/hypickle/Utils.py` & `hypickle-1.1.3/hypickle/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 def kdr_division(kills: int, deaths: int) -> float:
     return kills / deaths if deaths else float(kills)
 
 def date_to_epoch(date_string: str, in_seconds: bool) -> float:
     epoch = time.mktime(datetime.strptime(date_string, '%Y-%m-%d').timetuple())
     return epoch * 1000 if not in_seconds else epoch
 
-def epoch_to_date(epoch: float, in_seconds: bool) -> str:
-    return datetime.fromtimestamp(epoch / 1000 if not in_seconds else epoch).strftime('%Y-%m-%d')
+def epoch_to_date(epoch: float, epoch_in_seconds: bool) -> str:
+    return datetime.fromtimestamp(epoch / 1000 if not epoch_in_seconds else epoch).strftime('%Y-%m-%d')
 
 def find_dict_for_given_player(d: dict, uuid_or_ign: str, make_deep_copy: bool = True,
                                dict_must_have_friends_list: bool = True) -> Optional[dict]:
     """ d will be a dictionary read from a file in json format - it will have a uuid key, and possibly
     a name, fkdr, and friends key. The friends key would have a value that is a list of dictionaries,
     recursively following the same dictionary requirements."""
     if make_deep_copy:
@@ -161,15 +161,15 @@
         if (uuid not in dicts_unique_uuids or is_first_dict_more_valuable(d, dicts_unique_uuids[uuid],
         must_have_times_friended)):
             dicts_unique_uuids[uuid] = d
     return list(dicts_unique_uuids.values())
 
 def is_in_milliseconds(epoch_val: Union[float, int]) -> bool:
     """epoch_val is assumed to be in either seconds or milliseconds"""
-    return epoch_val > 10000000000
+    return epoch_val > 10_000_000_000
 
 def convert_to_seconds(time_val: Union[float, int, str, None]) -> float:
     """ Converts a datestring or epoch to epoch in seconds. If time_val is already an epoch, it must be
         in seconds or milliseconds form. """
     if time_val is None:
         return 0
     elif isinstance(time_val, str):
@@ -265,8 +265,13 @@
         return_val = default_val
     assert expected_type is None or type(return_val) == expected_type
     return return_val
 
 def print_diff_dicts(old_dict: dict, new_dict: dict, prepended_msg: str = '') -> None:
     from deepdiff import DeepDiff # type: ignore
     print(prepended_msg, end='')
-    pprint(DeepDiff(old_dict, new_dict), indent=2)
+    pprint(DeepDiff(old_dict, new_dict), indent=2)
+
+def content_in_file(filename: str) -> bool:
+    """Returns True if there is at least one non-whitespace character in the file."""
+    with open(filename, 'r') as f:
+        return f.read().strip() != ''
```

### Comparing `hypickle-1.1.2/hypickle/additional_friends.py` & `hypickle-1.1.3/hypickle/additional_friends.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import hypixel
 from .MyClasses import Specs
 from . import Files
 from .Player import Player
 
 def get_friends_from_user(friends_specs: Specs) -> List[Player]:
     friends: List[Player] = []
-    INPUT_MSG = "Enter the igns/uuids of additional friends, separated by spaces (or enter 'done' to stop): "
+    INPUT_MSG = "Enter the igns/uuids of new friends to add, separated by spaces (or enter 'done' to stop): "
     for i, user_input in enumerate(inputs := Files.apply_aliases(input(INPUT_MSG).split())):
         if user_input.lower() in ('done', 'stop'):
             assert i == len(inputs)-1
             return friends
         friends.append(Player(hypixel.get_uuid(user_input), specs=friends_specs,
                               time_friended_parent_player=Utils.get_current_date()))
     return friends + get_friends_from_user(friends_specs)
```

### Comparing `hypickle-1.1.2/hypickle/bedwars.py` & `hypickle-1.1.3/hypickle/bedwars.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/hypickle/hypixel.py` & `hypickle-1.1.3/hypickle/hypixel.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,73 +2,55 @@
     Modifications made by John (late 2022 to current) """
 __version__ = '0.8.0'
 # pylint: disable=C0103
 
 from random import choice
 from time import time, sleep
 from datetime import datetime, timedelta
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Dict
 import re
-from copy import deepcopy
 import os.path
 import requests
-import urllib3
 
-from .MyClasses import UUID_Plus_Time
+from .MyClasses import UUID_Plus_Time, args
 from . import Files
 from . import Utils
-from .Args import Args
 from . import leveling
 from .Rank import Rank
 
-def _get_api_keys_from_file() -> List[str]:
-    """ This function gets the api key(s) from `api-key.txt`, and returns them in a list. If the file doesn't
-        exist, it will ask the user for an api key and write it to the new file."""
-    FILENAME = 'api-key.txt'
-    if not os.path.isfile(FILENAME):
-        print("The script needs a hypixel api key. To get one, you can follow the first part of this guide: https://gist.github.com/camnwalter/c0156c68b1e2a21ec0b084c6f04b63f0#how-to-get-a-new-api-key-after-the-hypixel-api-changes")
-        api_key = input("Please enter your api key: ")
-        with open(FILENAME, 'w') as file:
-            file.write(api_key)
-    with open(FILENAME) as file:
-        return [line.rstrip() for line in file]
-
-API_KEYS: List[str] = _get_api_keys_from_file()
-HYPIXEL_API_URL: str = 'https://api.hypixel.net/'
 TIME_STARTED: float = time()
 num_api_calls_made: int = 0
-_args: Optional[Args] = None
 
-def set_args(args: Args) -> None:
-    global _args
-    assert not _args
-    _args = deepcopy(args)
-    if not _args.verify_requests():
-        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+def make_request_url(typeOfRequest: str, uuid_or_ign: Optional[str]) -> str:
+    assert (typeOfRequest == 'leaderboards') == (uuid_or_ign is None)
+    requestURL = 'https://api.hypixel.net/' + typeOfRequest
+    if uuid_or_ign is not None:
+        if (query_param_name := 'uuid' if Utils.is_uuid(uuid_or_ign) else 'name') == 'name':
+            assert typeOfRequest == 'player'
+        requestURL += f"?{query_param_name}={uuid_or_ign}"
+    return requestURL
 
 sleep_till: Optional[datetime] = None
-def getJSON(typeOfRequest: str, uuid_or_ign: str) -> dict:
+def getJSON(typeOfRequest: str, uuid_or_ign: Optional[str], specific_api_key: Optional[str] = None) -> dict:
     """ This function is used for getting a JSON from Hypixel's Public API. """
     global sleep_till, num_api_calls_made
-    assert _args
 
     if sleep_till and (sleep_duration := (sleep_till - datetime.now()).total_seconds()) >= 0:
         print(f"Sleeping until {sleep_till.strftime('%I:%M:%S %p')} for rate limiting.")
         sleep(sleep_duration)
     sleep_till = None
 
     num_api_calls_made += 1
-    if _args.debug_api():
+    if args().debug_api():
         print(f"{num_api_calls_made}\n{time() - TIME_STARTED}\n\n")
 
-    if typeOfRequest != 'player':
-        assert Utils.is_uuid(uuid_or_ign)
-    requestEnd = f"{'uuid' if Utils.is_uuid(uuid_or_ign) else 'name'}={uuid_or_ign}"
-    requestURL = f"{HYPIXEL_API_URL}{typeOfRequest}?{requestEnd}"
-    response = requests.get(requestURL, headers={"API-Key": choice(API_KEYS)}, verify=_args.verify_requests())
+    response = requests.get(
+        make_request_url(typeOfRequest, uuid_or_ign), verify=args().verify_requests(),
+        headers={"API-Key": _get_api_key() if specific_api_key is None else specific_api_key}
+    )
     try:
         responseHeaders, responseJSON = response.headers, response.json()
     except Exception as e:
         raise Exception(
             f'{response.content.decode()}\nresponse content ^\nuuid_or_ign: {uuid_or_ign}\n'
             f'typeOfRequest: {typeOfRequest}\nthere was a problem with response.json()'
         ) from e
@@ -81,14 +63,36 @@
     if typeOfRequest == 'player' and responseJSON['player'] is None:
         raise PlayerNotFoundException(uuid_or_ign)
     try:
         return responseJSON[typeOfRequest]
     except KeyError:
         return responseJSON
 
+def _get_api_key() -> str:
+    """ This function returns one of the key(s) in `api-key.txt`. If the file doesn't exist, it will ask the
+        user for an api key and write it to the new file. """
+    FILENAME = 'api-key.txt'
+    if not os.path.isfile(FILENAME) or not Utils.content_in_file(FILENAME):
+        print("The script needs a hypixel api key. To get one, you can follow the first part of this guide: https://gist.github.com/camnwalter/c0156c68b1e2a21ec0b084c6f04b63f0#how-to-get-a-new-api-key-after-the-hypixel-api-changes")
+        while not _validate_api_key(api_key := input("Please enter your api key: ").strip()):
+            print('Sorry, that api key is invalid.')
+        with open(FILENAME, 'w') as file:
+            file.write(api_key)
+    with open(FILENAME) as file:
+        return choice([x for line in file if (x := line.strip())])
+
+def _validate_api_key(key: str) -> bool:
+    try:
+        getJSON('leaderboards', None, specific_api_key=key)
+    except HypixelAPIError as e:
+        if "'cause': 'Invalid API key'" in repr(e):
+            return False
+        raise RuntimeError('Unexpected error') from e
+    return True
+
 def get_uuid(uuid_or_ign: str, call_api_last_resort: bool = True) -> str:
     """Param can be an ign or uuid. If it's a uuid, this function will return it immediately. Otherwise,
        it will try to get it from uuids.txt (and if so, then verify the player's current ign is still the same
        by using a temp hypixel object). Finally if this fails, a temp hypixel object is created in order to call
        getUUID() - unless `call_api_last_resort` is False, in which case the ign is just returned."""
 
     uuid_or_ign = uuid_or_ign.lower()
@@ -110,14 +114,17 @@
 
 class Player:
     def __init__(self, uuid_or_ign: str) -> None:
         self.JSON = getJSON('player', get_uuid(uuid_or_ign, call_api_last_resort=False))
         self._rank = Rank(self.JSON)
         self.updated_json: Optional[Tuple[dict, datetime]] = None
         """Stores the newest result of `getJSON('player')` that was updated from the previous call."""
+        self.recent_games_visible: Optional[bool] = None
+        """Recent games may not be visible if the player has turned off the api setting, or if they haven't
+           played a game in roughly 3 days it seems."""
 
     def getName(self, extra_safety_check=True) -> str:
         """ Just return player's name. """
         if not extra_safety_check:
             return self.JSON['displayname']
         sanitized_name = re.sub("[^A-Za-z0-9_]", "", self.JSON['displayname'])
         # Removes any leading whitespace, and only keeps alphanumerics and underscores.
@@ -135,38 +142,40 @@
             This function returns a list of the UUIDs of all the player's friends."""
         friends = []
         for friend in getJSON('friends', self.getUUID())['records']:
             friend_uuid = friend["uuidReceiver"] if friend["uuidReceiver"] != self.getUUID() else friend["uuidSender"]
             friends.append(UUID_Plus_Time(friend_uuid, friend['started']))
         return list(reversed(friends))
 
-    def isOnline(self, extra_online_checks: Tuple[bool, bool]) -> bool:
+    def isOnline(self, extra_online_checks: Tuple[bool, bool, bool]) -> bool:
         """ This function returns a bool representing whether the player is online.
             For `extra_online_checks`:
                 - The first bool is for players whose online status is shown. It determines whether to check
                   the current online statuses of players, irrespective of whether they were recorded as
                   online in the original self.JSON. So, this bool being true limits false negatives, at
                   the expense of more api calls.
                 - The second bool determines whether to call the api for the most recent json to see if
-                  it's changed, for players whose online status is disabled."""
+                  it's changed, for players whose online status is disabled.
+                - The third bool determines whether, as a last resort, to call the `recentgames` endpoint,
+                  in order to see if the most recent game is visible, and if it doesn't have an
+                  'ended' key; if so, the player is online."""
         if {'lastLogin', 'lastLogout'} <= self.JSON.keys():
             return (    (extra_online_checks[0] or self.JSON['lastLogin'] > self.JSON['lastLogout'])
                     and getJSON('status', self.getUUID())['session']['online'])
         # This player doesn't have the online status shown, but we can check if stats from
         # the original self.JSON have updated (if the caller has enabled this feature):
         if extra_online_checks[1] and self.JSON != (json := getJSON('player', self.getUUID())):
             self.set_updated_json_if_applicable(json)
             return True
-        return False
+        return extra_online_checks[2] and bool(games := self.getRecentGames()) and 'ended' not in games[0]
 
     def set_updated_json_if_applicable(self, new_json: dict) -> None:
-        assert _args
         if new_json == (curr_latest_json := self.updated_json[0] if self.updated_json else self.JSON):
             return
-        if _args.show_json_updates():
+        if args().show_json_updates():
             Utils.print_diff_dicts(curr_latest_json, new_json, f"\nUpdates to json for {self.getName()}: ")
         self.updated_json = (new_json, datetime.now())
 
     def getFKDR(self) -> float:
         return Utils.kdr_division(
             Utils.nested_get(self.JSON, ('stats', 'Bedwars', 'final_kills_bedwars'), 0, int),
             Utils.nested_get(self.JSON, ('stats', 'Bedwars', 'final_deaths_bedwars'), 0, int)
@@ -199,7 +208,13 @@
         return int(xp)
 
     def getExactNWLevel(self) -> float:
         return leveling.getExactLevel(self.getNetworkXP())
 
     def getNetworkRank(self) -> Rank:
         return self._rank
+
+    def getRecentGames(self) -> List[Dict]:
+        if self.recent_games_visible is False:
+            return []
+        self.recent_games_visible = bool(recent_games := getJSON('recentgames', self.getUUID())['games'])
+        return recent_games
```

### Comparing `hypickle-1.1.2/hypickle/leveling.py` & `hypickle-1.1.3/hypickle/leveling.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/hypickle/main.py` & `hypickle-1.1.3/hypickle/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import sys
-from typing import List, Tuple, Optional
+from typing import List, Tuple
 from itertools import permutations
 from copy import deepcopy
 
 from . import hypixel
-from .MyClasses import Specs, UUID_Plus_Time
+from . import MyClasses
+from .MyClasses import Specs, UUID_Plus_Time, args
 from . import Files
 from .Player import Player
-from .Args import Args
 from . import ProcessingResults
 from . import additional_friends
 from . import Utils
 from . import Pit
 from . import leveling
 from . import bedwars
 from . import Graphing
 from .Graphing import ScatterplotInfo
 
 def intersect_player_lists(l1: List[Player], l2: List[Player]) -> List[Player]:
     return [p for p in l1 if p.in_player_list(l2)]
 
-def combine_players(info_on_players: List[Player], args: Args) -> Player:
+def combine_players(info_on_players: List[Player]) -> Player:
     """This function runs through the Player list and adds/subtracts/intersects f lists. Whether a Player's f list
     is used to add/subtract/intersect depends on the bool value of their player.will_exclude_friends()
     and player.will_intersect() functions.
     If a player's f list is used to intersect, it will intersect the entire friends list up to that point,
     either for playerFriends or exclude_friends.
     Order of operations:
         union, intersect (left to right for precedence amongst these)
@@ -53,45 +53,45 @@
             else:
                 playerFriends.extend(player.friends())
                 playerNameForFileOutput += ' plus ' + player.name()
 
     player = Player(playerUUID, friends=playerFriends, name_for_file_output=playerNameForFileOutput,
                     specs=playerSpecs, date_cutoff_for_friends=date_cutoff_friends,
                     players_used_to_combine=deepcopy(info_on_players)
-                    if args.track_if_arg_players_online() else None)
+                    if args().track_if_arg_players_online() else None)
     player.polish_friends_list(exclude_friends)
     return player
 
-def diff_f_lists(players: List[Player], args: Args) -> None:
+def diff_f_lists(players: List[Player]) -> None:
     """Runs through all pairs of players and outputs the diff of their f lists"""
-    assert args.diff_f_lists()
+    assert args().diff_f_lists()
     list_friends = input("Enter y to list out all the friends in each diff: ") in ('y', 'Y')
     print('\n\n')
     for p1, p2 in permutations(players, 2):
         p1.diff_f_lists(p2, list_friends)
 
-def get_players_from_args(args: Args) -> Tuple[List[Player], List[str]]:
+def get_players_from_args() -> Tuple[List[Player], List[str]]:
     """The first item in the tuple will be a list of Players.
-       The second item will likely be empty for most use cases. However, if the user wants this feature,
+       The second item will likely be empty for most use cases. However, if the caller wants this feature,
        it will be a list if uuid strings, where it's intended for each uuid to be checked for when they
        were friended by a Player in the first list."""
 
-    specs = Specs.make_specs_object_and_initialize_common_specs(args)
-    args_no_keywords_or_date = args.get_args(True)
+    specs = Specs.make_specs_object_and_initialize_common_specs()
+    args_no_keywords_or_date = args().get_args(True)
     players: List[Player] = []
     in_minus_symbol_section = False
     in_friended_when_section = False
     is_intersect_player = False
     FRIENDED_WHEN = 'friendedwhen'
     INTERSECT = 'intersect'
     uuids_for_friended_when: List[str] = []
 
     for i, arg in enumerate(args_no_keywords_or_date):
         if in_minus_symbol_section or in_friended_when_section or is_intersect_player:
-            assert not args.do_mini_program()
+            assert not args().do_mini_program()
 
         if arg.endswith('.txt'):
             assert not in_friended_when_section
             continue
         if arg == '-':
             in_minus_symbol_section = True
             assert not in_friended_when_section
@@ -110,27 +110,27 @@
             continue
 
         next_arg = args_no_keywords_or_date[i+1] if i+1 < len(args_no_keywords_or_date) else None
         use_specific_textfile = next_arg and next_arg.endswith('.txt')
         num_friends_msgs = ['', '']
 
         if use_specific_textfile:
-            assert not args.do_file_output()
+            assert not args().do_file_output()
             player = Player.make_player_from_json_textfile(args_no_keywords_or_date[i+1], arg, specs=specs)
         else:
             hypixel_obj = hypixel.Player(arg)
             uuid = hypixel_obj.getUUID()
             all_friends: List[UUID_Plus_Time] = []
             standard_friends = ProcessingResults.get_best_f_list_for_player_in_results(
                 uuid, must_have_times_friended=FRIENDED_WHEN in args_no_keywords_or_date
             )
             num_friends_msgs[0] = f"{len(standard_friends)} friends in biggest single friends list/file\n"
-            if args.get_additional_friends():
+            if args().get_additional_friends():
                 all_friends = ProcessingResults.get_all_additional_friends_for_player(uuid)
-                num_friends_msgs[1] = f"{len(all_friends)} unique 'additional friends'\n"
+                num_friends_msgs[1] = f"{len(all_friends)} unique manually added friends\n"
                 for f in standard_friends:
                     ProcessingResults.update_list_if_applicable(all_friends, f)
             else:
                 all_friends = standard_friends
             all_friends.sort(key=UUID_Plus_Time.sort_key)
             player = Player(uuid, specs=specs, friends=all_friends, hypixel_object=hypixel_obj)
 
@@ -139,15 +139,15 @@
         player.print_dict_report(player.get_stats_dict())
         print(num_friends_msgs[0] + num_friends_msgs[1], end='')
         player.print_player_info()
 
         player.set_will_exclude_friends(in_minus_symbol_section)
         player.set_will_intersect(is_intersect_player)
         if not player.will_exclude_friends():
-            player.set_date_cutoff_for_friends(args.date_cutoff())
+            player.set_date_cutoff_for_friends(args().date_cutoff())
         players.append(player)
         is_intersect_player = False
 
     return (players, uuids_for_friended_when)
 
 def output_player_jsons_to_file(players: List[Player]) -> None:
     for player in players:
@@ -162,107 +162,103 @@
             time_friended = friend.time_friended_parent_player('date')
             if time_friended is not None:
                 assert isinstance(time_friended, str)
                 print(f'{player.name()} became friends with {friend.name()} on {time_friended}')
             else:
                 print(f'{player.name()} is friends with {friend.name()}, but no date recorded.')
 
-def set_args_in_files(args: Args) -> None:
-    ProcessingResults.set_args(args)
-    hypixel.set_args(args)
-
-def do_mini_program(args: Args) -> None:
-    if args.add_additional_friends():
-        additional_friends.add_additional_friends_to_file_system(args.get_args(True)[0])
-    elif args.update_aliases():
-        Files.update_aliases(args.get_keywords())
-    elif args.add_uuid_aliases():
+def do_mini_program() -> None:
+    if args().add_additional_friends():
+        additional_friends.add_additional_friends_to_file_system(args().get_args(True)[0])
+    elif args().update_aliases():
+        Files.update_aliases(args().get_keywords())
+    elif args().add_uuid_aliases():
         Files.update_aliases(
-            args.get_keywords(), ((p.name(), p.uuid()) for p in get_players_from_args(args)[0])
+            args().get_keywords(), ((p.name(), p.uuid()) for p in get_players_from_args()[0])
         )
-    elif args.print_aliases():
+    elif args().print_aliases():
         Files.print_aliases()
-    elif args.get_player_json():
-        output_player_jsons_to_file(get_players_from_args(args)[0])
-    elif args.pit_percent():
-        for arg in args.get_args(True):
+    elif args().get_player_json():
+        output_player_jsons_to_file(get_players_from_args()[0])
+    elif args().pit_percent():
+        for arg in args().get_args(True):
             Pit.PitStats(Pit.get_xp_req_for_rank(arg)).print_info()
-    elif args.pit_plot():
+    elif args().pit_plot():
         fig1 = ScatterplotInfo(Pit.xp_percent_levels(), range(1, 121), 'Levels',
                                'XP % Through a Prestige', 'Level')
         prestige_xps = Pit.PRESTIGE_XP[:50]
         fig2 = ScatterplotInfo(prestige_xps, range(1, len(prestige_xps)+1),
                                'XP vs Prestige', 'XP', 'Prestige')
         Graphing.output_scatterplots((fig1, fig1.invert(), fig2, fig2.invert()))
-    elif args.network_plot():
+    elif args().network_plot():
         level_range = range(1, 1001)
         fig = ScatterplotInfo((leveling.getTotalExpToLevelFloor(l) for l in level_range), level_range,
                               "XP vs Network Level", "XP", "Level")
         fig_inverted = fig.invert()
         print(f"level vs xp data fit to a quadratic: {fig_inverted.fit_to_polynomial(2)}\n")
         Graphing.output_scatterplots((fig, fig_inverted))
-    elif args.bedwars_plot():
+    elif args().bedwars_plot():
         print("Note that for some players, they may get to some levels with slightly less xp "
               "than required on the graph. Not exactly sure why this is. Made a bug report to "
               "hypixel, see if they get back to you with a reason for it.")
         level_range = range(0, 3001)
         fig = ScatterplotInfo(level_range, (bedwars.totalExpForLevel(l) for l in level_range),
                               "Bedwars Level vs XP", "Level", "XP")
         print(f"\nlevel vs xp data fit to a linear function: {fig.fit_to_polynomial(1)}\n")
         Graphing.output_scatterplots([fig])
-    elif args.contains_substr():
-        for substr in args.get_args(False)[1:]:
+    elif args().contains_substr():
+        for substr in args().get_args(False)[1:]:
             substr = substr.lower()
-            keyword_matches = sorted([keyword for keyword in args.get_keywords()
+            keyword_matches = sorted([keyword for keyword in args().get_keywords()
                                       if substr in keyword.lower()])
             print(f"Keyword matches for '{substr}':\n" + '\n'.join(keyword_matches))
             ign_matches = sorted([ign for ign in ProcessingResults.ign_uuid_pairs_in_results()
                                   if substr in ign.lower()])
             print(f"\nPlayer name matches for '{substr}':\n" + '\n'.join(ign_matches) + '\n')
     else:
         assert False
 
-def main(argv: Optional[List[str]] = None) -> None:
-    """argv is used when calling this function as a dev in the parent dir."""
-    args = Args(argv if argv is not None else sys.argv)
-    set_args_in_files(args)
+def main(argv: List[str]) -> None:
+    """When called as a script, `argv` is passed `sys.argv` from the if statement at the end of this file.
+       If called as a module (e.g., as a dev from the parent dir), argv is whatever the caller passes."""
+    MyClasses.set_args(argv)
 
-    if args.do_mini_program():
-        do_mini_program(args)
+    if args().do_mini_program():
+        do_mini_program()
         sys.exit(0)
 
     newest_n_friends, oldest_n_friends = None, None
-    if args.get_newest_friends():
+    if args().get_newest_friends():
         newest_n_friends = int(input("Enter the n newest friends you want: "))
-    elif args.get_oldest_friends():
+    elif args().get_oldest_friends():
         oldest_n_friends = int(input("Enter the n oldest friends you want: "))
 
-    if args.find_matching_igns_or_uuids_in_results():
-        ProcessingResults.print_all_matching_uuids_or_igns(args.get_args(True)[0])
-    players_from_args, uuids_for_friended_when = get_players_from_args(args)
-    if args.diff_f_lists():
-        diff_f_lists(players_from_args, args)
+    if args().find_matching_igns_or_uuids_in_results():
+        ProcessingResults.print_all_matching_uuids_or_igns(args().get_args(True)[0])
+    players_from_args, uuids_for_friended_when = get_players_from_args()
+    if args().diff_f_lists():
+        diff_f_lists(players_from_args)
     if uuids_for_friended_when:
         friended_when_feature(players_from_args, uuids_for_friended_when)
 
-    player = combine_players(players_from_args, args)
+    player = combine_players(players_from_args)
     player.keep_just_first_or_last_friends(newest_n_friends, oldest_n_friends)
     print(f"Now {len(player.friends())} friends after adjustments specified in args.\n\n")
 
-    if args.check_results():
+    if args().check_results():
         ProcessingResults.check_results(player.uuid(), player.name())
 
-    if args.update_uuids():
+    if args().update_uuids():
         Files.update_uuids_file(ProcessingResults.ign_uuid_pairs_in_results())
 
     report = player.create_dictionary_report(
-        sort_key = "star" if args.sort_by_star() else "pit_rank" if args.sort_by_pit_rank() else "fkdr",
-        should_terminate = args.do_file_output() or not args.just_online_friends()
+        sort_key = "star" if args().sort_by_star() else "pit_rank" if args().sort_by_pit_rank() else "fkdr",
+        should_terminate = args().do_file_output() or not args().just_online_friends()
     )
-    if args.do_file_output():
+    if args().do_file_output():
         filename = ("Friends of " +
-                    ("friends of " if args.find_friends_of_friends() else "") +
+                    ("friends of " if args().find_friends_of_friends() else "") +
                     player.name_for_file_output())
         Files.write_data_as_json_to_file(report, filename)
 
 if __name__ == '__main__':
-    main()
+    main(sys.argv)
```

### Comparing `hypickle-1.1.2/hypickle.egg-info/PKG-INFO` & `hypickle-1.1.3/hypickle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.2
+Version: 1.1.3
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,15 +40,15 @@
 with the `hypickle` script (explained below).
 
 ### Main features:
 
 - Basic usage is to run with `hypickle *username/uuid*`
   - This will output stats for the specified player, and then output any friends for them.
   - Since the `friends` endpoint of hypixel's API was deprecated, you must manually add any friends for them you want.
-    To do this, run `hypickle addadditionalfriends *username/uuid*`
+    To do this, run `hypickle addfriends *username/uuid*`
 - If there's a player you run the program on often, consider making an alias for their uuid:
   - Run `hypickle updateuuidaliases *username*`
   - Then when running `hypickle *username*`, the program will automatically substitute the username for the uuid.
     This is useful when running the program in quick succession for the same player, since the hypixel api forces a cooldown
     when sending in a username instead of a uuid.
 - You can also add an optional argument called 'all', if you'd like to output all friends (not just those currently online).
   - E.g., `hypickle *username/uuid* all`
@@ -56,15 +56,15 @@
 ### Developer commands:
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
-  - `pydeps main.py` will output a dependency graph of the project's modules.
+  - `pydeps hypickle` will output a dependency graph of the project's modules.
   - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
   - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.2/hypickle.egg-info/SOURCES.txt` & `hypickle-1.1.3/hypickle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.2/pyproject.toml` & `hypickle-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">= 3.0"
 name = "hypickle"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="John Doknjas", email="jdoknjas@sfu.ca" },
 ]
 description = "A script that outputs realtime stats for custom lists of friends you create."
 keywords = ["hypickle", "hypixel", "pit", "bedwars", "friends", "stats", "api"]
 dependencies = [
   "requests",
```

