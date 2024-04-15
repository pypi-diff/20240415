# Comparing `tmp/ResoluteCNS-0.0.1.tar.gz` & `tmp/ResoluteCNS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ResoluteCNS-0.0.1.tar", last modified: Mon Apr 15 16:35:57 2024, max compression
+gzip compressed data, was "ResoluteCNS-0.0.2.tar", last modified: Mon Apr 15 16:42:45 2024, max compression
```

## Comparing `ResoluteCNS-0.0.1.tar` & `ResoluteCNS-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:35:57.807778 ResoluteCNS-0.0.1/
--rw-rw-rw-   0        0        0      505 2024-04-15 16:35:57.799775 ResoluteCNS-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 16:35:57.790831 ResoluteCNS-0.0.1/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      505 2024-04-15 16:35:57.000000 ResoluteCNS-0.0.1/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2024-04-15 16:35:57.000000 ResoluteCNS-0.0.1/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:35:57.000000 ResoluteCNS-0.0.1/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:35:57.000000 ResoluteCNS-0.0.1/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 16:35:57.808779 ResoluteCNS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-15 16:22:49.000000 ResoluteCNS-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:42:45.403386 ResoluteCNS-0.0.2/
+-rw-rw-rw-   0        0        0      505 2024-04-15 16:42:45.400389 ResoluteCNS-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 16:42:45.396387 ResoluteCNS-0.0.2/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      505 2024-04-15 16:42:45.000000 ResoluteCNS-0.0.2/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2024-04-15 16:42:45.000000 ResoluteCNS-0.0.2/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:42:45.000000 ResoluteCNS-0.0.2/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:42:45.000000 ResoluteCNS-0.0.2/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 16:42:45.404384 ResoluteCNS-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-04-15 16:42:42.000000 ResoluteCNS-0.0.2/setup.py
```

### Comparing `ResoluteCNS-0.0.1/setup.py` & `ResoluteCNS-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

