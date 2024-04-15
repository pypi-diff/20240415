# Comparing `tmp/ebi_eva_common_pyutils-0.6.5.tar.gz` & `tmp/ebi_eva_common_pyutils-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.6.5.tar", last modified: Tue Apr  2 10:55:50 2024, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.6.6.tar", last modified: Mon Apr 15 15:13:43 2024, max compression
```

## Comparing `ebi_eva_common_pyutils-0.6.5.tar` & `ebi_eva_common_pyutils-0.6.6.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/
--rw-rw-r--   0 april     (1000) april     (1000)     2909 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/CHANGELOG.md
--rw-rw-r--   0 april     (1000) april     (1000)    11357 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/LICENSE
--rw-rw-r--   0 april     (1000) april     (1000)       28 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/MANIFEST.in
--rw-r--r--   0 april     (1000) april     (1000)      817 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/PKG-INFO
--rw-rw-r--   0 april     (1000) april     (1000)     1434 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/README.md
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.216831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/__init__.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/
--rw-rw-r--   0 april     (1000) april     (1000)       67 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     3142 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/assembly.py
--rw-rw-r--   0 april     (1000) april     (1000)     4018 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     2340 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/command_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     1192 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/common_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     4828 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/config.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     3056 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-rw-r--   0 april     (1000) april     (1000)     1465 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ena_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     1375 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/file_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     5093 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/logger.py
--rw-rw-r--   0 april     (1000) april     (1000)     4859 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ncbi_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     2648 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/network_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/
--rw-rw-r--   0 april     (1000) april     (1000)      134 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)    12162 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/assembly.py
--rw-rw-r--   0 april     (1000) april     (1000)     3911 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/sequence.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     2259 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     5230 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 april     (1000) april     (1000)      817 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-rw-r--   0 april     (1000) april     (1000)     1773 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-rw-r--   0 april     (1000) april     (1000)        1 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-rw-r--   0 april     (1000) april     (1000)       97 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-rw-r--   0 april     (1000) april     (1000)       48 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/top_level.txt
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     4989 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/archive_directory.py
--rw-rw-r--   0 april     (1000) april     (1000)     7909 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/config_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)    15090 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/metadata_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     3575 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongo_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/
--rw-rw-r--   0 april     (1000) april     (1000)       76 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     9596 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/mongo_database.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/
--rw-rw-r--   0 april     (1000) april     (1000)      122 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)    10114 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
--rw-rw-r--   0 april     (1000) april     (1000)     4398 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/pg_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)    15265 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/spring_properties.py
--rw-rw-r--   0 april     (1000) april     (1000)      225 2024-04-02 10:55:50.224830 ebi_eva_common_pyutils-0.6.5/setup.cfg
--rw-rw-r--   0 april     (1000) april     (1000)      926 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/setup.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/tests/
--rw-rw-r--   0 april     (1000) april     (1000)      724 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/tests/test_common.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.038334 ebi_eva_common_pyutils-0.6.6/
+-rw-r--r--   0 tcezard    (502) staff       (20)     2993 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/CHANGELOG.md
+-rw-r--r--   0 tcezard    (502) staff       (20)    11357 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/LICENSE
+-rw-r--r--   0 tcezard    (502) staff       (20)       28 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/MANIFEST.in
+-rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-04-15 15:13:43.038497 ebi_eva_common_pyutils-0.6.6/PKG-INFO
+-rw-r--r--   0 tcezard    (502) staff       (20)     1434 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/README.md
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.026939 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/__init__.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.029814 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 tcezard    (502) staff       (20)       67 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3142 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4187 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2340 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1192 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4828 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/config.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.030782 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3056 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1465 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1375 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5093 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5005 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2648 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.032161 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 tcezard    (502) staff       (20)      134 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    12162 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3911 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/sequence.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.032864 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2259 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.033541 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5230 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.029012 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 tcezard    (502) staff       (20)     1653 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)        1 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)       97 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)       48 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.036237 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4989 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/archive_directory.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     7909 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/config_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    15221 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/metadata_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3575 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongo_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.037125 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/
+-rw-r--r--   0 tcezard    (502) staff       (20)       76 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     9596 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/mongo_database.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.037942 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/
+-rw-r--r--   0 tcezard    (502) staff       (20)      122 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    10114 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4398 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/pg_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    15265 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/spring_properties.py
+-rw-r--r--   0 tcezard    (502) staff       (20)      225 2024-04-15 15:13:43.039066 ebi_eva_common_pyutils-0.6.6/setup.cfg
+-rw-r--r--   0 tcezard    (502) staff       (20)      926 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.6.5/CHANGELOG.md` & `ebi_eva_common_pyutils-0.6.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 Changelog for ebi_eva_common_pyutils
 ===========================
 
