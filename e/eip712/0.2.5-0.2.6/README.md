# Comparing `tmp/eip712-0.2.5.tar.gz` & `tmp/eip712-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eip712-0.2.5.tar", last modified: Tue Apr  9 17:46:59 2024, max compression
+gzip compressed data, was "eip712-0.2.6.tar", last modified: Mon Apr 15 17:37:36 2024, max compression
```

## Comparing `eip712-0.2.5.tar` & `eip712-0.2.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 17:46:37.000000 eip712-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 17:46:37.000000 eip712-0.2.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 17:46:37.000000 eip712-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 17:46:37.000000 eip712-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 17:46:37.000000 eip712-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 17:46:59.560602 eip712-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 17:46:37.000000 eip712-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-09 17:46:37.000000 eip712-0.2.5/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/methoddocs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/methoddocs/messages.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/eip712.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 17:46:37.000000 eip712-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 17:46:59.560602 eip712-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-09 17:46:37.000000 eip712-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.482351 eip712-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.474351 eip712-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.474351 eip712-0.2.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-15 17:37:20.000000 eip712-0.2.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-15 17:37:20.000000 eip712-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 17:37:20.000000 eip712-0.2.6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-15 17:37:20.000000 eip712-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 17:37:20.000000 eip712-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-15 17:37:20.000000 eip712-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-15 17:37:36.482351 eip712-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-15 17:37:20.000000 eip712-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-15 17:37:20.000000 eip712-0.2.6/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/methoddocs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/methoddocs/messages.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 17:37:20.000000 eip712-0.2.6/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.478351 eip712-0.2.6/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 17:37:20.000000 eip712-0.2.6/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-15 17:37:20.000000 eip712-0.2.6/eip712/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-15 17:37:20.000000 eip712-0.2.6/eip712/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:20.000000 eip712-0.2.6/eip712/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.482351 eip712-0.2.6/eip712.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 17:37:36.000000 eip712-0.2.6/eip712.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-15 17:37:20.000000 eip712-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 17:37:36.482351 eip712-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-15 17:37:20.000000 eip712-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:36.482351 eip712-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:37:20.000000 eip712-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 17:37:20.000000 eip712-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-15 17:37:20.000000 eip712-0.2.6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-15 17:37:20.000000 eip712-0.2.6/tests/test_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-15 17:37:20.000000 eip712-0.2.6/tests/test_messages.py
```

### Comparing `eip712-0.2.5/.github/ISSUE_TEMPLATE/bug.md` & `eip712-0.2.6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/ISSUE_TEMPLATE/feature.md` & `eip712-0.2.6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/ISSUE_TEMPLATE/work-item.md` & `eip712-0.2.6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/release-drafter.yml` & `eip712-0.2.6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/codeql.yaml` & `eip712-0.2.6/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/commitlint.yaml` & `eip712-0.2.6/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/docs.yaml` & `eip712-0.2.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/prtitle.yaml` & `eip712-0.2.6/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/publish.yaml` & `eip712-0.2.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.github/workflows/test.yaml` & `eip712-0.2.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.gitignore` & `eip712-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/.pre-commit-config.yaml` & `eip712-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/CONTRIBUTING.md` & `eip712-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/LICENSE` & `eip712-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/PKG-INFO` & `eip712-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712
-Version: 0.2.5
+Version: 0.2.6
 Summary: eip712: Message classes for typed structured data hashing and signing in Ethereum
 Home-page: https://github.com/ApeWorX/eip712
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eip712-0.2.5/README.md` & `eip712-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/build_docs.py` & `eip712-0.2.6/build_docs.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/_static/custom.css` & `eip712-0.2.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/_static/custom.js` & `eip712-0.2.6/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/_templates/layout.html` & `eip712-0.2.6/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/conf.py` & `eip712-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/favicon.ico` & `eip712-0.2.6/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/docs/logo.gif` & `eip712-0.2.6/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/eip712/common.py` & `eip712-0.2.6/eip712/common.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/eip712/messages.py` & `eip712-0.2.6/eip712/messages.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/eip712.egg-info/PKG-INFO` & `eip712-0.2.6/eip712.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712
-Version: 0.2.5
+Version: 0.2.6
 Summary: eip712: Message classes for typed structured data hashing and signing in Ethereum
 Home-page: https://github.com/ApeWorX/eip712
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eip712-0.2.5/eip712.egg-info/SOURCES.txt` & `eip712-0.2.6/eip712.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/eip712.egg-info/requires.txt` & `eip712-0.2.6/eip712.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 dataclassy<1,>=0.8.2
-eth-abi<5,>=4.2.1
+eth-abi<6,>=5.1.0
 eth-account<0.11,>=0.10.0
 eth-hash[pycryptodome]
 eth-typing<4,>=3.5.2
 eth-utils<3,>=2.3.1
 hexbytes<1,>=0.3.0
 
 [dev]
```

### Comparing `eip712-0.2.5/pyproject.toml` & `eip712-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/setup.py` & `eip712-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/eip712",
     include_package_data=True,
     install_requires=[
         "dataclassy>=0.8.2,<1",
-        "eth-abi>=4.2.1,<5",
+        "eth-abi>=5.1.0,<6",
         "eth-account>=0.10.0,<0.11",
         "eth-hash[pycryptodome]",  # NOTE: Pinned by eth-abi
         "eth-typing>=3.5.2,<4",
         "eth-utils>=2.3.1,<3",
         "hexbytes>=0.3.0,<1",
     ],
     python_requires=">=3.8,<4",
```

### Comparing `eip712-0.2.5/tests/conftest.py` & `eip712-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/tests/test_common.py` & `eip712-0.2.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/tests/test_fuzzing.py` & `eip712-0.2.6/tests/test_fuzzing.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.5/tests/test_messages.py` & `eip712-0.2.6/tests/test_messages.py`

 * *Files identical despite different names*

