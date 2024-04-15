# Comparing `tmp/elgas-24.1.0b2.tar.gz` & `tmp/elgas-24.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elgas-24.1.0b2.tar", last modified: Sun Apr 14 11:41:27 2024, max compression
+gzip compressed data, was "elgas-24.1.0b3.tar", last modified: Sun Apr 14 19:13:21 2024, max compression
```

## Comparing `elgas-24.1.0b2.tar` & `elgas-24.1.0b3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.124174 elgas-24.1.0b2/
--rw-r--r--   0 henrik     (501) staff       (20)     5243 2024-02-25 12:45:21.000000 elgas-24.1.0b2/LICENSE
--rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 11:41:27.124035 elgas-24.1.0b2/PKG-INFO
--rw-r--r--   0 henrik     (501) staff       (20)      685 2024-02-16 14:03:48.000000 elgas-24.1.0b2/README.md
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.118196 elgas-24.1.0b2/elgas/
--rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/__init__.py
--rw-r--r--   0 henrik     (501) staff       (20)    12129 2024-04-14 11:33:30.000000 elgas-24.1.0b2/elgas/application.py
--rw-r--r--   0 henrik     (501) staff       (20)     4809 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/client.py
--rw-r--r--   0 henrik     (501) staff       (20)     6889 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/connection.py
--rw-r--r--   0 henrik     (501) staff       (20)      749 2024-02-25 12:45:21.000000 elgas-24.1.0b2/elgas/constants.py
--rw-r--r--   0 henrik     (501) staff       (20)      878 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/exceptions.py
--rw-r--r--   0 henrik     (501) staff       (20)     7133 2024-02-25 12:45:21.000000 elgas-24.1.0b2/elgas/frames.py
--rw-r--r--   0 henrik     (501) staff       (20)     1023 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/integration.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.122397 elgas-24.1.0b2/elgas/parameters/
--rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/__init__.py
--rw-r--r--   0 henrik     (501) staff       (20)     6219 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/analog_quantity.py
--rw-r--r--   0 henrik     (501) staff       (20)     4376 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/binary.py
--rw-r--r--   0 henrik     (501) staff       (20)     4341 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/compressibility.py
--rw-r--r--   0 henrik     (501) staff       (20)     5043 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/conversion_coefficient.py
--rw-r--r--   0 henrik     (501) staff       (20)     6144 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     3718 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/device_error.py
--rw-r--r--   0 henrik     (501) staff       (20)     4778 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/diagnostics.py
--rw-r--r--   0 henrik     (501) staff       (20)     4782 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/difference_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     4896 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/energy.py
--rw-r--r--   0 henrik     (501) staff       (20)     1391 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/enumerations.py
--rw-r--r--   0 henrik     (501) staff       (20)     5100 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/error_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     4177 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/error_standard_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     7558 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/factory.py
--rw-r--r--   0 henrik     (501) staff       (20)     8143 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/flow_rate.py
--rw-r--r--   0 henrik     (501) staff       (20)     3792 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/gas_composition.py
--rw-r--r--   0 henrik     (501) staff       (20)     5027 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/modem.py
--rw-r--r--   0 henrik     (501) staff       (20)     3949 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/setpoint.py
--rw-r--r--   0 henrik     (501) staff       (20)     4495 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/standard_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     9441 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/statistics.py
--rw-r--r--   0 henrik     (501) staff       (20)     3716 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/sum_of_alarms.py
--rw-r--r--   0 henrik     (501) staff       (20)    15165 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/system_parameters.py
--rw-r--r--   0 henrik     (501) staff       (20)     9128 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/tariff_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     3630 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/time_window.py
--rw-r--r--   0 henrik     (501) staff       (20)     3159 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/timer.py
--rw-r--r--   0 henrik     (501) staff       (20)     1144 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parser.py
--rw-r--r--   0 henrik     (501) staff       (20)     3375 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/security.py
--rw-r--r--   0 henrik     (501) staff       (20)     3003 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/state.py
--rw-r--r--   0 henrik     (501) staff       (20)     8412 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/transport.py
--rw-r--r--   0 henrik     (501) staff       (20)     7307 2024-02-25 10:06:46.000000 elgas-24.1.0b2/elgas/utils.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.119044 elgas-24.1.0b2/elgas.egg-info/
--rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/PKG-INFO
--rw-r--r--   0 henrik     (501) staff       (20)     1457 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/SOURCES.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/dependency_links.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2024-02-16 14:09:11.000000 elgas-24.1.0b2/elgas.egg-info/not-zip-safe
--rw-r--r--   0 henrik     (501) staff       (20)      127 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/requires.txt
--rw-r--r--   0 henrik     (501) staff       (20)        6 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/top_level.txt
--rw-r--r--   0 henrik     (501) staff       (20)      324 2024-02-16 14:03:48.000000 elgas-24.1.0b2/pyproject.toml
--rw-r--r--   0 henrik     (501) staff       (20)       38 2024-04-14 11:41:27.124217 elgas-24.1.0b2/setup.cfg
--rw-r--r--   0 henrik     (501) staff       (20)     3324 2024-04-14 11:40:40.000000 elgas-24.1.0b2/setup.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.123803 elgas-24.1.0b2/tests/
--rw-r--r--   0 henrik     (501) staff       (20)     9252 2024-04-14 11:38:33.000000 elgas-24.1.0b2/tests/test_application.py
--rw-r--r--   0 henrik     (501) staff       (20)     5428 2024-02-25 12:45:21.000000 elgas-24.1.0b2/tests/test_call_to_dispatch.py
--rw-r--r--   0 henrik     (501) staff       (20)     2849 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_frames.py
--rw-r--r--   0 henrik     (501) staff       (20)    12259 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_parameters.py
--rw-r--r--   0 henrik     (501) staff       (20)    13302 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_parser.py
--rw-r--r--   0 henrik     (501) staff       (20)    24777 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_schema.py
--rw-r--r--   0 henrik     (501) staff       (20)     3659 2024-02-25 12:49:03.000000 elgas-24.1.0b2/tests/test_security.py
--rw-r--r--   0 henrik     (501) staff       (20)     4436 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_utils.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 19:13:21.717298 elgas-24.1.0b3/
+-rw-r--r--   0 henrik     (501) staff       (20)     5243 2024-02-25 12:45:21.000000 elgas-24.1.0b3/LICENSE
+-rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 19:13:21.717157 elgas-24.1.0b3/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)      685 2024-02-16 14:03:48.000000 elgas-24.1.0b3/README.md
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 19:13:21.710832 elgas-24.1.0b3/elgas/
+-rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)    12129 2024-04-14 11:33:30.000000 elgas-24.1.0b3/elgas/application.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4846 2024-04-14 19:11:38.000000 elgas-24.1.0b3/elgas/client.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6889 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/connection.py
+-rw-r--r--   0 henrik     (501) staff       (20)      749 2024-02-25 12:45:21.000000 elgas-24.1.0b3/elgas/constants.py
+-rw-r--r--   0 henrik     (501) staff       (20)      878 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/exceptions.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7133 2024-02-25 12:45:21.000000 elgas-24.1.0b3/elgas/frames.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1023 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/integration.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 19:13:21.715400 elgas-24.1.0b3/elgas/parameters/
+-rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6219 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/analog_quantity.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4376 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/binary.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4341 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/compressibility.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5043 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/conversion_coefficient.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6144 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3718 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/device_error.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4778 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/diagnostics.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4782 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/difference_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4896 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/energy.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1391 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/enumerations.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5100 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/error_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4177 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/error_standard_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7558 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/factory.py
+-rw-r--r--   0 henrik     (501) staff       (20)     8143 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/flow_rate.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3792 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/gas_composition.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5027 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/modem.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3949 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/setpoint.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4495 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/standard_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     9441 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/statistics.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3716 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/sum_of_alarms.py
+-rw-r--r--   0 henrik     (501) staff       (20)    15165 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/system_parameters.py
+-rw-r--r--   0 henrik     (501) staff       (20)     9128 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/tariff_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3630 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/time_window.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3159 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parameters/timer.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1144 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/parser.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3375 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/security.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3003 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/state.py
+-rw-r--r--   0 henrik     (501) staff       (20)     8412 2024-02-16 14:03:48.000000 elgas-24.1.0b3/elgas/transport.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7307 2024-02-25 10:06:46.000000 elgas-24.1.0b3/elgas/utils.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 19:13:21.711720 elgas-24.1.0b3/elgas.egg-info/
+-rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 19:13:21.000000 elgas-24.1.0b3/elgas.egg-info/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)     1457 2024-04-14 19:13:21.000000 elgas-24.1.0b3/elgas.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2024-04-14 19:13:21.000000 elgas-24.1.0b3/elgas.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2024-02-16 14:09:11.000000 elgas-24.1.0b3/elgas.egg-info/not-zip-safe
+-rw-r--r--   0 henrik     (501) staff       (20)      127 2024-04-14 19:13:21.000000 elgas-24.1.0b3/elgas.egg-info/requires.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        6 2024-04-14 19:13:21.000000 elgas-24.1.0b3/elgas.egg-info/top_level.txt
+-rw-r--r--   0 henrik     (501) staff       (20)      324 2024-02-16 14:03:48.000000 elgas-24.1.0b3/pyproject.toml
+-rw-r--r--   0 henrik     (501) staff       (20)       38 2024-04-14 19:13:21.717336 elgas-24.1.0b3/setup.cfg
+-rw-r--r--   0 henrik     (501) staff       (20)     3324 2024-04-14 19:13:11.000000 elgas-24.1.0b3/setup.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 19:13:21.716967 elgas-24.1.0b3/tests/
+-rw-r--r--   0 henrik     (501) staff       (20)     9252 2024-04-14 11:38:33.000000 elgas-24.1.0b3/tests/test_application.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5428 2024-02-25 12:45:21.000000 elgas-24.1.0b3/tests/test_call_to_dispatch.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2849 2024-02-16 14:03:48.000000 elgas-24.1.0b3/tests/test_frames.py
+-rw-r--r--   0 henrik     (501) staff       (20)    12259 2024-02-16 14:03:48.000000 elgas-24.1.0b3/tests/test_parameters.py
+-rw-r--r--   0 henrik     (501) staff       (20)    13302 2024-02-16 14:03:48.000000 elgas-24.1.0b3/tests/test_parser.py
+-rw-r--r--   0 henrik     (501) staff       (20)    24777 2024-02-16 14:03:48.000000 elgas-24.1.0b3/tests/test_schema.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3659 2024-02-25 12:49:03.000000 elgas-24.1.0b3/tests/test_security.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4436 2024-02-16 14:03:48.000000 elgas-24.1.0b3/tests/test_utils.py
```

### Comparing `elgas-24.1.0b2/LICENSE` & `elgas-24.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/PKG-INFO` & `elgas-24.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgas
-Version: 24.1.0b2
+Version: 24.1.0b3
 Summary: A Python library for the ELGAS protocol
 Home-page: https://github.com/u9n/elgas
 Author: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Author-email: henrik.wahlgren@utilitarian.io
 Maintainer: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Maintainer-email: henrik.wahlgren@utilitarian.io
 Project-URL: Bug Tracker, https://github.com/u9n/elgas/issues
