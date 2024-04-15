# Comparing `tmp/gmp-0.0.8.tar.gz` & `tmp/gmp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmp-0.0.8.tar", last modified: Wed Feb  7 21:27:44 2024, max compression
+gzip compressed data, was "gmp-0.0.9.tar", last modified: Wed Feb  7 21:29:08 2024, max compression
```

## Comparing `gmp-0.0.8.tar` & `gmp-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:27:44.128291 gmp-0.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-07 21:27:44.128291 gmp-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:27:44.128291 gmp-0.0.8/gmp/
--rw-r--r--   0 runner    (1000) runner    (1000)      264 2024-02-07 21:23:02.000000 gmp-0.0.8/gmp/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1469 2024-02-07 21:22:14.000000 gmp-0.0.8/gmp/lolcat.py
--rw-------   0 runner    (1000) runner    (1000)     1711 2024-02-02 14:04:16.000000 gmp-0.0.8/gmp/printing.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:27:44.128291 gmp-0.0.8/gmp.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-07 21:27:44.000000 gmp-0.0.8/gmp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      203 2024-02-07 21:27:44.000000 gmp-0.0.8/gmp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-02-07 21:27:44.000000 gmp-0.0.8/gmp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-02-07 21:27:44.000000 gmp-0.0.8/gmp.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-02-07 21:27:44.000000 gmp-0.0.8/gmp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-02-01 02:05:51.000000 gmp-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-02-07 21:27:44.128291 gmp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1035 2024-02-07 21:27:39.000000 gmp-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:29:08.720210 gmp-0.0.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-07 21:29:08.720210 gmp-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:29:08.716210 gmp-0.0.9/gmp/
+-rw-r--r--   0 runner    (1000) runner    (1000)      264 2024-02-07 21:23:02.000000 gmp-0.0.9/gmp/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1469 2024-02-07 21:22:14.000000 gmp-0.0.9/gmp/lolcat.py
+-rw-------   0 runner    (1000) runner    (1000)     1711 2024-02-02 14:04:16.000000 gmp-0.0.9/gmp/printing.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-07 21:29:08.720210 gmp-0.0.9/gmp.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-07 21:29:08.000000 gmp-0.0.9/gmp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      203 2024-02-07 21:29:08.000000 gmp-0.0.9/gmp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-02-07 21:29:08.000000 gmp-0.0.9/gmp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-02-07 21:29:08.000000 gmp-0.0.9/gmp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-02-07 21:29:08.000000 gmp-0.0.9/gmp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-02-01 02:05:51.000000 gmp-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-02-07 21:29:08.720210 gmp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1029 2024-02-07 21:29:02.000000 gmp-0.0.9/setup.py
```

### Comparing `gmp-0.0.8/gmp/lolcat.py` & `gmp-0.0.9/gmp/lolcat.py`

 * *Files identical despite different names*

### Comparing `gmp-0.0.8/gmp/printing.py` & `gmp-0.0.9/gmp/printing.py`

 * *Files identical despite different names*

### Comparing `gmp-0.0.8/setup.py` & `gmp-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'A little package for GMP'
 LONG_DESCRIPTION = 'This is just a little package I made for my GMP teacher.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="gmp", 
         version=VERSION,
         author="Oz Abramovich",
         author_email="oz@abramovich.net",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['string-color', 're'], # add any additional packages that 
+        install_requires=['string-color'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
 
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

