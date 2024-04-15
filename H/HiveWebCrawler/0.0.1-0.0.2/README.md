# Comparing `tmp/hivewebcrawler-0.0.1.tar.gz` & `tmp/hivewebcrawler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivewebcrawler-0.0.1.tar", last modified: Mon Apr 15 10:10:36 2024, max compression
+gzip compressed data, was "hivewebcrawler-0.0.2.tar", last modified: Mon Apr 15 10:52:21 2024, max compression
```

## Comparing `hivewebcrawler-0.0.1.tar` & `hivewebcrawler-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:10:36.236839 hivewebcrawler-0.0.1/
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:10:36.232839 hivewebcrawler-0.0.1/HiveWebCrawler/
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:10:36.236839 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/
--rw-r--r--   0 delta     (1000) delta     (1000)      351 2024-04-15 10:10:36.000000 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)      282 2024-04-15 10:10:36.000000 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/SOURCES.txt
--rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:10:36.000000 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/dependency_links.txt
--rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 10:10:36.000000 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/requires.txt
--rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:10:36.000000 hivewebcrawler-0.0.1/HiveWebCrawler/HiveWebCrawler.egg-info/top_level.txt
--rw-r--r--   0 delta     (1000) delta     (1000)      351 2024-04-15 10:10:36.236839 hivewebcrawler-0.0.1/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)       58 2024-04-15 10:03:56.000000 hivewebcrawler-0.0.1/README.md
--rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-15 10:10:36.236839 hivewebcrawler-0.0.1/setup.cfg
--rw-r--r--   0 delta     (1000) delta     (1000)      534 2024-04-15 10:10:14.000000 hivewebcrawler-0.0.1/setup.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/HiveWebCrawler/
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/
+-rw-r--r--   0 delta     (1000) delta     (1000)      685 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)      282 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/requires.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/top_level.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)      685 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)       58 2024-04-15 10:03:56.000000 hivewebcrawler-0.0.2/README.md
+-rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/setup.cfg
+-rw-r--r--   0 delta     (1000) delta     (1000)     1048 2024-04-15 10:52:12.000000 hivewebcrawler-0.0.2/setup.py
```

