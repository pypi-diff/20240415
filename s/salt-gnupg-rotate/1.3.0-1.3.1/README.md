# Comparing `tmp/salt_gnupg_rotate-1.3.0.tar.gz` & `tmp/salt_gnupg_rotate-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salt_gnupg_rotate-1.3.0.tar", max compression
+gzip compressed data, was "salt_gnupg_rotate-1.3.1.tar", max compression
```

## Comparing `salt_gnupg_rotate-1.3.0.tar` & `salt_gnupg_rotate-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1317 2024-01-29 04:06:33.106128 salt_gnupg_rotate-1.3.0/LICENSE
--rw-r--r--   0        0        0     2861 2024-02-06 23:44:56.027541 salt_gnupg_rotate-1.3.0/README.md
--rw-r--r--   0        0        0     4973 2024-02-06 23:44:56.028542 salt_gnupg_rotate-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      133 2024-02-06 23:44:56.028542 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/__init__.py
--rw-r--r--   0        0        0     4210 2024-01-30 04:56:47.396268 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/cli.py
--rw-r--r--   0        0        0      688 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/config.py
--rw-r--r--   0        0        0      230 2024-01-29 04:06:33.108128 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/exceptions.py
--rw-r--r--   0        0        0      243 2024-01-29 04:06:33.108128 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/logger.py
--rw-r--r--   0        0        0     1708 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/logging_mixins.py
--rw-r--r--   0        0        0     3323 2024-01-30 04:56:47.397268 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/main.py
--rw-r--r--   0        0        0    11909 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/rotate.py
--rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 salt_gnupg_rotate-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1317 2024-01-29 04:06:33.106128 salt_gnupg_rotate-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2861 2024-02-06 23:44:56.027541 salt_gnupg_rotate-1.3.1/README.md
+-rw-r--r--   0        0        0     5225 2024-04-15 16:07:24.606262 salt_gnupg_rotate-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-15 16:07:24.606262 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/__init__.py
+-rw-r--r--   0        0        0     4210 2024-01-30 04:56:47.396268 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/cli.py
+-rw-r--r--   0        0        0      688 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/config.py
+-rw-r--r--   0        0        0      230 2024-01-29 04:06:33.108128 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/exceptions.py
+-rw-r--r--   0        0        0      243 2024-01-29 04:06:33.108128 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/logger.py
+-rw-r--r--   0        0        0     1708 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/logging_mixins.py
+-rw-r--r--   0        0        0     3323 2024-01-30 04:56:47.397268 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/main.py
+-rw-r--r--   0        0        0    11909 2024-02-03 22:40:41.930074 salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/rotate.py
+-rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 salt_gnupg_rotate-1.3.1/PKG-INFO
```

### Comparing `salt_gnupg_rotate-1.3.0/LICENSE` & `salt_gnupg_rotate-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/README.md` & `salt_gnupg_rotate-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/pyproject.toml` & `salt_gnupg_rotate-1.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 [project]
 name = "salt-gnupg-rotate"
 requires-python = ">=3.8"
 
 # Poetry package config
 [tool.poetry]
 name = "salt-gnupg-rotate"
-version = "1.3.0"
+version = "1.3.1"
 description = "Easily rotate gnupg encryption keys of fully or partially encrypted files."
 authors = ["Ryan Addessi <raddessi@users.noreply.github.com>"]
 license = "BSD 2-Clause 'Simplified' License"
 readme = "README.md"
 repository = "https://github.com/raddessi/salt-gnupg-rotate"
 homepage = "https://github.com/raddessi/salt-gnupg-rotate"
 keywords = []
 packages = [{ include = "salt_gnupg_rotate" }]
 classifiers = []
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.7"
-rich = ">=10.14.0"
+rich = ">=13.7.1"
 python-gnupg = ">=0.5.2"
 sphinx-click = "^5.1.0"
 
 [tool.poetry.dev-dependencies]
-"ruamel.yaml" = ">=0.17.17"
-coverage = {extras = ["toml"], version = ">=6.2"}
-furo = ">=2022.1.2"
+"ruamel.yaml" = ">=0.18.6"
+coverage = {extras = ["toml"], version = ">=7.4.4"}
+furo = ">=2024.1.29"
 jinja2-time = ">=0.2.0"
