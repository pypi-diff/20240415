# Comparing `tmp/qiskit_alice_bob_provider-0.5.3.tar.gz` & `tmp/qiskit_alice_bob_provider-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.5.3.tar", last modified: Thu Mar 14 13:55:44 2024, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.5.4.tar", last modified: Mon Apr 15 14:53:07 2024, max compression
```

## Comparing `qiskit_alice_bob_provider-0.5.3.tar` & `qiskit_alice_bob_provider-0.5.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.934144 qiskit_alice_bob_provider-0.5.3/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)    11342 2023-09-27 07:33:55.000000 qiskit_alice_bob_provider-0.5.3/LICENSE
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)       91 2023-10-10 15:21:00.000000 qiskit_alice_bob_provider-0.5.3/MANIFEST.in
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     5650 2024-03-14 13:55:44.934144 qiskit_alice_bob_provider-0.5.3/PKG-INFO
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     3577 2024-02-06 15:25:32.000000 qiskit_alice_bob_provider-0.5.3/README.md
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2669 2024-03-14 13:55:28.000000 qiskit_alice_bob_provider-0.5.3/pyproject.toml
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.926144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      867 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2490 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     1039 2023-09-27 07:33:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/errors.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      827 2023-10-10 15:21:00.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     7765 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/backend.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     1905 2024-02-07 15:54:31.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/coupling_maps.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     7453 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/instruction_durations.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2295 2023-10-10 15:21:00.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/job.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/patch/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)        0 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/patch/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     7427 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2694 2023-11-30 11:14:42.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/proc_to_qiskit.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     6679 2024-02-07 15:54:38.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/provider.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)    11750 2024-02-15 14:08:27.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/quantum_errors.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     4375 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/readout_errors.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/resources/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)   257895 2023-10-10 15:21:00.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     4429 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/target.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)        0 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     6613 2024-03-14 13:54:22.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/sk_synthesis.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     9375 2024-02-16 14:04:59.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/state_preparation.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     1226 2023-10-12 08:00:50.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     4840 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/description.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     3112 2023-10-12 08:00:50.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/interpolated_cat.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     8903 2024-02-07 15:54:37.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/logical_cat.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     9624 2024-02-07 15:54:36.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/physical_cat.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     1005 2023-10-12 08:00:50.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     7780 2023-10-12 08:00:50.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/interpolate.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     4002 2023-10-12 08:00:50.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/model.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     7850 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/utils.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      828 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/__init__.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      760 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/__init__.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     3681 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/client.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     4469 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/jobs.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     1286 2023-10-12 08:06:55.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/targets.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     5862 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/backend.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     8063 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/job.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2923 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/provider.py
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     5878 2023-11-30 11:14:45.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
-drwxr-xr-x   0 mdrutel  (10121) mdrutel  (10121)        0 2024-03-14 13:55:44.930144 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     5650 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)     2162 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)        1 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      207 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)      387 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)       26 2024-03-14 13:55:44.000000 qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)       38 2024-03-14 13:55:44.934144 qiskit_alice_bob_provider-0.5.3/setup.cfg
--rw-r--r--   0 mdrutel  (10121) mdrutel  (10121)       69 2023-09-27 07:33:55.000000 qiskit_alice_bob_provider-0.5.3/setup.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.968111 qiskit_alice_bob_provider-0.5.4/
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11342 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/LICENSE
+-rw-r--r--   0 mdrutel    (501) staff       (20)       91 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/MANIFEST.in
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-15 14:53:07.967845 qiskit_alice_bob_provider-0.5.4/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3577 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/README.md
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2669 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/pyproject.toml
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.959881 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      867 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2490 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1039 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962413 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      827 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7765 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1905 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/coupling_maps.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7453 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/instruction_durations.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2295 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/job.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962670 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7427 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2694 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/proc_to_qiskit.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6679 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11750 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/quantum_errors.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/readout_errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962821 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/
+-rw-r--r--   0 mdrutel    (501) staff       (20)   257895 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4429 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/target.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.963534 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6613 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/sk_synthesis.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/state_preparation.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.964320 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1226 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4840 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/description.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3112 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/interpolated_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     8903 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/logical_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9624 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/physical_cat.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.964738 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1005 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7780 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/interpolate.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4002 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/model.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7850 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/utils.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.965572 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      828 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/__init__.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.966187 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      760 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3681 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/client.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4469 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/jobs.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1286 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/targets.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5862 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     8063 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/job.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2923 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6149 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.966379 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2162 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)        1 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      207 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      387 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       26 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       38 2024-04-15 14:53:07.968159 qiskit_alice_bob_provider-0.5.4/setup.cfg
+-rw-r--r--   0 mdrutel    (501) staff       (20)       69 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/setup.py
```

### Comparing `qiskit_alice_bob_provider-0.5.3/LICENSE` & `qiskit_alice_bob_provider-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/PKG-INFO` & `qiskit_alice_bob_provider-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.5.3
+Version: 0.5.4
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.5.3/README.md` & `qiskit_alice_bob_provider-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/pyproject.toml` & `qiskit_alice_bob_provider-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.5.3"
+version = "0.5.4"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/backend.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/coupling_maps.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/coupling_maps.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/instruction_durations.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/instruction_durations.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/job.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/patch/local_noise_pass.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/local_noise_pass.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/proc_to_qiskit.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/proc_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/provider.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/quantum_errors.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/quantum_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/readout_errors.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/readout_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/resources/lescanne_2020.json` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/lescanne_2020.json`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/local/target.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/target.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/sk_synthesis.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/sk_synthesis.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/plugins/state_preparation.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/state_preparation.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/description.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/description.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/interpolated_cat.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/interpolated_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/logical_cat.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/logical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/physical_cat.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/physical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/interpolate.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/interpolate.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/serialization/model.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/model.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/processor/utils.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/__init__.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/client.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/jobs.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/api/targets.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/backend.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/job.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/provider.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider/remote/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/qir_to_qiskit.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     HGate,
     RXGate,
     RYGate,
     RZGate,
     RZZGate,
     SGate,
     SwapGate,
