# Comparing `tmp/cmonkey2-1.2.8.tar.gz` & `tmp/cmonkey2-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmonkey2-1.2.8.tar", last modified: Wed Jun 20 18:14:15 2018, max compression
+gzip compressed data, was "dist/cmonkey2-1.2.9.tar", last modified: Wed Jun 20 20:52:43 2018, max compression
```

## Comparing `cmonkey2-1.2.8.tar` & `cmonkey2-1.2.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/
--rw-r--r--   0 weiju     (1000) weiju     (1000)      360 2016-08-08 21:00:46.000000 cmonkey2-1.2.8/README.rst
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/bin/
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)      110 2016-08-08 21:00:46.000000 cmonkey2-1.2.8/bin/cm2view
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)     1716 2017-05-08 22:39:22.000000 cmonkey2-1.2.8/bin/cm2export
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)     1495 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/bin/cmonkey2
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)     2168 2017-05-08 22:39:22.000000 cmonkey2-1.2.8/bin/cm2plot
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1158 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/PKG-INFO
--rw-r--r--   0 weiju     (1000) weiju     (1000)     2717 2018-06-20 18:12:14.000000 cmonkey2-1.2.8/setup.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)       67 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/setup.cfg
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/test/
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1590 2016-08-08 18:18:26.000000 cmonkey2-1.2.8/test/testutil.py
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey2.egg-info/
--rw-r--r--   0 weiju     (1000) weiju     (1000)        8 2018-06-20 18:14:14.000000 cmonkey2-1.2.8/cmonkey2.egg-info/top_level.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1158 2018-06-20 18:14:14.000000 cmonkey2-1.2.8/cmonkey2.egg-info/PKG-INFO
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1126 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey2.egg-info/SOURCES.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2018-05-15 21:39:37.000000 cmonkey2-1.2.8/cmonkey2.egg-info/not-zip-safe
--rw-r--r--   0 weiju     (1000) weiju     (1000)      148 2018-06-20 18:14:14.000000 cmonkey2-1.2.8/cmonkey2.egg-info/requires.txt
--rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2018-06-20 18:14:14.000000 cmonkey2-1.2.8/cmonkey2.egg-info/dependency_links.txt
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey/
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)     6566 2016-05-18 21:10:03.000000 cmonkey2-1.2.8/cmonkey/weederlauncher.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    10591 2016-05-18 21:10:03.000000 cmonkey2-1.2.8/cmonkey/weeder.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     3603 2018-06-20 17:31:24.000000 cmonkey2-1.2.8/cmonkey/debug.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     6144 2018-05-15 21:31:45.000000 cmonkey2-1.2.8/cmonkey/microarray.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    13572 2018-04-04 14:30:43.000000 cmonkey2-1.2.8/cmonkey/organism.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    10026 2016-08-02 18:31:58.000000 cmonkey2-1.2.8/cmonkey/BSCM.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     9929 2018-05-15 21:31:45.000000 cmonkey2-1.2.8/cmonkey/database.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    34045 2018-06-20 17:33:37.000000 cmonkey2-1.2.8/cmonkey/cmonkey_run.py
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey/cmviewer/
--rwxr-xr-x   0 weiju     (1000) weiju     (1000)    42105 2018-06-19 21:49:17.000000 cmonkey2-1.2.8/cmonkey/cmviewer/webapp.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2016-08-08 17:15:54.000000 cmonkey2-1.2.8/cmonkey/cmviewer/__init__.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    13921 2018-05-15 21:31:45.000000 cmonkey2-1.2.8/cmonkey/set_enrichment.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    10112 2018-04-04 14:41:17.000000 cmonkey2-1.2.8/cmonkey/rsat.py
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey/meme/
--rw-r--r--   0 weiju     (1000) weiju     (1000)    10862 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/meme/mast.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)      928 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/meme/util.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    12280 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/meme/meme.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/meme/__init__.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    13490 2018-05-15 21:31:45.000000 cmonkey2-1.2.8/cmonkey/network.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    16517 2016-08-18 21:43:10.000000 cmonkey2-1.2.8/cmonkey/util.py
-drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 18:14:15.000000 cmonkey2-1.2.8/cmonkey/tools/
--rw-r--r--   0 weiju     (1000) weiju     (1000)     2029 2017-03-15 21:50:34.000000 cmonkey2-1.2.8/cmonkey/tools/plot_expressions.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     4882 2017-03-16 18:18:03.000000 cmonkey2-1.2.8/cmonkey/tools/export.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)      256 2016-09-07 16:58:43.000000 cmonkey2-1.2.8/cmonkey/tools/util.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1279 2017-03-15 22:35:48.000000 cmonkey2-1.2.8/cmonkey/tools/plot_motifs.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     4255 2017-03-15 22:23:56.000000 cmonkey2-1.2.8/cmonkey/tools/plot_motif_positions.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2016-09-06 19:46:31.000000 cmonkey2-1.2.8/cmonkey/tools/__init__.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     5374 2016-02-24 18:20:57.000000 cmonkey2-1.2.8/cmonkey/pssm.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    35676 2017-03-15 22:29:17.000000 cmonkey2-1.2.8/cmonkey/membership.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     5590 2017-09-15 17:32:04.000000 cmonkey2-1.2.8/cmonkey/stringdb.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    27295 2018-06-20 17:35:21.000000 cmonkey2-1.2.8/cmonkey/config.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    19101 2016-08-21 20:20:36.000000 cmonkey2-1.2.8/cmonkey/datamatrix.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    22055 2018-06-19 21:49:17.000000 cmonkey2-1.2.8/cmonkey/scoring.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     2244 2016-05-18 21:10:03.000000 cmonkey2-1.2.8/cmonkey/thesaurus.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    10048 2016-11-16 16:57:47.000000 cmonkey2-1.2.8/cmonkey/microbes_online.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     8470 2016-05-18 21:10:03.000000 cmonkey2-1.2.8/cmonkey/seqtools.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    24536 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/meme_suite.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)    25624 2018-06-19 21:50:03.000000 cmonkey2-1.2.8/cmonkey/motif.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)       22 2016-08-08 21:00:46.000000 cmonkey2-1.2.8/cmonkey/__init__.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     2133 2015-06-03 01:34:06.000000 cmonkey2-1.2.8/cmonkey/schedule.py
--rw-r--r--   0 weiju     (1000) weiju     (1000)     1412 2015-06-03 01:34:06.000000 cmonkey2-1.2.8/cmonkey/patches.py
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/
+-rw-r--r--   0 weiju     (1000) weiju     (1000)      360 2016-08-08 21:00:46.000000 cmonkey2-1.2.9/README.rst
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/bin/
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)      110 2016-08-08 21:00:46.000000 cmonkey2-1.2.9/bin/cm2view
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)     1716 2017-05-08 22:39:22.000000 cmonkey2-1.2.9/bin/cm2export
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)     1495 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/bin/cmonkey2
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)     2168 2017-05-08 22:39:22.000000 cmonkey2-1.2.9/bin/cm2plot
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1158 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/PKG-INFO
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     2717 2018-06-20 20:38:01.000000 cmonkey2-1.2.9/setup.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)       67 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/setup.cfg
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/test/
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1590 2016-08-08 18:18:26.000000 cmonkey2-1.2.9/test/testutil.py
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        8 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/top_level.txt
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1158 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/PKG-INFO
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1126 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2018-05-15 21:39:37.000000 cmonkey2-1.2.9/cmonkey2.egg-info/not-zip-safe
+-rw-r--r--   0 weiju     (1000) weiju     (1000)      148 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/requires.txt
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        1 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey2.egg-info/dependency_links.txt
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey/
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)     6566 2016-05-18 21:10:03.000000 cmonkey2-1.2.9/cmonkey/weederlauncher.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    10591 2016-05-18 21:10:03.000000 cmonkey2-1.2.9/cmonkey/weeder.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     3603 2018-06-20 17:31:24.000000 cmonkey2-1.2.9/cmonkey/debug.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     6144 2018-05-15 21:31:45.000000 cmonkey2-1.2.9/cmonkey/microarray.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    13572 2018-04-04 14:30:43.000000 cmonkey2-1.2.9/cmonkey/organism.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    10026 2016-08-02 18:31:58.000000 cmonkey2-1.2.9/cmonkey/BSCM.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     9929 2018-05-15 21:31:45.000000 cmonkey2-1.2.9/cmonkey/database.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    34045 2018-06-20 17:33:37.000000 cmonkey2-1.2.9/cmonkey/cmonkey_run.py
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey/cmviewer/
+-rwxr-xr-x   0 weiju     (1000) weiju     (1000)    42105 2018-06-19 21:49:17.000000 cmonkey2-1.2.9/cmonkey/cmviewer/webapp.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2016-08-08 17:15:54.000000 cmonkey2-1.2.9/cmonkey/cmviewer/__init__.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    13935 2018-06-20 20:46:03.000000 cmonkey2-1.2.9/cmonkey/set_enrichment.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    10112 2018-04-04 14:41:17.000000 cmonkey2-1.2.9/cmonkey/rsat.py
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey/meme/
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    10862 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/meme/mast.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)      928 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/meme/util.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    12280 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/meme/meme.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/meme/__init__.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    13490 2018-05-15 21:31:45.000000 cmonkey2-1.2.9/cmonkey/network.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    16517 2016-08-18 21:43:10.000000 cmonkey2-1.2.9/cmonkey/util.py
+drwxr-xr-x   0 weiju     (1000) weiju     (1000)        0 2018-06-20 20:52:43.000000 cmonkey2-1.2.9/cmonkey/tools/
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     2029 2017-03-15 21:50:34.000000 cmonkey2-1.2.9/cmonkey/tools/plot_expressions.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     4882 2017-03-16 18:18:03.000000 cmonkey2-1.2.9/cmonkey/tools/export.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)      256 2016-09-07 16:58:43.000000 cmonkey2-1.2.9/cmonkey/tools/util.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1279 2017-03-15 22:35:48.000000 cmonkey2-1.2.9/cmonkey/tools/plot_motifs.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     4255 2017-03-15 22:23:56.000000 cmonkey2-1.2.9/cmonkey/tools/plot_motif_positions.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)        0 2016-09-06 19:46:31.000000 cmonkey2-1.2.9/cmonkey/tools/__init__.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     5374 2016-02-24 18:20:57.000000 cmonkey2-1.2.9/cmonkey/pssm.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    35676 2017-03-15 22:29:17.000000 cmonkey2-1.2.9/cmonkey/membership.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     5590 2017-09-15 17:32:04.000000 cmonkey2-1.2.9/cmonkey/stringdb.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    27295 2018-06-20 17:35:21.000000 cmonkey2-1.2.9/cmonkey/config.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    19101 2016-08-21 20:20:36.000000 cmonkey2-1.2.9/cmonkey/datamatrix.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    22055 2018-06-19 21:49:17.000000 cmonkey2-1.2.9/cmonkey/scoring.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     2244 2016-05-18 21:10:03.000000 cmonkey2-1.2.9/cmonkey/thesaurus.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    10048 2016-11-16 16:57:47.000000 cmonkey2-1.2.9/cmonkey/microbes_online.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     8470 2016-05-18 21:10:03.000000 cmonkey2-1.2.9/cmonkey/seqtools.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    24536 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/meme_suite.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)    25624 2018-06-19 21:50:03.000000 cmonkey2-1.2.9/cmonkey/motif.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)       22 2016-08-08 21:00:46.000000 cmonkey2-1.2.9/cmonkey/__init__.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     2133 2015-06-03 01:34:06.000000 cmonkey2-1.2.9/cmonkey/schedule.py
+-rw-r--r--   0 weiju     (1000) weiju     (1000)     1412 2015-06-03 01:34:06.000000 cmonkey2-1.2.9/cmonkey/patches.py
```

### Comparing `cmonkey2-1.2.8/bin/cm2export` & `cmonkey2-1.2.9/bin/cm2export`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/bin/cmonkey2` & `cmonkey2-1.2.9/bin/cmonkey2`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/bin/cm2plot` & `cmonkey2-1.2.9/bin/cm2plot`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/PKG-INFO` & `cmonkey2-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmonkey2
-Version: 1.2.8
+Version: 1.2.9
 Summary: cmonkey2 is an implementation of the cmonkey biclustering method in Python
 Home-page: https://github.com/baliga-lab/cmonkey2
 Author: Baliga Lab, Institute for Systems Biology
 Author-email: wwu@systemsbiology.net
 License: LGPL V3
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `cmonkey2-1.2.8/setup.py` & `cmonkey2-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'cmonkey2'
 PACKAGES = ['cmonkey', 'cmonkey.cmviewer', 'cmonkey.tools', 'cmonkey.meme']
 DESCRIPTION = 'cmonkey2 is an implementation of the cmonkey biclustering method in Python'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/cmonkey2'
 AUTHOR = 'Baliga Lab, Institute for Systems Biology'