-mypy = ">=0.931"
-myst-parser = ">=0.16.1"
-nox = ">=2021.10.1"
-nox-poetry = ">=0.9.0"
-pre-commit = ">=2.16.0"
-pytest = ">=6.2.5"
-pytest-mock = ">=3.6.1"
-safety = ">=1.10.3"
-sphinx = ">=4.3.2"
-sphinx-autobuild = ">=2021.3.14"
-sphinx-click = ">=3.0.2"
-sphinx-copybutton = ">=0.4.0"
-sphinx-inline-tabs = {version = ">=2022.1.2b11", python = ">=3.8,<4.0"}
-sphinxcontrib-mermaid = ">=0.7.1"
-sphinxcontrib-spelling = ">=7.3.2"
+mypy = ">=1.9.0"
+myst-parser = ">=2.0.0"
+nox = ">=2024.4.15"
+nox-poetry = ">=1.0.3"
+pre-commit = [
+    {version = ">=2.16.0", python = "<3.9"},
+    {version = ">=2.16.0", python = ">=3.9"},
+]
+pytest = ">=8.1.1"
+pytest-mock = ">=3.14.0"
+safety = ">=3.1.0"
+sphinx = [
+    {version = ">=4.3.2", python = "<3.9"},
+    {version = ">=4.3.2", python = ">=3.9"},
+]
+sphinx-autobuild = [
+    {version = ">=2021.3.14", python = "<3.9"},
+    {version = ">=2021.3.14", python = ">=3.9"},
+]
+sphinx-click = ">=5.1.0"
+sphinx-copybutton = ">=0.5.2"
+sphinx-inline-tabs = {version = ">=2023.4.21", python = ">=3.8,<4.0"}
+sphinxcontrib-mermaid = ">=0.9.2"
+sphinxcontrib-spelling = ">=8.0.0"
 sphinxcontrib-versioning = "2.2.1"
 sphinxemoji = [
     {version = "<3", python = "<3.9"},
     {version = "0.3.1", python = ">=3.9"},
 ]
-typeguard = "^4.0.0"
+typeguard = "^4.2.1"
 xdoctest = {extras = ["colors"], version = "1.1.3"}
 
 
 [tool.poetry.scripts]
 salt-gnupg-rotate = "salt_gnupg_rotate.cli:cli"
 
 [tool.poetry.urls]
```

### Comparing `salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/cli.py` & `salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/cli.py`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/config.py` & `salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/config.py`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/logging_mixins.py` & `salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/logging_mixins.py`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/main.py` & `salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/main.py`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/salt_gnupg_rotate/rotate.py` & `salt_gnupg_rotate-1.3.1/salt_gnupg_rotate/rotate.py`

 * *Files identical despite different names*

### Comparing `salt_gnupg_rotate-1.3.0/PKG-INFO` & `salt_gnupg_rotate-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-gnupg-rotate
-Version: 1.3.0
+Version: 1.3.1
 Summary: Easily rotate gnupg encryption keys of fully or partially encrypted files.
 Home-page: https://github.com/raddessi/salt-gnupg-rotate
 License: BSD 2-Clause 'Simplified' License
 Author: Ryan Addessi
 Author-email: raddessi@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: python-gnupg (>=0.5.2)
-Requires-Dist: rich (>=10.14.0)
+Requires-Dist: rich (>=13.7.1)
 Requires-Dist: sphinx-click (>=5.1.0,<6.0.0)
 Project-URL: Changelog, https://github.com/raddessi/salt-gnupg-rotate/releases
 Project-URL: Repository, https://github.com/raddessi/salt-gnupg-rotate
 Description-Content-Type: text/markdown
 
 [![CI](https://github.com/raddessi/salt-gnupg-rotate/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/raddessi/salt-gnupg-rotate/actions/workflows/ci.yaml)
 [![documentation](https://img.shields.io/badge/docs-sphinx%20furo-blue.svg?style=flat)](https://github.com/pradyunsg/furo)
```

