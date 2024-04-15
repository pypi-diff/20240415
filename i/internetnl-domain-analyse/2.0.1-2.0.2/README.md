# Comparing `tmp/internetnl_domain_analyse-2.0.1.tar.gz` & `tmp/internetnl_domain_analyse-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-2.0.1.tar", last modified: Mon Apr 15 19:16:33 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-2.0.2.tar", last modified: Mon Apr 15 19:55:20 2024, max compression
```

## Comparing `internetnl_domain_analyse-2.0.1.tar` & `internetnl_domain_analyse-2.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.1/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 19:15:35.000000 internetnl_domain_analyse-2.0.1/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.177320 internetnl_domain_analyse-2.0.1/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.177320 internetnl_domain_analyse-2.0.1/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.1/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.1/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.1/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.181320 internetnl_domain_analyse-2.0.1/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.1/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.173320 internetnl_domain_analyse-2.0.1/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.185320 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    73451 2024-04-15 19:14:41.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17347 2024-04-15 19:14:23.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 19:16:33.000000 internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:16:33.189320 internetnl_domain_analyse-2.0.1/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.1/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.1/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-2.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-2.0.2/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      992 2024-04-15 19:15:35.000000 internetnl_domain_analyse-2.0.2/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-2.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.531249 internetnl_domain_analyse-2.0.2/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.531249 internetnl_domain_analyse-2.0.2/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-2.0.2/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-2.0.2/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-2.0.2/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.535250 internetnl_domain_analyse-2.0.2/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-2.0.2/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.527249 internetnl_domain_analyse-2.0.2/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.539250 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    73505 2024-04-15 19:54:36.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44715 2024-04-15 10:51:41.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17421 2024-04-15 19:42:57.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15482 2024-04-15 18:48:04.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.543250 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-15 19:55:20.000000 internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-15 19:55:20.539250 internetnl_domain_analyse-2.0.2/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-2.0.2/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-2.0.2/tox.ini
```

### Comparing `internetnl_domain_analyse-2.0.1/.coveragerc` & `internetnl_domain_analyse-2.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/.gitignore` & `internetnl_domain_analyse-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/.readthedocs.yml` & `internetnl_domain_analyse-2.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/CHANGELOG.rst` & `internetnl_domain_analyse-2.0.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/CONTRIBUTING.rst` & `internetnl_domain_analyse-2.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/LICENSE.txt` & `internetnl_domain_analyse-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/PKG-INFO` & `internetnl_domain_analyse-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.1
+Version: 2.0.2
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.1/docs/Makefile` & `internetnl_domain_analyse-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/docs/conf.py` & `internetnl_domain_analyse-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/docs/index.rst` & `internetnl_domain_analyse-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-2.0.2/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/setup.cfg` & `internetnl_domain_analyse-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/setup.py` & `internetnl_domain_analyse-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,28 +1098,28 @@
                 tex_prepend_path=self.tex_prepend_path,
                 tex_horizontal_shift=tex_horizontal_shift,
                 bovenschrift=bovenschrift,
                 module_info=module_info,
             )
 
     #
-    def get_plot_cache(self, scan_data_key, plot_key, year):
-        last_two_digits = f"{year}"[-2:]
-        cache_directory = "_".join([self.cache_directory.as_posix(), last_two_digits])
+    def get_plot_cache(self, scan_data_key, plot_key, year_key):
+        year_label = f"{year_key}"
+        cache_directory = "_".join([self.cache_directory.as_posix(), year_label])
         cache_file = make_plot_cache_file_name(
             cache_directory=Path(cache_directory),
             prefix=scan_data_key,
             file_base=plot_key,
         )
         _logger.debug(f"Reading {cache_file}")
         try:
             with open(cache_file, "rb") as stream:
                 stats_df_per_year = pickle.load(stream)
         except FileNotFoundError as err:
-            if self.scan_data[scan_data_key][year].get("data_file") is None:
+            if self.scan_data[scan_data_key][year_key].get("data_file") is None:
                 _logger.debug("We are skipping this year as the data is not available.")
             else:
                 # we missen de pkl file terwijl we wel een data file hebben. Genereer de foutmelding
                 _logger.warning(err)
                 _logger.warning("Run script with option '--statistics_to_xls'  first")
             stats_df_per_year = None
         return stats_df_per_year
@@ -1155,15 +1155,15 @@
             module_info = scan_data_analyses.module_info
 
             stats_df_per_year = {}
             last_year = None
             df_index_names = None
             for year in scan_data_per_year.keys():
                 df = self.get_plot_cache(
-                    scan_data_key=scan_data_key, plot_key=plot_key, year=year
+                    scan_data_key=scan_data_key, plot_key=plot_key, year_key=year
                 )
                 if df is not None:
                     stats_df_per_year[year] = df
                     last_year = year
                     df_index_names = list(df.index.names)
 
             if not self.english:
@@ -1229,15 +1229,17 @@
             subplot_adjust = plot_prop.get("subplot_adjust")
             reference_lines = plot_prop.get("reference_lines")
             if reference_lines is not None:
                 for ref_key, ref_prop in reference_lines.items():
                     stat_prop = self.statistics[ref_key]
                     scan_data_key = stat_prop.get("scan_data", self.default_scan)
                     ref_stat = self.get_plot_cache(
-                        scan_data_key=scan_data_key, plot_key=plot_key, year=last_year
+                        scan_data_key=scan_data_key,
+                        plot_key=plot_key,
+                        year_key=last_year,
                     )
                     reference_lines[ref_key]["data"] = ref_stat
 
             if plot_prop.get("use_breakdown_keys", False):
                 breakdown = self.breakdown_labels[plot_key]
                 renames = {v: k for k, v in breakdown.items()}
                 stats_df.rename(columns=renames, inplace=True)
```

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,16 @@
 
         years_to_add_to_plot_legend = list()
         for scan_year, scan_prop in scan_prop_per_year.items():
 
             if not scan_prop.get("do_it", True):
                 continue
             filename = scan_prop["data_file"]
-            years_to_add_to_plot_legend.append(scan_year)
+            legend_year_label = scan_prop.get("label", scan_year)
+            years_to_add_to_plot_legend.append(legend_year_label)
             if filename is None:
                 _logger.info(
                     f"File name for year {scan_year} was None. Skip it but add it to"
                     f"the plot legend"
                 )
                 continue
             internet_nl_filename = Path(filename)
```

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 2.0.1
+Version: 2.0.2
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-2.0.1/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-2.0.2/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-2.0.1/tox.ini` & `internetnl_domain_analyse-2.0.2/tox.ini`

 * *Files identical despite different names*

