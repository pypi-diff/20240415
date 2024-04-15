# Comparing `tmp/fews-3di-3.4.3.tar.gz` & `tmp/fews_3di-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fews-3di-3.4.3.tar", last modified: Wed Feb 28 01:01:54 2024, max compression
+gzip compressed data, was "fews_3di-3.5.tar", last modified: Mon Apr 15 11:49:54 2024, max compression
```

## Comparing `fews-3di-3.4.3.tar` & `fews_3di-3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.875123 fews-3di-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-02-28 01:01:38.000000 fews-3di-3.4.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-02-28 01:01:38.000000 fews-3di-3.4.3/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-28 01:01:38.000000 fews-3di-3.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-28 01:01:38.000000 fews-3di-3.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-02-28 01:01:54.875123 fews-3di-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-28 01:01:38.000000 fews-3di-3.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.839123 fews-3di-3.4.3/fews_3di/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.843123 fews-3di-3.4.3/fews_3di/output/
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/output/log_files_sim_19655.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/output/log_files_sim_19670.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/output/log_files_sim_19671.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/output/log_files_sim_29442.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28619 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.843123 fews-3di-3.4.3/fews_3di/states/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/states/3di-cold-state-id.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/states/3di-saved-state-id.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.875123 fews-3di-3.4.3/fews_3di/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)   244431 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/evaporation.nc
--rw-r--r--   0 runner    (1001) docker     (127)    19828 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/example_lateral.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/example_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127) 24490957 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/gridadmin.h5
--rw-r--r--   0 runner    (1001) docker     (127)   440252 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/ow.nc
--rw-r--r--   0 runner    (1001) docker     (127)   478893 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/precipitation.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/settings_with_old_username.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/settings_without_api_token.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-02-28 01:01:38.000000 fews-3di-3.4.3/fews_3di/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 01:01:54.875123 fews-3di-3.4.3/fews_3di.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-28 01:01:54.000000 fews-3di-3.4.3/fews_3di.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-28 01:01:38.000000 fews-3di-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 01:01:54.875123 fews-3di-3.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.638219 fews_3di-3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-15 11:49:41.000000 fews_3di-3.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-15 11:49:41.000000 fews_3di-3.5/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-15 11:49:41.000000 fews_3di-3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 11:49:41.000000 fews_3di-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-04-15 11:49:54.638219 fews_3di-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-15 11:49:41.000000 fews_3di-3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.602219 fews_3di-3.5/fews_3di/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.602219 fews_3di-3.5/fews_3di/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/output/log_files_sim_19655.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/output/log_files_sim_19670.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/output/log_files_sim_19671.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/output/log_files_sim_29442.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28619 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.602219 fews_3di-3.5/fews_3di/states/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/states/3di-cold-state-id.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/states/3di-saved-state-id.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.638219 fews_3di-3.5/fews_3di/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   244431 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/evaporation.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    19828 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/example_lateral.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/example_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127) 24490957 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/gridadmin.h5
+-rw-r--r--   0 runner    (1001) docker     (127)   440252 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/ow.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   478893 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/precipitation.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/settings_with_old_username.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/settings_without_api_token.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-04-15 11:49:41.000000 fews_3di-3.5/fews_3di/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:54.638219 fews_3di-3.5/fews_3di.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 11:49:54.000000 fews_3di-3.5/fews_3di.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-15 11:49:41.000000 fews_3di-3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:49:54.638219 fews_3di-3.5/setup.cfg
```

### Comparing `fews-3di-3.4.3/CHANGES.rst` & `fews_3di-3.5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog of fews-3di
 ===================================================
 
 
+3.5 (2024-04-15)
+----------------
+
+- Increased the file processing time for boundary files.
+
+
 3.4.3 (2024-02-28)
 ------------------
 
 - Fixed faulty packaging.
 
 
 3.4.2 (2024-02-27)
