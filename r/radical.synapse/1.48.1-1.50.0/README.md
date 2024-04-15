# Comparing `tmp/radical_synapse-1.48.1.tar.gz` & `tmp/radical_synapse-1.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_synapse-1.48.1.tar", last modified: Mon Apr 15 06:15:24 2024, max compression
+gzip compressed data, was "radical_synapse-1.50.0.tar", last modified: Mon Apr 15 07:51:07 2024, max compression
```

## Comparing `radical_synapse-1.48.1.tar` & `radical_synapse-1.50.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3853 2024-03-24 08:01:52.000000 radical_synapse-1.48.1/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      201 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1320 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7560 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 06:15:22.000000 radical_synapse-1.48.1/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.395441 radical_synapse-1.48.1/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1455 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-emulate
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      385 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-execute
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1867 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-fixdocs
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      460 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/bin/radical-synapse-iotrace.sh
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    19306 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-dummy.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7484 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-emulate.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5105 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-master.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7238 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-profile.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     6242 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-worker.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      655 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-profile
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7118 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-sample
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    26673 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-stats
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9501 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/bin/radical-synapse-stats.plot
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)       83 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/bin/radical-synapse-version
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       54 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    12047 2024-04-15 06:15:16.000000 radical_synapse-1.48.1/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.391441 radical_synapse-1.48.1/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.391441 radical_synapse-1.48.1/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.395441 radical_synapse-1.48.1/src/radical/synapse/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       30 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical/synapse/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical/synapse/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      956 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/__init__.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.395441 radical_synapse-1.48.1/src/radical/synapse/atoms/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      517 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4629 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/atoms.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      725 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/atoms.h
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3258 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/base.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1598 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/compute.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      353 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1313 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/memory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2078 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/network.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1897 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/storage.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2737 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_compute.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5855 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_compute_asm.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      136 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_compute_test.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2789 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_memory.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4625 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_network.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5956 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_storage.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2467 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_time.c
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1128 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/atoms/timer.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4436 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/description.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11180 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/synapse.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1740 2023-10-17 06:30:41.000000 radical_synapse-1.48.1/src/radical/synapse/synapsify.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/src/radical/synapse/utils/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      325 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/utils/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    12194 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/utils/misc.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/src/radical/synapse/watcher/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      453 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2555 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_base.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    13465 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_cpu.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2624 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_mem.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2362 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_sto.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2971 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_sys.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/src/radical.synapse.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1320 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1993 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       21 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       37 2024-04-15 06:15:24.000000 radical_synapse-1.48.1/src/radical.synapse.egg-info/top_level.txt
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:15:24.399442 radical_synapse-1.48.1/tests/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      791 2024-03-24 08:01:16.000000 radical_synapse-1.48.1/tests/test_base.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4049 2024-04-15 07:51:00.000000 radical_synapse-1.50.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      201 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/MANIFEST.in
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1320 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     7560 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 07:50:42.000000 radical_synapse-1.50.0/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1455 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-emulate
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      385 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-execute
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1867 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-fixdocs
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      460 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/bin/radical-synapse-iotrace.sh
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)    19306 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-dummy.py
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7484 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-emulate.py
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5105 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-master.py
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7238 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-profile.py
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     6242 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-worker.py
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      655 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-profile
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)     7118 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-sample
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)    26673 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-stats
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     9501 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/bin/radical-synapse-stats.plot
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)       83 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/bin/radical-synapse-version
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       54 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    12047 2024-04-15 07:41:00.000000 radical_synapse-1.50.0/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical/synapse/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       30 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical/synapse/SDIST
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical/synapse/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      956 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/__init__.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical/synapse/atoms/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      517 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4629 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/atoms.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      725 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/atoms.h
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     3258 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/base.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1598 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/compute.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      353 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/constants.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1313 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/memory.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2078 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/network.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1897 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/storage.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2737 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_compute.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     5855 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_compute_asm.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      136 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_compute_test.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2789 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_memory.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4625 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_network.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     5956 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_storage.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2467 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_time.c
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1128 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/atoms/timer.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4436 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/description.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    11180 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/synapse.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1740 2023-10-17 06:30:41.000000 radical_synapse-1.50.0/src/radical/synapse/synapsify.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical/synapse/utils/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      325 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/utils/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    12194 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/utils/misc.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical/synapse/watcher/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      453 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2555 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_base.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    13465 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_cpu.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2624 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_mem.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2362 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_sto.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2971 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_sys.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/src/radical.synapse.egg-info/
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1320 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1993 2024-04-15 07:51:07.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       21 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       37 2024-04-15 07:51:06.000000 radical_synapse-1.50.0/src/radical.synapse.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 07:51:07.017879 radical_synapse-1.50.0/tests/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      791 2024-03-24 08:01:16.000000 radical_synapse-1.50.0/tests/test_base.py
```

### Comparing `radical_synapse-1.48.1/CHANGES.md` & `radical_synapse-1.50.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 
   - For a list of bug fixes, see
     https://github.com/radical-cybertools/radical.synapse/issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
   - For a list of open issues and known problems, see
     https://github.com/radical-cybertools/radical.synapse/issues?q=is%3Aissue+is%3Aopen+
 
 