-VERSION = '1.2.8'
+VERSION = '1.2.9'
 
 KEYWORDS = ['class', 'cmonkey2']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

### Comparing `cmonkey2-1.2.8/test/testutil.py` & `cmonkey2-1.2.9/test/testutil.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey2.egg-info/PKG-INFO` & `cmonkey2-1.2.9/cmonkey2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmonkey2
-Version: 1.2.8
+Version: 1.2.9
 Summary: cmonkey2 is an implementation of the cmonkey biclustering method in Python
 Home-page: https://github.com/baliga-lab/cmonkey2
 Author: Baliga Lab, Institute for Systems Biology
 Author-email: wwu@systemsbiology.net
 License: LGPL V3
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `cmonkey2-1.2.8/cmonkey2.egg-info/SOURCES.txt` & `cmonkey2-1.2.9/cmonkey2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/weederlauncher.py` & `cmonkey2-1.2.9/cmonkey/weederlauncher.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/weeder.py` & `cmonkey2-1.2.9/cmonkey/weeder.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/debug.py` & `cmonkey2-1.2.9/cmonkey/debug.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/microarray.py` & `cmonkey2-1.2.9/cmonkey/microarray.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/organism.py` & `cmonkey2-1.2.9/cmonkey/organism.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/BSCM.py` & `cmonkey2-1.2.9/cmonkey/BSCM.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/database.py` & `cmonkey2-1.2.9/cmonkey/database.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/cmonkey_run.py` & `cmonkey2-1.2.9/cmonkey/cmonkey_run.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/cmviewer/webapp.py` & `cmonkey2-1.2.9/cmonkey/cmviewer/webapp.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/set_enrichment.py` & `cmonkey2-1.2.9/cmonkey/set_enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
 
 
 class ScoringFunction(scoring.ScoringFunctionBase):
     """Set enrichment scoring function"""
     def __init__(self, function_id, cmrun):
         """Create scoring function instance"""
         scoring.ScoringFunctionBase.__init__(self, function_id, cmrun)
-        self.__set_types = read_set_types(config_params, organism.thesaurus(),
-                                          ratios.row_names)
-        self.run_log = scoring.RunLog(function_id, cmrun.dbsession(), cmrun.config_params)
+        self.__set_types = read_set_types(self.config_params, self.organism.thesaurus(),
+                                          self.ratios.row_names)
+        self.run_log = scoring.RunLog(function_id, cmrun.dbsession(), self.config_params)
 
     def bonferroni_cutoff(self):
         """Bonferroni cutoff value"""
         return 0.05 / float(self.num_clusters())
 
     def do_compute(self, iteration_result, ref_matrix):
         """compute method
```

