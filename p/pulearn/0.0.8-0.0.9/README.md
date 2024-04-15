# Comparing `tmp/pulearn-0.0.8.tar.gz` & `tmp/pulearn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulearn-0.0.8.tar", last modified: Tue Aug 15 18:24:33 2023, max compression
+gzip compressed data, was "pulearn-0.0.9.tar", last modified: Mon Apr 15 09:47:56 2024, max compression
```

## Comparing `pulearn-0.0.8.tar` & `pulearn-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.189246 pulearn-0.0.8/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      425 2023-02-15 09:46:49.000000 pulearn-0.0.8/.codecov.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      344 2023-02-15 09:46:49.000000 pulearn-0.0.8/.coveragerc
--rw-r--r--   0 shaypalachy   (501) staff       (20)       36 2023-08-15 18:23:44.000000 pulearn-0.0.8/.fdignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2023-02-15 09:46:49.000000 pulearn-0.0.8/.gitattributes
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.177435 pulearn-0.0.8/.github/
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3209 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2768 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/CONTRIBUTING.md
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.178281 pulearn-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      356 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/ISSUE_TEMPLATE/Bug_report.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)       72 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/ISSUE_TEMPLATE/Feature_request.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)      525 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)      126 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/issue_template.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)      684 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/stale.yml
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.179670 pulearn-0.0.8/.github/workflows/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      786 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/workflows/checkdocs.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      765 2023-02-15 09:46:49.000000 pulearn-0.0.8/.github/workflows/lint.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1004 2023-08-15 18:23:44.000000 pulearn-0.0.8/.github/workflows/test.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1199 2023-02-15 09:46:49.000000 pulearn-0.0.8/.gitignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2023-08-15 18:23:44.000000 pulearn-0.0.8/.ignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1488 2023-02-15 09:46:49.000000 pulearn-0.0.8/ELKANOTO_LICENSE.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1457 2023-02-15 09:46:49.000000 pulearn-0.0.8/LICENSE.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)      656 2023-02-15 09:46:49.000000 pulearn-0.0.8/LICENSE_NOTICE.md
--rw-r--r--   0 shaypalachy   (501) staff       (20)       77 2023-02-15 09:46:49.000000 pulearn-0.0.8/MANIFEST.in
--rw-r--r--   0 shaypalachy   (501) staff       (20)    11057 2023-08-15 18:24:33.189428 pulearn-0.0.8/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)    10193 2023-08-15 18:23:44.000000 pulearn-0.0.8/README.rst
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.181263 pulearn-0.0.8/doc/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      141 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/README.md
--rwxr-xr-x   0 shaypalachy   (501) staff       (20)     2577 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/build.sh
--rw-r--r--   0 shaypalachy   (501) staff       (20)      106 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/build_w_pipenv.sh
--rw-r--r--   0 shaypalachy   (501) staff       (20)    15333 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/logo.png
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.182412 pulearn-0.0.8/doc/pulearn_template/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      113 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/pulearn_template/config.mako
--rw-r--r--   0 shaypalachy   (501) staff       (20)       48 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/pulearn_template/credits.mako
--rw-r--r--   0 shaypalachy   (501) staff       (20)      713 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/pulearn_template/head.mako
--rw-r--r--   0 shaypalachy   (501) staff       (20)      205 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/pulearn_template/logo.mako
--rw-r--r--   0 shaypalachy   (501) staff       (20)      220 2023-02-15 09:46:49.000000 pulearn-0.0.8/doc/sidebar_header.html
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.183183 pulearn-0.0.8/examples/
--rw-r--r--   0 shaypalachy   (501) staff       (20)     4971 2023-02-15 09:46:49.000000 pulearn-0.0.8/examples/BreastCancerElkanotoExample.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1364 2023-08-15 17:02:05.000000 pulearn-0.0.8/examples/ElkanotoPuClassifierExample.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.183723 pulearn-0.0.8/examples/datasets/
--rw-r--r--   0 shaypalachy   (501) staff       (20)    19889 2023-02-15 09:46:49.000000 pulearn-0.0.8/examples/datasets/breast-cancer-wisconsin.data
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.184339 pulearn-0.0.8/notebooks/
--rw-r--r--   0 shaypalachy   (501) staff       (20)   768567 2023-02-15 09:46:49.000000 pulearn-0.0.8/notebooks/bagging_blobs.ipynb
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.190418 pulearn-0.0.8/pulearn/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      435 2023-02-15 09:46:49.000000 pulearn-0.0.8/pulearn/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      497 2023-08-15 18:24:33.190535 pulearn-0.0.8/pulearn/_version.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    30115 2023-08-15 18:23:44.000000 pulearn-0.0.8/pulearn/bagging.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     9388 2023-08-15 17:02:05.000000 pulearn-0.0.8/pulearn/elkanoto.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3283 2023-02-15 09:46:49.000000 pulearn-0.0.8/pulearn/metrics.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.188110 pulearn-0.0.8/pulearn.egg-info/
--rw-r--r--   0 shaypalachy   (501) staff       (20)    11057 2023-08-15 18:24:32.000000 pulearn-0.0.8/pulearn.egg-info/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1222 2023-08-15 18:24:33.000000 pulearn-0.0.8/pulearn.egg-info/SOURCES.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-08-15 18:24:32.000000 pulearn-0.0.8/pulearn.egg-info/dependency_links.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      115 2023-08-15 18:24:32.000000 pulearn-0.0.8/pulearn.egg-info/requires.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-08-15 18:24:32.000000 pulearn-0.0.8/pulearn.egg-info/top_level.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)    85457 2023-02-15 09:46:49.000000 pulearn-0.0.8/pulearn_breast_cancer_f1_scores.png
--rw-r--r--   0 shaypalachy   (501) staff       (20)      154 2023-02-15 09:46:49.000000 pulearn-0.0.8/pytest.ini
--rw-r--r--   0 shaypalachy   (501) staff       (20)      384 2023-08-15 18:24:33.190043 pulearn-0.0.8/setup.cfg
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1822 2023-08-15 18:23:44.000000 pulearn-0.0.8/setup.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-08-15 18:24:33.189041 pulearn-0.0.8/tests/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2023-02-15 09:46:49.000000 pulearn-0.0.8/tests/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     5533 2023-02-15 09:46:49.000000 pulearn-0.0.8/tests/test_bagging.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3155 2023-02-15 09:46:49.000000 pulearn-0.0.8/tests/test_elkanoto.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1289 2023-02-15 09:46:49.000000 pulearn-0.0.8/tests/test_metrics.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    68611 2023-02-15 09:46:49.000000 pulearn-0.0.8/versioneer.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.443260 pulearn-0.0.9/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      425 2023-02-15 09:46:49.000000 pulearn-0.0.9/.codecov.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      344 2023-02-15 09:46:49.000000 pulearn-0.0.9/.coveragerc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       36 2023-08-15 18:23:44.000000 pulearn-0.0.9/.fdignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2023-02-15 09:46:49.000000 pulearn-0.0.9/.gitattributes
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.421343 pulearn-0.0.9/.github/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3209 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2768 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/CONTRIBUTING.md
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.422565 pulearn-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      356 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/ISSUE_TEMPLATE/Bug_report.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       72 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/ISSUE_TEMPLATE/Feature_request.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      525 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      126 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/issue_template.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      684 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/stale.yml
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.424409 pulearn-0.0.9/.github/workflows/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      786 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/workflows/checkdocs.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      765 2023-02-15 09:46:49.000000 pulearn-0.0.9/.github/workflows/lint.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1004 2023-08-15 18:23:44.000000 pulearn-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1199 2023-02-15 09:46:49.000000 pulearn-0.0.9/.gitignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2023-08-15 18:23:44.000000 pulearn-0.0.9/.ignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1488 2023-02-15 09:46:49.000000 pulearn-0.0.9/ELKANOTO_LICENSE.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1457 2023-02-15 09:46:49.000000 pulearn-0.0.9/LICENSE.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      656 2023-02-15 09:46:49.000000 pulearn-0.0.9/LICENSE_NOTICE.md
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       77 2023-02-15 09:46:49.000000 pulearn-0.0.9/MANIFEST.in
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    11057 2024-04-15 09:47:56.443453 pulearn-0.0.9/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    10193 2023-08-15 18:23:44.000000 pulearn-0.0.9/README.rst
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.428047 pulearn-0.0.9/doc/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      141 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/README.md
+-rwxr-xr-x   0 shaypalachy   (501) staff       (20)     2577 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/build.sh
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      106 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/build_w_pipenv.sh
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    15333 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/logo.png
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.430342 pulearn-0.0.9/doc/pulearn_template/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      113 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/pulearn_template/config.mako
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       48 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/pulearn_template/credits.mako
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      713 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/pulearn_template/head.mako
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      205 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/pulearn_template/logo.mako
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      220 2023-02-15 09:46:49.000000 pulearn-0.0.9/doc/sidebar_header.html
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.431800 pulearn-0.0.9/examples/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     4971 2023-02-15 09:46:49.000000 pulearn-0.0.9/examples/BreastCancerElkanotoExample.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1364 2023-08-15 17:02:05.000000 pulearn-0.0.9/examples/ElkanotoPuClassifierExample.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.432617 pulearn-0.0.9/examples/datasets/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    19889 2023-02-15 09:46:49.000000 pulearn-0.0.9/examples/datasets/breast-cancer-wisconsin.data
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.433506 pulearn-0.0.9/notebooks/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)   768567 2023-02-15 09:46:49.000000 pulearn-0.0.9/notebooks/bagging_blobs.ipynb
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.444376 pulearn-0.0.9/pulearn/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      435 2023-02-15 09:46:49.000000 pulearn-0.0.9/pulearn/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      497 2024-04-15 09:47:56.444431 pulearn-0.0.9/pulearn/_version.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    30085 2024-04-15 09:45:47.000000 pulearn-0.0.9/pulearn/bagging.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     9388 2023-08-15 17:02:05.000000 pulearn-0.0.9/pulearn/elkanoto.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3283 2023-02-15 09:46:49.000000 pulearn-0.0.9/pulearn/metrics.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.441515 pulearn-0.0.9/pulearn.egg-info/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    11057 2024-04-15 09:47:56.000000 pulearn-0.0.9/pulearn.egg-info/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1222 2024-04-15 09:47:56.000000 pulearn-0.0.9/pulearn.egg-info/SOURCES.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2024-04-15 09:47:56.000000 pulearn-0.0.9/pulearn.egg-info/dependency_links.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      115 2024-04-15 09:47:56.000000 pulearn-0.0.9/pulearn.egg-info/requires.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2024-04-15 09:47:56.000000 pulearn-0.0.9/pulearn.egg-info/top_level.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    85457 2023-02-15 09:46:49.000000 pulearn-0.0.9/pulearn_breast_cancer_f1_scores.png
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      154 2023-02-15 09:46:49.000000 pulearn-0.0.9/pytest.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      384 2024-04-15 09:47:56.444117 pulearn-0.0.9/setup.cfg
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1822 2023-08-15 18:23:44.000000 pulearn-0.0.9/setup.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2024-04-15 09:47:56.442818 pulearn-0.0.9/tests/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2023-02-15 09:46:49.000000 pulearn-0.0.9/tests/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     5513 2024-04-15 09:45:47.000000 pulearn-0.0.9/tests/test_bagging.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3155 2023-02-15 09:46:49.000000 pulearn-0.0.9/tests/test_elkanoto.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1289 2023-02-15 09:46:49.000000 pulearn-0.0.9/tests/test_metrics.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    68611 2023-02-15 09:46:49.000000 pulearn-0.0.9/versioneer.py
```

### Comparing `pulearn-0.0.8/.github/CODE_OF_CONDUCT.md` & `pulearn-0.0.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/CONTRIBUTING.md` & `pulearn-0.0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/PULL_REQUEST_TEMPLATE.md` & `pulearn-0.0.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/stale.yml` & `pulearn-0.0.9/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/workflows/checkdocs.yml` & `pulearn-0.0.9/.github/workflows/checkdocs.yml`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/workflows/lint.yml` & `pulearn-0.0.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.github/workflows/test.yml` & `pulearn-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/.gitignore` & `pulearn-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/ELKANOTO_LICENSE.md` & `pulearn-0.0.9/ELKANOTO_LICENSE.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/LICENSE.md` & `pulearn-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/LICENSE_NOTICE.md` & `pulearn-0.0.9/LICENSE_NOTICE.md`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/PKG-INFO` & `pulearn-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulearn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Positive-unlabeled learning with Python
 Home-page: https://pulearn.github.io/pulearn/
 Author: Shay Palachy
 Author-email: shaypal5@gmail.com
 License: BSD 3-Clause
 Keywords: classifier learning sklearn
 Platform: any
