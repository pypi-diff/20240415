# Comparing `tmp/fdamages-0.0.7.tar.gz` & `tmp/fdamages-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdamages-0.0.7.tar", last modified: Mon Apr 15 08:31:36 2024, max compression
+gzip compressed data, was "fdamages-0.0.8.tar", last modified: Mon Apr 15 08:32:19 2024, max compression
```

## Comparing `fdamages-0.0.7.tar` & `fdamages-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:31:36.303420 fdamages-0.0.7/
--rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      469 2024-04-15 08:31:36.302168 fdamages-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 08:31:36.303420 fdamages-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      850 2024-04-15 08:31:34.000000 fdamages-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:31:36.293792 fdamages-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:31:36.296791 fdamages-0.0.7/src/fdamages/
--rw-rw-rw-   0        0        0       73 2024-04-15 08:31:10.000000 fdamages-0.0.7/src/fdamages/__init__.py
--rw-rw-rw-   0        0        0     4750 2024-04-15 08:30:58.000000 fdamages-0.0.7/src/fdamages/module_fdamage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:31:36.302168 fdamages-0.0.7/src/fdamages.egg-info/
--rw-rw-rw-   0        0        0      469 2024-04-15 08:31:36.000000 fdamages-0.0.7/src/fdamages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-15 08:31:36.000000 fdamages-0.0.7/src/fdamages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:31:36.000000 fdamages-0.0.7/src/fdamages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 08:31:36.000000 fdamages-0.0.7/src/fdamages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 08:31:36.000000 fdamages-0.0.7/src/fdamages.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.989437 fdamages-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-04-15 08:32:19.989437 fdamages-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:32:19.989437 fdamages-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-04-15 08:32:17.000000 fdamages-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.981689 fdamages-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.984689 fdamages-0.0.8/src/fdamages/
+-rw-rw-rw-   0        0        0       88 2024-04-15 08:32:15.000000 fdamages-0.0.8/src/fdamages/__init__.py
+-rw-rw-rw-   0        0        0     4750 2024-04-15 08:30:58.000000 fdamages-0.0.8/src/fdamages/module_fdamage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.988432 fdamages-0.0.8/src/fdamages.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/top_level.txt
```

### Comparing `fdamages-0.0.7/LICENSE` & `fdamages-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fdamages-0.0.7/setup.py` & `fdamages-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 PACKAGE_NAME = "fdamages"
 AUTHOR = "Valerio Luzzi"
 EMAIL = "valerio.luzzi@gecosistema.com"
 GITHUB = f"https://github.com/valluzzi/{PACKAGE_NAME}.git"
 DESCRIPTION = "A fdamage utility for reading damage functions"
 
 setup(
@@ -31,14 +31,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `fdamages-0.0.7/src/fdamages/module_fdamage.py` & `fdamages-0.0.8/src/fdamages/module_fdamage.py`

 * *Files identical despite different names*