```

### Comparing `fews-3di-3.4.3/DEVELOPMENT.rst` & `fews_3di-3.5/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/LICENSE` & `fews_3di-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/PKG-INFO` & `fews_3di-3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fews-3di
-Version: 3.4.3
+Version: 3.5
 Summary: FEWS-3Di coupling
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: The MIT License
         
         Copyright 2018 Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,16 +82,16 @@
       <endDateTime date="2020-01-30" time="12:00:00"/>
       <properties>
           <string key="api_token" value="aBCd1234.5678tOkeNabcde"/>
           <string key="organisation" value="12345678abcd"/>
           <string key="modelrevision" value="abcd123456787"/>
           <string key="simulationname" value="Simulation name"/>
           <string key="save_state" value="True"/>
-          <string key="save_state_time" value="1400" />
           <string key="use_last_available_state" value="False" />
+          <string key="save_state_time" value="1400"/>
           <string key="saved_state_expiry_days" value="5"/>
           <string key="rain_type" value="radar"/>
           <string key="rain_input" value="730d6675-35dd-4a35-aa9b-bfb8155f9ca7"/>
           <string key="rain_radar_multiplier" value="0.8"/>
           <string key="fews_pre_processing" value="True"/>
           <string key="lizard_results_scenario_name" value="Testsimulatie"/>
           <string key="lizard_results_scenario_uuid" value=""/>
@@ -104,25 +104,32 @@
 
 
 
 **Note:** ``saved_state_expiry_days`` used to be spelled as
 ``save_state_expiry_days``, without a "d". The example radar uuid is the Dutch
 rainfall radar (NRR).
 
-**save_state:** To use a warm state provide a text file with id in the
-states folder using the name ``states/3di-saved-state-id.txt``.  A cold state
-is supplied in a similar way with the name: ``states/3di-cold-state-id.txt``.
+**save_state:** This option enables using and saving state files. To use a warm
+state provide a text file with id in the states folder using the name
+``states/3di-saved-state-id.txt``.  A cold state is supplied in a similar way
+with the name: ``states/3di-cold-state-id.txt``. If this option is enabled, after
+the simulation the id of the saved state at is updated in same file
+``states/3di-saved-state-id.txt``.
 
 **use_last_available_state:** To overpass the state management system and
 directly take the last available state in the 3Di database the option:
 ``use_last_available_state`` can be set to True.
 
-**save_state_time:** When saving a state a ``save_state_time`` can be specified.
-This parameter defines the time in the simulation (in seconds) when the state
-should be saved. If left empty the end of the simulation is used.
+**save_state_time:** This parameter defines the time in the simulation
+(in seconds) when the state should be saved. If left empty the end of
+the simulation is used.
+
+**saved_state_expiry_days:** The expiry time can be set to store states
+for a relevant period to enable hindcasting and at the same time prevent
+the usage of too much storage space.
 
 **rain_type:** multipe rain-types can be used in the configuration:
 
 - ``constant``
 
 - ``radar``
```

### Comparing `fews-3di-3.4.3/README.rst` & `fews_3di-3.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,16 @@
       <endDateTime date="2020-01-30" time="12:00:00"/>
       <properties>
           <string key="api_token" value="aBCd1234.5678tOkeNabcde"/>
           <string key="organisation" value="12345678abcd"/>
           <string key="modelrevision" value="abcd123456787"/>
           <string key="simulationname" value="Simulation name"/>
           <string key="save_state" value="True"/>
-          <string key="save_state_time" value="1400" />
           <string key="use_last_available_state" value="False" />
+          <string key="save_state_time" value="1400"/>
           <string key="saved_state_expiry_days" value="5"/>
           <string key="rain_type" value="radar"/>
           <string key="rain_input" value="730d6675-35dd-4a35-aa9b-bfb8155f9ca7"/>
           <string key="rain_radar_multiplier" value="0.8"/>
           <string key="fews_pre_processing" value="True"/>
           <string key="lizard_results_scenario_name" value="Testsimulatie"/>
           <string key="lizard_results_scenario_uuid" value=""/>
