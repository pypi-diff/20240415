# Comparing `tmp/resolutecns-0.0.3.tar.gz` & `tmp/resolutecns-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.3.tar", last modified: Mon Apr 15 16:53:55 2024, max compression
+gzip compressed data, was "resolutecns-0.0.4.tar", last modified: Mon Apr 15 17:00:35 2024, max compression
```

## Comparing `resolutecns-0.0.3.tar` & `resolutecns-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:53:55.808126 resolutecns-0.0.3/
--rw-rw-rw-   0        0        0      505 2024-04-15 16:53:55.804121 resolutecns-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 16:53:55.779390 resolutecns-0.0.3/ResoluteCNS/
--rw-rw-rw-   0        0        0     3164 2024-04-15 16:37:48.000000 resolutecns-0.0.3/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       27 2024-04-15 16:52:12.000000 resolutecns-0.0.3/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:53:55.799148 resolutecns-0.0.3/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      505 2024-04-15 16:53:55.000000 resolutecns-0.0.3/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-04-15 16:53:55.000000 resolutecns-0.0.3/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:53:55.000000 resolutecns-0.0.3/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 16:53:55.000000 resolutecns-0.0.3/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 16:53:55.809122 resolutecns-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-15 16:53:40.000000 resolutecns-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.333739 resolutecns-0.0.4/
+-rw-rw-rw-   0        0        0      505 2024-04-15 17:00:35.327720 resolutecns-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.301718 resolutecns-0.0.4/ResoluteCNS/
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.4/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.322722 resolutecns-0.0.4/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      505 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:00:35.333739 resolutecns-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-04-15 17:00:32.000000 resolutecns-0.0.4/setup.py
```

### Comparing `resolutecns-0.0.3/setup.py` & `resolutecns-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

