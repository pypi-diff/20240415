# Comparing `tmp/arlecchino-1.0.tar.gz` & `tmp/arlecchino-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlecchino-1.0.tar", last modified: Mon Apr 15 12:53:00 2024, max compression
+gzip compressed data, was "arlecchino-1.1.tar", last modified: Mon Apr 15 14:21:11 2024, max compression
```

## Comparing `arlecchino-1.0.tar` & `arlecchino-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 12:53:00.738342 arlecchino-1.0/
--rw-rw-rw-   0        0        0       24 2024-04-15 12:50:46.000000 arlecchino-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      466 2024-04-15 12:53:00.736334 arlecchino-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-04-15 12:50:46.000000 arlecchino-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 12:53:00.696615 arlecchino-1.0/arlecchino/
--rw-rw-rw-   0        0        0      715 2024-04-15 12:50:46.000000 arlecchino-1.0/arlecchino/__init__.py
--rw-rw-rw-   0        0        0     3397 2024-04-15 12:50:46.000000 arlecchino-1.0/arlecchino/colors.txt
--rw-rw-rw-   0        0        0      151 2024-04-15 12:50:46.000000 arlecchino-1.0/arlecchino/shades.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 12:53:00.734335 arlecchino-1.0/arlecchino.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-15 12:53:00.000000 arlecchino-1.0/arlecchino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-15 12:53:00.000000 arlecchino-1.0/arlecchino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 12:53:00.000000 arlecchino-1.0/arlecchino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 12:53:00.000000 arlecchino-1.0/arlecchino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      520 2024-04-15 12:50:46.000000 arlecchino-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 12:53:00.738342 arlecchino-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 14:21:11.637620 arlecchino-1.1/
+-rw-rw-rw-   0        0        0       24 2024-04-15 12:50:46.000000 arlecchino-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      466 2024-04-15 14:21:11.635614 arlecchino-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-04-15 12:50:46.000000 arlecchino-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:21:11.588860 arlecchino-1.1/arlecchino/
+-rw-rw-rw-   0        0        0     1037 2024-04-15 14:12:57.000000 arlecchino-1.1/arlecchino/__init__.py
+-rw-rw-rw-   0        0        0     3397 2024-04-15 12:50:46.000000 arlecchino-1.1/arlecchino/colors.txt
+-rw-rw-rw-   0        0        0      151 2024-04-15 12:50:46.000000 arlecchino-1.1/arlecchino/shades.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:21:11.632617 arlecchino-1.1/arlecchino.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-15 14:21:11.000000 arlecchino-1.1/arlecchino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-15 14:21:11.000000 arlecchino-1.1/arlecchino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:21:11.000000 arlecchino-1.1/arlecchino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 14:21:11.000000 arlecchino-1.1/arlecchino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      520 2024-04-15 14:19:48.000000 arlecchino-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:21:11.638999 arlecchino-1.1/setup.cfg
```

### Comparing `arlecchino-1.0/arlecchino/colors.txt` & `arlecchino-1.1/arlecchino/colors.txt`

 * *Files identical despite different names*

### Comparing `arlecchino-1.0/pyproject.toml` & `arlecchino-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arlecchino"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Martin Ranieri"},
 ]
 description = "Italian color names generator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

