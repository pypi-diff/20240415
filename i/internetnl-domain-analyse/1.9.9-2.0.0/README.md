# Comparing `tmp/internetnl_domain_analyse-1.9.9.tar.gz` & `tmp/internetnl_domain_analyse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.9.9.tar", last modified: Mon Apr 15 18:06:31 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-2.0.0.tar", last modified: Mon Apr 15 18:49:41 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.9.9.tar` & `internetnl_domain_analyse-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.9/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.9/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 18:05:19.000000 internetnl_domain_analyse-1.9.9/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.9/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.9/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.9/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.9/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.9/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.621448 internetnl_domain_analyse-1.9.9/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    72610 2024-04-15 18:04:36.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.9/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.0/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 18:48:14.000000 internetnl_domain_analyse-2.0.0/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.0/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.0/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.0/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.806024 internetnl_domain_analyse-2.0.0/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.0/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.798024 internetnl_domain_analyse-2.0.0/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.810025 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    73501 2024-04-15 18:46:27.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17349 2024-04-15 18:34:51.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 18:49:41.000000 internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:49:41.814025 internetnl_domain_analyse-2.0.0/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.0/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.0/tox.ini
```

### Comparing `internetnl_domain_analyse-1.9.9/.coveragerc` & `internetnl_domain_analyse-2.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/.gitignore` & `internetnl_domain_analyse-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/.readthedocs.yml` & `internetnl_domain_analyse-2.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/CHANGELOG.rst` & `internetnl_domain_analyse-2.0.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========
 Changelog
 =========
 
-Version 1.9.9
+Version 2.0.0
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
 - Bar width can now be adjusted
 
 Version 1.8.7
```

### Comparing `internetnl_domain_analyse-1.9.9/CONTRIBUTING.rst` & `internetnl_domain_analyse-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/LICENSE.txt` & `internetnl_domain_analyse-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/PKG-INFO` & `internetnl_domain_analyse-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.9
+Version: 2.0.0
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.9/docs/Makefile` & `internetnl_domain_analyse-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/docs/conf.py` & `internetnl_domain_analyse-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/docs/index.rst` & `internetnl_domain_analyse-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-2.0.0/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/setup.cfg` & `internetnl_domain_analyse-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/setup.py` & `internetnl_domain_analyse-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,29 @@
         with codecs.open(
             self.cache_file_name.as_posix(), "w", encoding="UTF-8"
         ) as stream:
             yaml.dump(data=self.data, stream=stream, Dumper=yaml.Dumper)
 
 
 class RecordsCacheInfo:
-    def __init__(self, records_cache_data: dict, year: str, stat_directory: str = None):
+    def __init__(
+        self, records_cache_data: dict, year_key: str, stat_directory: str = None
+    ):
         """
         Store the properties of the cache file in a class
         """
         self.records_cache_data = records_cache_data
         self.stat_directory = stat_directory
 
-        self.year_digits = f"{year}"
+        self.year_key = f"{year_key}"
+        match = re.search("20(\d\d)", self.year_key)
+        if match:
+            self.year_digits = match.group(1)
+        else:
+            self.year_digits = year_key[-2:]
 
         self.cache_dir = None
         self.file_name = None
         self.table_names = None
 
         self.get_cache_file_name()
         self.get_cache_table_names()
@@ -150,15 +157,15 @@
     def get_cache_file_name(self):
         """
         Retrieve the cache file name from the dictionary. If environment variables are given,
         base the directory on the environment name. Names are given like RECORDS_CACHE_DIR_20,
         RECORDS_CACHE_DIR_21, for 2020, 2021 resp.
         """
 
-        records_environment_variable = "_".join(["RECORDS_CACHE_DIR", self.year_digits])
+        records_environment_variable = "_".join(["RECORDS_CACHE_DIR", self.year_key])
         records_cache_dir_name = os.getenv(records_environment_variable)
 
         if records_cache_dir_name is None:
             records_cache_dir_name = self.records_cache_data.get(
                 "records_cache_directory", "."
             )
 
@@ -172,20 +179,35 @@
 
         self.file_name = self.cache_dir / records_file_basename
 
     def get_cache_table_names(self):
         """
         Get the table names of the cache files.
         """