@@ -61,25 +61,32 @@
 
 
 
 **Note:** ``saved_state_expiry_days`` used to be spelled as
 ``save_state_expiry_days``, without a "d". The example radar uuid is the Dutch
 rainfall radar (NRR).
 
-**save_state:** To use a warm state provide a text file with id in the
-states folder using the name ``states/3di-saved-state-id.txt``.  A cold state
-is supplied in a similar way with the name: ``states/3di-cold-state-id.txt``.
+**save_state:** This option enables using and saving state files. To use a warm
+state provide a text file with id in the states folder using the name
+``states/3di-saved-state-id.txt``.  A cold state is supplied in a similar way
+with the name: ``states/3di-cold-state-id.txt``. If this option is enabled, after
+the simulation the id of the saved state at is updated in same file
+``states/3di-saved-state-id.txt``.
 
 **use_last_available_state:** To overpass the state management system and
 directly take the last available state in the 3Di database the option:
 ``use_last_available_state`` can be set to True.
 
-**save_state_time:** When saving a state a ``save_state_time`` can be specified.
-This parameter defines the time in the simulation (in seconds) when the state
-should be saved. If left empty the end of the simulation is used.
+**save_state_time:** This parameter defines the time in the simulation
+(in seconds) when the state should be saved. If left empty the end of
+the simulation is used.
+
+**saved_state_expiry_days:** The expiry time can be set to store states
+for a relevant period to enable hindcasting and at the same time prevent
+the usage of too much storage space.
 
 **rain_type:** multipe rain-types can be used in the configuration:
 
 - ``constant``
 
 - ``radar``
```

### Comparing `fews-3di-3.4.3/fews_3di/output/log_files_sim_19655.zip` & `fews_3di-3.5/fews_3di/output/log_files_sim_19655.zip`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/output/log_files_sim_19670.zip` & `fews_3di-3.5/fews_3di/output/log_files_sim_19670.zip`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/output/log_files_sim_19671.zip` & `fews_3di-3.5/fews_3di/output/log_files_sim_19671.zip`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/output/log_files_sim_29442.zip` & `fews_3di-3.5/fews_3di/output/log_files_sim_29442.zip`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/scripts.py` & `fews_3di-3.5/fews_3di/scripts.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/simulation.py` & `fews_3di-3.5/fews_3di/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 OffsetAndValue = namedtuple("OffsetAndValue", ["offset", "value"])
 NULL_VALUE = -999  # nodata value in FEWS
 CHUNK_SIZE = 1024 * 1024  # 1MB
 SAVED_STATE_ID_FILENAME = "3di-saved-state-id.txt"
 COLD_STATE_ID_FILENAME = "3di-cold-state-id.txt"
 SIMULATION_STATUS_CHECK_INTERVAL = 30
-UPLOAD_STATUS_CHECK_INTERVAL = 2
+UPLOAD_STATUS_CHECK_INTERVAL = 5
 USER_AGENT = "fews-3di (https://github.com/nens/fews-3di/)"
 logger = logging.getLogger(__name__)
 
 
 class NotFoundError(Exception):
     pass