```

### Comparing `elgas-24.1.0b2/README.md` & `elgas-24.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/application.py` & `elgas-24.1.0b3/elgas/application.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/client.py` & `elgas-24.1.0b3/elgas/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,18 @@
         LOG.info("Reading device time")
         request = application.ReadTimeRequest()
         self.send(request)
         response: application.ReadTimeResponse = self.next_event()
         LOG.info("Got device time", time=response.time.isoformat())
         return response.time
 
-    def write_time(self, device_time: datetime):
+    def write_time(self, device_time: datetime, cryout: bool = False):
         LOG.info("Writing time to device", time=device_time.isoformat())
         request = application.WriteTimeRequest(
-            password=self.password, device_time=device_time
+            password=self.password, device_time=device_time, cryout=cryout
         )
         self.send(request)
         self.next_event()
         LOG.info("Finished writing time to device")
 
     def read_parameters(self, read_from: int = 0) -> List[Any]:
         LOG.info(f"Reading device parameters", read_from=read_from)
```

### Comparing `elgas-24.1.0b2/elgas/connection.py` & `elgas-24.1.0b3/elgas/connection.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/constants.py` & `elgas-24.1.0b3/elgas/constants.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/exceptions.py` & `elgas-24.1.0b3/elgas/exceptions.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/frames.py` & `elgas-24.1.0b3/elgas/frames.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/integration.py` & `elgas-24.1.0b3/elgas/integration.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/analog_quantity.py` & `elgas-24.1.0b3/elgas/parameters/analog_quantity.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/binary.py` & `elgas-24.1.0b3/elgas/parameters/binary.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/compressibility.py` & `elgas-24.1.0b3/elgas/parameters/compressibility.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/conversion_coefficient.py` & `elgas-24.1.0b3/elgas/parameters/conversion_coefficient.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/counter.py` & `elgas-24.1.0b3/elgas/parameters/counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/device_error.py` & `elgas-24.1.0b3/elgas/parameters/device_error.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/diagnostics.py` & `elgas-24.1.0b3/elgas/parameters/diagnostics.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/difference_counter.py` & `elgas-24.1.0b3/elgas/parameters/difference_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/energy.py` & `elgas-24.1.0b3/elgas/parameters/energy.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/enumerations.py` & `elgas-24.1.0b3/elgas/parameters/enumerations.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/error_counter.py` & `elgas-24.1.0b3/elgas/parameters/error_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/error_standard_counter.py` & `elgas-24.1.0b3/elgas/parameters/error_standard_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/factory.py` & `elgas-24.1.0b3/elgas/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/flow_rate.py` & `elgas-24.1.0b3/elgas/parameters/flow_rate.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/gas_composition.py` & `elgas-24.1.0b3/elgas/parameters/gas_composition.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/modem.py` & `elgas-24.1.0b3/elgas/parameters/modem.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/setpoint.py` & `elgas-24.1.0b3/elgas/parameters/setpoint.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/standard_counter.py` & `elgas-24.1.0b3/elgas/parameters/standard_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/statistics.py` & `elgas-24.1.0b3/elgas/parameters/statistics.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/sum_of_alarms.py` & `elgas-24.1.0b3/elgas/parameters/sum_of_alarms.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/system_parameters.py` & `elgas-24.1.0b3/elgas/parameters/system_parameters.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/tariff_counter.py` & `elgas-24.1.0b3/elgas/parameters/tariff_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/time_window.py` & `elgas-24.1.0b3/elgas/parameters/time_window.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parameters/timer.py` & `elgas-24.1.0b3/elgas/parameters/timer.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/parser.py` & `elgas-24.1.0b3/elgas/parser.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/security.py` & `elgas-24.1.0b3/elgas/security.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/state.py` & `elgas-24.1.0b3/elgas/state.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/transport.py` & `elgas-24.1.0b3/elgas/transport.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas/utils.py` & `elgas-24.1.0b3/elgas/utils.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/elgas.egg-info/PKG-INFO` & `elgas-24.1.0b3/elgas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgas
-Version: 24.1.0b2
+Version: 24.1.0b3
 Summary: A Python library for the ELGAS protocol
 Home-page: https://github.com/u9n/elgas
 Author: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Author-email: henrik.wahlgren@utilitarian.io
 Maintainer: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Maintainer-email: henrik.wahlgren@utilitarian.io
 Project-URL: Bug Tracker, https://github.com/u9n/elgas/issues
