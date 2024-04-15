# Comparing `tmp/intropy-0.3.1.tar.gz` & `tmp/intropy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intropy-0.3.1.tar", last modified: Mon Apr  8 23:09:08 2024, max compression
+gzip compressed data, was "intropy-0.4.0.tar", last modified: Mon Apr 15 20:53:16 2024, max compression
```

## Comparing `intropy-0.3.1.tar` & `intropy-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:09:08.741523 intropy-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 23:09:04.000000 intropy-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-08 23:09:08.741523 intropy-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 23:09:04.000000 intropy-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:09:08.733523 intropy-0.3.1/intropy/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 23:09:04.000000 intropy-0.3.1/intropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-08 23:09:04.000000 intropy-0.3.1/intropy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:09:08.733523 intropy-0.3.1/intropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 23:09:08.000000 intropy-0.3.1/intropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 23:09:04.000000 intropy-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-08 23:09:04.000000 intropy-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 23:09:04.000000 intropy-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:09:08.741523 intropy-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:09:08.733523 intropy-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 23:09:04.000000 intropy-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-08 23:09:04.000000 intropy-0.3.1/tests/test_cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 23:09:04.000000 intropy-0.3.1/tests/test_generated_project_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.078311 intropy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 20:53:10.000000 intropy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-15 20:53:16.078311 intropy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-15 20:53:10.000000 intropy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.062310 intropy-0.4.0/intropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 20:53:10.000000 intropy-0.4.0/intropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-15 20:53:10.000000 intropy-0.4.0/intropy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/intropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 20:53:10.000000 intropy-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-style.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:53:16.078311 intropy-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_generated_project_test_suite.py
```

### Comparing `intropy-0.3.1/LICENSE` & `intropy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intropy-0.3.1/PKG-INFO` & `intropy-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intropy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Jump-start your python project
 License: MIT License
         
         Copyright (c) 2024 Richard Nordström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,15 +31,15 @@
 Requires-Dist: arrow==1.3.0; python_version >= "3.8"
 Requires-Dist: binaryornot==0.4.4
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: chardet==5.2.0; python_version >= "3.7"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: cookiecutter==2.6.0; python_version >= "3.7"
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: jinja2==3.1.3; python_version >= "3.7"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8"
 Requires-Dist: markupsafe==2.1.5; python_version >= "3.7"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-slugify==8.0.4; python_version >= "3.7"
@@ -60,77 +60,130 @@
 Requires-Dist: cfgv==3.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: chardet==5.2.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "dev"
 Requires-Dist: click==8.1.7; python_version >= "3.7" and extra == "dev"
 Requires-Dist: cookiecutter==2.6.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: coverage[toml]==7.4.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
-Requires-Dist: filelock==3.13.3; python_version >= "3.8" and extra == "dev"
+Requires-Dist: filelock==3.13.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: identify==2.5.35; python_version >= "3.8" and extra == "dev"
-Requires-Dist: idna==3.6; python_version >= "3.5" and extra == "dev"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "dev"
 Requires-Dist: iniconfig==2.0.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: jinja2==3.1.3; python_version >= "3.7" and extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: markupsafe==2.1.5; python_version >= "3.7" and extra == "dev"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "dev"
 Requires-Dist: mypy==1.9.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "dev"
 Requires-Dist: nodeenv==1.8.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "dev"
 Requires-Dist: packaging==24.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pluggy==1.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
 Requires-Dist: prompt-toolkit==3.0.36; python_full_version >= "3.6.2" and extra == "dev"
-Requires-Dist: pydantic==2.6.4; python_version >= "3.8" and extra == "dev"
-Requires-Dist: pydantic-core==2.16.3; python_version >= "3.8" and extra == "dev"
+Requires-Dist: pydantic==2.7.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: pydantic-core==2.18.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pydantic-settings==2.2.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pyproject-hooks==1.0.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pytest==8.1.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pytest-cookies==0.7.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: python-dateutil==2.9.0.post0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "dev"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: python-slugify==8.0.4; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "dev"
 Requires-Dist: questionary==2.0.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0" and extra == "dev"
 Requires-Dist: rich-click==1.7.4; python_version >= "3.7" and extra == "dev"