+## 0.6.6 (2024-04-15)
+---------------------
+
+- Allow NCBI function ot use API key
+
+
 ## 0.6.5 (2024-04-02)
 ---------------------
 
 - Ensure that the port forwarding command is running before returning the process.
 
 
 ## 0.6.4 (2024-03-21)
```

### Comparing `ebi_eva_common_pyutils-0.6.5/LICENSE` & `ebi_eva_common_pyutils-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/README.md` & `ebi_eva_common_pyutils-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,36 +36,40 @@
     xml_root = download_xml_from_ena(f'https://www.ebi.ac.uk/ena/browser/api/xml/{assembly_accession}')
     xml_assembly = xml_root.xpath("//ASSEMBLY_ATTRIBUTE[TAG='count-patches']/VALUE")
     if len(xml_assembly) == 0:
         return False
     return int(xml_assembly[0].text) > 0
 
 
-def retrieve_genbank_assembly_accessions_from_ncbi(assembly_txt):
+def retrieve_genbank_assembly_accessions_from_ncbi(assembly_txt, api_key=None):
     """
     Attempt to find any assembly genebank accession base on a free text search.
     """
     assembly_accessions = set()
     payload = {'db': 'Assembly', 'term': '"{}"'.format(assembly_txt), 'retmode': 'JSON'}
+    if api_key:
+        payload['api_key'] = api_key
     data = requests.get(ESEARCH_URL, params=payload).json()
     if data and data.get('esearchresult', {}).get('idlist'):
         assembly_id_list = data.get('esearchresult').get('idlist')
         payload = {'db': 'Assembly', 'id': ','.join(assembly_id_list), 'retmode': 'JSON'}
+        if api_key:
+            payload['api_key'] = api_key
         summary_list = requests.get(ESUMMARY_URL, params=payload).json()
         for assembly_id in summary_list.get('result', {}).get('uids', []):
             assembly_info = summary_list.get('result').get(assembly_id)
             if 'genbank' in assembly_info['synonym']:
                 assembly_accessions.add(assembly_info['synonym']['genbank'])
     if len(assembly_accessions) != 1:
         logger.warning('%s Genbank synonyms found for assembly %s ', len(assembly_accessions), assembly_txt)
     return list(assembly_accessions)
 
 
-def retrieve_genbank_equivalent_for_GCF_accession(assembly_accession):
-    genbank_synonyms = retrieve_genbank_assembly_accessions_from_ncbi(assembly_accession)
+def retrieve_genbank_equivalent_for_GCF_accession(assembly_accession, ncbi_api_key=None):
+    genbank_synonyms = retrieve_genbank_assembly_accessions_from_ncbi(assembly_accession, api_key=ncbi_api_key)
     if len(genbank_synonyms) != 1:
         raise ValueError('%s Genbank synonyms found for assembly %s ' % (len(genbank_synonyms), assembly_accession))
     return genbank_synonyms.pop()
 
 
 def resolve_assembly_name_to_GCA_accession(assembly_name):
     ENA_ASSEMBLY_NAME_QUERY_URL = "https://www.ebi.ac.uk/ena/portal/api/search" \