```

### Comparing `elgas-24.1.0b2/elgas.egg-info/SOURCES.txt` & `elgas-24.1.0b3/elgas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/setup.py` & `elgas-24.1.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 PROJECT_URLS = {
     "Bug Tracker": "https://github.com/u9n/elgas/issues",
     "Source Code": "https://github.com/u9n/elgas",
 }
 EMAIL = "henrik.wahlgren@utilitarian.io"
 AUTHOR = "Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB"
 REQUIRES_PYTHON = "~=3.7"
-VERSION = "24.1.0b2"
+VERSION = "24.1.0b3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "attrs>=21.4.0",
     "cryptography==42.0.5",
     "marshmallow>=3.14.1",
     "structlog>=21.5.0",
```

### Comparing `elgas-24.1.0b2/tests/test_application.py` & `elgas-24.1.0b3/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_call_to_dispatch.py` & `elgas-24.1.0b3/tests/test_call_to_dispatch.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_frames.py` & `elgas-24.1.0b3/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_parameters.py` & `elgas-24.1.0b3/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_parser.py` & `elgas-24.1.0b3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_schema.py` & `elgas-24.1.0b3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_security.py` & `elgas-24.1.0b3/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b2/tests/test_utils.py` & `elgas-24.1.0b3/tests/test_utils.py`

 * *Files identical despite different names*

