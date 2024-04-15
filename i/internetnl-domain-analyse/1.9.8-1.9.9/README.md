# Comparing `tmp/internetnl_domain_analyse-1.9.8.tar.gz` & `tmp/internetnl_domain_analyse-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.9.8.tar", last modified: Mon Apr 15 10:55:17 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-1.9.9.tar", last modified: Mon Apr 15 18:06:31 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.9.8.tar` & `internetnl_domain_analyse-1.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.8/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.8/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 10:54:19.000000 internetnl_domain_analyse-1.9.8/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.8/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.8/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.8/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.8/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.8/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.673805 internetnl_domain_analyse-1.9.8/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.681805 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    72663 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.8/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.9/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.9/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 18:05:19.000000 internetnl_domain_analyse-1.9.9/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.9/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.9/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.9/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.9/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.629448 internetnl_domain_analyse-1.9.9/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.9/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 18:06:31.641448 internetnl_domain_analyse-1.9.9/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.621448 internetnl_domain_analyse-1.9.9/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    72610 2024-04-15 18:04:36.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 18:06:31.000000 internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 18:06:31.637448 internetnl_domain_analyse-1.9.9/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.9/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.9/tox.ini
```

### Comparing `internetnl_domain_analyse-1.9.8/.coveragerc` & `internetnl_domain_analyse-1.9.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/.gitignore` & `internetnl_domain_analyse-1.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/.readthedocs.yml` & `internetnl_domain_analyse-1.9.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/CHANGELOG.rst` & `internetnl_domain_analyse-1.9.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========
 Changelog
 =========
 
-Version 1.9.8
+Version 1.9.9
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
 - Bar width can now be adjusted
 
 Version 1.8.7
```

### Comparing `internetnl_domain_analyse-1.9.8/CONTRIBUTING.rst` & `internetnl_domain_analyse-1.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/LICENSE.txt` & `internetnl_domain_analyse-1.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/PKG-INFO` & `internetnl_domain_analyse-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.8
+Version: 1.9.9
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.8/docs/Makefile` & `internetnl_domain_analyse-1.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/docs/conf.py` & `internetnl_domain_analyse-1.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/docs/index.rst` & `internetnl_domain_analyse-1.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-1.9.9/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/setup.cfg` & `internetnl_domain_analyse-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/setup.py` & `internetnl_domain_analyse-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,32 +129,31 @@
         ) as stream:
             yaml.dump(data=self.data, stream=stream, Dumper=yaml.Dumper)
 
 
 class RecordsCacheInfo:
     def __init__(self, records_cache_data: dict, year: str, stat_directory: str = None):
         """
-        Store the properties of the caches file in a class
+        Store the properties of the cache file in a class
         """
         self.records_cache_data = records_cache_data
         self.stat_directory = stat_directory
 
-        # pick the last two digit of the year
-        self.year_digits = f"{year}"[-2:]
+        self.year_digits = f"{year}"
 
         self.cache_dir = None
         self.file_name = None
         self.table_names = None
 
         self.get_cache_file_name()
         self.get_cache_table_names()
 
     def get_cache_file_name(self):
         """
-        Retrieve the cache file name from the dictionary. If environments variables are given,
+        Retrieve the cache file name from the dictionary. If environment variables are given,
         base the directory on the environment name. Names are given like RECORDS_CACHE_DIR_20,
         RECORDS_CACHE_DIR_21, for 2020, 2021 resp.
         """
 
         records_environment_variable = "_".join(["RECORDS_CACHE_DIR", self.year_digits])
         records_cache_dir_name = os.getenv(records_environment_variable)
```

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.8
+Version: 1.9.9
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-1.9.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.8/tox.ini` & `internetnl_domain_analyse-1.9.9/tox.ini`

 * *Files identical despite different names*

