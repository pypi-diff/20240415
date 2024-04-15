# Comparing `tmp/pyblindrl-0.0.2rc57.post1.tar.gz` & `tmp/pyblindrl-0.0.2rc58.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblindrl-0.0.2rc57.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyblindrl-0.0.2rc58.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyblindrl-0.0.2rc57.post1.tar` & `pyblindrl-0.0.2rc58.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      340 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      418 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1132 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/LICENSE
--rw-r--r--   0        0        0    14946 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/README.md
--rw-r--r--   0        0        0     2780 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/SUPPORT.md
--rw-r--r--   0        0        0      634 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/docs/Makefile
--rw-r--r--   0        0        0     2320 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/docs/developer.md
--rw-r--r--   0        0        0      461 2024-04-15 14:24:19.916042 pyblindrl-0.0.2rc57.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/make.bat
--rw-r--r--   0        0        0       57 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/docs/workflows.md
--rw-r--r--   0        0        0     6567 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/pyproject.toml
--rw-r--r--   0        0        0       44 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/src/README.md
--rw-r--r--   0        0        0     5149 2024-04-15 14:24:33.984060 pyblindrl-0.0.2rc57.post1/src/pyBlindRL/__init__.py
--rw-r--r--   0        0        0      584 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/src/pyBlindRL/hello_world.py
--rw-r--r--   0        0        0      989 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/tests/conftest.py
--rw-r--r--   0        0        0     1212 2024-04-15 14:24:19.920042 pyblindrl-0.0.2rc57.post1/tests/test_methods.py
--rw-r--r--   0        0        0    16709 1970-01-01 00:00:00.000000 pyblindrl-0.0.2rc57.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      418 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1132 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/LICENSE
+-rw-r--r--   0        0        0    14946 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/SUPPORT.md
+-rw-r--r--   0        0        0      634 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/Makefile
+-rw-r--r--   0        0        0     2320 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/developer.md
+-rw-r--r--   0        0        0      461 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6567 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/src/README.md
+-rw-r--r--   0        0        0     5149 2024-04-15 14:24:52.206620 pyblindrl-0.0.2rc58.post1/src/pyBlindRL/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/src/pyBlindRL/hello_world.py
+-rw-r--r--   0        0        0      989 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/tests/conftest.py
+-rw-r--r--   0        0        0     1212 2024-04-15 14:24:34.690667 pyblindrl-0.0.2rc58.post1/tests/test_methods.py
+-rw-r--r--   0        0        0    16709 1970-01-01 00:00:00.000000 pyblindrl-0.0.2rc58.post1/PKG-INFO
```

### Comparing `pyblindrl-0.0.2rc57.post1/.devcontainer/devcontainer.json` & `pyblindrl-0.0.2rc58.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/.github/workflows/schedule-update-actions.yml` & `pyblindrl-0.0.2rc58.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/.gitignore` & `pyblindrl-0.0.2rc58.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/.pre-commit-config.yaml` & `pyblindrl-0.0.2rc58.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/.vscode/settings.json` & `pyblindrl-0.0.2rc58.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/LICENSE` & `pyblindrl-0.0.2rc58.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/README.md` & `pyblindrl-0.0.2rc58.post1/README.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/SECURITY.md` & `pyblindrl-0.0.2rc58.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/SUPPORT.md` & `pyblindrl-0.0.2rc58.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/docs/Makefile` & `pyblindrl-0.0.2rc58.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/docs/conf.py` & `pyblindrl-0.0.2rc58.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/docs/make.bat` & `pyblindrl-0.0.2rc58.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/docs/pylint.md` & `pyblindrl-0.0.2rc58.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/pyproject.toml` & `pyblindrl-0.0.2rc58.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.optional-dependencies]
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
     "bandit[toml]==1.7.8",
-    "black==24.3.0",
+    "black==24.4.0",
     "check-manifest==0.49",
     "flake8-bugbear==24.2.6",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
     "pre-commit==3.7.0",
```

### Comparing `pyblindrl-0.0.2rc57.post1/src/pyBlindRL/__init__.py` & `pyblindrl-0.0.2rc58.post1/src/pyBlindRL/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   -------------------------------------------------------------
 """A Python implementation of blind Richardson-Lucy deconvolution"""
 from __future__ import annotations
 
 import numpy as np
 import torch
 
-__version__ = "0.0.2""-rc57-post1"
+__version__ = "0.0.2""-rc58-post1"
 
 
 def gaussian_3d(shape, center=None, sigma=None):
     """
     Generate a 3D Gaussian array.
 
     Parameters:
```

### Comparing `pyblindrl-0.0.2rc57.post1/src/pyBlindRL/hello_world.py` & `pyblindrl-0.0.2rc58.post1/src/pyBlindRL/hello_world.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/tests/conftest.py` & `pyblindrl-0.0.2rc58.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/tests/test_methods.py` & `pyblindrl-0.0.2rc58.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc57.post1/PKG-INFO` & `pyblindrl-0.0.2rc58.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyBlindRL
-Version: 0.0.2rc57.post1
+Version: 0.0.2rc58.post1
 Summary: A Python implementation of blind Richardson-Lucy deconvolution
 Author-email: "Logan Walker, PhD" <loganaw@umich.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: pyspark>=3.0.0 ; extra == "spark"
 Requires-Dist: bandit[toml]==1.7.8 ; extra == "test"
-Requires-Dist: black==24.3.0 ; extra == "test"
+Requires-Dist: black==24.4.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: flake8-bugbear==24.2.6 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flake8-pyproject ; extra == "test"
 Requires-Dist: pre-commit==3.7.0 ; extra == "test"
```