```

### Comparing `pulearn-0.0.8/README.rst` & `pulearn-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/doc/build.sh` & `pulearn-0.0.9/doc/build.sh`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/doc/logo.png` & `pulearn-0.0.9/doc/logo.png`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/doc/pulearn_template/head.mako` & `pulearn-0.0.9/doc/pulearn_template/head.mako`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/examples/BreastCancerElkanotoExample.py` & `pulearn-0.0.9/examples/BreastCancerElkanotoExample.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/examples/ElkanotoPuClassifierExample.py` & `pulearn-0.0.9/examples/ElkanotoPuClassifierExample.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/examples/datasets/breast-cancer-wisconsin.data` & `pulearn-0.0.9/examples/datasets/breast-cancer-wisconsin.data`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/notebooks/bagging_blobs.ipynb` & `pulearn-0.0.9/notebooks/bagging_blobs.ipynb`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/pulearn/bagging.py` & `pulearn-0.0.9/pulearn/bagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,27 +211,27 @@
 
     Warning: This class should not be used directly. Use derived classes
     instead.
     """
 
     @abstractmethod
     def __init__(self,
-                 base_estimator=None,
+                 estimator=None,
                  n_estimators=10,
                  max_samples=1.0,
                  max_features=1.0,
                  bootstrap=True,
                  bootstrap_features=False,
                  oob_score=True,
                  warm_start=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0):
         super(BaseBaggingPU, self).__init__(
-            base_estimator=base_estimator,
+            estimator=estimator,
             n_estimators=n_estimators)
 
         self.max_samples = max_samples
         self.max_features = max_features
         self.bootstrap = bootstrap
         self.bootstrap_features = bootstrap_features
         self.oob_score = oob_score
@@ -539,28 +539,28 @@
         Decision function computed with out-of-bag estimate on the training
         set. Positive data points, and perhaps some of the unlabeled,
         are left out during the bootstrap. In these cases,
         `oob_decision_function_` contains NaN.
 
     """
     def __init__(self,
-                 base_estimator=None,
+                 estimator=None,
                  n_estimators=10,
                  max_samples=1.0,
                  max_features=1.0,
                  bootstrap=True,
                  bootstrap_features=False,
                  oob_score=True,
                  warm_start=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0):
 
         super(BaggingPuClassifier, self).__init__(
-            base_estimator,
+            estimator,
             n_estimators=n_estimators,
             max_samples=max_samples,
             max_features=max_features,
             bootstrap=bootstrap,
             bootstrap_features=bootstrap_features,
             oob_score=oob_score,
             warm_start=warm_start,
@@ -738,15 +738,15 @@
             log_proba -= np.log(self.n_estimators)
 
             return log_proba
         # else, the base estimator has no predict_log_proba, so...
         return np.log(self.predict_proba(X))
 
     @available_if(
-        lambda self: hasattr(self.base_estimator, "decision_function"))
+        lambda self: hasattr(self.estimator, "decision_function"))
     def decision_function(self, X):
         """Average of the decision functions of the base classifiers.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape = [n_samples, n_features]
             The training input samples. Sparse matrices are accepted only if
```

