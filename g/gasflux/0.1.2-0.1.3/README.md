# Comparing `tmp/gasflux-0.1.2.tar.gz` & `tmp/gasflux-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasflux-0.1.2.tar", last modified: Sun Apr 14 15:09:30 2024, max compression
+gzip compressed data, was "gasflux-0.1.3.tar", last modified: Sun Apr 14 23:17:27 2024, max compression
```

## Comparing `gasflux-0.1.2.tar` & `gasflux-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.552122 gasflux-0.1.2/.github/
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.552122 gasflux-0.1.2/.github/workflows/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1641 2024-04-14 13:40:10.000000 gasflux-0.1.2/.github/workflows/CI.yml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      439 2024-04-14 13:40:10.000000 gasflux-0.1.2/.github/workflows/python-semantic-release.yml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1913 2024-04-14 14:28:45.000000 gasflux-0.1.2/.gitignore
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2982 2024-04-14 13:40:10.000000 gasflux-0.1.2/.pre-commit-config.yaml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     5646 2024-04-14 15:09:18.000000 gasflux-0.1.2/CHANGELOG.md
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    35184 2024-04-14 13:40:10.000000 gasflux-0.1.2/LICENSE
--rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6493 2024-04-14 15:09:30.556122 gasflux-0.1.2/PKG-INFO
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     5013 2024-04-14 13:40:10.000000 gasflux-0.1.2/README.md
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      132 2024-04-14 14:28:45.000000 gasflux-0.1.2/dev-requirements.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1098 2024-04-14 14:22:57.000000 gasflux-0.1.2/mass_balance_template.html
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     3000 2024-04-14 15:09:02.000000 gasflux-0.1.2/pyproject.toml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      351 2024-04-14 13:40:10.000000 gasflux-0.1.2/requirements.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       38 2024-04-14 15:09:30.556122 gasflux-0.1.2/setup.cfg
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.552122 gasflux-0.1.2/src/
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.552122 gasflux-0.1.2/src/gasflux/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      469 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/__init__.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1333 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/background.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     8544 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/cli.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2170 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/gas.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1260 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/gasflux_config.yaml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    14691 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/generate_test_data.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4688 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/interpolation.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2463 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/ml.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    13985 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/plotting.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4391 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/pre_processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    26870 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    10582 2024-04-14 13:40:10.000000 gasflux-0.1.2/src/gasflux/processing_pipelines.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4246 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/reporting.py
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/src/gasflux/resources/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)   237042 2024-04-03 14:12:12.000000 gasflux-0.1.2/src/gasflux/resources/model.pkl
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/src/gasflux/templates/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1098 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/templates/mass_balance_template.html
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/src/gasflux/testdata/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)   167026 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/testdata/exampledata.csv
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2409 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/testdata/testconfig.yaml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)   349755 2024-04-14 14:28:45.000000 gasflux-0.1.2/src/gasflux/testdata/testdata.csv
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/src/gasflux.egg-info/
--rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6493 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/PKG-INFO
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1067 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/SOURCES.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        1 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/dependency_links.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       49 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/entry_points.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      403 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/requires.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        8 2024-04-14 15:09:30.000000 gasflux-0.1.2/src/gasflux.egg-info/top_level.txt
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/tests/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-03 14:12:12.000000 gasflux-0.1.2/tests/__init__.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     7565 2024-04-14 14:28:45.000000 gasflux-0.1.2/tests/test_processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2291 2024-04-14 14:28:45.000000 gasflux-0.1.2/tests/test_processing_pipelines.py
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 15:09:30.556122 gasflux-0.1.2/tools/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4510 2024-04-14 13:40:10.000000 gasflux-0.1.2/tools/mono_flight_splitter.py
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.451517 gasflux-0.1.3/
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/.github/
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/.github/workflows/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1641 2024-04-14 22:53:13.000000 gasflux-0.1.3/.github/workflows/CI.yml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      949 2024-04-14 23:14:12.000000 gasflux-0.1.3/.github/workflows/build-release.yml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      691 2024-04-14 23:15:46.000000 gasflux-0.1.3/.github/workflows/deploy.yml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      489 2024-04-14 23:15:42.000000 gasflux-0.1.3/.github/workflows/release.yml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1913 2024-04-14 20:55:42.000000 gasflux-0.1.3/.gitignore
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     2982 2024-04-14 13:40:10.000000 gasflux-0.1.3/.pre-commit-config.yaml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     5646 2024-04-14 23:13:16.000000 gasflux-0.1.3/CHANGELOG.md
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)    35184 2024-04-14 20:55:42.000000 gasflux-0.1.3/LICENSE
+-rw-r--r--   0 a71546jm  (1001) docker     (139)     6573 2024-04-14 23:17:27.451517 gasflux-0.1.3/PKG-INFO
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     5013 2024-04-14 20:55:42.000000 gasflux-0.1.3/README.md
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      149 2024-04-14 22:53:13.000000 gasflux-0.1.3/dev-requirements.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1098 2024-04-14 20:55:42.000000 gasflux-0.1.3/mass_balance_template.html
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     3061 2024-04-14 23:13:16.000000 gasflux-0.1.3/pyproject.toml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      351 2024-04-14 20:55:42.000000 gasflux-0.1.3/requirements.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)       38 2024-04-14 23:17:27.451517 gasflux-0.1.3/setup.cfg
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/gasflux/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      469 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/__init__.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1333 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/background.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     8544 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/cli.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     2170 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/gas.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1260 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/gasflux_config.yaml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)    14691 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/generate_test_data.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     4688 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/interpolation.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     2463 2024-04-14 13:40:10.000000 gasflux-0.1.3/src/gasflux/ml.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)    13985 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/plotting.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     4391 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/pre_processing.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)    26870 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/processing.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)    10582 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/processing_pipelines.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     4246 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/reporting.py
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/gasflux/resources/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)   237042 2024-04-03 14:12:12.000000 gasflux-0.1.3/src/gasflux/resources/model.pkl
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/gasflux/templates/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1098 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/templates/mass_balance_template.html
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/gasflux/testdata/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)   167026 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/testdata/exampledata.csv
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     2409 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/testdata/testconfig.yaml
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)   349755 2024-04-14 20:55:42.000000 gasflux-0.1.3/src/gasflux/testdata/testdata.csv
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/src/gasflux.egg-info/
+-rw-r--r--   0 a71546jm  (1001) docker     (139)     6573 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/PKG-INFO
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     1116 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/SOURCES.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)        1 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/dependency_links.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)       49 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/entry_points.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)      420 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/requires.txt
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)        8 2024-04-14 23:17:27.000000 gasflux-0.1.3/src/gasflux.egg-info/top_level.txt
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/tests/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)        0 2024-04-03 14:12:12.000000 gasflux-0.1.3/tests/__init__.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     7565 2024-04-14 20:55:42.000000 gasflux-0.1.3/tests/test_processing.py
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     2291 2024-04-14 20:55:42.000000 gasflux-0.1.3/tests/test_processing_pipelines.py
+drwxrwxr-x   0 a71546jm  (1001) docker     (139)        0 2024-04-14 23:17:27.447517 gasflux-0.1.3/tools/
+-rw-rw-r--   0 a71546jm  (1001) docker     (139)     4510 2024-04-14 13:40:10.000000 gasflux-0.1.3/tools/mono_flight_splitter.py
```

### Comparing `gasflux-0.1.2/.github/workflows/CI.yml` & `gasflux-0.1.3/.github/workflows/CI.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 1
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
 
       - name: Install Dependencies
         run: pip install -r requirements.txt
         if: steps.cache.outputs.cache-hit != 'true'