+    TdgGate,
     TGate,
     XGate,
     YGate,
     ZGate,
 )
 from qiskit.extensions.quantum_initializer import Initialize
 from qiskit.transpiler import Target
@@ -124,14 +125,16 @@
         return [('rz', RZGate(phi))]
     elif instr_short_name == 's':
         return [('s', SGate())]
     elif instr_short_name == 'swap':
         return [('swap', SwapGate())]
     elif instr_short_name == 't':
         return [('t', TGate())]
+    elif instr_short_name == 'tdg':
+        return [('tdg', TdgGate())]
     elif instr_short_name == 'x':
         return [('x', XGate())]
     elif instr_short_name == 'y':
         return [('y', YGate())]
     elif instr_short_name == 'z':
         return [('z', ZGate())]
     elif instr_short_name == 'mx':
@@ -162,15 +165,21 @@
     for arg in arguments_str.split(','):
         arguments.append(arg.strip())
     return _QirFunction(
         name=name, return_type=return_type, arguments=arguments
     )
 
 
-_QIS_FUNCTION_PATTERN = r'__quantum__qis__([a-z0-9_]+)__body'
+_QIS_FUNCTION_PATTERN = r'__quantum__qis__([a-z0-9_]+)__(body|adj)'
 
 
 def _parse_function_name(name: str) -> Optional[str]:
     m = re.search(_QIS_FUNCTION_PATTERN, name)
     if m is None:
         return None
-    return m.group(1)
+    call_name = m.group(1)
+
+    # QIR uses the pattern "adj" instead of "body" for the adjoint gates
+    # (such as sdg, tdg).
+    if m.group(2) == 'adj':
+        call_name += 'dg'
+    return call_name
```

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.5.3
+Version: 0.5.4
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.5.3/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