```

### Comparing `fews-3di-3.4.3/fews_3di/tests/conftest.py` & `fews_3di-3.5/fews_3di/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/evaporation.nc` & `fews_3di-3.5/fews_3di/tests/evaporation.nc`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/example_lateral.csv` & `fews_3di-3.5/fews_3di/tests/example_lateral.csv`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/example_settings.xml` & `fews_3di-3.5/fews_3di/tests/example_settings.xml`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/gridadmin.h5` & `fews_3di-3.5/fews_3di/tests/gridadmin.h5`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/ow.nc` & `fews_3di-3.5/fews_3di/tests/ow.nc`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/precipitation.nc` & `fews_3di-3.5/fews_3di/tests/precipitation.nc`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/settings_with_old_username.xml` & `fews_3di-3.5/fews_3di/tests/settings_with_old_username.xml`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/settings_without_api_token.xml` & `fews_3di-3.5/fews_3di/tests/settings_without_api_token.xml`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/test_scripts.py` & `fews_3di-3.5/fews_3di/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/test_simulation.py` & `fews_3di-3.5/fews_3di/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/tests/test_utils.py` & `fews_3di-3.5/fews_3di/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di/utils.py` & `fews_3di-3.5/fews_3di/utils.py`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/fews_3di.egg-info/PKG-INFO` & `fews_3di-3.5/fews_3di.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fews-3di
-Version: 3.4.3
+Version: 3.5
 Summary: FEWS-3Di coupling
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: The MIT License
         
         Copyright 2018 Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,16 +82,16 @@
       <endDateTime date="2020-01-30" time="12:00:00"/>
       <properties>
           <string key="api_token" value="aBCd1234.5678tOkeNabcde"/>
           <string key="organisation" value="12345678abcd"/>
           <string key="modelrevision" value="abcd123456787"/>
           <string key="simulationname" value="Simulation name"/>
           <string key="save_state" value="True"/>
-          <string key="save_state_time" value="1400" />
           <string key="use_last_available_state" value="False" />
+          <string key="save_state_time" value="1400"/>
           <string key="saved_state_expiry_days" value="5"/>
           <string key="rain_type" value="radar"/>
           <string key="rain_input" value="730d6675-35dd-4a35-aa9b-bfb8155f9ca7"/>
           <string key="rain_radar_multiplier" value="0.8"/>
           <string key="fews_pre_processing" value="True"/>
           <string key="lizard_results_scenario_name" value="Testsimulatie"/>
           <string key="lizard_results_scenario_uuid" value=""/>
@@ -104,25 +104,32 @@
 
 
 
 **Note:** ``saved_state_expiry_days`` used to be spelled as
 ``save_state_expiry_days``, without a "d". The example radar uuid is the Dutch
 rainfall radar (NRR).
 
-**save_state:** To use a warm state provide a text file with id in the
-states folder using the name ``states/3di-saved-state-id.txt``.  A cold state
-is supplied in a similar way with the name: ``states/3di-cold-state-id.txt``.
+**save_state:** This option enables using and saving state files. To use a warm
+state provide a text file with id in the states folder using the name
+``states/3di-saved-state-id.txt``.  A cold state is supplied in a similar way
+with the name: ``states/3di-cold-state-id.txt``. If this option is enabled, after
+the simulation the id of the saved state at is updated in same file
+``states/3di-saved-state-id.txt``.
 
 **use_last_available_state:** To overpass the state management system and
 directly take the last available state in the 3Di database the option:
 ``use_last_available_state`` can be set to True.
 
-**save_state_time:** When saving a state a ``save_state_time`` can be specified.
-This parameter defines the time in the simulation (in seconds) when the state
-should be saved. If left empty the end of the simulation is used.
+**save_state_time:** This parameter defines the time in the simulation
+(in seconds) when the state should be saved. If left empty the end of
+the simulation is used.
+
+**saved_state_expiry_days:** The expiry time can be set to store states
+for a relevant period to enable hindcasting and at the same time prevent
+the usage of too much storage space.
 
 **rain_type:** multipe rain-types can be used in the configuration:
 
 - ``constant``
 
 - ``radar``
```

### Comparing `fews-3di-3.4.3/fews_3di.egg-info/SOURCES.txt` & `fews_3di-3.5/fews_3di.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fews-3di-3.4.3/pyproject.toml` & `fews_3di-3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=69"]
 
 [project]
 name = "fews-3di"
 requires-python = ">=3.8"
-version = "3.4.3"
+version = "3.5"
 dependencies = [
   "netCDF4",
   "pandas",
   "requests",
   "threedi-api-client >= 4.0.1",
   "threedigrid",
 ]
```

