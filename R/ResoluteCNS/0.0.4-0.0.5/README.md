# Comparing `tmp/resolutecns-0.0.4.tar.gz` & `tmp/resolutecns-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.4.tar", last modified: Mon Apr 15 17:00:35 2024, max compression
+gzip compressed data, was "resolutecns-0.0.5.tar", last modified: Mon Apr 15 17:12:45 2024, max compression
```

## Comparing `resolutecns-0.0.4.tar` & `resolutecns-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.333739 resolutecns-0.0.4/
--rw-rw-rw-   0        0        0      505 2024-04-15 17:00:35.327720 resolutecns-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.301718 resolutecns-0.0.4/ResoluteCNS/
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.4/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:00:35.322722 resolutecns-0.0.4/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      505 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:00:35.000000 resolutecns-0.0.4/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:00:35.333739 resolutecns-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-15 17:00:32.000000 resolutecns-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.368214 resolutecns-0.0.5/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:12:45.363213 resolutecns-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.336211 resolutecns-0.0.5/ResoluteCNS/
+-rw-rw-rw-   0        0        0     3164 2024-04-15 17:09:41.000000 resolutecns-0.0.5/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.5/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.358215 resolutecns-0.0.5/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:12:45.368214 resolutecns-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-04-15 17:12:17.000000 resolutecns-0.0.5/setup.py
```

### Comparing `resolutecns-0.0.4/setup.py` & `resolutecns-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS", 
         version=VERSION,
         author="Ryan Detlaff",
         author_email="rdetlaff@resolutecommercial.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], # add any additional packages that 
+        install_requires=['selenium', 'pandas'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

