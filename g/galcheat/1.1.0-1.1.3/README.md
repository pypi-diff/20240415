# Comparing `tmp/galcheat-1.1.0.tar.gz` & `tmp/galcheat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galcheat-1.1.0.tar", last modified: Tue Apr  9 17:46:02 2024, max compression
+gzip compressed data, was "galcheat-1.1.3.tar", last modified: Mon Apr 15 20:45:08 2024, max compression
```

## Comparing `galcheat-1.1.0.tar` & `galcheat-1.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-09 17:45:52.000000 galcheat-1.1.0/.all-contributorsrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/check_style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-09 17:45:52.000000 galcheat-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:45:52.000000 galcheat-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 17:45:52.000000 galcheat-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:45:52.000000 galcheat-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-09 17:46:02.000000 galcheat-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-09 17:45:52.000000 galcheat-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/filter.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/helpers.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/survey.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/create-galaxy.md
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/heritage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   159096 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/images/galaxy.png
--rw-r--r--   0 runner    (1001) docker     (127)    89915 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/images/galcheat_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/parameters.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/CFHTLS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/COSMOS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/DES.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/Euclid_VIS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/HSC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/LSST.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/survey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 17:45:52.000000 galcheat-1.1.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/check_effective_wavelengths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/check_zeropoints.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 17:46:02.000000 galcheat-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 17:45:52.000000 galcheat-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 17:45:52.000000 galcheat-1.1.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-15 20:45:01.000000 galcheat-1.1.3/.all-contributorsrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.104835 galcheat-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.108835 galcheat-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-15 20:45:01.000000 galcheat-1.1.3/.github/workflows/check_style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-15 20:45:01.000000 galcheat-1.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 20:45:01.000000 galcheat-1.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-15 20:45:01.000000 galcheat-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-15 20:45:01.000000 galcheat-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-15 20:45:01.000000 galcheat-1.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 20:45:01.000000 galcheat-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-15 20:45:08.112836 galcheat-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-15 20:45:01.000000 galcheat-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.108835 galcheat-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.108835 galcheat-1.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/api/filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/api/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/api/survey.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/api/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.108835 galcheat-1.1.3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/guides/create-galaxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/guides/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/guides/heritage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.108835 galcheat-1.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   159096 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/images/galaxy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89915 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/images/galcheat_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/parameters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 20:45:01.000000 galcheat-1.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/galcheat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/galcheat/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/CFHTLS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/COSMOS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/DES.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/Euclid_VIS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/HSC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/data/LSST.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-15 20:45:01.000000 galcheat-1.1.3/galcheat/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/galcheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-15 20:45:08.000000 galcheat-1.1.3/galcheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 20:45:07.000000 galcheat-1.1.3/galcheat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-15 20:45:01.000000 galcheat-1.1.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-15 20:45:01.000000 galcheat-1.1.3/scripts/check_effective_wavelengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-15 20:45:01.000000 galcheat-1.1.3/scripts/check_zeropoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 20:45:01.000000 galcheat-1.1.3/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-15 20:45:08.116835 galcheat-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 20:45:01.000000 galcheat-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:45:08.112836 galcheat-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 20:45:01.000000 galcheat-1.1.3/tests/test_utilities.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galcheat-1.1.0/.all-contributorsrc` & `galcheat-1.1.3/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/.github/workflows/python-package.yml` & `galcheat-1.1.3/.github/workflows/python-package.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install the library and dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r scripts/requirements.txt
         pip install ".[dev]"
```

### Comparing `galcheat-1.1.0/.github/workflows/python-publish.yml` & `galcheat-1.1.3/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v3
       with:
-        python-version: '3.7'
+        python-version: '3.9'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install wheel
     - name: Build package
       run: |
         python setup.py sdist bdist_wheel
```

### Comparing `galcheat-1.1.0/.gitignore` & `galcheat-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/.pre-commit-config.yaml` & `galcheat-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/CONTRIBUTING.md` & `galcheat-1.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/LICENSE` & `galcheat-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/PKG-INFO` & `galcheat-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,141 +1,148 @@
 Metadata-Version: 2.1
 Name: galcheat
