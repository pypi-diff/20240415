# Comparing `tmp/db_cache_manager-0.1.0.tar.gz` & `tmp/db_cache_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ramtinyazdanian/PycharmProjects/db-cache-manager/dist/.tmp-6a4oz5cc/db_cache_manager-0.1.0.tar", last modified: Mon Feb 19 09:25:13 2024, max compression
+gzip compressed data, was "db_cache_manager-0.1.1.tar", last modified: Mon Apr 15 08:45:13 2024, max compression
```

## Comparing `db_cache_manager-0.1.0.tar` & `db_cache_manager-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ramtinyazdanian   (501) staff       (20)        0 2024-02-19 09:25:13.546534 db_cache_manager-0.1.0/
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)     1067 2023-10-30 15:43:51.000000 db_cache_manager-0.1.0/LICENSE
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)    11968 2024-02-19 09:25:13.545583 db_cache_manager-0.1.0/PKG-INFO
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)    11142 2024-02-15 15:02:56.000000 db_cache_manager-0.1.0/README.md
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)      897 2024-02-15 14:10:06.000000 db_cache_manager-0.1.0/pyproject.toml
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)       38 2024-02-19 09:25:13.546683 db_cache_manager-0.1.0/setup.cfg
-drwxr-xr-x   0 ramtinyazdanian   (501) staff       (20)        0 2024-02-19 09:25:13.536821 db_cache_manager-0.1.0/src/
-drwxr-xr-x   0 ramtinyazdanian   (501) staff       (20)        0 2024-02-19 09:25:13.539924 db_cache_manager-0.1.0/src/db_cache_manager/
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)        1 2023-10-30 15:29:34.000000 db_cache_manager-0.1.0/src/db_cache_manager/__init__.py
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)    32149 2024-02-15 15:22:58.000000 db_cache_manager-0.1.0/src/db_cache_manager/db.py
-drwxr-xr-x   0 ramtinyazdanian   (501) staff       (20)        0 2024-02-19 09:25:13.544774 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)    11968 2024-02-19 09:25:13.000000 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)      339 2024-02-19 09:25:13.000000 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)        1 2024-02-19 09:25:13.000000 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)       35 2024-02-19 09:25:13.000000 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/requires.txt
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)       17 2024-02-19 09:25:13.000000 db_cache_manager-0.1.0/src/db_cache_manager.egg-info/top_level.txt
-drwxr-xr-x   0 ramtinyazdanian   (501) staff       (20)        0 2024-02-19 09:25:13.543645 db_cache_manager-0.1.0/tests/
--rw-r--r--   0 ramtinyazdanian   (501) staff       (20)     5485 2024-02-19 09:11:22.000000 db_cache_manager-0.1.0/tests/test_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.926033 db_cache_manager-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.926033 db_cache_manager-0.1.1/src/db_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/src/db_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/src/db_cache_manager/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/tests/test_cache_manager.py
```

### Comparing `db_cache_manager-0.1.0/LICENSE` & `db_cache_manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.0/PKG-INFO` & `db_cache_manager-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.0/README.md` & `db_cache_manager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.0/pyproject.toml` & `db_cache_manager-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "db_cache_manager"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" },
   { name="Aitor Pérez", email="aitor.perez@epfl.ch" }
 ]
 description = "Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `db_cache_manager-0.1.0/src/db_cache_manager/db.py` & `db_cache_manager-0.1.1/src/db_cache_manager/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -680,26 +680,32 @@
             equality_conditions: Dict of equality conditions
             do_date_sort: If False, the results will NOT be sorted by `date_added`, but by `id_token` (FASTER)
             use_date_modified_col: If True, date_modified will be used for earliest/latest date comparisons (
                 instead of date_added)
         Returns:
             Dict mapping id tokens to colname->value dicts
         """
-        # If we want to exclude a token, all the tokens whose closest match is the former should also be excluded
-        # in order not to create cycles.
+        # If we want to exclude one or more tokens, all the tokens whose closest match is the former should
+        # also be excluded in order not to create cycles.
         if exclude_token is not None:
+            # Convert exclude_token into a set
+            if isinstance(exclude_token, list):
+                exclude_token = set(exclude_token)
+            if not isinstance(exclude_token, set):
+                exclude_token = {exclude_token}
             all_closest_matches = self.get_all_closest_matches()
             if all_closest_matches is not None:
-                exclude_tokens = {k for k, v in all_closest_matches.items() if v == exclude_token}
+                all_tokens_to_exclude = {k for k, v in all_closest_matches.items() if v in exclude_token}
             else:
-                exclude_tokens = set()
-            exclude_tokens.add(exclude_token)
+                all_tokens_to_exclude = set()
+            all_tokens_to_exclude = all_tokens_to_exclude.union(exclude_token)
         else:
-            exclude_tokens = None
-        results = self._get_all_details(self.cache_table, cols, start=start, limit=limit, exclude_token=exclude_tokens,
+            all_tokens_to_exclude = None
+        results = self._get_all_details(self.cache_table, cols, start=start, limit=limit,
+                                        exclude_token=all_tokens_to_exclude,
                                         allow_nulls=allow_nulls, earliest_date=earliest_date, latest_date=latest_date,
                                         equality_conditions=equality_conditions, has_date_col=True,
                                         sort_by_date_col=do_date_sort, use_date_modified_col=use_date_modified_col)
         return results
 
     def get_cache_count(self, non_null_cols=None, equality_conditions=None):
         """
```

### Comparing `db_cache_manager-0.1.0/src/db_cache_manager.egg-info/PKG-INFO` & `db_cache_manager-0.1.1/src/db_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.0/tests/test_cache_manager.py` & `db_cache_manager-0.1.1/tests/test_cache_manager.py`

 * *Files identical despite different names*

