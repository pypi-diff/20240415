# Comparing `tmp/Mojo2py-1.0.tar.gz` & `tmp/Mojo2py-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mojo2py-1.0.tar", last modified: Mon Apr 15 19:21:06 2024, max compression
+gzip compressed data, was "Mojo2py-1.1.tar", last modified: Mon Apr 15 19:23:52 2024, max compression
```

## Comparing `Mojo2py-1.0.tar` & `Mojo2py-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:21:06.861751 Mojo2py-1.0/
-drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:21:06.860343 Mojo2py-1.0/Mojo2py.egg-info/
--rw-r--r--   0 vishalvenkat   (501) staff       (20)      583 2024-04-15 19:21:06.000000 Mojo2py-1.0/Mojo2py.egg-info/PKG-INFO
--rw-r--r--   0 vishalvenkat   (501) staff       (20)      181 2024-04-15 19:21:06.000000 Mojo2py-1.0/Mojo2py.egg-info/SOURCES.txt
--rw-r--r--   0 vishalvenkat   (501) staff       (20)        1 2024-04-15 19:21:06.000000 Mojo2py-1.0/Mojo2py.egg-info/dependency_links.txt
--rw-r--r--   0 vishalvenkat   (501) staff       (20)        8 2024-04-15 19:21:06.000000 Mojo2py-1.0/Mojo2py.egg-info/top_level.txt
--rw-r--r--   0 vishalvenkat   (501) staff       (20)      583 2024-04-15 19:21:06.861012 Mojo2py-1.0/PKG-INFO
--rw-r--r--   0 vishalvenkat   (501) staff       (20)       80 2024-04-15 18:43:05.000000 Mojo2py-1.0/README.md
-drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:21:06.860674 Mojo2py-1.0/mojo2py/
--rw-r--r--   0 vishalvenkat   (501) staff       (20)       30 2024-04-15 18:42:32.000000 Mojo2py-1.0/mojo2py/__init__.py
--rw-r--r--   0 vishalvenkat   (501) staff       (20)     2049 2024-04-15 18:42:32.000000 Mojo2py-1.0/mojo2py/mojo2py.py
--rw-r--r--   0 vishalvenkat   (501) staff       (20)       38 2024-04-15 19:21:06.861797 Mojo2py-1.0/setup.cfg
--rw-r--r--   0 vishalvenkat   (501) staff       (20)      814 2024-04-15 19:11:27.000000 Mojo2py-1.0/setup.py
+drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:23:52.937712 Mojo2py-1.1/
+drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:23:52.936256 Mojo2py-1.1/Mojo2py.egg-info/
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)     2525 2024-04-15 19:23:52.000000 Mojo2py-1.1/Mojo2py.egg-info/PKG-INFO
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)      181 2024-04-15 19:23:52.000000 Mojo2py-1.1/Mojo2py.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)        1 2024-04-15 19:23:52.000000 Mojo2py-1.1/Mojo2py.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)        8 2024-04-15 19:23:52.000000 Mojo2py-1.1/Mojo2py.egg-info/top_level.txt
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)     2525 2024-04-15 19:23:52.936955 Mojo2py-1.1/PKG-INFO
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)     2023 2024-04-15 19:22:59.000000 Mojo2py-1.1/README.md
+drwxr-xr-x   0 vishalvenkat   (501) staff       (20)        0 2024-04-15 19:23:52.936658 Mojo2py-1.1/mojo2py/
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)       30 2024-04-15 18:42:32.000000 Mojo2py-1.1/mojo2py/__init__.py
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)     2049 2024-04-15 18:42:32.000000 Mojo2py-1.1/mojo2py/mojo2py.py
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)       38 2024-04-15 19:23:52.937756 Mojo2py-1.1/setup.cfg
+-rw-r--r--   0 vishalvenkat   (501) staff       (20)      812 2024-04-15 19:23:42.000000 Mojo2py-1.1/setup.py
```

### Comparing `Mojo2py-1.0/mojo2py/mojo2py.py` & `Mojo2py-1.1/mojo2py/mojo2py.py`

 * *Files identical despite different names*

### Comparing `Mojo2py-1.0/setup.py` & `Mojo2py-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '1.1'
 DESCRIPTION = 'A python package which converts a mojo file (.mojo or .🔥) into a python file.'
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Mojo2py",
-    version="1.0",
+    version="1.1",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vishal",
     author_email="vishalvenkat2604@gmail.com",
     license='MIT',
     packages=find_packages(),
```

