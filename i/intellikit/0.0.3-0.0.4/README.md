# Comparing `tmp/intellikit-0.0.3.tar.gz` & `tmp/intellikit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellikit-0.0.3.tar", last modified: Fri Mar 22 10:32:09 2024, max compression
+gzip compressed data, was "intellikit-0.0.4.tar", last modified: Mon Apr 15 00:06:51 2024, max compression
```

## Comparing `intellikit-0.0.3.tar` & `intellikit-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-22 10:31:58.000000 intellikit-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.573456 intellikit-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.577456 intellikit-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.577456 intellikit-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-22 10:31:58.000000 intellikit-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-22 10:31:58.000000 intellikit-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:31:58.000000 intellikit-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-22 10:31:58.000000 intellikit-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-22 10:32:09.581456 intellikit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-22 10:31:58.000000 intellikit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.577456 intellikit-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.577456 intellikit-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/intellikit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 10:31:58.000000 intellikit-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-03-22 10:31:58.000000 intellikit-0.0.3/examples/datasets/cars-1k.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 10:31:58.000000 intellikit-0.0.3/examples/intro.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/intellikit/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-22 10:31:58.000000 intellikit-0.0.3/intellikit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-22 10:31:58.000000 intellikit-0.0.3/intellikit/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-22 10:31:58.000000 intellikit-0.0.3/intellikit/intellikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/intellikit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 10:32:09.000000 intellikit-0.0.3/intellikit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-22 10:31:58.000000 intellikit-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-22 10:31:58.000000 intellikit-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-22 10:31:58.000000 intellikit-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-22 10:31:58.000000 intellikit-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 10:32:09.581456 intellikit-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:32:09.581456 intellikit-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-22 10:31:58.000000 intellikit-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-22 10:31:58.000000 intellikit-0.0.3/tests/test_intellikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-15 00:06:40.000000 intellikit-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.216092 intellikit-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.220092 intellikit-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.220092 intellikit-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-15 00:06:40.000000 intellikit-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:06:40.000000 intellikit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 00:06:40.000000 intellikit-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 00:06:51.228092 intellikit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 00:06:40.000000 intellikit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Car_Search_System.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Document_Search_System.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Recommendation_System.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/datasets/cars-1k.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/similarity_output.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/intellikit.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/ir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/sim.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/Car_Search_System.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/datasets/cars-1k.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/similarity_output.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/intellikit/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/intellikit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/intellikit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-15 00:06:40.000000 intellikit-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-15 00:06:40.000000 intellikit-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 00:06:40.000000 intellikit-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 00:06:40.000000 intellikit-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:06:51.228092 intellikit-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 00:06:40.000000 intellikit-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 00:06:40.000000 intellikit-0.0.4/tests/test_intellikit.py
```

### Comparing `intellikit-0.0.3/.github/ISSUE_TEMPLATE/config.yml` & `intellikit-0.0.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/docs-build.yml` & `intellikit-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/docs.yml` & `intellikit-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/installation.yml` & `intellikit-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/macos.yml` & `intellikit-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/pypi.yml` & `intellikit-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/ubuntu.yml` & `intellikit-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.github/workflows/windows.yml` & `intellikit-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/.gitignore` & `intellikit-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/docs/contributing.md` & `intellikit-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/docs/installation.md` & `intellikit-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/examples/datasets/cars-1k.csv` & `intellikit-0.0.4/docs/examples/datasets/cars-1k.csv`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.3/intellikit/intellikit.py` & `intellikit-0.0.4/intellikit/intellikit.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 from sklearn.metrics.pairwise import cosine_similarity
 from sklearn.preprocessing import LabelEncoder
 from sklearn.feature_extraction.text import TfidfVectorizer
 from scipy.stats import pearsonr
 import numpy as np
 
+
 def calculate_word_similarity(df, query, text_columns):
     """Calculate the similarity score between the query and the case. This basic function returns a value of 1 for all words that match and a value of zero when the words differ
 
     Args:
         df (dataframme, required): The dataframme containing the cases
         query (dictionary, required): The search query corresponding to a case you are looking for.
         text_columns (list, required): The columns from the dataframme for which to compare with the query values.
```

### Comparing `intellikit-0.0.3/intellikit.egg-info/SOURCES.txt` & `intellikit-0.0.4/intellikit.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -20,22 +20,33 @@
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/intellikit.md
+docs/ir.md
+docs/sim.md
 docs/usage.md
+docs/examples/Car_Search_System.ipynb
+docs/examples/Document_Search_System.ipynb
+docs/examples/Recommendation_System.ipynb
 docs/examples/intro.ipynb
+docs/examples/similarity_output.csv
+docs/examples/datasets/cars-1k.csv
 docs/overrides/main.html
+examples/Car_Search_System.ipynb
 examples/intro.ipynb
+examples/similarity_output.csv
 examples/datasets/cars-1k.csv
 intellikit/__init__.py
 intellikit/common.py
 intellikit/intellikit.py
+intellikit/ir.py
+intellikit/sim.py
 intellikit.egg-info/PKG-INFO
 intellikit.egg-info/SOURCES.txt
 intellikit.egg-info/dependency_links.txt
 intellikit.egg-info/entry_points.txt
 intellikit.egg-info/requires.txt
 intellikit.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `intellikit-0.0.3/mkdocs.yml` & `intellikit-0.0.4/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -77,10 +77,16 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/ArthurKakande/intellikit/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/Car_Search_System.ipynb
+        - examples/Document_Search_System.ipynb
+        - examples/Recommendation_System.ipynb
     - API Reference:
           - intellikit module: intellikit.md
           - common module: common.md
+          - ir module: ir.md
+          - sim module: sim.md
+
```

### Comparing `intellikit-0.0.3/pyproject.toml` & `intellikit-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "intellikit"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "A python toolkit for case based reasoning, information retrieval, natural language processing and other techniques for AI and intelligent systems."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

