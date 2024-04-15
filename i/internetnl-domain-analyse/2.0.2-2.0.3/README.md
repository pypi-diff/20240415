# Comparing `tmp/internetnl_domain_analyse-2.0.2.tar.gz` & `tmp/internetnl_domain_analyse-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-2.0.2.tar", last modified: Mon Apr 15 19:55:20 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-2.0.3.tar", last modified: Mon Apr 15 20:33:41 2024, max compression
```

## Comparing `internetnl_domain_analyse-2.0.2.tar` & `internetnl_domain_analyse-2.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.2/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 19:15:35.000000 internetnl_domain_analyse-2.0.2/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.531249 internetnl_domain_analyse-2.0.2/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.531249 internetnl_domain_analyse-2.0.2/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.2/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.2/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.2/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.535250 internetnl_domain_analyse-2.0.2/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.2/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.527249 internetnl_domain_analyse-2.0.2/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.539250 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    73505 2024-04-15 19:54:36.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17421 2024-04-15 19:42:57.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.539250 internetnl_domain_analyse-2.0.2/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.2/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.969854 internetnl_domain_analyse-2.0.3/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.3/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 20:33:25.000000 internetnl_domain_analyse-2.0.3/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 20:33:41.969854 internetnl_domain_analyse-2.0.3/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.957854 internetnl_domain_analyse-2.0.3/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.957854 internetnl_domain_analyse-2.0.3/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.3/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.3/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.3/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.957854 internetnl_domain_analyse-2.0.3/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.3/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 20:33:41.969854 internetnl_domain_analyse-2.0.3/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.953854 internetnl_domain_analyse-2.0.3/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.965855 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    73617 2024-04-15 20:31:42.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17421 2024-04-15 19:42:57.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.965855 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 20:33:41.000000 internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 20:33:41.965855 internetnl_domain_analyse-2.0.3/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.3/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.3/tox.ini
```

### Comparing `internetnl_domain_analyse-2.0.2/.coveragerc` & `internetnl_domain_analyse-2.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/.gitignore` & `internetnl_domain_analyse-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/.readthedocs.yml` & `internetnl_domain_analyse-2.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/CHANGELOG.rst` & `internetnl_domain_analyse-2.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========
 Changelog
 =========
 
-Version 2.0.1
+Version 2.0.3
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
 - Bar width can now be adjusted
 
 Version 1.8.7
```

### Comparing `internetnl_domain_analyse-2.0.2/CONTRIBUTING.rst` & `internetnl_domain_analyse-2.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/LICENSE.txt` & `internetnl_domain_analyse-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/PKG-INFO` & `internetnl_domain_analyse-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.2
+Version: 2.0.3
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.2/docs/Makefile` & `internetnl_domain_analyse-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/docs/conf.py` & `internetnl_domain_analyse-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/docs/index.rst` & `internetnl_domain_analyse-2.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-2.0.3/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/setup.cfg` & `internetnl_domain_analyse-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/setup.py` & `internetnl_domain_analyse-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1123,14 +1123,16 @@
                 _logger.warning("Run script with option '--statistics_to_xls'  first")
             stats_df_per_year = None
         return stats_df_per_year
 
     def make_plots(self):
         _logger.info("Making the plot")
 
+        legend_translates = dict()
+
         for plot_key, plot_prop in self.plot_info.items():
             if not plot_prop.get("do_it", True):
                 _logger.debug(f"Skipping plot {plot_key}")
                 continue
 
             _logger.debug(f"Plotting plot {plot_key}")
             label = plot_prop.get("label", plot_key)
@@ -1153,20 +1155,21 @@
                 variables.loc[report_number_empty, "report_number"] = False
 
             module_info = scan_data_analyses.module_info
 
             stats_df_per_year = {}
             last_year = None
             df_index_names = None
-            for year in scan_data_per_year.keys():
+            for year, scan_info in scan_data_per_year.items():
                 df = self.get_plot_cache(
                     scan_data_key=scan_data_key, plot_key=plot_key, year_key=year
                 )
+                year_label = scan_info.get("label", year)
                 if df is not None:
-                    stats_df_per_year[year] = df
+                    stats_df_per_year[year_label] = df
                     last_year = year
                     df_index_names = list(df.index.names)
 
             if not self.english:
                 jaar_level_name = "Jaar"
             else:
                 jaar_level_name = "Year"
```

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.2
+Version: 2.0.3
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-2.0.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.2/tox.ini` & `internetnl_domain_analyse-2.0.3/tox.ini`

 * *Files identical despite different names*