### Comparing `pulearn-0.0.8/pulearn/elkanoto.py` & `pulearn-0.0.9/pulearn/elkanoto.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/pulearn/metrics.py` & `pulearn-0.0.9/pulearn/metrics.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/pulearn.egg-info/PKG-INFO` & `pulearn-0.0.9/pulearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulearn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Positive-unlabeled learning with Python
 Home-page: https://pulearn.github.io/pulearn/
 Author: Shay Palachy
 Author-email: shaypal5@gmail.com
 License: BSD 3-Clause
 Keywords: classifier learning sklearn
 Platform: any
```

### Comparing `pulearn-0.0.8/pulearn.egg-info/SOURCES.txt` & `pulearn-0.0.9/pulearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/pulearn_breast_cancer_f1_scores.png` & `pulearn-0.0.9/pulearn_breast_cancer_f1_scores.png`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/setup.py` & `pulearn-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/tests/test_bagging.py` & `pulearn-0.0.9/tests/test_bagging.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     with pytest.raises(NotFittedError):
         pu_estimator.predict_proba(X)
 
 
 @pytest.mark.parametrize("kwargs_n_fit_kwargs", [
     {'kwargs': {'verbose': 2, 'max_samples': 4}},
     {'kwargs': {'n_jobs': 2}},
-    {'kwargs': {'base_estimator': KNeighborsClassifier()}},
+    {'kwargs': {'estimator': KNeighborsClassifier()}},
     {
-        'kwargs': {'base_estimator': SVC()},
+        'kwargs': {'estimator': SVC()},
         'fit_kwargs': {'sample_weight': N_SAMPLES * [1]},
     },
     {'kwargs': {'bootstrap': False, 'oob_score': False}},
     {'kwargs': {'max_samples': 0.5}},
     {'kwargs': {'max_features': 2}},
 ])
 def test_bagging_various_kwargs(dataset, kwargs_n_fit_kwargs):
@@ -130,15 +130,15 @@
     pu_estimator.fit(X, y, **fit_kwargs)
     print(pu_estimator)
     print(pu_estimator.predict(X))
 
 
 @pytest.mark.parametrize("kwargs_n_fit_kwargs", [
     {
-        'kwargs': {'base_estimator': KNeighborsClassifier()},
+        'kwargs': {'estimator': KNeighborsClassifier()},
         'fit_kwargs': {'sample_weight': N_SAMPLES * [1]},
     },
     {'kwargs': {'bootstrap': False}},
     {'kwargs': {'max_samples': 1.2}},
     {'kwargs': {'max_features': 999999}},
     {'kwargs': {'oob_score': True, 'warm_start': True}},
     {'kwargs': {'n_estimators': -2}},
@@ -178,11 +178,11 @@
     pu_estimator.fit(X, y)
     with pytest.raises(ValueError):
         pu_estimator.predict_log_proba(X[:, :2])
 
 
 def test_bagging_bad_shape_decision_function(dataset):
     X, y = dataset
-    pu_estimator = BaggingPuClassifier(base_estimator=SVC())
+    pu_estimator = BaggingPuClassifier(estimator=SVC())
     pu_estimator.fit(X, y)
     with pytest.raises(ValueError):
         pu_estimator.decision_function(X[:, :2])
```

### Comparing `pulearn-0.0.8/tests/test_elkanoto.py` & `pulearn-0.0.9/tests/test_elkanoto.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/tests/test_metrics.py` & `pulearn-0.0.9/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pulearn-0.0.8/versioneer.py` & `pulearn-0.0.9/versioneer.py`

 * *Files identical despite different names*

