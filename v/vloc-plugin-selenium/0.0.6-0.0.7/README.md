# Comparing `tmp/vloc_plugin_selenium-0.0.6.tar.gz` & `tmp/vloc_plugin_selenium-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin_selenium-0.0.6.tar", last modified: Wed Apr 10 06:48:14 2024, max compression
+gzip compressed data, was "vloc_plugin_selenium-0.0.7.tar", last modified: Mon Apr 15 08:07:40 2024, max compression
```

## Comparing `vloc_plugin_selenium-0.0.6.tar` & `vloc_plugin_selenium-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:48:14.760389 vloc_plugin_selenium-0.0.6/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.6/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-10 06:48:14.760159 vloc_plugin_selenium-0.0.6/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.6/README.md
--rw-r--r--   0 byron      (501) staff       (20)      528 2024-04-10 06:47:44.000000 vloc_plugin_selenium-0.0.6/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-10 06:48:14.760428 vloc_plugin_selenium-0.0.6/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:48:14.758070 vloc_plugin_selenium-0.0.6/vloc/
--rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:42:34.000000 vloc_plugin_selenium-0.0.6/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:48:14.758368 vloc_plugin_selenium-0.0.6/vloc/plugin/
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 02:42:18.000000 vloc_plugin_selenium-0.0.6/vloc/plugin/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:48:14.758767 vloc_plugin_selenium-0.0.6/vloc/plugin/__selenium__/
--rw-r--r--   0 byron      (501) staff       (20)      660 2024-04-08 06:42:15.000000 vloc_plugin_selenium-0.0.6/vloc/plugin/__selenium__/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 02:42:26.000000 vloc_plugin_selenium-0.0.6/vloc/plugin/__selenium__/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:48:14.759906 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-10 06:48:14.000000 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      370 2024-04-10 06:48:14.000000 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-10 06:48:14.000000 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       12 2024-04-10 06:48:14.000000 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-10 06:48:14.000000 vloc_plugin_selenium-0.0.6/vloc_plugin_selenium.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:07:40.996781 vloc_plugin_selenium-0.0.7/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.7/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-15 08:07:40.996552 vloc_plugin_selenium-0.0.7/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.7/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      528 2024-04-15 07:50:55.000000 vloc_plugin_selenium-0.0.7/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-15 08:07:40.996833 vloc_plugin_selenium-0.0.7/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:07:40.994349 vloc_plugin_selenium-0.0.7/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)      180 2024-04-15 07:49:09.000000 vloc_plugin_selenium-0.0.7/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:07:40.994602 vloc_plugin_selenium-0.0.7/vloc/plugin/
+-rw-r--r--   0 byron      (501) staff       (20)      145 2024-04-15 07:48:56.000000 vloc_plugin_selenium-0.0.7/vloc/plugin/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:07:40.995272 vloc_plugin_selenium-0.0.7/vloc/plugin/__selenium__/
+-rw-r--r--   0 byron      (501) staff       (20)      666 2024-04-14 09:54:05.000000 vloc_plugin_selenium-0.0.7/vloc/plugin/__selenium__/__info__.py
+-rw-r--r--   0 byron      (501) staff       (20)     1117 2024-04-14 09:52:22.000000 vloc_plugin_selenium-0.0.7/vloc/plugin/__selenium__/__selenium__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:07:40.996338 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-15 08:07:40.000000 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      374 2024-04-15 08:07:40.000000 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-15 08:07:40.000000 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)       12 2024-04-15 08:07:40.000000 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-15 08:07:40.000000 vloc_plugin_selenium-0.0.7/vloc_plugin_selenium.egg-info/top_level.txt
```

### Comparing `vloc_plugin_selenium-0.0.6/LICENSE.txt` & `vloc_plugin_selenium-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin_selenium-0.0.6/pyproject.toml` & `vloc_plugin_selenium-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "vloc_plugin_selenium"
-version = "0.0.6"
+version = "0.0.7"
 urls = { GitHub = "https://github.com/linyeh1129/vloc_plugin_selenium" }
 authors = [{ name = 'Lin Yeh', email = 'lin_yeh@outlook.com' }]
 description = "Plugin functions for vloc"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ['ui aumomation', 'computer vision']
```

### Comparing `vloc_plugin_selenium-0.0.6/vloc/plugin/__selenium__/__info__.py` & `vloc_plugin_selenium-0.0.7/vloc/plugin/__selenium__/__info__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from typing import Any
 from selenium.webdriver import ActionChains
 
 
-class Action:
+class DetectAction:
     x: int = None
     y: int = None
     action_chain: ActionChains = None
 
     def __init__(self,
                  x: int,
                  y: int,
```

