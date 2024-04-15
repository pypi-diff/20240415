# Comparing `tmp/pih-plb_db-0.15.tar.gz` & `tmp/pih-plb_db-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.15.tar", last modified: Wed Apr 10 02:14:51 2024, max compression
+gzip compressed data, was "pih-plb_db-0.16.tar", last modified: Mon Apr 15 00:55:24 2024, max compression
```

## Comparing `pih-plb_db-0.15.tar` & `pih-plb_db-0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.499494 pih-plb_db-0.15/
--rw-rw-rw-   0        0        0      276 2024-04-10 02:14:51.451561 pih-plb_db-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.076582 pih-plb_db-0.15/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.15/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.15/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0     6528 2024-03-30 01:06:51.000000 pih-plb_db-0.15/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0      564 2024-04-10 00:38:15.000000 pih-plb_db-0.15/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1146 2024-04-10 00:35:00.000000 pih-plb_db-0.15/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.404686 pih-plb_db-0.15/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      276 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:14:51.499494 pih-plb_db-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 00:55:25.027242 pih-plb_db-0.16/
+-rw-rw-rw-   0        0        0      280 2024-04-15 00:55:24.994954 pih-plb_db-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 00:55:24.551223 pih-plb_db-0.16/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.16/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.16/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0     6528 2024-03-30 01:06:51.000000 pih-plb_db-0.16/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0      568 2024-04-15 00:44:28.000000 pih-plb_db-0.16/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1146 2024-04-10 00:35:00.000000 pih-plb_db-0.16/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:55:24.948083 pih-plb_db-0.16/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-04-15 00:55:23.000000 pih-plb_db-0.16/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:55:25.027242 pih-plb_db-0.16/setup.cfg
```

### Comparing `pih-plb_db-0.15/PolibaseDatabaseService/api.py` & `pih-plb_db-0.16/PolibaseDatabaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb_db-0.15/PolibaseDatabaseService/const.py` & `pih-plb_db-0.16/PolibaseDatabaseService/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = Hosts.POLIBASE
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
-    description="Polibase database api",
+    description="Polibase database service",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
     run_from_system_account=True,
     python_executable_path=CONST.UNKNOWN,
 )
```

### Comparing `pih-plb_db-0.15/PolibaseDatabaseService/service.py` & `pih-plb_db-0.16/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