+1.50.0 Release                                                        2024-04-15
+--------------------------------------------------------------------------------
+
+  - fix for setuptools upgrade
+
+
 1.48.0 Release                                                        2024-03-24
 --------------------------------------------------------------------------------
 
   - convert to py3, update deployment etc.
 
 
 1.47.0 Release                                                        2024-02-08
```

### Comparing `radical_synapse-1.48.1/PKG-INFO` & `radical_synapse-1.50.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.synapse
-Version: 1.48.1
+Version: 1.50.0
 Summary: SYNthetic APplicationS Emulator
 Home-page: http://radical-cybertools.github.io/radical.synapse/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: LGPLv3+
```

### Comparing `radical_synapse-1.48.1/README.md` & `radical_synapse-1.50.0/README.md`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-emulate` & `radical_synapse-1.50.0/bin/radical-synapse-emulate`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-fixdocs` & `radical_synapse-1.50.0/bin/radical-synapse-fixdocs`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-dummy.py` & `radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-dummy.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-emulate.py` & `radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-emulate.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-master.py` & `radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-master.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-profile.py` & `radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-profile.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-mandelbrot-worker.py` & `radical_synapse-1.50.0/bin/radical-synapse-mandelbrot-worker.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-profile` & `radical_synapse-1.50.0/bin/radical-synapse-profile`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-sample` & `radical_synapse-1.50.0/bin/radical-synapse-sample`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-stats` & `radical_synapse-1.50.0/bin/radical-synapse-stats`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/bin/radical-synapse-stats.plot` & `radical_synapse-1.50.0/bin/radical-synapse-stats.plot`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/setup.py` & `radical_synapse-1.50.0/setup.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/__init__.py` & `radical_synapse-1.50.0/src/radical/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/__init__.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/atoms.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/atoms.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/atoms.h` & `radical_synapse-1.50.0/src/radical/synapse/atoms/atoms.h`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/base.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/base.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/compute.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/compute.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/memory.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/memory.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/network.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/network.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/storage.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/storage.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_compute.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_compute.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_compute_asm.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_compute_asm.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_memory.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_memory.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_network.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_network.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_storage.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_storage.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/synapse_time.c` & `radical_synapse-1.50.0/src/radical/synapse/atoms/synapse_time.c`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/atoms/timer.py` & `radical_synapse-1.50.0/src/radical/synapse/atoms/timer.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/description.py` & `radical_synapse-1.50.0/src/radical/synapse/description.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/synapse.py` & `radical_synapse-1.50.0/src/radical/synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/synapsify.py` & `radical_synapse-1.50.0/src/radical/synapse/synapsify.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/utils/misc.py` & `radical_synapse-1.50.0/src/radical/synapse/utils/misc.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_base.py` & `radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_base.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_cpu.py` & `radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_cpu.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_mem.py` & `radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_mem.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_sto.py` & `radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_sto.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical/synapse/watcher/watcher_sys.py` & `radical_synapse-1.50.0/src/radical/synapse/watcher/watcher_sys.py`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/src/radical.synapse.egg-info/PKG-INFO` & `radical_synapse-1.50.0/src/radical.synapse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.synapse
-Version: 1.48.1
+Version: 1.50.0
 Summary: SYNthetic APplicationS Emulator
 Home-page: http://radical-cybertools.github.io/radical.synapse/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: LGPLv3+
```

### Comparing `radical_synapse-1.48.1/src/radical.synapse.egg-info/SOURCES.txt` & `radical_synapse-1.50.0/src/radical.synapse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radical_synapse-1.48.1/tests/test_base.py` & `radical_synapse-1.50.0/tests/test_base.py`

 * *Files identical despite different names*

