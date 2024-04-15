# Comparing `tmp/aero-svo-api-0.1.2.tar.gz` & `tmp/aero_svo_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aero-svo-api-0.1.2.tar", last modified: Fri Apr 12 14:29:32 2024, max compression
+gzip compressed data, was "aero_svo_api-0.1.3.tar", last modified: Mon Apr 15 10:58:10 2024, max compression
```

## Comparing `aero-svo-api-0.1.2.tar` & `aero_svo_api-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.259559 aero-svo-api-0.1.2/
--rw-rw-rw-   0        0        0     1092 2023-12-19 10:48:38.000000 aero-svo-api-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2734 2024-04-12 14:29:32.257565 aero-svo-api-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/README.md
--rw-rw-rw-   0        0        0      949 2024-03-13 09:24:18.000000 aero-svo-api-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       33 2024-03-29 11:09:09.000000 aero-svo-api-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 14:29:32.259559 aero-svo-api-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.213559 aero-svo-api-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.231559 aero-svo-api-0.1.2/src/aero_svo_api/
--rw-rw-rw-   0        0        0       81 2024-04-12 14:13:15.000000 aero-svo-api-0.1.2/src/aero_svo_api/__init__.py
--rw-rw-rw-   0        0        0     2719 2024-03-13 09:00:37.000000 aero-svo-api-0.1.2/src/aero_svo_api/api.py
--rw-rw-rw-   0        0        0     5150 2024-04-12 14:05:36.000000 aero-svo-api-0.1.2/src/aero_svo_api/models.py
--rw-rw-rw-   0        0        0      372 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/src/aero_svo_api/urls.py
--rw-rw-rw-   0        0        0      143 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/src/aero_svo_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.256559 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/
--rw-rw-rw-   0        0        0     2734 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.253559 aero-svo-api-0.1.2/tests/
--rw-rw-rw-   0        0        0     3211 2024-03-13 09:00:37.000000 aero-svo-api-0.1.2/tests/test_api.py
--rw-rw-rw-   0        0        0     1079 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/tests/test_models.py
--rw-rw-rw-   0        0        0      370 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:58:10.174759 aero_svo_api-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2023-12-19 10:48:38.000000 aero_svo_api-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2734 2024-04-15 10:58:10.172760 aero_svo_api-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-03-13 08:31:50.000000 aero_svo_api-0.1.3/README.md
+-rw-rw-rw-   0        0        0      949 2024-03-13 09:24:18.000000 aero_svo_api-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       33 2024-03-29 11:09:09.000000 aero_svo_api-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:58:10.174759 aero_svo_api-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 10:58:10.098162 aero_svo_api-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:58:10.127174 aero_svo_api-0.1.3/src/aero_svo_api/
+-rw-rw-rw-   0        0        0       81 2024-04-15 10:52:17.000000 aero_svo_api-0.1.3/src/aero_svo_api/__init__.py
+-rw-rw-rw-   0        0        0     2719 2024-03-13 09:00:37.000000 aero_svo_api-0.1.3/src/aero_svo_api/api.py
+-rw-rw-rw-   0        0        0     5173 2024-04-15 10:44:35.000000 aero_svo_api-0.1.3/src/aero_svo_api/models.py
+-rw-rw-rw-   0        0        0      372 2024-03-13 08:31:50.000000 aero_svo_api-0.1.3/src/aero_svo_api/urls.py
+-rw-rw-rw-   0        0        0      143 2024-03-13 08:31:50.000000 aero_svo_api-0.1.3/src/aero_svo_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:58:10.170771 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/
+-rw-rw-rw-   0        0        0     2734 2024-04-15 10:58:10.000000 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-15 10:58:10.000000 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:58:10.000000 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-15 10:58:10.000000 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 10:58:10.000000 aero_svo_api-0.1.3/src/aero_svo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 10:58:10.168770 aero_svo_api-0.1.3/tests/
+-rw-rw-rw-   0        0        0     3211 2024-03-13 09:00:37.000000 aero_svo_api-0.1.3/tests/test_api.py
+-rw-rw-rw-   0        0        0     2089 2024-04-15 10:44:35.000000 aero_svo_api-0.1.3/tests/test_models.py
+-rw-rw-rw-   0        0        0      370 2024-03-13 08:31:50.000000 aero_svo_api-0.1.3/tests/test_utils.py
```

### Comparing `aero-svo-api-0.1.2/LICENSE` & `aero_svo_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.2/PKG-INFO` & `aero_svo_api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aero-svo-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unoficial api wrapper for Sheremetyevo International Airport
 Author-email: Nikita Bulavinov <jktujgxtu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nikita Bulavinov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aero-svo-api-0.1.2/README.md` & `aero_svo_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.2/pyproject.toml` & `aero_svo_api-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.2/src/aero_svo_api/api.py` & `aero_svo_api-0.1.3/src/aero_svo_api/api.py`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.2/src/aero_svo_api/models.py` & `aero_svo_api-0.1.3/src/aero_svo_api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     chin_id: str | None = None
     chin_start: datetime | None = Field(None, alias='t_chin_start')
     chin_end: datetime | None = Field(None, alias='t_chin_finish')
     chin_start_et: datetime | None = Field(None, alias='estimated_chin_start')
     chin_end_et: datetime | None = Field(None, alias='estimated_chin_finish')
     # boarding
     boarding_start: datetime | None = Field(None, alias='t_boarding_start')
-    boarding_end: datetime | None = Field(None, alias='t_boarding_finish')
+    boarding_end: datetime | None = Field(None, alias='t_bording_finish')           # typo in api
     gate_id: str | None = None
     gate_id_prev: str | None = Field(None, alias='old_gate_id')
     # terminal
     term_local: str | None = Field(None, alias='term')
     term_local_prev: str | None = Field(None, alias='old_term')
     # bag belt
     bbel_id: str | None = None
```

### Comparing `aero-svo-api-0.1.2/src/aero_svo_api.egg-info/PKG-INFO` & `aero_svo_api-0.1.3/src/aero_svo_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aero-svo-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unoficial api wrapper for Sheremetyevo International Airport
 Author-email: Nikita Bulavinov <jktujgxtu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nikita Bulavinov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aero-svo-api-0.1.2/tests/test_api.py` & `aero_svo_api-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