```

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,51 +65,53 @@
     req.raise_for_status()
     summary_list = req.json()
     for taxonomy_id in summary_list.get('result', {}).get('uids', []):
         taxonomy_dicts.append(summary_list.get('result').get(taxonomy_id))
     return taxonomy_dicts
 
 
-def get_ncbi_assembly_name_from_term(term):
-    assembl_dicts = get_ncbi_assembly_dicts_from_term(term)
+def get_ncbi_assembly_name_from_term(term, api_key=None):
+    assembl_dicts = get_ncbi_assembly_dicts_from_term(term, api_key=api_key)
     assembly_names = set([d.get('assemblyname') for d in assembl_dicts])
     if len(assembly_names) > 1:
         # Only keep the one that have the assembly accession as a synonymous and check again
         assembly_names = set([d.get('assemblyname') for d in assembl_dicts
                               if term in d['synonym'].values() or term == d['assemblyaccession']])
     if len(assembly_names) != 1:
         raise ValueError(f'Cannot resolve assembly name for assembly {term} in NCBI. '
                          f'Found {",".join([str(a) for a in assembly_names])}')
     return assembly_names.pop() if assembly_names else None
 
 
-def retrieve_species_scientific_name_from_tax_id_ncbi(taxid):
+def retrieve_species_scientific_name_from_tax_id_ncbi(taxid, api_key=None):
     payload = {'db': 'Taxonomy', 'id': taxid}
+    if api_key:
+        payload['api_key'] = api_key
     r = requests.get(efetch_url, params=payload)
     match = re.search('<Rank>(.+?)</Rank>', r.text, re.MULTILINE)
     rank = None
     if match:
         rank = match.group(1)
     if rank not in ['species', 'subspecies']:
         logger.warning('Taxonomy id %s does not point to a species', taxid)
     match = re.search('<ScientificName>(.+?)</ScientificName>', r.text, re.MULTILINE)
     if match:
         return match.group(1)
 
 
-def get_species_name_from_ncbi(assembly_acc):
+def get_species_name_from_ncbi(assembly_acc, api_key=None):
     # We first need to search for the species associated with the assembly
-    assembly_dicts = get_ncbi_assembly_dicts_from_term(assembly_acc)
+    assembly_dicts = get_ncbi_assembly_dicts_from_term(assembly_acc, api_key=api_key)
     taxids = set([assembly_dict.get('taxid')
         for assembly_dict in assembly_dicts
         if assembly_dict.get('assemblyaccession') == assembly_acc or
            assembly_dict.get('synonym', {}).get('genbank') == assembly_acc])
 
     # This is a search so could retrieve multiple results
     if len(taxids) != 1:
         raise ValueError(f'Multiple species found for {assembly_acc}. '
                          f'Cannot resolve single species for assembly {assembly_acc} in NCBI.')
 
     taxonomy_id = taxids.pop()
 
-    scientific_name = retrieve_species_scientific_name_from_tax_id_ncbi(taxonomy_id)
+    scientific_name = retrieve_species_scientific_name_from_tax_id_ncbi(taxonomy_id, api_key=api_key)
     return scientific_name.replace(' ', '_').lower()
```

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-/tmp/ebi_eva_common_pyutils-v0.6.5-999yjogj/gitclone/ebi_eva_internal_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/assembly_utils.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/ena_utils.py
 ebi_eva_common_pyutils/file_utils.py
@@ -37,9 +36,8 @@
 ebi_eva_internal_pyutils/metadata_utils.py
 ebi_eva_internal_pyutils/mongo_utils.py
 ebi_eva_internal_pyutils/pg_utils.py
 ebi_eva_internal_pyutils/spring_properties.py
 ebi_eva_internal_pyutils/mongodb/__init__.py
 ebi_eva_internal_pyutils/mongodb/mongo_database.py
 ebi_eva_internal_pyutils/nextflow/__init__.py
-ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
-tests/test_common.py
+ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
```

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/metadata_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,18 +113,18 @@
     )
 
 
 # For backward compatibility
 get_variant_warehouse_db_name_from_assembly_and_taxonomy = resolve_existing_variant_warehouse_db_name
 
 
-def get_assembly_code(metadata_connection_handle, assembly):
+def get_assembly_code(metadata_connection_handle, assembly, ncbi_api_key=None):
     assembly_code = get_assembly_code_from_metadata(metadata_connection_handle, assembly)
     if not assembly_code:
-        assembly_name = get_ncbi_assembly_name_from_term(assembly)
+        assembly_name = get_ncbi_assembly_name_from_term(assembly, api_key=ncbi_api_key)
         # If the assembly is a patch assembly ex: GRCh37.p8, drop the trailing patch i.e., just return grch37
         if is_patch_assembly(assembly):
             assembly_name = re.sub('\\.p[0-9]+$', '', assembly_name.lower())
         assembly_code = re.sub('[^0-9a-zA-Z]+', '', assembly_name.lower())
     return assembly_code
 
 
@@ -137,44 +137,43 @@
     taxonomy_code = get_taxonomy_code_from_metadata(metadata_connection_handle, taxonomy)
     if not taxonomy_code:
         scientific_name = get_scientific_name_from_ensembl(taxonomy)
         taxonomy_code = build_taxonomy_code(scientific_name)
     return taxonomy_code
 
 
-def resolve_variant_warehouse_db_name(metadata_connection_handle, assembly, taxonomy):
+def resolve_variant_warehouse_db_name(metadata_connection_handle, assembly, taxonomy, ncbi_api_key=None):
     """
     Retrieve the database name for this taxonomy/assembly pair whether it exists or not.
     It will use existing taxonomy code or assembly code if available in the metadata database.
     """
     taxonomy_code = get_taxonomy_code(metadata_connection_handle, taxonomy)
-    assembly_code = get_assembly_code(metadata_connection_handle, assembly)
+    assembly_code = get_assembly_code(metadata_connection_handle, assembly, ncbi_api_key=ncbi_api_key)
     return build_variant_warehouse_database_name(taxonomy_code, assembly_code)
 
 
 def insert_new_assembly_and_taxonomy(metadata_connection_handle, assembly_accession, taxonomy_id, eva_species_name=None,
-                                     in_accessioning=True):
+                                     in_accessioning=True, ncbi_api_key=None):
     """
     This script adds new assemblies and taxonomies to EVAPRO.
     You can also add the assembly with a different taxonomy if you provide the
     taxonomy parameters. Example taxonomy page:
     https://www.ebi.ac.uk/ena/data/view/Taxon:9031
 
     :param assembly_accession: Assembly accession (Example: GCA_000002315.3)
     :param metadata_connection_handle: Metadata DB connection
     :param taxonomy_id: Taxonomy id (Example: 9031)
     :param eva_species_name: EVA species name (Example: chicken).
         Not required if the taxonomy exists or ENA has a common name available.
     :param in_accessioning: Flag that this assembly is in the accessioning data store.
     """
-    assembly_name = get_ncbi_assembly_name_from_term(assembly_accession)
-
     # check if assembly is already in EVAPRO, adding it if not
     assembly_set_id = get_assembly_set_from_metadata(metadata_connection_handle, taxonomy_id, assembly_accession)
     if assembly_set_id is None:
+        assembly_name = get_ncbi_assembly_name_from_term(assembly_accession, api_key=ncbi_api_key)
         ensure_taxonomy_is_in_evapro(metadata_connection_handle, taxonomy_id, eva_species_name)
         assembly_code = get_assembly_code(metadata_connection_handle, assembly_accession)
         insert_assembly_in_evapro(metadata_connection_handle, taxonomy_id, assembly_accession, assembly_name, assembly_code)
 
     update_accessioning_status(metadata_connection_handle, assembly_accession, in_accessioning)
     metadata_connection_handle.commit()
```

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/spring_properties.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.5/setup.py` & `ebi_eva_common_pyutils-0.6.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_internal_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.6.5',
+    version='0.6.6',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['requests', 'lxml', 'pyyaml', 'cached-property', 'retry'],
     extras_require={'eva-internal': ['psycopg2-binary', 'pymongo', 'networkx<=2.5']},
     classifiers=[
```