### Comparing `cmonkey2-1.2.8/cmonkey/rsat.py` & `cmonkey2-1.2.9/cmonkey/rsat.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/meme/mast.py` & `cmonkey2-1.2.9/cmonkey/meme/mast.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/meme/util.py` & `cmonkey2-1.2.9/cmonkey/meme/util.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/meme/meme.py` & `cmonkey2-1.2.9/cmonkey/meme/meme.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/network.py` & `cmonkey2-1.2.9/cmonkey/network.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/util.py` & `cmonkey2-1.2.9/cmonkey/util.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/tools/plot_expressions.py` & `cmonkey2-1.2.9/cmonkey/tools/plot_expressions.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/tools/export.py` & `cmonkey2-1.2.9/cmonkey/tools/export.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/tools/plot_motifs.py` & `cmonkey2-1.2.9/cmonkey/tools/plot_motifs.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/tools/plot_motif_positions.py` & `cmonkey2-1.2.9/cmonkey/tools/plot_motif_positions.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/pssm.py` & `cmonkey2-1.2.9/cmonkey/pssm.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/membership.py` & `cmonkey2-1.2.9/cmonkey/membership.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/stringdb.py` & `cmonkey2-1.2.9/cmonkey/stringdb.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/config.py` & `cmonkey2-1.2.9/cmonkey/config.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/datamatrix.py` & `cmonkey2-1.2.9/cmonkey/datamatrix.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/scoring.py` & `cmonkey2-1.2.9/cmonkey/scoring.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/thesaurus.py` & `cmonkey2-1.2.9/cmonkey/thesaurus.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/microbes_online.py` & `cmonkey2-1.2.9/cmonkey/microbes_online.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/seqtools.py` & `cmonkey2-1.2.9/cmonkey/seqtools.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/meme_suite.py` & `cmonkey2-1.2.9/cmonkey/meme_suite.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/motif.py` & `cmonkey2-1.2.9/cmonkey/motif.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/schedule.py` & `cmonkey2-1.2.9/cmonkey/schedule.py`

 * *Files identical despite different names*

### Comparing `cmonkey2-1.2.8/cmonkey/patches.py` & `cmonkey2-1.2.9/cmonkey/patches.py`

 * *Files identical despite different names*