-        self.table_names = self.records_cache_data.get("records_table_names")
-        if self.table_names is None:
-            self.table_names = [
-                f"records_df_{self.year_digits}_2",
-                f"info_records_df_{self.year_digits}",
-            ]
+
+        table_records_environment_variable = "_".join(
+            ["RECORDS_TABLE_RECS", self.year_key]
+        )
+        table_records_name = os.environ.get(table_records_environment_variable)
+        table_info_environment_variable = "_".join(
+            ["RECORDS_TABLE_INFO", self.year_key]
+        )
+        tabl_info_name = os.environ.get(table_info_environment_variable)
+
+        if table_records_name is None:
+            # the environment variabel RECORDS_TABLE_INFO is not set. read from the settings file
+            self.table_names = self.records_cache_data.get("records_table_names")
+            if self.table_names is None:
+                # It is also not found in the settings file. Make a guess
+                self.table_names = [
+                    f"records_df_{self.year_digits}_2",
+                    f"info_records_df_{self.year_digits}",
+                ]
+        else:
+            self.table_names = [table_records_name, tabl_info_name]
 
 
 class DomainAnalyser:
     def __init__(
         self,
         scan_data_key=None,
         cache_file_base="tables_df",
```

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
                     f"the plot legend"
                 )
                 continue
             internet_nl_filename = Path(filename)
             records_cache_data = records_cache_data_per_year[scan_year]
             records_cache_info = RecordsCacheInfo(
                 records_cache_data=records_cache_data,
-                year=scan_year,
+                year_key=scan_year,
                 stat_directory=stat_directory,
             )
 
             _logger.info(f"Start analyse {scan_year}: {internet_nl_filename}")
             domain_analyses = DomainAnalyser(
                 scan_data_key=key_scan_type,
                 records_cache_info=records_cache_info,
```

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 def read_tables_from_sqlite(filename: Path, table_names, index_name) -> pd.DataFrame:
     if isinstance(table_names, str):
         table_names = [table_names]
 
     if not filename.exists():
         _logger.warning(
             "Records file not found. Make sure you set the environment variable "
-            "RECORDS_CACHE_DIR or pass it via the command line argument "
+            "RECORDS_CACHE_DIR_<yearkey> for the file and RECORDS_TABLE_RECS_<yearkey> and "
+            "RECORDS_TABLE_INFO<yearkey> for the tables or pass it via the command line argument "
             "--records_cache_dir"
         )
         raise FileNotFoundError(f"Records file not found {filename.absolute()}")
 
     _logger.info(f"Reading from {filename}")
     connection = sqlite3.connect(filename.as_posix())
     tables = list()
@@ -112,22 +113,22 @@
                             mask = tables[col] == key
                             if any(mask):
                                 tables.loc[mask, col] = float(val)
     return tables
 
 
 def prepare_stat_data_for_write(
-        all_stats,
-        file_base,
-        variables,
-        module_key,
-        variable_key,
-        breakdown_labels=None,
-        n_digits=3,
-        connection=None,
+    all_stats,
+    file_base,
+    variables,
+    module_key,
+    variable_key,
+    breakdown_labels=None,
+    n_digits=3,
+    connection=None,
 ):
     data = pd.DataFrame.from_dict(all_stats)
     if connection is not None:
         data.to_sql(name=file_base, con=connection, if_exists="replace")
 
     stat_df = reorganise_stat_df(
         records_stats=data,
@@ -169,15 +170,15 @@
     else:
         mask_total = pd.Series(True, index=question_df.index)
 
     return mask_total
 
 
 def impose_variable_defaults(
-        variables, module_info: dict = None, module_key: str = None
+    variables, module_info: dict = None, module_key: str = None
 ):
     """
     Impose default values to  the variables data frame
 
     Parameters
     ----------
     variables: pd.DataFrame
@@ -223,29 +224,29 @@
         var_prop = var_row["properties"]
         # loop over the given column names as try to read the value from 'properties' field
         # in the variables dataframe. This properties field is the dict we have read from
         # the settings file which may contain the same key  with a value. If this value was
         # defined for the current variable, copy it to the associate column in the data frame
         # such that we can access it more easily
         for name in (
-                "type",
-                "fixed",
-                "original_name",
-                "question",
-                "label",
-                "check",
-                "optional",
-                "gewicht",
-                "no_impute",
-                "info_per_breakdown",
-                "report_number",
-                "section",
-                "keep_options",
-                "eval",
-                "unit",
+            "type",
+            "fixed",
+            "original_name",
+            "question",
+            "label",
+            "check",
+            "optional",
+            "gewicht",
+            "no_impute",
+            "info_per_breakdown",
+            "report_number",
+            "section",
+            "keep_options",
+            "eval",
+            "unit",
         ):
             try:
                 variables.loc[var_key, name] = var_prop[name]
             except ValueError:
                 # de info_per_breakdown is een dictionary die we met 'at' moeten imposen
                 variables.at[var_key, name] = var_prop.get(name)
             except KeyError:
```

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.9
+Version: 2.0.0
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-2.0.0/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.9/tox.ini` & `internetnl_domain_analyse-2.0.0/tox.ini`

 * *Files identical despite different names*

