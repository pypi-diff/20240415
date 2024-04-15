# Comparing `tmp/erlcpy-1.1.3.tar.gz` & `tmp/erlcpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlcpy-1.1.3.tar", last modified: Mon Apr  8 20:39:21 2024, max compression
+gzip compressed data, was "erlcpy-1.1.4.tar", last modified: Mon Apr 15 20:41:41 2024, max compression
```

## Comparing `erlcpy-1.1.3.tar` & `erlcpy-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:39:21.114465 erlcpy-1.1.3/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      363 2024-04-08 20:39:21.113463 erlcpy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 20:39:21.091887 erlcpy-1.1.3/erlcpy/
--rw-rw-rw-   0        0        0      381 2024-04-08 19:44:43.000000 erlcpy-1.1.3/erlcpy/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-04-08 20:38:56.000000 erlcpy-1.1.3/erlcpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:39:21.112457 erlcpy-1.1.3/erlcpy.egg-info/
--rw-rw-rw-   0        0        0      363 2024-04-08 20:39:20.000000 erlcpy-1.1.3/erlcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-08 20:39:21.000000 erlcpy-1.1.3/erlcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:39:20.000000 erlcpy-1.1.3/erlcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 20:39:20.000000 erlcpy-1.1.3/erlcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-08 20:39:20.000000 erlcpy-1.1.3/erlcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 20:39:21.114465 erlcpy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-08 20:39:18.000000 erlcpy-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.312086 erlcpy-1.1.4/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      363 2024-04-15 20:41:41.312086 erlcpy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.296085 erlcpy-1.1.4/erlcpy/
+-rw-rw-rw-   0        0        0       46 2024-04-15 20:39:04.000000 erlcpy-1.1.4/erlcpy/__init__.py
+-rw-rw-rw-   0        0        0     2204 2024-04-15 20:38:09.000000 erlcpy-1.1.4/erlcpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.311088 erlcpy-1.1.4/erlcpy.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 20:41:41.313085 erlcpy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-15 20:41:31.000000 erlcpy-1.1.4/setup.py
```

### Comparing `erlcpy-1.1.3/LICENSE` & `erlcpy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.3/README.md` & `erlcpy-1.1.4/README.md`

 * *Files identical despite different names*

