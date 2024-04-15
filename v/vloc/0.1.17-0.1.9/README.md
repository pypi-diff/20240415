# Comparing `tmp/vloc-0.1.17.tar.gz` & `tmp/vloc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc-0.1.17.tar", last modified: Mon Apr 15 08:10:32 2024, max compression
+gzip compressed data, was "vloc-0.1.9.tar", last modified: Tue Apr  9 04:08:57 2024, max compression
```

## Comparing `vloc-0.1.17.tar` & `vloc-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.771481 vloc-0.1.17/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.17/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      493 2024-04-15 08:10:32.771286 vloc-0.1.17/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.17/README.md
--rw-r--r--   0 byron      (501) staff       (20)      585 2024-04-15 07:51:05.000000 vloc-0.1.17/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-15 08:10:32.771525 vloc-0.1.17/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.767919 vloc-0.1.17/vloc/
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.769256 vloc-0.1.17/vloc/__detect__/
--rw-r--r--   0 byron      (501) staff       (20)     5816 2024-04-14 08:37:23.000000 vloc-0.1.17/vloc/__detect__/__detect__.py
--rw-r--r--   0 byron      (501) staff       (20)      152 2024-04-14 08:00:11.000000 vloc-0.1.17/vloc/__detect__/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)      180 2024-04-15 07:32:15.000000 vloc-0.1.17/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.769773 vloc-0.1.17/vloc/exception/
--rw-r--r--   0 byron      (501) staff       (20)      209 2024-04-14 08:37:23.000000 vloc-0.1.17/vloc/exception/__exception__.py
--rw-r--r--   0 byron      (501) staff       (20)      114 2024-04-14 08:37:23.000000 vloc-0.1.17/vloc/exception/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.770806 vloc-0.1.17/vloc/module/
--rw-r--r--   0 byron      (501) staff       (20)     2293 2024-04-14 07:39:20.000000 vloc-0.1.17/vloc/module/__config__.py
--rw-r--r--   0 byron      (501) staff       (20)       67 2024-04-14 07:41:04.000000 vloc-0.1.17/vloc/module/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      813 2024-04-14 07:39:54.000000 vloc-0.1.17/vloc/module/__module__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:10:32.771062 vloc-0.1.17/vloc.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      493 2024-04-15 08:10:32.000000 vloc-0.1.17/vloc.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      385 2024-04-15 08:10:32.000000 vloc-0.1.17/vloc.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-15 08:10:32.000000 vloc-0.1.17/vloc.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-15 08:10:32.000000 vloc-0.1.17/vloc.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-15 08:10:32.000000 vloc-0.1.17/vloc.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.549106 vloc-0.1.9/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.9/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.548887 vloc-0.1.9/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.9/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      625 2024-04-09 04:08:12.000000 vloc-0.1.9/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 04:08:57.549143 vloc-0.1.9/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.547789 vloc-0.1.9/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 03:59:47.000000 vloc-0.1.9/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.548685 vloc-0.1.9/vloc.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      192 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/top_level.txt
```

### Comparing `vloc-0.1.17/LICENSE.txt` & `vloc-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc-0.1.17/pyproject.toml` & `vloc-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+include = ["vloc"]
 
 [project]
 name = "vloc"
-version = "0.1.17"
+version = "0.1.9"
 urls = { GitHub = "https://github.com/linyeh1129/vloc" }
 authors = [{ name = 'Lin Yeh', email = 'lin_yeh@outlook.com' }]
-description = "An UI antomation tool based by YOLO"
+description = "Plugin functions for vloc"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ['ui aumomation', 'computer vision']
 classifiers = ['Programming Language :: Python :: 3']
 dependencies = [
     'opencv-python >= 4.9.0.80',
```