-Requires-Dist: ruff==0.3.5; python_version >= "3.7" and extra == "dev"
-Requires-Dist: setuptools==69.2.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: ruff==0.3.7; python_version >= "3.7" and extra == "dev"
+Requires-Dist: setuptools==69.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "dev"
 Requires-Dist: text-unidecode==1.3; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; python_version >= "3.7" and extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; python_version >= "3.8" and extra == "dev"
 Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: virtualenv==20.25.1; python_version >= "3.7" and extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: alabaster==0.7.16; python_version >= "3.9" and extra == "docs"
+Requires-Dist: babel==2.14.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: certifi==2024.2.2; python_version >= "3.6" and extra == "docs"
+Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "docs"
+Requires-Dist: colorama==0.4.6; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "docs"
+Requires-Dist: docutils==0.20.1; python_version >= "3.7" and extra == "docs"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "docs"
+Requires-Dist: imagesize==1.4.1; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "docs"
+Requires-Dist: jinja2==3.1.3; python_version >= "3.7" and extra == "docs"
+Requires-Dist: livereload==2.6.3; extra == "docs"
+Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: markupsafe==2.1.5; python_version >= "3.7" and extra == "docs"
+Requires-Dist: mdit-py-plugins==0.4.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "docs"
+Requires-Dist: myst-parser==2.0.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: packaging==24.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "docs"
+Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "docs"
+Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "docs"
+Requires-Dist: snowballstemmer==2.2.0; extra == "docs"
+Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-rtd-theme==2.0.0; python_version >= "3.6" and extra == "docs"
+Requires-Dist: sphinxcontrib-applehelp==1.0.8; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-devhelp==1.0.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-htmlhelp==2.0.5; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-jquery==4.1; python_version >= "2.7" and extra == "docs"
+Requires-Dist: sphinxcontrib-jsmath==1.0.1; python_version >= "3.5" and extra == "docs"
+Requires-Dist: sphinxcontrib-qthelp==1.0.7; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-serializinghtml==1.1.10; python_version >= "3.9" and extra == "docs"
+Requires-Dist: tornado==6.4; python_version > "2.7" and extra == "docs"
+Requires-Dist: urllib3==2.2.1; python_version >= "3.8" and extra == "docs"
+Provides-Extra: style
+Requires-Dist: mypy==1.9.0; python_version >= "3.8" and extra == "style"
+Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "style"
+Requires-Dist: ruff==0.3.7; python_version >= "3.7" and extra == "style"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "style"
+
+# Intropy
+
+[![Version](https://img.shields.io/pypi/v/intropy?color=blue)](https://pypi.org/project/intropy/)
+[![Build Status](https://github.com/RicNord/intropy/actions/workflows/ci.yaml/badge.svg)](https://github.com/RicNord/intropy/actions)
+
+Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter),
+intropy is a framework for jump-starting production-ready python projects. The
+python project will be generated and configured automatically with:
+
+- Build system
+- Test and code quality tooling
+- Documentation
+- Automation pipelines
+- etc...
 
-# intropy
-
-Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter), intropy
-is a framework for jump-starting production-ready python projects.
-
-## Tools
+## Features
 
 - [Ruff](https://docs.astral.sh/ruff/) | Linter and formatter
 - [Pytest](https://docs.pytest.org/en/latest/) | Test framework
-- [Coverage](https://coverage.readthedocs.io/en/latest/) | Code coverage
 - [Tox](https://tox.wiki/en/latest/) | Standardized testing and automation
+- [Coverage](https://coverage.readthedocs.io/en/latest/) | Code coverage
+- [Mypy](https://www.mypy-lang.org/) | Static type checker
 - [Pipenv](https://pipenv.pypa.io/en/latest/) | Package management
 - [Pre-commit](https://pre-commit.com/) | pre-commit hooks
 - [Bump my version](https://callowayproject.github.io/bump-my-version/) | Bump
   semantic version
+- [Sphinx](https://www.sphinx-doc.org/) | Documentation tool
+- Github workflows | CI and publishing to PyPi
+- Github templates | Pull Requests and Issues
 - Makefile for convenience
 
-## Optional tools
+## Optional feature alternatives
 
-- [Black](https://black.readthedocs.io/en/stable/) | Formatter
+- [Black](https://black.readthedocs.io/en/stable/) | Code formatter
 
 ## Usage
 
 Install cookiecutter:
 
 ```shell
 pip install cookiecutter
@@ -138,8 +191,23 @@
 
 Create project:
 
 ```shell
 cookiecutter https://github.com/RicNord/intropy
 ```
 
-You will be prompted for some values. Provide them and you are ready to code!
+You will be prompted for some values. After that the project will be generated!
+
+### (Optional) CLI
+
+A wrapper around the `cookiecutter` CLI is also provided and can be installed
+with:
+
+```shell
+pip install intropy
+```
+
+For API reference see:
+
+```shell
+intropy --help
+```
```

### Comparing `intropy-0.3.1/intropy/cli.py` & `intropy-0.4.0/intropy/cli.py`

 * *Files identical despite different names*

### Comparing `intropy-0.3.1/intropy.egg-info/PKG-INFO` & `intropy-0.4.0/intropy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intropy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Jump-start your python project
 License: MIT License
         
         Copyright (c) 2024 Richard Nordström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,15 +31,15 @@
 Requires-Dist: arrow==1.3.0; python_version >= "3.8"
 Requires-Dist: binaryornot==0.4.4
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: chardet==5.2.0; python_version >= "3.7"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: cookiecutter==2.6.0; python_version >= "3.7"
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: jinja2==3.1.3; python_version >= "3.7"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8"
 Requires-Dist: markupsafe==2.1.5; python_version >= "3.7"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-slugify==8.0.4; python_version >= "3.7"
@@ -60,77 +60,130 @@
 Requires-Dist: cfgv==3.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: chardet==5.2.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "dev"
 Requires-Dist: click==8.1.7; python_version >= "3.7" and extra == "dev"
 Requires-Dist: cookiecutter==2.6.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: coverage[toml]==7.4.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
-Requires-Dist: filelock==3.13.3; python_version >= "3.8" and extra == "dev"
+Requires-Dist: filelock==3.13.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: identify==2.5.35; python_version >= "3.8" and extra == "dev"
-Requires-Dist: idna==3.6; python_version >= "3.5" and extra == "dev"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "dev"
 Requires-Dist: iniconfig==2.0.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: jinja2==3.1.3; python_version >= "3.7" and extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: markupsafe==2.1.5; python_version >= "3.7" and extra == "dev"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "dev"
 Requires-Dist: mypy==1.9.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "dev"
 Requires-Dist: nodeenv==1.8.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "dev"
 Requires-Dist: packaging==24.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pluggy==1.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
 Requires-Dist: prompt-toolkit==3.0.36; python_full_version >= "3.6.2" and extra == "dev"
-Requires-Dist: pydantic==2.6.4; python_version >= "3.8" and extra == "dev"
-Requires-Dist: pydantic-core==2.16.3; python_version >= "3.8" and extra == "dev"
+Requires-Dist: pydantic==2.7.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: pydantic-core==2.18.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pydantic-settings==2.2.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pyproject-hooks==1.0.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pytest==8.1.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pytest-cookies==0.7.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: python-dateutil==2.9.0.post0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "dev"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: python-slugify==8.0.4; python_version >= "3.7" and extra == "dev"
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "dev"
 Requires-Dist: questionary==2.0.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "dev"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0" and extra == "dev"
 Requires-Dist: rich-click==1.7.4; python_version >= "3.7" and extra == "dev"
-Requires-Dist: ruff==0.3.5; python_version >= "3.7" and extra == "dev"
-Requires-Dist: setuptools==69.2.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: ruff==0.3.7; python_version >= "3.7" and extra == "dev"
+Requires-Dist: setuptools==69.4.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "dev"
 Requires-Dist: text-unidecode==1.3; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; python_version >= "3.7" and extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; python_version >= "3.8" and extra == "dev"
 Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "dev"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: virtualenv==20.25.1; python_version >= "3.7" and extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: alabaster==0.7.16; python_version >= "3.9" and extra == "docs"
+Requires-Dist: babel==2.14.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: certifi==2024.2.2; python_version >= "3.6" and extra == "docs"
+Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "docs"
+Requires-Dist: colorama==0.4.6; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "docs"
+Requires-Dist: docutils==0.20.1; python_version >= "3.7" and extra == "docs"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "docs"
+Requires-Dist: imagesize==1.4.1; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "docs"
+Requires-Dist: jinja2==3.1.3; python_version >= "3.7" and extra == "docs"
+Requires-Dist: livereload==2.6.3; extra == "docs"
+Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: markupsafe==2.1.5; python_version >= "3.7" and extra == "docs"
+Requires-Dist: mdit-py-plugins==0.4.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "docs"
+Requires-Dist: myst-parser==2.0.0; python_version >= "3.8" and extra == "docs"
+Requires-Dist: packaging==24.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "docs"
+Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "docs"
+Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "docs"
+Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "docs"
+Requires-Dist: snowballstemmer==2.2.0; extra == "docs"
+Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-rtd-theme==2.0.0; python_version >= "3.6" and extra == "docs"
+Requires-Dist: sphinxcontrib-applehelp==1.0.8; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-devhelp==1.0.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-htmlhelp==2.0.5; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-jquery==4.1; python_version >= "2.7" and extra == "docs"
+Requires-Dist: sphinxcontrib-jsmath==1.0.1; python_version >= "3.5" and extra == "docs"
+Requires-Dist: sphinxcontrib-qthelp==1.0.7; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinxcontrib-serializinghtml==1.1.10; python_version >= "3.9" and extra == "docs"
+Requires-Dist: tornado==6.4; python_version > "2.7" and extra == "docs"
+Requires-Dist: urllib3==2.2.1; python_version >= "3.8" and extra == "docs"
+Provides-Extra: style
+Requires-Dist: mypy==1.9.0; python_version >= "3.8" and extra == "style"
+Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "style"
+Requires-Dist: ruff==0.3.7; python_version >= "3.7" and extra == "style"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "style"
+
+# Intropy
+
+[![Version](https://img.shields.io/pypi/v/intropy?color=blue)](https://pypi.org/project/intropy/)
+[![Build Status](https://github.com/RicNord/intropy/actions/workflows/ci.yaml/badge.svg)](https://github.com/RicNord/intropy/actions)
+
+Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter),
+intropy is a framework for jump-starting production-ready python projects. The
+python project will be generated and configured automatically with:
+
+- Build system
+- Test and code quality tooling
+- Documentation
+- Automation pipelines
+- etc...
 
-# intropy
-
-Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter), intropy
-is a framework for jump-starting production-ready python projects.
-
-## Tools
+## Features
 
 - [Ruff](https://docs.astral.sh/ruff/) | Linter and formatter
 - [Pytest](https://docs.pytest.org/en/latest/) | Test framework
-- [Coverage](https://coverage.readthedocs.io/en/latest/) | Code coverage
 - [Tox](https://tox.wiki/en/latest/) | Standardized testing and automation
+- [Coverage](https://coverage.readthedocs.io/en/latest/) | Code coverage
+- [Mypy](https://www.mypy-lang.org/) | Static type checker
 - [Pipenv](https://pipenv.pypa.io/en/latest/) | Package management
 - [Pre-commit](https://pre-commit.com/) | pre-commit hooks
 - [Bump my version](https://callowayproject.github.io/bump-my-version/) | Bump
   semantic version
+- [Sphinx](https://www.sphinx-doc.org/) | Documentation tool
+- Github workflows | CI and publishing to PyPi
+- Github templates | Pull Requests and Issues
 - Makefile for convenience
 
-## Optional tools
+## Optional feature alternatives
 
-- [Black](https://black.readthedocs.io/en/stable/) | Formatter
+- [Black](https://black.readthedocs.io/en/stable/) | Code formatter
 
 ## Usage
 
 Install cookiecutter:
 
 ```shell
 pip install cookiecutter
@@ -138,8 +191,23 @@
 
 Create project:
 
 ```shell
 cookiecutter https://github.com/RicNord/intropy
 ```
 
-You will be prompted for some values. Provide them and you are ready to code!
+You will be prompted for some values. After that the project will be generated!
+
+### (Optional) CLI
+
+A wrapper around the `cookiecutter` CLI is also provided and can be installed
+with:
+
+```shell
+pip install intropy
+```
+
+For API reference see:
+
+```shell
+intropy --help
+```
```

### Comparing `intropy-0.3.1/intropy.egg-info/requires.txt` & `intropy-0.4.0/intropy.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 rich==13.7.1
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 python-dateutil==2.9.0.post0
 six==1.16.0
 
 [:python_version >= "3.5"]
-idna==3.6
+idna==3.7
 
 [:python_version >= "3.6"]
 certifi==2024.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.7"]
 chardet==5.2.0
@@ -50,15 +50,15 @@
 python-dateutil==2.9.0.post0
 six==1.16.0
 
 [dev:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6"]
 nodeenv==1.8.0
 
 [dev:python_version >= "3.5"]
-idna==3.6
+idna==3.7
 mypy-extensions==1.0.0
 
 [dev:python_version >= "3.6"]
 certifi==2024.2.2
 pyyaml==6.0.1
 
 [dev:python_version >= "3.7"]
@@ -72,38 +72,105 @@
 packaging==24.0
 pygments==2.17.2
 pyproject-hooks==1.0.0
 pytest-cookies==0.7.0
 python-slugify==8.0.4
 requests==2.31.0
 rich-click==1.7.4
-ruff==0.3.5
+ruff==0.3.7
 tomlkit==0.12.4
 virtualenv==20.25.1
 
 [dev:python_version >= "3.8"]
 annotated-types==0.6.0
 arrow==1.3.0
 build==1.2.1
 bump-my-version==0.20.0
 cfgv==3.4.0
 coverage[toml]==7.4.4
-filelock==3.13.3
+filelock==3.13.4
 identify==2.5.35
 markdown-it-py==3.0.0
 mypy==1.9.0
 platformdirs==4.2.0
 pluggy==1.4.0
-pydantic==2.6.4
-pydantic-core==2.16.3
+pydantic==2.7.0
+pydantic-core==2.18.1
 pydantic-settings==2.2.1
 pytest==8.1.1
 pytest-cov==5.0.0
 python-dotenv==1.0.1
 questionary==2.0.1
-setuptools==69.2.0
+setuptools==69.4.0
 types-python-dateutil==2.9.0.20240316
 typing-extensions==4.11.0
 urllib3==2.2.1
 
 [dev:python_version >= "3.9"]
 pre-commit==3.7.0
+
+[docs]
+livereload==2.6.3
+snowballstemmer==2.2.0
+
+[docs:python_full_version >= "3.7.0"]
+charset-normalizer==3.3.2
+
+[docs:python_version > "2.7"]
+tornado==6.4
+
+[docs:python_version >= "2.7"]
+sphinxcontrib-jquery==4.1
+
+[docs:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
+imagesize==1.4.1
+six==1.16.0
+
+[docs:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6"]
+colorama==0.4.6
+
+[docs:python_version >= "3.5"]
+idna==3.7
+sphinxcontrib-jsmath==1.0.1
+
+[docs:python_version >= "3.6"]
+certifi==2024.2.2
+pyyaml==6.0.1
+sphinx-rtd-theme==2.0.0
+
+[docs:python_version >= "3.7"]
+babel==2.14.0
+docutils==0.20.1
+jinja2==3.1.3
+markupsafe==2.1.5
+mdurl==0.1.2
+packaging==24.0
+pygments==2.17.2
+requests==2.31.0
+
+[docs:python_version >= "3.8"]
+markdown-it-py==3.0.0
+mdit-py-plugins==0.4.0
+myst-parser==2.0.0
+urllib3==2.2.1
+
+[docs:python_version >= "3.9"]
+alabaster==0.7.16
+sphinx==7.2.6
+sphinx-autobuild==2024.2.4
+sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-serializinghtml==1.1.10
+
+[style]
+
+[style:python_version >= "3.5"]
+mypy-extensions==1.0.0
+
+[style:python_version >= "3.7"]
+ruff==0.3.7
+
+[style:python_version >= "3.8"]
+mypy==1.9.0
+typing-extensions==4.11.0
```

### Comparing `intropy-0.3.1/pyproject.toml` & `intropy-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 intropy = "intropy.cli:main"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-optional-dependencies = { dev = { file = ["requirements-dev.txt"] } }
+dependencies = { file = ["requirements/requirements.txt"] }
+optional-dependencies = { dev = { file = [
+    "requirements/requirements-dev.txt",
+] }, docs = { file = [
+    "requirements/requirements-docs.txt",
+] }, style = { file = [
+    "requirements/requirements-style.txt",
+] } }
 version = { attr = "intropy.__version__" }
 
 [tool.setuptools.packages.find]
 include = ["intropy"]
 exclude = ["{{cookiecutter.project_slug}}*", "tests*", "hooks*"]
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 required_plugins = ["pytest-cov", "pytest-cookies"]
 addopts = [
     "--strict-config",
     "--ignore=setup.py",
+    "--ignore={{cookiecutter.project_slug}}",
     "--cov=intropy",
     "--cov-config=pyproject.toml",
     "--cov-append",
     "--cov-report=term-missing",
 ]
 
 [tool.isort]
@@ -100,15 +107,15 @@
 
     # Dont complain typing
     "@(typing(_extensions)?\\.)?overload",
     "if (typing(_extensions)?\\.)?TYPE_CHECKING:",
 ]
 
 [tool.bumpversion]
-current_version = "0.3.1"
+current_version = "0.4.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
@@ -121,12 +128,13 @@
 message = "Bump version: {current_version} -> {new_version}"
 commit_args = ""
 
 [[tool.bumpversion.files]]
 filename = "intropy/__init__.py"
 
 [tool.mypy]
+files = ["intropy/**.py", "tests/**.py"]
 exclude = ["\\{\\{cookiecutter.project_slug\\}\\}*", "hooks*"]
 
 [[tool.mypy.overrides]]
 module = "cookiecutter.main"
 ignore_missing_imports = true
```

### Comparing `intropy-0.3.1/requirements-dev.txt` & `intropy-0.4.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,48 +7,48 @@
 cfgv==3.4.0; python_version >= '3.8'
 chardet==5.2.0; python_version >= '3.7'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
 cookiecutter==2.6.0; python_version >= '3.7'
 coverage[toml]==7.4.4; python_version >= '3.8'
 distlib==0.3.8
-filelock==3.13.3; python_version >= '3.8'
+filelock==3.13.4; python_version >= '3.8'
 identify==2.5.35; python_version >= '3.8'
-idna==3.6; python_version >= '3.5'
+idna==3.7; python_version >= '3.5'
 iniconfig==2.0.0; python_version >= '3.7'
 jinja2==3.1.3; python_version >= '3.7'
 markdown-it-py==3.0.0; python_version >= '3.8'
 markupsafe==2.1.5; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 mypy==1.9.0; python_version >= '3.8'
 mypy-extensions==1.0.0; python_version >= '3.5'
 nodeenv==1.8.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 packaging==24.0; python_version >= '3.7'
 platformdirs==4.2.0; python_version >= '3.8'
 pluggy==1.4.0; python_version >= '3.8'
 pre-commit==3.7.0; python_version >= '3.9'
 prompt-toolkit==3.0.36; python_full_version >= '3.6.2'
-pydantic==2.6.4; python_version >= '3.8'
-pydantic-core==2.16.3; python_version >= '3.8'
+pydantic==2.7.0; python_version >= '3.8'
+pydantic-core==2.18.1; python_version >= '3.8'
 pydantic-settings==2.2.1; python_version >= '3.8'
 pygments==2.17.2; python_version >= '3.7'
 pyproject-hooks==1.0.0; python_version >= '3.7'
 pytest==8.1.1; python_version >= '3.8'
 pytest-cookies==0.7.0; python_version >= '3.7'
 pytest-cov==5.0.0; python_version >= '3.8'
 python-dateutil==2.9.0.post0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-slugify==8.0.4; python_version >= '3.7'
 pyyaml==6.0.1; python_version >= '3.6'
 questionary==2.0.1; python_version >= '3.8'
 requests==2.31.0; python_version >= '3.7'
 rich==13.7.1; python_full_version >= '3.7.0'
 rich-click==1.7.4; python_version >= '3.7'
-ruff==0.3.5; python_version >= '3.7'
-setuptools==69.2.0; python_version >= '3.8'
+ruff==0.3.7; python_version >= '3.7'
+setuptools==69.4.0; python_version >= '3.8'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 text-unidecode==1.3
 tomlkit==0.12.4; python_version >= '3.7'
 types-python-dateutil==2.9.0.20240316; python_version >= '3.8'
 typing-extensions==4.11.0; python_version >= '3.8'
 urllib3==2.2.1; python_version >= '3.8'
 virtualenv==20.25.1; python_version >= '3.7'
```

### Comparing `intropy-0.3.1/requirements.txt` & `intropy-0.4.0/requirements/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 arrow==1.3.0; python_version >= '3.8'
 binaryornot==0.4.4
 certifi==2024.2.2; python_version >= '3.6'
 chardet==5.2.0; python_version >= '3.7'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
 cookiecutter==2.6.0; python_version >= '3.7'
-idna==3.6; python_version >= '3.5'
+idna==3.7; python_version >= '3.5'
 jinja2==3.1.3; python_version >= '3.7'
 markdown-it-py==3.0.0; python_version >= '3.8'
 markupsafe==2.1.5; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 pygments==2.17.2; python_version >= '3.7'
 python-dateutil==2.9.0.post0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-slugify==8.0.4; python_version >= '3.7'
```

### Comparing `intropy-0.3.1/tests/test_cli.py` & `intropy-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `intropy-0.3.1/tests/test_cookiecutter.py` & `intropy-0.4.0/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `intropy-0.3.1/tests/test_generated_project_test_suite.py` & `intropy-0.4.0/tests/test_generated_project_test_suite.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import subprocess
 import sys
 
+TIMEOUT_DURATION_SEC = 180
+
 
 def test_tox_py(cookies):
     pyenv = sys.version_info
     result = cookies.bake()
 
     p = subprocess.Popen(
-        ["tox", "-e", f"py{pyenv.major}{pyenv.minor}"],
+        ["tox", "-e", f"py{pyenv.major}{pyenv.minor}", "-vv", "--", "-v"],
         cwd=result.project_path,
         stderr=subprocess.PIPE,
         universal_newlines=True,
     )
-    _, err = p.communicate(timeout=100)
+    _, err = p.communicate(timeout=TIMEOUT_DURATION_SEC)
 
     if p.returncode != 0:
         raise RuntimeError(err)
 
 
 def test_tox_style(cookies):
     result = cookies.bake()
 
     p = subprocess.Popen(
-        ["tox", "-m", "style"],
+        ["tox", "-m", "style", "-vv", "--", "-v"],
         cwd=result.project_path,
         stderr=subprocess.PIPE,
         universal_newlines=True,
     )
-    _, err = p.communicate(timeout=100)
+    _, err = p.communicate(timeout=TIMEOUT_DURATION_SEC)
 
     if p.returncode != 0:
         raise RuntimeError(err)
```

