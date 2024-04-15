# Comparing `tmp/internetnl_domain_analyse-1.9.6.tar.gz` & `tmp/internetnl_domain_analyse-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.9.6.tar", last modified: Thu Apr 11 20:38:30 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-1.9.8.tar", last modified: Mon Apr 15 10:55:17 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.9.6.tar` & `internetnl_domain_analyse-1.9.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.534838 internetnl_domain_analyse-1.9.6/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.6/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.6/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      960 2024-04-11 20:37:00.000000 internetnl_domain_analyse-1.9.6/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.6/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 20:38:30.534838 internetnl_domain_analyse-1.9.6/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.522838 internetnl_domain_analyse-1.9.6/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.522838 internetnl_domain_analyse-1.9.6/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.6/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.6/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.6/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.522838 internetnl_domain_analyse-1.9.6/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.6/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 20:38:30.534838 internetnl_domain_analyse-1.9.6/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.514838 internetnl_domain_analyse-1.9.6/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.530838 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    72265 2024-04-11 20:36:49.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.530838 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 20:38:30.000000 internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:38:30.530838 internetnl_domain_analyse-1.9.6/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.6/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.6/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.8/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.8/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 10:54:19.000000 internetnl_domain_analyse-1.9.8/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.8/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.8/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.8/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.8/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.677805 internetnl_domain_analyse-1.9.8/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.8/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.673805 internetnl_domain_analyse-1.9.8/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.681805 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    72663 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 10:55:17.000000 internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 10:55:17.685805 internetnl_domain_analyse-1.9.8/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.8/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.8/tox.ini
```

### Comparing `internetnl_domain_analyse-1.9.6/.coveragerc` & `internetnl_domain_analyse-1.9.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/.gitignore` & `internetnl_domain_analyse-1.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/.readthedocs.yml` & `internetnl_domain_analyse-1.9.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/CHANGELOG.rst` & `internetnl_domain_analyse-1.9.8/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 =========
 Changelog
 =========
 
-Version 1.9.6
+Version 1.9.8
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
+- Bar width can now be adjusted
 
 Version 1.8.7
 =============
 - Nu kan je breakdowns ook als combinaties geven. Nodig voor publicatie 2023
 - legend default aan plaatjes toegevoegd nu we meerdere jaren hebben
 - eval statement kan gebruikt worden om afgeleide kolommen te maken
 - dump cache as sqlite optie. Duplicated kolommen worden verwijderd
```

### Comparing `internetnl_domain_analyse-1.9.6/CONTRIBUTING.rst` & `internetnl_domain_analyse-1.9.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/LICENSE.txt` & `internetnl_domain_analyse-1.9.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/PKG-INFO` & `internetnl_domain_analyse-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.6
+Version: 1.9.8
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.6/docs/Makefile` & `internetnl_domain_analyse-1.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/docs/conf.py` & `internetnl_domain_analyse-1.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/docs/index.rst` & `internetnl_domain_analyse-1.9.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-1.9.8/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/setup.cfg` & `internetnl_domain_analyse-1.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/setup.py` & `internetnl_domain_analyse-1.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1198,14 +1198,15 @@
 
             y_max_pdf_plot = plot_prop.get("y_max_pdf_plot", 10)
             y_spacing_pdf_plot = plot_prop.get("y_spacing_pdf_plot", 5)
             y_max_bar_plot = plot_prop.get("y_max_bar_plot")
             legend_position = plot_prop.get("legend_position")
             legend_max_columns = plot_prop.get("legend_max_columns")
             y_spacing_bar_plot = plot_prop.get("y_spacing_bar_plot")
+            bar_width = plot_prop.get("bar_width")
 
             box_margin = plot_prop.get("box_margin")
 
             sort_values = plot_prop.get("sort_values", False)
             subplot_adjust = plot_prop.get("subplot_adjust")
             reference_lines = plot_prop.get("reference_lines")
             if reference_lines is not None:
@@ -1347,14 +1348,19 @@
                             legend_pos = legend_position
 
                         if plot_info.y_spacing is not None:
                             y_spacing = plot_info.y_spacing
                         else:
                             y_spacing = y_spacing_bar_plot
 