@@ -48,15 +48,15 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 1
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           # architecture: x64
 
       - name: Install Dependencies
         run: pip install -r requirements.txt
         if: steps.cache.outputs.cache-hit != 'true'
```

### Comparing `gasflux-0.1.2/.gitignore` & `gasflux-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/.pre-commit-config.yaml` & `gasflux-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/CHANGELOG.md` & `gasflux-0.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/LICENSE` & `gasflux-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/PKG-INFO` & `gasflux-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gasflux
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to calculate gas emissions fluxes from natural and anthropogenic sources
 Author-email: Jamie McQuilkin <jamie.mcquilkin@gmail.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://gasflux.github.io
 Project-URL: Bug Tracker, https://github.com/gasflux/gasflux/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama==0.4.6
 Requires-Dist: geopandas==0.14.3
 Requires-Dist: geopy==2.4.1
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: joblib==1.3.2
@@ -24,24 +24,26 @@
 Requires-Dist: pytest==8.1.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: scikit-gstat==1.0.16
 Requires-Dist: scipy==1.12.0
 Requires-Dist: setuptools==69.2.0
 Requires-Dist: simplekml==1.3.6
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pigar; extra == "dev"
 Requires-Dist: pip>23.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: safety; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
 
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Tests](https://github.com/gasflux/gasflux/workflows/CI/badge.svg)](https://github.com/gasflux/gasflux/actions?query=workflow%3A%22CI%22)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
```

### Comparing `gasflux-0.1.2/README.md` & `gasflux-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/mass_balance_template.html` & `gasflux-0.1.3/mass_balance_template.html`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/pyproject.toml` & `gasflux-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "gasflux"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package to calculate gas emissions fluxes from natural and anthropogenic sources"
 authors = [{ name = "Jamie McQuilkin", email = "jamie.mcquilkin@gmail.com" }]
 license = { text = "AGPL-3.0" }
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 
 dynamic = ["dependencies", "optional-dependencies"]
 
 [project.scripts]
 gasflux = "gasflux.cli:main_cli"
 
 [project.urls]
@@ -57,14 +57,15 @@
 assets = []
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
+version_variables = ["src/gasflux/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 
 [tool.semantic_release.branches.main]
 match = "(main|master)"
 prerelease_token = "rc"
 prerelease = false
```

### Comparing `gasflux-0.1.2/src/gasflux/background.py` & `gasflux-0.1.3/src/gasflux/background.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/cli.py` & `gasflux-0.1.3/src/gasflux/cli.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/gas.py` & `gasflux-0.1.3/src/gasflux/gas.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/gasflux_config.yaml` & `gasflux-0.1.3/src/gasflux/gasflux_config.yaml`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/generate_test_data.py` & `gasflux-0.1.3/src/gasflux/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/interpolation.py` & `gasflux-0.1.3/src/gasflux/interpolation.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/ml.py` & `gasflux-0.1.3/src/gasflux/ml.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/plotting.py` & `gasflux-0.1.3/src/gasflux/plotting.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/pre_processing.py` & `gasflux-0.1.3/src/gasflux/pre_processing.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/processing.py` & `gasflux-0.1.3/src/gasflux/processing.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/processing_pipelines.py` & `gasflux-0.1.3/src/gasflux/processing_pipelines.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/reporting.py` & `gasflux-0.1.3/src/gasflux/reporting.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/resources/model.pkl` & `gasflux-0.1.3/src/gasflux/resources/model.pkl`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/templates/mass_balance_template.html` & `gasflux-0.1.3/src/gasflux/templates/mass_balance_template.html`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/testdata/exampledata.csv` & `gasflux-0.1.3/src/gasflux/testdata/exampledata.csv`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/testdata/testconfig.yaml` & `gasflux-0.1.3/src/gasflux/testdata/testconfig.yaml`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux/testdata/testdata.csv` & `gasflux-0.1.3/src/gasflux/testdata/testdata.csv`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/src/gasflux.egg-info/PKG-INFO` & `gasflux-0.1.3/src/gasflux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gasflux
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to calculate gas emissions fluxes from natural and anthropogenic sources
 Author-email: Jamie McQuilkin <jamie.mcquilkin@gmail.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://gasflux.github.io
 Project-URL: Bug Tracker, https://github.com/gasflux/gasflux/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama==0.4.6
 Requires-Dist: geopandas==0.14.3
 Requires-Dist: geopy==2.4.1
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: joblib==1.3.2
@@ -24,24 +24,26 @@
 Requires-Dist: pytest==8.1.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: scikit-gstat==1.0.16
 Requires-Dist: scipy==1.12.0
 Requires-Dist: setuptools==69.2.0
 Requires-Dist: simplekml==1.3.6
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pigar; extra == "dev"
 Requires-Dist: pip>23.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: safety; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
 
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Tests](https://github.com/gasflux/gasflux/workflows/CI/badge.svg)](https://github.com/gasflux/gasflux/actions?query=workflow%3A%22CI%22)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
```

### Comparing `gasflux-0.1.2/src/gasflux.egg-info/SOURCES.txt` & `gasflux-0.1.3/src/gasflux.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 LICENSE
 README.md
 dev-requirements.txt
 mass_balance_template.html
 pyproject.toml
 requirements.txt
 .github/workflows/CI.yml
-.github/workflows/python-semantic-release.yml
+.github/workflows/build-release.yml
+.github/workflows/deploy.yml
+.github/workflows/release.yml
 src/gasflux/__init__.py
 src/gasflux/background.py
 src/gasflux/cli.py
 src/gasflux/gas.py
 src/gasflux/gasflux_config.yaml
 src/gasflux/generate_test_data.py
 src/gasflux/interpolation.py
```

### Comparing `gasflux-0.1.2/tests/test_processing.py` & `gasflux-0.1.3/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/tests/test_processing_pipelines.py` & `gasflux-0.1.3/tests/test_processing_pipelines.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.2/tools/mono_flight_splitter.py` & `gasflux-0.1.3/tools/mono_flight_splitter.py`

 * *Files identical despite different names*

