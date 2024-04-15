# Comparing `tmp/internetnl_domain_analyse-2.0.0.tar.gz` & `tmp/internetnl_domain_analyse-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-2.0.0.tar", last modified: Mon Apr 15 18:49:41 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-2.0.1.tar", last modified: Mon Apr 15 19:16:33 2024, max compression
```

## Comparing `internetnl_domain_analyse-2.0.0.tar` & `internetnl_domain_analyse-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.0/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 18:48:14.000000 internetnl_domain_analyse-2.0.0/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.0/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.0/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.0/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.0/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.798024 internetnl_domain_analyse-2.0.0/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.810025 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    73501 2024-04-15 18:46:27.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17349 2024-04-15 18:34:51.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.0/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.1/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 19:15:35.000000 internetnl_domain_analyse-2.0.1/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.177320 internetnl_domain_analyse-2.0.1/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.177320 internetnl_domain_analyse-2.0.1/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.1/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.1/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.1/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.181320 internetnl_domain_analyse-2.0.1/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.1/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.173320 internetnl_domain_analyse-2.0.1/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.185320 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    73451 2024-04-15 19:14:41.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17347 2024-04-15 19:14:23.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.1/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/tox.ini
```

### Comparing `internetnl_domain_analyse-2.0.0/.coveragerc` & `internetnl_domain_analyse-2.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/.gitignore` & `internetnl_domain_analyse-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/.readthedocs.yml` & `internetnl_domain_analyse-2.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/CHANGELOG.rst` & `internetnl_domain_analyse-2.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========
 Changelog
 =========
 
-Version 2.0.0
+Version 2.0.1
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
 - Bar width can now be adjusted
 
 Version 1.8.7
```

### Comparing `internetnl_domain_analyse-2.0.0/CONTRIBUTING.rst` & `internetnl_domain_analyse-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/LICENSE.txt` & `internetnl_domain_analyse-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/PKG-INFO` & `internetnl_domain_analyse-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.0
+Version: 2.0.1
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.0/docs/Makefile` & `internetnl_domain_analyse-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/docs/conf.py` & `internetnl_domain_analyse-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/docs/index.rst` & `internetnl_domain_analyse-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-2.0.1/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/setup.cfg` & `internetnl_domain_analyse-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/setup.py` & `internetnl_domain_analyse-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             file_name=file_name,
             tex_right_shift=tex_right_shift,
             sub_image_label=sub_image_label,
         )
         if section:
             self.data[image_key][plot_key]["section"] = section
 
-        # in order to get the key order in the dict the same as in the input file, alter the order
+        # To get the key order in the dict the same as in the input file, alter the order
         if len(self.data[image_key].keys()) > 1:
             tmp_data = self.data[image_key].copy()
             self.data[image_key] = dict()
             for plot_key in plot_info.keys():
                 try:
                     tex_prop = tmp_data[plot_key]
                 except KeyError as err:
@@ -126,15 +126,15 @@
         """Schrijf de cache"""
         with codecs.open(
             self.cache_file_name.as_posix(), "w", encoding="UTF-8"
         ) as stream:
             yaml.dump(data=self.data, stream=stream, Dumper=yaml.Dumper)
 
 
-class RecordsCacheInfo:
+class RecordCacheInfo:
     def __init__(
         self, records_cache_data: dict, year_key: str, stat_directory: str = None
     ):
         """
         Store the properties of the cache file in a class
         """
         self.records_cache_data = records_cache_data
@@ -211,15 +211,15 @@
         self,
         scan_data_key=None,
         cache_file_base="tables_df",
         cache_directory_base_name=None,
         tld_extract_cache_directory=None,
         output_file=None,
         reset=None,
-        records_cache_info: RecordsCacheInfo = None,
+        records_cache_info: RecordCacheInfo = None,
         internet_nl_filename=None,
         breakdown_labels=None,
         statistics: dict = None,
         default_scan=None,
         variables: dict = None,
         module_info: dict = None,
         weights=None,
@@ -250,15 +250,15 @@
         self.output_directory = Path("output")
         self.output_directory.mkdir(exist_ok=True)
         self.output_file = self.output_directory / self.output_file
 
         outfile_suff = self.output_file.suffixes
         outfile_base = self.output_file.with_suffix("").with_suffix("").as_posix()
         outfile_year = Path(
-            "_".join([outfile_base, scan_data_key, self.records_cache_info.year_digits])
+            "_".join([outfile_base, scan_data_key, self.records_cache_info.year_key])
         )
         self.output_file = outfile_year.with_suffix(".".join(outfile_suff))
         self.dump_cache_as_sqlite = dump_cache_as_sqlite
 
         self.scan_data_key = scan_data_key
         self.breakdown_labels = breakdown_labels
 
@@ -286,25 +286,23 @@
 
         if internet_nl_filename is not None:
             self.internet_nl_filename = internet_nl_filename
         else:
             self.internet_nl_filename = Path("internet_nl.sqlite")
 
         self.cache_directory = Path(
-            "_".join([cache_directory_base_name, self.records_cache_info.year_digits])
+            "_".join([cache_directory_base_name, self.records_cache_info.year_key])
         )
         self.cache_directory.mkdir(exist_ok=True)
         if tld_extract_cache_directory is None:
             self.tld_extract_cache_directory = "tld_cache"
         else:
             self.tld_extract_cache_directory = tld_extract_cache_directory
         cache_file_base = Path(
-            "_".join(
-                [cache_file_base, self.records_cache_info.year_digits, scan_data_key]
-            )
+            "_".join([cache_file_base, self.records_cache_info.year_key, scan_data_key])
             + ".pkl"
         )
         self.cache_file = self.cache_directory / cache_file_base
         self.cate_outfile = None
         self.cate_pkl_file = None
         self.corr_outfile = None
         self.corr_pkl_file = None
```

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import yaml
 
 from internetnl_domain_analyse import __version__
 from internetnl_domain_analyse.domain_analyse_classes import (
     DomainAnalyser,
     DomainPlotter,
-    RecordsCacheInfo,
+    RecordCacheInfo,
 )
 from internetnl_domain_analyse.domain_plots import (
     make_heatmap,
     make_conditional_score_plot,
     make_conditional_pdf_plot,
     make_verdeling_per_aantal_categorie,
 )
@@ -374,15 +374,15 @@
                 _logger.info(
                     f"File name for year {scan_year} was None. Skip it but add it to"
                     f"the plot legend"
                 )
                 continue
             internet_nl_filename = Path(filename)
             records_cache_data = records_cache_data_per_year[scan_year]
-            records_cache_info = RecordsCacheInfo(
+            records_cache_info = RecordCacheInfo(
                 records_cache_data=records_cache_data,
                 year_key=scan_year,
                 stat_directory=stat_directory,
             )
 
             _logger.info(f"Start analyse {scan_year}: {internet_nl_filename}")
             domain_analyses = DomainAnalyser(
```

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.0
+Version: 2.0.1
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.0/tox.ini` & `internetnl_domain_analyse-2.0.1/tox.ini`

 * *Files identical despite different names*