+                        if plot_info.bar_width is not None:
+                            bar_width = plot_info.bar_width
+                        else:
+                            bar_width = bar_width
+
                         if keep_options:
                             # als keep options gegeven is dan houden we alle opties
                             valide_opties = variables.loc[
                                 original_name, "options"
                             ].values()
                             mask = get_option_mask(
                                 question_df=question_df_clean,
@@ -1499,14 +1505,15 @@
                                     legend_position=legend_pos,
                                     legend_max_columns=legend_max_columns,
                                     normalize_data=normalize_data,
                                     force_plot=self.force_plots,
                                     enable_highcharts_legend=plot_info.enable_highcharts_legend,
                                     unit=unit,
                                     english=self.english,
+                                    bar_width=bar_width,
                                 )
 
                                 _logger.debug(
                                     f"Store [{original_name}][{label}] : {image_file}"
                                 )
                                 self.image_info.add_entry(
                                     plot_key=plot_key,
@@ -1588,14 +1595,15 @@
 
         self.label = None
         self.directory = None
         self.y_max = None
         self.y_spacing = None
         self.legend_position = None
         self.enable_highcharts_legend = True
+        self.bar_width = None
 
         self.get_plot_info()
 
     def get_plot_info(self):
         """In de variables dataframe kunnen we ook uitdrukkelijk de highcharts directory en highcharts
         label opgeven per variabele. Zoek dat hier op"""
         label = None
@@ -1618,14 +1626,15 @@
                 else:
                     self.directory = info.get("highcharts_directory")
                     if self.directory is not None:
                         self.directory = Path(self.directory)
                     self.label = info.get("highcharts_label")
                     self.y_max = info.get("y_max")
                     self.y_spacing = info.get("y_spacing")
+                    self.bar_width = info.get("bar_width")
                     self.legend_position = get_windows_or_linux_value(
                         info.get("legend_position")
                     )
                     self.enable_highcharts_legend = info.get(
                         "enable_highcharts_legend", True
                     )
```

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domain_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,18 +247,25 @@
     trans,
     y_spacing_bar_plot,
     y_max_bar_plot,
     legend_position,
     legend_max_columns,
     unit=None,
     english=False,
+    bar_width=None,
 ):
     x_range = None
+
+    if bar_width is not None:
+        kwargs = dict(width=bar_width)
+    else:
+        kwargs = {}
+
     try:
-        plot_df.plot(kind="barh", ax=axis, rot=0, legend=None)
+        plot_df.plot(kind="barh", ax=axis, rot=0, legend=None, **kwargs)
     except IndexError as err:
         _logger.warning(err)
         _logger.warning(f"skip {plot_title}")
         pass
     else:
 
         # put the high
@@ -432,14 +439,15 @@
     highcharts_directory=None,
     title=None,
     normalize_data=False,
     force_plot=False,
     enable_highcharts_legend=True,
     unit=None,
     english=False,
+    bar_width=None,
 ):
     image_name = re.sub("_\d(\.\d){0,1}$", "", plot_variable)
     image_file = image_directory / Path(
         "_".join([scan_data_key, plot_key, ".".join([image_name, image_type])])
     )
     image_file_name = image_file.as_posix()
     if image_file.exists() and not force_plot:
@@ -520,14 +528,15 @@
             trans=trans,
             y_spacing_bar_plot=y_spacing_bar_plot,
             y_max_bar_plot=y_max_bar_plot,
             legend_position=legend_position,
             legend_max_columns=legend_max_columns,
             unit=unit,
             english=english,
+            bar_width=bar_width,
         )
 
     _logger.info(f"Saving plot {image_file_name}")
     fig.savefig(image_file)
 
     if highcharts_directory is not None:
         highcharts_directory.mkdir(exist_ok=True, parents=True)
```

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.6
+Version: 1.9.8
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.6/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-1.9.8/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.6/tox.ini` & `internetnl_domain_analyse-1.9.8/tox.ini`

 * *Files identical despite different names*