-Version: 1.1.0
+Version: 1.1.3
 Summary: Tiny library of galaxy surveys most useful parameters with units
 Home-page: https://github.com/aboucaud/galcheat
 Author: Alexandre Boucaud
 Author-email: aboucaud@apc.in2p3.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aboucaud/galcheat/issues
-Description: [**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
-        
-        <br>
-        <img src="docs/images/galcheat_logo.png" alt="galcheat" height=200px>
-        </p>
-        
-        [![Python package][gh-workflow-badge]][gh-workflow]
-        [![License][license-badge]](LICENSE)
-        ![Python supported versions][pyversion-badge]
-        [![PyPI][pypi-badge]][pypi]<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [gh-workflow]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml
-        [gh-workflow-badge]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml/badge.svg
-        [license-badge]: https://img.shields.io/github/license/aboucaud/galcheat?color=blue
-        [pyversion-badge]: https://img.shields.io/pypi/pyversions/galcheat?color=yellow&logo=pypi
-        [pypi-badge]: https://badge.fury.io/py/galcheat.svg
-        [pypi]: https://pypi.org/project/galcheat/
-        
-        Tiny package containing useful parameters from main galaxy surveys (**with units**).
-        
-        The goal of this project is to provide a Python library with minimal dependencies that centralises galaxy survey properties with adequate reference. Such information tends to be scattered in many places or is often copy/pasted without all of the relevant information like units or sources.
-        
-        The current parameters and the corresponding units are specified in the [documentation](https://aboucaud.github.io/galcheat/parameters.html)
-        
-        Getting started
-        ---------------
-        Install the latest version of the library
-        ```sh
-        pip install -U galcheat
-        ```
-        
-        CLI
-        ---
-        
-        Print the available surveys and associated filters
-        
-        ```sh
-        galcheat
-        ```
-        
-        ### Options
-        - **`-s <survey>`**: print information for a given survey
-        - **`--refs`**: print the source for each parameter
-        - **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
-        - **`-h, --help`**: get help
-        
-        ### Examples
-        ```sh
-        galcheat -s LSST         # LSST info
-        galcheat --refs          # all surveys info with refs
-        galcheat --refs -s HSC   # HSC info with refs
-        galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
-        ```
-        
-        API
-        ---
-        ```python
-        import galcheat
-        
-        # Start with the list of available surveys
-        galcheat.available_surveys
-        
-        # Retrieve a Survey instance
-        LSST = galcheat.get_survey("LSST")
-        
-        # List the available survey filters
-        LSST.available_filters
-        
-        # Pick a Filter instance
-        u_band = LSST.get_filter("u")
-        
-        # Both Survey and Filter objects have physical attributes
-        LSST.mirror_diameter
-        
-        u_band.full_exposure_time
-        
-        # These attributes are Astropy Quantity objects
-        # whose value can be retrieved in any desired unit
-        u_band.psf_fwhm.to_value('arcmin')
-        ```
-        
-        ## Contributing ✨
-        
-        This project was started in the context of the [BlendingToolKit (BTK)][github-btk] and [WeakLensingDeblending][github-wld] projects and has received contributions from these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-        
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="https://aboucaud.github.io"><img src="https://avatars.githubusercontent.com/u/3065310?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandre Boucaud</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=aboucaud" title="Code">💻</a> <a href="#ideas-aboucaud" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-aboucaud" title="Maintenance">🚧</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aaboucaud" title="Reviewed Pull Requests">👀</a></td>
-            <td align="center"><a href="https://github.com/mpaillassa"><img src="https://avatars.githubusercontent.com/u/9745094?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mpaillassa</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=mpaillassa" title="Code">💻</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Ampaillassa" title="Reviewed Pull Requests">👀</a> <a href="#data-mpaillassa" title="Data">🔣</a></td>
-            <td align="center"><a href="https://ismael-mendoza.github.io/"><img src="https://avatars.githubusercontent.com/u/11745764?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismael Mendoza</b></sub></a><br /><a href="#ideas-ismael-mendoza" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aismael-mendoza" title="Reviewed Pull Requests">👀</a> <a href="#data-ismael-mendoza" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/HironaoMiyatake"><img src="https://avatars.githubusercontent.com/u/1507529?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hironao Miyatake</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=HironaoMiyatake" title="Code">💻</a> <a href="#data-HironaoMiyatake" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/aguinot"><img src="https://avatars.githubusercontent.com/u/39480528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Axel Guinot</b></sub></a><br /><a href="#data-aguinot" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/thuiop"><img src="https://avatars.githubusercontent.com/u/1338337?v=4?s=100" width="100px;" alt=""/><br /><sub><b>thuiop</b></sub></a><br /><a href="#ideas-thuiop" title="Ideas, Planning, & Feedback">🤔</a></td>
-            <td align="center"><a href="https://remyjoseph.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/16084926?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rémy Joseph</b></sub></a><br /><a href="#ideas-herjy" title="Ideas, Planning, & Feedback">🤔</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-restore -->
-        <!-- prettier-ignore-end -->
-        
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
-        This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
-        
-        A number is missing? An error slipped into the files? A survey is not included in the list and you can provide the relevant information or some of it?
-        
-        Contributions of any kind are welcome! Head over to the [contributing guidelines](CONTRIBUTING.md) to learn how to participate into making this library more robust and complete.
-        
-        [github-wld]: https://github.com/LSSTDESC/WeakLensingDeblending
-        [github-btk]: https://github.com/LSSTDESC/BlendingToolKit
-        
-        License
-        -------
-        This project is developed under an MIT-license. See [LICENSE file](LICENSE) for more information.
-        
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: scripts
+License-File: LICENSE
+
+[**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
+
+<br>
+<img src="docs/images/galcheat_logo.png" alt="galcheat" height=200px>
+</p>
+
+[![Python package][gh-workflow-badge]][gh-workflow]
+[![License][license-badge]](LICENSE)
+![Python supported versions][pyversion-badge]
+[![PyPI][pypi-badge]][pypi]<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[gh-workflow]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml
+[gh-workflow-badge]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml/badge.svg
+[license-badge]: https://img.shields.io/github/license/aboucaud/galcheat?color=blue
+[pyversion-badge]: https://img.shields.io/pypi/pyversions/galcheat?color=yellow&logo=pypi
+[pypi-badge]: https://badge.fury.io/py/galcheat.svg
+[pypi]: https://pypi.org/project/galcheat/
+
+Tiny package containing useful parameters from main galaxy surveys (**with units**).
+
+The goal of this project is to provide a Python library with minimal dependencies that centralises galaxy survey properties with adequate reference. Such information tends to be scattered in many places or is often copy/pasted without all of the relevant information like units or sources.
+
+The current parameters and the corresponding units are specified in the [documentation](https://aboucaud.github.io/galcheat/parameters.html)
+
+Getting started
+---------------
+Install the latest version of the library
+```sh
+pip install -U galcheat
+```
+
+CLI
+---
+
+Print the available surveys and associated filters
+
+```sh
+galcheat
+```
+
+### Options
+- **`-s <survey>`**: print information for a given survey
+- **`--refs`**: print the source for each parameter
+- **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
+- **`-h, --help`**: get help
+
+### Examples
+```sh
+galcheat -s LSST         # LSST info
+galcheat --refs          # all surveys info with refs
+galcheat --refs -s HSC   # HSC info with refs
+galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
+```
+
+API
+---
+```python
+import galcheat
+
+# Start with the list of available surveys
+galcheat.available_surveys
+
+# Retrieve a Survey instance
+LSST = galcheat.get_survey("LSST")
+
+# List the available survey filters
+LSST.available_filters
+
+# Pick a Filter instance
+u_band = LSST.get_filter("u")
+
+# Both Survey and Filter objects have physical attributes
+LSST.mirror_diameter
+
+u_band.full_exposure_time
+
+# These attributes are Astropy Quantity objects
+# whose value can be retrieved in any desired unit
+u_band.psf_fwhm.to_value('arcmin')
+```
+
+## Contributing ✨
+
+This project was started in the context of the [BlendingToolKit (BTK)][github-btk] and [WeakLensingDeblending][github-wld] projects and has received contributions from these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="https://aboucaud.github.io"><img src="https://avatars.githubusercontent.com/u/3065310?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandre Boucaud</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=aboucaud" title="Code">💻</a> <a href="#ideas-aboucaud" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-aboucaud" title="Maintenance">🚧</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aaboucaud" title="Reviewed Pull Requests">👀</a></td>
+    <td align="center"><a href="https://github.com/mpaillassa"><img src="https://avatars.githubusercontent.com/u/9745094?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mpaillassa</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=mpaillassa" title="Code">💻</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Ampaillassa" title="Reviewed Pull Requests">👀</a> <a href="#data-mpaillassa" title="Data">🔣</a></td>
+    <td align="center"><a href="https://ismael-mendoza.github.io/"><img src="https://avatars.githubusercontent.com/u/11745764?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismael Mendoza</b></sub></a><br /><a href="#ideas-ismael-mendoza" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aismael-mendoza" title="Reviewed Pull Requests">👀</a> <a href="#data-ismael-mendoza" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/HironaoMiyatake"><img src="https://avatars.githubusercontent.com/u/1507529?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hironao Miyatake</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=HironaoMiyatake" title="Code">💻</a> <a href="#data-HironaoMiyatake" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/aguinot"><img src="https://avatars.githubusercontent.com/u/39480528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Axel Guinot</b></sub></a><br /><a href="#data-aguinot" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/thuiop"><img src="https://avatars.githubusercontent.com/u/1338337?v=4?s=100" width="100px;" alt=""/><br /><sub><b>thuiop</b></sub></a><br /><a href="#ideas-thuiop" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://remyjoseph.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/16084926?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rémy Joseph</b></sub></a><br /><a href="#ideas-herjy" title="Ideas, Planning, & Feedback">🤔</a></td>
+  </tr>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
+
+A number is missing? An error slipped into the files? A survey is not included in the list and you can provide the relevant information or some of it?
+
+Contributions of any kind are welcome! Head over to the [contributing guidelines](CONTRIBUTING.md) to learn how to participate into making this library more robust and complete.
+
+[github-wld]: https://github.com/LSSTDESC/WeakLensingDeblending
+[github-btk]: https://github.com/LSSTDESC/BlendingToolKit
+
+License
+-------
+This project is developed under an MIT-license. See [LICENSE file](LICENSE) for more information.
+
+
```

### Comparing `galcheat-1.1.0/README.md` & `galcheat-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/guides/create-galaxy.md` & `galcheat-1.1.3/docs/guides/create-galaxy.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/guides/getting-started.md` & `galcheat-1.1.3/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/guides/heritage.md` & `galcheat-1.1.3/docs/guides/heritage.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/images/galaxy.png` & `galcheat-1.1.3/docs/images/galaxy.png`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/images/galcheat_logo.png` & `galcheat-1.1.3/docs/images/galcheat_logo.png`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/index.md` & `galcheat-1.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/docs/parameters.md` & `galcheat-1.1.3/docs/parameters.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/__init__.py` & `galcheat-1.1.3/galcheat/__init__.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/__main__.py` & `galcheat-1.1.3/galcheat/__main__.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/CFHTLS.yaml` & `galcheat-1.1.3/galcheat/data/CFHTLS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/COSMOS.yaml` & `galcheat-1.1.3/galcheat/data/COSMOS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/DES.yaml` & `galcheat-1.1.3/galcheat/data/DES.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/Euclid_VIS.yaml` & `galcheat-1.1.3/galcheat/data/Euclid_VIS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/HSC.yaml` & `galcheat-1.1.3/galcheat/data/HSC.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/data/LSST.yaml` & `galcheat-1.1.3/galcheat/data/LSST.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/filter.py` & `galcheat-1.1.3/galcheat/filter.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/helpers.py` & `galcheat-1.1.3/galcheat/helpers.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/rich.py` & `galcheat-1.1.3/galcheat/rich.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,38 +53,38 @@
 def _survey_table(survey):
     from rich.table import Table
 
     survey_info = Table.grid()
     survey_info.add_column(justify="left")
     survey_info.add_column(justify="left")
 
-    survey_info.add_row("Pixel scale: ", f"{survey.pixel_scale}")
-    survey_info.add_row("Mirror diameter: ", f"{survey.mirror_diameter}")
+    survey_info.add_row("Pixel scale: ", f"{survey.pixel_scale:.3f}")
+    survey_info.add_row("Mirror diameter: ", f"{survey.mirror_diameter:.2f}")
     survey_info.add_row("Effective area: ", f"{survey.effective_area:.2f}")
     survey_info.add_row("Obscuration: ", f"{survey.obscuration:.2f}")
-    survey_info.add_row("Gain: ", f"{survey.gain}")
-    survey_info.add_row("Zeropoint airmass: ", f"{survey.zeropoint_airmass}")
+    survey_info.add_row("Gain: ", f"{survey.gain:.2f}")
+    survey_info.add_row("Zeropoint airmass: ", f"{survey.zeropoint_airmass:.1f}")
     survey_info.add_row("Available filters: ", ", ".join(survey.available_filters))
 
     return survey_info
 
 
 def _filter_panel(filter):
     from rich.panel import Panel
     from rich.table import Table
 
     filter_info = Table.grid()
     filter_info.add_column(justify="left")
     filter_info.add_column(justify="left")
 
-    filter_info.add_row("PSF FWHM: ", f"{filter.psf_fwhm}")
-    filter_info.add_row("Zeropoint: ", f"{filter.zeropoint}")
+    filter_info.add_row("PSF FWHM: ", f"{filter.psf_fwhm:.2f}")
+    filter_info.add_row("Zeropoint: ", f"{filter.zeropoint:.2f}")
     filter_info.add_row("Sky brightness: ", f"{filter.sky_brightness:.2f}")
-    filter_info.add_row("Full exposure time: ", f"{filter.full_exposure_time}")
-    filter_info.add_row("Effective wavelength: ", f"{filter.effective_wavelength}")
+    filter_info.add_row("Full exposure time: ", f"{filter.full_exposure_time:0.0f}")
+    filter_info.add_row("Effective wavelength: ", f"{filter.effective_wavelength:.1f}")
 
     return Panel(
         filter_info,
         padding=0,
         expand=False,
         title=f"[b]{filter.name}[/]",
         title_align="left",
```

### Comparing `galcheat-1.1.0/galcheat/survey.py` & `galcheat-1.1.3/galcheat/survey.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat/utilities.py` & `galcheat-1.1.3/galcheat/utilities.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/galcheat.egg-info/PKG-INFO` & `galcheat-1.1.3/galcheat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,141 +1,148 @@
 Metadata-Version: 2.1
 Name: galcheat
-Version: 1.1.0
+Version: 1.1.3
 Summary: Tiny library of galaxy surveys most useful parameters with units
 Home-page: https://github.com/aboucaud/galcheat
 Author: Alexandre Boucaud
 Author-email: aboucaud@apc.in2p3.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aboucaud/galcheat/issues
-Description: [**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
-        
-        <br>
-        <img src="docs/images/galcheat_logo.png" alt="galcheat" height=200px>
-        </p>
-        
-        [![Python package][gh-workflow-badge]][gh-workflow]
-        [![License][license-badge]](LICENSE)
-        ![Python supported versions][pyversion-badge]
-        [![PyPI][pypi-badge]][pypi]<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [gh-workflow]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml
-        [gh-workflow-badge]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml/badge.svg
-        [license-badge]: https://img.shields.io/github/license/aboucaud/galcheat?color=blue
-        [pyversion-badge]: https://img.shields.io/pypi/pyversions/galcheat?color=yellow&logo=pypi
-        [pypi-badge]: https://badge.fury.io/py/galcheat.svg
-        [pypi]: https://pypi.org/project/galcheat/
-        
-        Tiny package containing useful parameters from main galaxy surveys (**with units**).
-        
-        The goal of this project is to provide a Python library with minimal dependencies that centralises galaxy survey properties with adequate reference. Such information tends to be scattered in many places or is often copy/pasted without all of the relevant information like units or sources.
-        
-        The current parameters and the corresponding units are specified in the [documentation](https://aboucaud.github.io/galcheat/parameters.html)
-        
-        Getting started
-        ---------------
-        Install the latest version of the library
-        ```sh
-        pip install -U galcheat
-        ```
-        
-        CLI
-        ---
-        
-        Print the available surveys and associated filters
-        
-        ```sh
-        galcheat
-        ```
-        
-        ### Options
-        - **`-s <survey>`**: print information for a given survey
-        - **`--refs`**: print the source for each parameter
-        - **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
-        - **`-h, --help`**: get help
-        
-        ### Examples
-        ```sh
-        galcheat -s LSST         # LSST info
-        galcheat --refs          # all surveys info with refs
-        galcheat --refs -s HSC   # HSC info with refs
-        galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
-        ```
-        
-        API
-        ---
-        ```python
-        import galcheat
-        
-        # Start with the list of available surveys
-        galcheat.available_surveys
-        
-        # Retrieve a Survey instance
-        LSST = galcheat.get_survey("LSST")
-        
-        # List the available survey filters
-        LSST.available_filters
-        
-        # Pick a Filter instance
-        u_band = LSST.get_filter("u")
-        
-        # Both Survey and Filter objects have physical attributes
-        LSST.mirror_diameter
-        
-        u_band.full_exposure_time
-        
-        # These attributes are Astropy Quantity objects
-        # whose value can be retrieved in any desired unit
-        u_band.psf_fwhm.to_value('arcmin')
-        ```
-        
-        ## Contributing ✨
-        
-        This project was started in the context of the [BlendingToolKit (BTK)][github-btk] and [WeakLensingDeblending][github-wld] projects and has received contributions from these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-        
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="https://aboucaud.github.io"><img src="https://avatars.githubusercontent.com/u/3065310?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandre Boucaud</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=aboucaud" title="Code">💻</a> <a href="#ideas-aboucaud" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-aboucaud" title="Maintenance">🚧</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aaboucaud" title="Reviewed Pull Requests">👀</a></td>
-            <td align="center"><a href="https://github.com/mpaillassa"><img src="https://avatars.githubusercontent.com/u/9745094?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mpaillassa</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=mpaillassa" title="Code">💻</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Ampaillassa" title="Reviewed Pull Requests">👀</a> <a href="#data-mpaillassa" title="Data">🔣</a></td>
-            <td align="center"><a href="https://ismael-mendoza.github.io/"><img src="https://avatars.githubusercontent.com/u/11745764?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismael Mendoza</b></sub></a><br /><a href="#ideas-ismael-mendoza" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aismael-mendoza" title="Reviewed Pull Requests">👀</a> <a href="#data-ismael-mendoza" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/HironaoMiyatake"><img src="https://avatars.githubusercontent.com/u/1507529?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hironao Miyatake</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=HironaoMiyatake" title="Code">💻</a> <a href="#data-HironaoMiyatake" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/aguinot"><img src="https://avatars.githubusercontent.com/u/39480528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Axel Guinot</b></sub></a><br /><a href="#data-aguinot" title="Data">🔣</a></td>
-            <td align="center"><a href="https://github.com/thuiop"><img src="https://avatars.githubusercontent.com/u/1338337?v=4?s=100" width="100px;" alt=""/><br /><sub><b>thuiop</b></sub></a><br /><a href="#ideas-thuiop" title="Ideas, Planning, & Feedback">🤔</a></td>
-            <td align="center"><a href="https://remyjoseph.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/16084926?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rémy Joseph</b></sub></a><br /><a href="#ideas-herjy" title="Ideas, Planning, & Feedback">🤔</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-restore -->
-        <!-- prettier-ignore-end -->
-        
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
-        This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
-        
-        A number is missing? An error slipped into the files? A survey is not included in the list and you can provide the relevant information or some of it?
-        
-        Contributions of any kind are welcome! Head over to the [contributing guidelines](CONTRIBUTING.md) to learn how to participate into making this library more robust and complete.
-        
-        [github-wld]: https://github.com/LSSTDESC/WeakLensingDeblending
-        [github-btk]: https://github.com/LSSTDESC/BlendingToolKit
-        
-        License
-        -------
-        This project is developed under an MIT-license. See [LICENSE file](LICENSE) for more information.
-        
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: scripts
+License-File: LICENSE
+
+[**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
+
+<br>
+<img src="docs/images/galcheat_logo.png" alt="galcheat" height=200px>
+</p>
+
+[![Python package][gh-workflow-badge]][gh-workflow]
+[![License][license-badge]](LICENSE)
+![Python supported versions][pyversion-badge]
+[![PyPI][pypi-badge]][pypi]<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[gh-workflow]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml
+[gh-workflow-badge]: https://github.com/aboucaud/galcheat/actions/workflows/python-package.yml/badge.svg
+[license-badge]: https://img.shields.io/github/license/aboucaud/galcheat?color=blue
+[pyversion-badge]: https://img.shields.io/pypi/pyversions/galcheat?color=yellow&logo=pypi
+[pypi-badge]: https://badge.fury.io/py/galcheat.svg
+[pypi]: https://pypi.org/project/galcheat/
+
+Tiny package containing useful parameters from main galaxy surveys (**with units**).
+
+The goal of this project is to provide a Python library with minimal dependencies that centralises galaxy survey properties with adequate reference. Such information tends to be scattered in many places or is often copy/pasted without all of the relevant information like units or sources.
+
+The current parameters and the corresponding units are specified in the [documentation](https://aboucaud.github.io/galcheat/parameters.html)
+
+Getting started
+---------------
+Install the latest version of the library
+```sh
+pip install -U galcheat
+```
+
+CLI
+---
+
+Print the available surveys and associated filters
+
+```sh
+galcheat
+```
+
+### Options
+- **`-s <survey>`**: print information for a given survey
+- **`--refs`**: print the source for each parameter
+- **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
+- **`-h, --help`**: get help
+
+### Examples
+```sh
+galcheat -s LSST         # LSST info
+galcheat --refs          # all surveys info with refs
+galcheat --refs -s HSC   # HSC info with refs
+galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
+```
+
+API
+---
+```python
+import galcheat
+
+# Start with the list of available surveys
+galcheat.available_surveys
+
+# Retrieve a Survey instance
+LSST = galcheat.get_survey("LSST")
+
+# List the available survey filters
+LSST.available_filters
+
+# Pick a Filter instance
+u_band = LSST.get_filter("u")
+
+# Both Survey and Filter objects have physical attributes
+LSST.mirror_diameter
+
+u_band.full_exposure_time
+
+# These attributes are Astropy Quantity objects
+# whose value can be retrieved in any desired unit
+u_band.psf_fwhm.to_value('arcmin')
+```
+
+## Contributing ✨
+
+This project was started in the context of the [BlendingToolKit (BTK)][github-btk] and [WeakLensingDeblending][github-wld] projects and has received contributions from these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="https://aboucaud.github.io"><img src="https://avatars.githubusercontent.com/u/3065310?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandre Boucaud</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=aboucaud" title="Code">💻</a> <a href="#ideas-aboucaud" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-aboucaud" title="Maintenance">🚧</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aaboucaud" title="Reviewed Pull Requests">👀</a></td>
+    <td align="center"><a href="https://github.com/mpaillassa"><img src="https://avatars.githubusercontent.com/u/9745094?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mpaillassa</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=mpaillassa" title="Code">💻</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Ampaillassa" title="Reviewed Pull Requests">👀</a> <a href="#data-mpaillassa" title="Data">🔣</a></td>
+    <td align="center"><a href="https://ismael-mendoza.github.io/"><img src="https://avatars.githubusercontent.com/u/11745764?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismael Mendoza</b></sub></a><br /><a href="#ideas-ismael-mendoza" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/aboucaud/galcheat/pulls?q=is%3Apr+reviewed-by%3Aismael-mendoza" title="Reviewed Pull Requests">👀</a> <a href="#data-ismael-mendoza" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/HironaoMiyatake"><img src="https://avatars.githubusercontent.com/u/1507529?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hironao Miyatake</b></sub></a><br /><a href="https://github.com/aboucaud/galcheat/commits?author=HironaoMiyatake" title="Code">💻</a> <a href="#data-HironaoMiyatake" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/aguinot"><img src="https://avatars.githubusercontent.com/u/39480528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Axel Guinot</b></sub></a><br /><a href="#data-aguinot" title="Data">🔣</a></td>
+    <td align="center"><a href="https://github.com/thuiop"><img src="https://avatars.githubusercontent.com/u/1338337?v=4?s=100" width="100px;" alt=""/><br /><sub><b>thuiop</b></sub></a><br /><a href="#ideas-thuiop" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://remyjoseph.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/16084926?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rémy Joseph</b></sub></a><br /><a href="#ideas-herjy" title="Ideas, Planning, & Feedback">🤔</a></td>
+  </tr>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
+
+A number is missing? An error slipped into the files? A survey is not included in the list and you can provide the relevant information or some of it?
+
+Contributions of any kind are welcome! Head over to the [contributing guidelines](CONTRIBUTING.md) to learn how to participate into making this library more robust and complete.
+
+[github-wld]: https://github.com/LSSTDESC/WeakLensingDeblending
+[github-btk]: https://github.com/LSSTDESC/BlendingToolKit
+
+License
+-------
+This project is developed under an MIT-license. See [LICENSE file](LICENSE) for more information.
+
+
```

### Comparing `galcheat-1.1.0/galcheat.egg-info/SOURCES.txt` & `galcheat-1.1.3/galcheat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/mkdocs.yml` & `galcheat-1.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/scripts/check_effective_wavelengths.py` & `galcheat-1.1.3/scripts/check_effective_wavelengths.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/scripts/check_zeropoints.py` & `galcheat-1.1.3/scripts/check_zeropoints.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.1.0/setup.cfg` & `galcheat-1.1.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 platforms = any
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering :: Astronomy
 	Development Status :: 3 - Alpha
 project_urls = 
 	Bug Tracker = https://github.com/aboucaud/galcheat/issues
 
 [options]
 zip_safe = False
@@ -39,19 +42,21 @@
 
 [options.extras_require]
 dev = 
 	pre-commit>=2.17
 	pytest>=6.0
 	pytest-cov>=3.0
 	pytest_astropy_header>=0.2
+	rich>=13.7
+docs = 
 	mkdocs>=1.2
 	mkdocs-material>=8.2
 	mkdocstrings>=0.18
+	mkdocstrings-python>=1.9
 	pytkdocs[numpy-style]>=0.16
-	rich>=13.7
 scripts = 
 	speclite>=0.15
 
 [options.package_data]
 galcheat = data/*
 
 [bdist_wheel]
```

### Comparing `galcheat-1.1.0/tests/test_utilities.py` & `galcheat-1.1.3/tests/test_utilities.py`

 * *Files identical despite different names*

