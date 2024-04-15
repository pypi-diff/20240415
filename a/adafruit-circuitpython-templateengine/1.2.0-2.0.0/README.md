# Comparing `tmp/adafruit-circuitpython-templateengine-1.2.0.tar.gz` & `tmp/adafruit_circuitpython_templateengine-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-templateengine-1.2.0.tar", last modified: Wed Mar  6 22:39:50 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_templateengine-2.0.0.tar", last modified: Mon Apr 15 17:39:59 2024, max compression
```

## Comparing `adafruit-circuitpython-templateengine-1.2.0.tar` & `adafruit_circuitpython_templateengine-2.0.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.876254 adafruit-circuitpython-templateengine-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.864254 adafruit-circuitpython-templateengine-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.868254 adafruit-circuitpython-templateengine-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.868254 adafruit-circuitpython-templateengine-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.868254 adafruit-circuitpython-templateengine-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-03-06 22:39:50.876254 adafruit-circuitpython-templateengine-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.876254 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-03-06 22:39:50.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-06 22:39:50.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 22:39:50.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-06 22:39:50.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-06 22:39:50.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/adafruit_templateengine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.872254 adafruit-circuitpython-templateengine-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.872254 adafruit-circuitpython-templateengine-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:39:50.876254 adafruit-circuitpython-templateengine-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/autoescape.html
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/base_without_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/child.html
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/comments.html
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/examples/parent_layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_blocks_extends.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_for_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_if_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_includes.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_reusing.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_while_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-06 22:39:48.000000 adafruit-circuitpython-templateengine-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-06 22:39:39.000000 adafruit-circuitpython-templateengine-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 22:39:50.876254 adafruit-circuitpython-templateengine-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.937862 adafruit_circuitpython_templateengine-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.929862 adafruit_circuitpython_templateengine-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.929862 adafruit_circuitpython_templateengine-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.933862 adafruit_circuitpython_templateengine-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.933862 adafruit_circuitpython_templateengine-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-15 17:39:59.937862 adafruit_circuitpython_templateengine-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.937862 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-15 17:39:59.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 17:39:59.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:39:59.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 17:39:59.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 17:39:59.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/adafruit_templateengine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.933862 adafruit_circuitpython_templateengine-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.933862 adafruit_circuitpython_templateengine-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:39:59.937862 adafruit_circuitpython_templateengine-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/autoescape.html
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/base_without_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/child.html
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/comments.html
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/examples/parent_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_blocks_extends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_for_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_if_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_reusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_while_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 17:39:57.000000 adafruit_circuitpython_templateengine-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 17:39:51.000000 adafruit_circuitpython_templateengine-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:39:59.937862 adafruit_circuitpython_templateengine-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_templateengine-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/.gitignore` & `adafruit_circuitpython_templateengine-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/.pre-commit-config.yaml` & `adafruit_circuitpython_templateengine-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/.pylintrc` & `adafruit_circuitpython_templateengine-2.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_templateengine-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/LICENSE` & `adafruit_circuitpython_templateengine-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_templateengine-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/LICENSES/MIT.txt` & `adafruit_circuitpython_templateengine-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_templateengine-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/PKG-INFO` & `adafruit_circuitpython_templateengine-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-templateengine
-Version: 1.2.0
+Version: 2.0.0
 Summary: Templating engine to substitute variables into a template string. Templates can also include conditional logic and loops. Often used for web pages.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TemplateEngine
-Keywords: adafruit,blinka,circuitpython,micropython,templateengine,template,string,substitution,web,html,xml,escaping,syntax
+Keywords: adafruit,blinka,circuitpython,micropython,templateengine,template,string,substitution,web,html,escaping,syntax
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/README.rst` & `adafruit_circuitpython_templateengine-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/PKG-INFO` & `adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-templateengine
-Version: 1.2.0
+Version: 2.0.0
 Summary: Templating engine to substitute variables into a template string. Templates can also include conditional logic and loops. Often used for web pages.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TemplateEngine
-Keywords: adafruit,blinka,circuitpython,micropython,templateengine,template,string,substitution,web,html,xml,escaping,syntax
+Keywords: adafruit,blinka,circuitpython,micropython,templateengine,template,string,substitution,web,html,escaping,syntax
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/adafruit_circuitpython_templateengine.egg-info/SOURCES.txt` & `adafruit_circuitpython_templateengine-2.0.0/adafruit_circuitpython_templateengine.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/autoescape.html
-examples/autoescape.md
 examples/base_without_footer.html
 examples/child.html
 examples/comments.html
 examples/footer.html
 examples/parent_layout.html
 examples/templateengine_autoescape.py
 examples/templateengine_blocks_extends.py
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/adafruit_templateengine.py` & `adafruit_circuitpython_templateengine-2.0.0/adafruit_templateengine.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "1.2.0"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TemplateEngine.git"
 
 try:
     from typing import Any, Generator
 except ImportError:
     pass
 
@@ -38,27 +38,102 @@
             " will have limited functionality when using block comments and non-ASCII characters."
         )
 finally:
     # Unimport sys to prevent accidental use
     del implementation
 
 
-class Language:  # pylint: disable=too-few-public-methods
-    """
-    Enum-like class that contains languages supported for escaping.
-    """
+class Token:  # pylint: disable=too-few-public-methods
+    """Stores a token with its position in a template."""
+
+    def __init__(self, template: str, start_position: int, end_position: int):
+        self.template = template
+        self.start_position = start_position
+        self.end_position = end_position
+
+        self.content = template[start_position:end_position]
+
+
+class TemplateNotFoundError(OSError):
+    """Raised when a template file is not found."""
+
+    def __init__(self, path: str):
+        """Specified template file that was not found."""
+        super().__init__(f"Template file not found: {path}")
+
+
+class TemplateSyntaxError(SyntaxError):
+    """Raised when a syntax error is encountered in a template."""
+
+    def __init__(self, token: Token, reason: str):
+        """Provided token is not a valid template syntax at the specified position."""
+        super().__init__(self._underline_token_in_template(token) + f"\n\n{reason}")
+
+    @staticmethod
+    def _skipped_lines_message(nr_of_lines: int) -> str:
+        return f"[{nr_of_lines} line{'s' if nr_of_lines > 1 else ''} skipped]"
+
+    @classmethod
+    def _underline_token_in_template(
+        cls, token: Token, *, lines_around: int = 4, symbol: str = "^"
+    ) -> str:
+        """
+        Return ``number_of_lines`` lines before and after ``token``, with the token content
+        underlined with ``symbol`` e.g.:
+
+        ```html
+        [8 lines skipped]
+                Shopping list:
+                <ul>
+                    {% for item in context["items"] %}
+                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+                        <li>{{ item["name"] }} - ${{ item["price"] }}</li>
+                    {% empty %}
+        [5 lines skipped]
+        ```
+        """
+
+        template_before_token = token.template[: token.start_position]
+        if skipped_lines := template_before_token.count("\n") - lines_around:
+            template_before_token = (
+                f"{cls._skipped_lines_message(skipped_lines)}\n"
+                + "\n".join(template_before_token.split("\n")[-(lines_around + 1) :])
+            )
+
+        template_after_token = token.template[token.end_position :]
+        if skipped_lines := template_after_token.count("\n") - lines_around:
+            template_after_token = (
+                "\n".join(template_after_token.split("\n")[: (lines_around + 1)])
+                + f"\n{cls._skipped_lines_message(skipped_lines)}"
+            )
 
-    HTML = "html"
-    """HTML language"""
+        lines_before_line_with_token = template_before_token.rsplit("\n", 1)[0]
 
-    XML = "xml"
-    """XML language"""
+        line_with_token = (
+            template_before_token.rsplit("\n", 1)[-1]
+            + token.content
+            + template_after_token.split("\n")[0]
+        )
+
+        line_with_underline = (
+            " " * len(template_before_token.rsplit("\n", 1)[-1])
+            + symbol * len(token.content)
+            + " " * len(template_after_token.split("\n")[0])
+        )
 
-    MARKDOWN = "markdown"
-    """Markdown language"""
+        lines_after_line_with_token = template_after_token.split("\n", 1)[-1]
+
+        return "\n".join(
+            [
+                lines_before_line_with_token,
+                line_with_token,
+                line_with_underline,
+                lines_after_line_with_token,
+            ]
+        )
 
 
 def safe_html(value: Any) -> str:
     """
     Encodes unsafe symbols in ``value`` to HTML entities and returns the string that can be safely
     used in HTML.
 
@@ -107,92 +182,64 @@
         .replace(">", "&gt;")
         .replace("|", "&vert;")
         .replace("~", "&tilde;")
         .replace("$", "&dollar;")
     )
 
 
-def safe_xml(value: Any) -> str:
-    """
-    Encodes unsafe symbols in ``value`` to XML entities and returns the string that can be safely
-    used in XML.
-
-    Example::
-
-        safe_xml('<a href="https://circuitpython.org/">CircuitPython</a>')
-        # &lt;a href=&quot;https://circuitpython.org/&quot;&gt;CircuitPython&lt;/a&gt;
-    """
-
-    return (
-        str(value)
-        .replace("&", "&amp;")
-        .replace('"', "&quot;")
-        .replace("'", "&apos;")
-        .replace("<", "&lt;")
-        .replace(">", "&gt;")
-    )
-
-
-def safe_markdown(value: Any) -> str:
-    """
-    Encodes unsafe symbols in ``value`` and returns the string that can be safely used in Markdown.
-
-    Example::
-
-        safe_markdown('[CircuitPython](https://circuitpython.org/)')
-        # \\[CircuitPython\\]\\(https://circuitpython.org/\\)
-    """
-
-    return (
-        str(value)
-        .replace("_", "\\_")
-        .replace("-", "\\-")
-        .replace("!", "\\!")
-        .replace("(", "\\(")
-        .replace(")", "\\)")
-        .replace("[", "\\[")
-        .replace("]", "\\]")
-        .replace("*", "\\*")
-        .replace("*", "\\*")
-        .replace("&", "\\&")
-        .replace("#", "\\#")
-        .replace("`", "\\`")
-        .replace("+", "\\+")
-        .replace("<", "\\<")
-        .replace(">", "\\>")
-        .replace("|", "\\|")
-        .replace("~", "\\~")
-    )
-
-
 _EXTENDS_PATTERN = re.compile(r"{% extends '.+?' %}|{% extends \".+?\" %}")
 _BLOCK_PATTERN = re.compile(r"{% block \w+? %}")
 _INCLUDE_PATTERN = re.compile(r"{% include '.+?' %}|{% include \".+?\" %}")
 _HASH_COMMENT_PATTERN = re.compile(r"{# .+? #}")
 _BLOCK_COMMENT_PATTERN = re.compile(
     r"{% comment ('.*?' |\".*?\" )?%}[\s\S]*?{% endcomment %}"
 )
 _TOKEN_PATTERN = re.compile(r"{{ .+? }}|{% .+? %}")
-_LSTRIP_BLOCK_PATTERN = re.compile(r"\n( )+$")
+_LSTRIP_BLOCK_PATTERN = re.compile(r"\n +$")
+_YIELD_PATTERN = re.compile(r"\n +yield ")
 
 
 def _find_extends(template: str):
     return _EXTENDS_PATTERN.search(template)
 
 
 def _find_block(template: str):
     return _BLOCK_PATTERN.search(template)
 
 
+def _find_any_non_whitespace(template: str):
+    return re.search(r"\S+", template)
+
+
+def _find_endblock(template: str, name: str = r"\w+?"):
+    return re.search(r"{% endblock " + name + r" %}", template)
+
+
 def _find_include(template: str):
     return _INCLUDE_PATTERN.search(template)
 
 
-def _find_named_endblock(template: str, name: str):
-    return re.search(r"{% endblock " + name + r" %}", template)
+def _find_hash_comment(template: str):
+    return _HASH_COMMENT_PATTERN.search(template)
+
+
+def _find_block_comment(template: str):
+    return _BLOCK_COMMENT_PATTERN.search(template)
+
+
+def _find_token(template: str):
+    return _TOKEN_PATTERN.search(template)
+
+
+def _token_is_on_own_line(text_before_token: str) -> bool:
+    return _LSTRIP_BLOCK_PATTERN.search(text_before_token) is not None
+
+
+def _contains_any_yield_statement(function_def: str) -> bool:
+    return _YIELD_PATTERN.search(function_def) is not None
 
 
 def _exists_and_is_file(path: str) -> bool:
     try:
         return (os.stat(path)[0] & 0b_11110000_00000000) == 0b_10000000_00000000
     except OSError:
         return False
@@ -201,72 +248,132 @@
 def _resolve_includes(template: str):
     while (include_match := _find_include(template)) is not None:
         template_path = include_match.group(0)[12:-4]
 
         # TODO: Restrict include to specific directory
 
         if not _exists_and_is_file(template_path):
-            raise OSError(f"Include template not found: {template_path}")
+            raise TemplateNotFoundError(template_path)
 
         # Replace the include with the template content
         with open(template_path, "rt", encoding="utf-8") as template_file:
             template = (
                 template[: include_match.start()]
                 + template_file.read()
                 + template[include_match.end() :]
             )
     return template
 
 
-def _check_for_unsupported_nested_blocks(template: str):
-    if _find_block(template) is not None:
-        raise SyntaxError("Nested blocks are not supported")
-
-
-def _resolve_includes_blocks_and_extends(template: str):
+def _resolve_includes_blocks_and_extends(  # pylint: disable=,too-many-locals
+    template: str,
+):
+    extended_templates: "set[str]" = set()
     block_replacements: "dict[str, str]" = {}
 
     # Processing nested child templates
     while (extends_match := _find_extends(template)) is not None:
-        extended_template_name = extends_match.group(0)[12:-4]
+        extended_template_path = extends_match.group(0)[12:-4]
+
+        if not _exists_and_is_file(extended_template_path):
+            raise TemplateNotFoundError(extended_template_path)
+
+        # Check for circular extends
+        if extended_template_path in extended_templates:
+            raise TemplateSyntaxError(
+                Token(
+                    template,
+                    extends_match.start(),
+                    extends_match.end(),
+                ),
+                "Circular extends",
+            )
 
         # Load extended template
+        extended_templates.add(extended_template_path)
         with open(
-            extended_template_name, "rt", encoding="utf-8"
+            extended_template_path, "rt", encoding="utf-8"
         ) as extended_template_file:
             extended_template = extended_template_file.read()
 
-        # Removed the extend tag
-        template = template[extends_match.end() :]
+        offset = extends_match.end()
 
         # Resolve includes
         template = _resolve_includes(template)
 
+        # Check for any stacked extends
+        if stacked_extends_match := _find_extends(template[extends_match.end() :]):
+            raise TemplateSyntaxError(
+                Token(
+                    template,
+                    extends_match.end() + stacked_extends_match.start(),
+                    extends_match.end() + stacked_extends_match.end(),
+                ),
+                "Incorrect use of {% extends ... %}",
+            )
+
         # Save block replacements
-        while (block_match := _find_block(template)) is not None:
+        while (block_match := _find_block(template[offset:])) is not None:
             block_name = block_match.group(0)[9:-3]
 
-            endblock_match = _find_named_endblock(template, block_name)
-
-            if endblock_match is None:
-                raise SyntaxError("Missing {% endblock %} for block: " + block_name)
+            # Check for anything between blocks
+            if content_between_blocks := _find_any_non_whitespace(
+                template[offset : offset + block_match.start()]
+            ):
+                raise TemplateSyntaxError(
+                    Token(
+                        template,
+                        offset + content_between_blocks.start(),
+                        offset + content_between_blocks.end(),
+                    ),
+                    "Content outside block",
+                )
 
-            block_content = template[block_match.end() : endblock_match.start()]
+            if not (endblock_match := _find_endblock(template[offset:], block_name)):
+                raise TemplateSyntaxError(
+                    Token(
+                        template,
+                        offset + block_match.start(),
+                        offset + block_match.end(),
+                    ),
+                    "No matching {% endblock %}",
+                )
 
-            _check_for_unsupported_nested_blocks(block_content)
+            block_content = template[
+                offset + block_match.end() : offset + endblock_match.start()
+            ]
+
+            # Check for unsupported nested blocks
+            if (nested_block_match := _find_block(block_content)) is not None:
+                raise TemplateSyntaxError(
+                    Token(
+                        template,
+                        offset + block_match.end() + nested_block_match.start(),
+                        offset + block_match.end() + nested_block_match.end(),
+                    ),
+                    "Nested blocks are not supported",
+                )
 
             if block_name in block_replacements:
                 block_replacements[block_name] = block_replacements[block_name].replace(
                     r"{{ block.super }}", block_content
                 )
             else:
                 block_replacements.setdefault(block_name, block_content)
 
-            template = (
-                template[: block_match.start()] + template[endblock_match.end() :]
+            offset += endblock_match.end()
+
+        if content_after_last_endblock := _find_any_non_whitespace(template[offset:]):
+            raise TemplateSyntaxError(
+                Token(
+                    template,
+                    offset + content_after_last_endblock.start(),
+                    offset + content_after_last_endblock.end(),
+                ),
+                "Content outside block",
             )
 
         template = extended_template
 
     # Resolve includes in top-level template
     template = _resolve_includes(template)
 
@@ -275,28 +382,37 @@
 
 def _replace_blocks_with_replacements(template: str, replacements: "dict[str, str]"):
     # Replace blocks in top-level template
     while (block_match := _find_block(template)) is not None:
         block_name = block_match.group(0)[9:-3]
 
         # Self-closing block tag without default content
-        if (endblock_match := _find_named_endblock(template, block_name)) is None:
+        if (endblock_match := _find_endblock(template, block_name)) is None:
             replacement = replacements.get(block_name, "")
 
             template = (
                 template[: block_match.start()]
                 + replacement
                 + template[block_match.end() :]
             )
 
         # Block with default content
         else:
             block_content = template[block_match.end() : endblock_match.start()]
 
-            _check_for_unsupported_nested_blocks(block_content)
+            # Check for unsupported nested blocks
+            if (nested_block_match := _find_block(block_content)) is not None:
+                raise TemplateSyntaxError(
+                    Token(
+                        template,
+                        block_match.end() + nested_block_match.start(),
+                        block_match.end() + nested_block_match.end(),
+                    ),
+                    "Nested blocks are not supported",
+                )
 
             # No replacement for this block, use default content
             if block_name not in replacements:
                 template = (
                     template[: block_match.start()]
                     + block_content
                     + template[endblock_match.end() :]
@@ -313,22 +429,14 @@
                     + replacement
                     + template[endblock_match.end() :]
                 )
 
     return template
 
 
-def _find_hash_comment(template: str):
-    return _HASH_COMMENT_PATTERN.search(template)
-
-
-def _find_block_comment(template: str):
-    return _BLOCK_COMMENT_PATTERN.search(template)
-
-
 def _remove_comments(
     template: str,
     *,
     trim_blocks: bool = True,
     lstrip_blocks: bool = True,
 ):
     def _remove_matched_comment(template: str, comment_match: re.Match):
@@ -354,262 +462,255 @@
     # Remove block comments: {% comment %} ... {% endcomment %}
     while (comment_match := _find_block_comment(template)) is not None:
         template = _remove_matched_comment(template, comment_match)
 
     return template
 
 
-def _find_token(template: str):
-    return _TOKEN_PATTERN.search(template)
-
-
-def _token_is_on_own_line(text_before_token: str) -> bool:
-    return _LSTRIP_BLOCK_PATTERN.search(text_before_token) is not None
-
-
 def _create_template_rendering_function(  # pylint: disable=,too-many-locals,too-many-branches,too-many-statements
     template: str,
-    language: str = Language.HTML,
     *,
     trim_blocks: bool = True,
     lstrip_blocks: bool = True,
     function_name: str = "__template_rendering_function",
     context_name: str = "context",
-    dry_run: bool = False,
-) -> "Generator[str] | str":
+) -> "Generator[str]":
     # Resolve includes, blocks and extends
     template = _resolve_includes_blocks_and_extends(template)
 
     # Remove comments
     template = _remove_comments(template)
 
     # Create definition of the template function
-    function_string = f"def {function_name}({context_name}):\n"
-    indent, indentation_level = "    ", 1
+    function_def = f"def {function_name}({context_name}):\n"
+    indent_level = 1
+
+    def indented(fragment: str, end: str = "\n") -> str:
+        nonlocal indent_level
+        return "    " * indent_level + fragment + end
 
     # Keep track of the template state
-    nested_if_statements: "list[str]" = []
-    nested_for_loops: "list[str]" = []
-    nested_while_loops: "list[str]" = []
-    nested_autoescape_modes: "list[str]" = []
+    nested_if_statements: "list[Token]" = []
+    nested_for_loops: "list[Token]" = []
+    nested_while_loops: "list[Token]" = []
+    nested_autoescape_modes: "list[Token]" = []
     last_token_was_block = False
+    offset = 0
 
     # Resolve tokens
-    while (token_match := _find_token(template)) is not None:
-        token = token_match.group(0)
+    while (token_match := _find_token(template[offset:])) is not None:
+        token = Token(
+            template,
+            offset + token_match.start(),
+            offset + token_match.end(),
+        )
 
         # Add the text before the token
-        if text_before_token := template[: token_match.start()]:
-            if lstrip_blocks and token.startswith(r"{% "):
+        if text_before_token := template[offset : offset + token_match.start()]:
+            if lstrip_blocks and token.content.startswith(r"{% "):
                 if _token_is_on_own_line(text_before_token):
                     text_before_token = text_before_token.rstrip(" ")
 
             if trim_blocks:
                 if last_token_was_block and text_before_token.startswith("\n"):
                     text_before_token = text_before_token[1:]
 
         if text_before_token:
-            function_string += (
-                indent * indentation_level + f"yield {repr(text_before_token)}\n"
-            )
+            function_def += indented(f"yield {repr(text_before_token)}")
         else:
-            function_string += indent * indentation_level + "pass\n"
+            function_def += indented("pass")
 
         # Token is an expression
-        if token.startswith(r"{{ "):
+        if token.content.startswith(r"{{ "):
             last_token_was_block = False
 
             if nested_autoescape_modes:
-                autoescape = nested_autoescape_modes[-1][14:-3] == "on"
+                autoescape = nested_autoescape_modes[-1].content[14:-3] == "on"
             else:
                 autoescape = True
 
-            # Expression should be escaped with language-specific function
+            # Expression should be escaped
             if autoescape:
-                function_string += (
-                    indent * indentation_level
-                    + f"yield safe_{language.lower()}({token[3:-3]})\n"
-                )
+                function_def += indented(f"yield safe_html({token.content[3:-3]})")
             # Expression should not be escaped
             else:
-                function_string += (
-                    indent * indentation_level + f"yield str({token[3:-3]})\n"
-                )
+                function_def += indented(f"yield {token.content[3:-3]}")
 
         # Token is a statement
-        elif token.startswith(r"{% "):
+        elif token.content.startswith(r"{% "):
             last_token_was_block = True
 
             # Token is a some sort of if statement
-            if token.startswith(r"{% if "):
-                function_string += indent * indentation_level + f"{token[3:-3]}:\n"
-                indentation_level += 1
+            if token.content.startswith(r"{% if "):
+                function_def += indented(f"if {token.content[6:-3]}:")
+                indent_level += 1
 
                 nested_if_statements.append(token)
-            elif token.startswith(r"{% elif "):
-                indentation_level -= 1
-                function_string += indent * indentation_level + f"{token[3:-3]}:\n"
-                indentation_level += 1
-            elif token == r"{% else %}":
-                indentation_level -= 1
-                function_string += indent * indentation_level + "else:\n"
-                indentation_level += 1
-            elif token == r"{% endif %}":
-                indentation_level -= 1
+            elif token.content.startswith(r"{% elif "):
+                if not nested_if_statements:
+                    raise TemplateSyntaxError(token, "No matching {% if ... %}")
 
+                indent_level -= 1
+                function_def += indented(f"elif {token.content[8:-3]}:")
+                indent_level += 1
+            elif token.content == r"{% else %}":
                 if not nested_if_statements:
-                    raise SyntaxError("Missing {% if ... %} block for {% endif %}")
+                    raise TemplateSyntaxError(token, "No matching {% if ... %}")
 
+                indent_level -= 1
+                function_def += indented("else:")
+                indent_level += 1
+            elif token.content == r"{% endif %}":
+                if not nested_if_statements:
+                    raise TemplateSyntaxError(token, "No matching {% if ... %}")
+
+                indent_level -= 1
                 nested_if_statements.pop()
 
             # Token is a for loop
-            elif token.startswith(r"{% for "):
-                function_string += indent * indentation_level + f"{token[3:-3]}:\n"
-                indentation_level += 1
+            elif token.content.startswith(r"{% for "):
+                function_def += indented(f"for {token.content[7:-3]}:")
+                indent_level += 1
 
                 nested_for_loops.append(token)
-            elif token == r"{% empty %}":
-                indentation_level -= 1
-                last_forloop_iterable = nested_for_loops[-1][3:-3].split(" in ", 1)[1]
+            elif token.content == r"{% empty %}":
+                if not nested_for_loops:
+                    raise TemplateSyntaxError(token, "No matching {% for ... %}")
 
-                function_string += (
-                    indent * indentation_level + f"if not {last_forloop_iterable}:\n"
+                last_forloop_iterable = (
+                    nested_for_loops[-1].content[3:-3].split(" in ", 1)[1]
                 )
-                indentation_level += 1
-            elif token == r"{% endfor %}":
-                indentation_level -= 1
 
+                indent_level -= 1
+                function_def += indented(f"if not {last_forloop_iterable}:")
+                indent_level += 1
+            elif token.content == r"{% endfor %}":
                 if not nested_for_loops:
-                    raise SyntaxError("Missing {% for ... %} block for {% endfor %}")
+                    raise TemplateSyntaxError(token, "No matching {% for ... %}")
 
+                indent_level -= 1
                 nested_for_loops.pop()
 
             # Token is a while loop
-            elif token.startswith(r"{% while "):
-                function_string += indent * indentation_level + f"{token[3:-3]}:\n"
-                indentation_level += 1
+            elif token.content.startswith(r"{% while "):
+                function_def += indented(f"while {token.content[9:-3]}:")
+                indent_level += 1
 
                 nested_while_loops.append(token)
-            elif token == r"{% endwhile %}":
-                indentation_level -= 1
-
+            elif token.content == r"{% endwhile %}":
                 if not nested_while_loops:
-                    raise SyntaxError(
-                        "Missing {% while ... %} block for {% endwhile %}"
-                    )
+                    raise TemplateSyntaxError(token, "No matching {% while ... %}")
 
+                indent_level -= 1
                 nested_while_loops.pop()
 
             # Token is a Python code
-            elif token.startswith(r"{% exec "):
-                expression = token[8:-3]
-                function_string += indent * indentation_level + f"{expression}\n"
-
-            # Token is autoescape mode change
-            elif token.startswith(r"{% autoescape "):
-                mode = token[14:-3]
+            elif token.content.startswith(r"{% exec "):
+                function_def += indented(f"{token.content[8:-3]}")
+
+            # Token is a autoescape mode change
+            elif token.content.startswith(r"{% autoescape "):
+                mode = token.content[14:-3]
                 if mode not in ("on", "off"):
                     raise ValueError(f"Unknown autoescape mode: {mode}")
 
                 nested_autoescape_modes.append(token)
 
-            elif token == r"{% endautoescape %}":
+            elif token.content == r"{% endautoescape %}":
                 if not nested_autoescape_modes:
-                    raise SyntaxError(
-                        "Missing {% autoescape ... %} block for {% endautoescape %}"
-                    )
+                    raise TemplateSyntaxError(token, "No matching {% autoescape ... %}")
 
                 nested_autoescape_modes.pop()
 
+            # Token is a endblock in top-level template
+            elif token.content.startswith(r"{% endblock "):
+                raise TemplateSyntaxError(token, "No matching {% block ... %}")
+
+            # Token is a extends in top-level template
+            elif token.content.startswith(r"{% extends "):
+                raise TemplateSyntaxError(token, "Incorrect use of {% extends ... %}")
+
             else:
-                raise SyntaxError(f"Unknown token type: {token}")
+                raise TemplateSyntaxError(token, f"Unknown token: {token.content}")
 
         else:
-            raise SyntaxError(f"Unknown token type: {token}")
+            raise TemplateSyntaxError(token, f"Unknown token: {token.content}")
 
-        # Continue with the rest of the template
-        template = template[token_match.end() :]
+        # Move offset to the end of the token
+        offset += token_match.end()
 
     # Checking for unclosed blocks
     if len(nested_if_statements) > 0:
         last_if_statement = nested_if_statements[-1]
-        raise SyntaxError("Missing {% endif %} for " + last_if_statement)
+        raise TemplateSyntaxError(last_if_statement, "No matching {% endif %}")
 
     if len(nested_for_loops) > 0:
         last_for_loop = nested_for_loops[-1]
-        raise SyntaxError("Missing {% endfor %} for " + last_for_loop)
+        raise TemplateSyntaxError(last_for_loop, "No matching {% endfor %}")
 
     if len(nested_while_loops) > 0:
         last_while_loop = nested_while_loops[-1]
-        raise SyntaxError("Missing {% endwhile %} for " + last_while_loop)
+        raise TemplateSyntaxError(last_while_loop, "No matching {% endwhile %}")
 
     # No check for unclosed autoescape blocks, as they are optional and do not result in errors
 
     # Add the text after the last token (if any)
-    text_after_last_token = template
+    text_after_last_token = template[offset:]
 
     if text_after_last_token:
         if trim_blocks and text_after_last_token.startswith("\n"):
             text_after_last_token = text_after_last_token[1:]
 
-        function_string += (
-            indent * indentation_level + f"yield {repr(text_after_last_token)}\n"
-        )
+        function_def += indented(f"yield {repr(text_after_last_token)}")
 
-    # If dry run, return the template function string
-    if dry_run:
-        return function_string
+    # Make sure the function definition contains at least one yield statement
+    if not _contains_any_yield_statement(function_def):
+        function_def += indented('yield ""')
 
     # Create and return the template function
-    exec(function_string)  # pylint: disable=exec-used
+    exec(function_def)  # pylint: disable=exec-used
     return locals()[function_name]
 
 
 def _yield_as_sized_chunks(
     generator: "Generator[str]", chunk_size: int
 ) -> "Generator[str]":
     """Yields resized chunks from the ``generator``."""
 
     # Yield chunks with a given size
     chunk = ""
+    already_yielded = False
+
     for item in generator:
         chunk += item
 
         if chunk_size <= len(chunk):
             yield chunk[:chunk_size]
             chunk = chunk[chunk_size:]
+            already_yielded = True
 
     # Yield the last chunk
-    if chunk:
+    if chunk or not already_yielded:
         yield chunk
 
 
 class Template:
     """
     Class that loads a template from ``str`` and allows to rendering it with different contexts.
     """
 
     _template_function: "Generator[str]"
 
-    def __init__(self, template_string: str, *, language: str = Language.HTML) -> None:
+    def __init__(self, template_string: str) -> None:
         """
         Creates a reusable template from the given template string.
 
-        For better performance, instantiate the template in global scope and reuse it as many times.
-        If memory is a concern, instantiate the template in a function or method that uses it.
-
-        By default, the template is rendered as HTML. To render it as XML or Markdown, use the
-        ``language`` parameter.
-
         :param str template_string: String containing the template to be rendered
-        :param str language: Language for autoescaping. Defaults to HTML
         """
-        self._template_function = _create_template_rendering_function(
-            template_string, language
-        )
+        self._template_function = _create_template_rendering_function(template_string)
 
     def render_iter(
         self, context: dict = None, *, chunk_size: int = None
     ) -> "Generator[str]":
         """
         Renders the template using the provided context and returns a generator that yields the
         rendered output.
@@ -651,123 +752,180 @@
 
 
 class FileTemplate(Template):
     """
     Class that loads a template from a file and allows to rendering it with different contexts.
     """
 
-    def __init__(self, template_path: str, *, language: str = Language.HTML) -> None:
+    def __init__(self, template_path: str) -> None:
         """
         Loads a file and creates a reusable template from its contents.
 
-        For better performance, instantiate the template in global scope and reuse it as many times.
-        If memory is a concern, instantiate the template in a function or method that uses it.
-
-        By default, the template is rendered as HTML. To render it as XML or Markdown, use the
-        ``language`` parameter.
-
         :param str template_path: Path to a file containing the template to be rendered
-        :param str language: Language for autoescaping. Defaults to HTML
         """
+
+        if not _exists_and_is_file(template_path):
+            raise TemplateNotFoundError(template_path)
+
         with open(template_path, "rt", encoding="utf-8") as template_file:
             template_string = template_file.read()
-        super().__init__(template_string, language=language)
+        super().__init__(template_string)
+
+
+_CACHE: "dict[int, Template| FileTemplate]" = {}
 
 
 def render_string_iter(
     template_string: str,
     context: dict = None,
     *,
     chunk_size: int = None,
-    language: str = Language.HTML,
+    cache: bool = True,
 ):
     """
     Creates a `Template` from the given ``template_string`` and renders it using the provided
     ``context``. Returns a generator that yields the rendered output.
 
+    If ``cache`` is ``True``, the template is saved and reused on next calls, even with different
+    contexts.
+
     :param dict context: Dictionary containing the context for the template
     :param int chunk_size: Size of the chunks to be yielded. If ``None``, the generator yields
         the template in chunks sized specifically for the given template
-    :param str language: Language for autoescaping. Defaults to HTML
+    :param bool cache: When ``True``, the template is saved and reused on next calls.
 
     Example::
 
         list(render_string_iter(r"Hello {{ name }}!", {"name": "World"}))
         # ['Hello ', 'World', '!']
 
         list(render_string_iter(r"Hello {{ name }}!", {"name": "CircuitPython"}, chunk_size=3))
         # ['Hel', 'lo ', 'Cir', 'cui', 'tPy', 'tho', 'n!']
     """
-    return Template(template_string, language=language).render_iter(
-        context or {}, chunk_size=chunk_size
+    key = hash(template_string)
+
+    if cache and key in _CACHE:
+        return _yield_as_sized_chunks(
+            _CACHE[key].render_iter(context or {}, chunk_size), chunk_size
+        )
+
+    template = Template(template_string)
+
+    if cache:
+        _CACHE[key] = template
+
+    return _yield_as_sized_chunks(
+        template.render_iter(context or {}), chunk_size=chunk_size
     )
 
 
 def render_string(
     template_string: str,
     context: dict = None,
     *,
-    language: str = Language.HTML,
+    cache: bool = True,
 ):
     """
     Creates a `Template` from the given ``template_string`` and renders it using the provided
     ``context``. Returns the rendered output as a string.
 
+    If ``cache`` is ``True``, the template is saved and reused on next calls, even with different
+    contexts.
+
     :param dict context: Dictionary containing the context for the template
-    :param str language: Language for autoescaping. Defaults to HTML
+    :param bool cache: When ``True``, the template is saved and reused on next calls.
 
     Example::
 
         render_string(r"Hello {{ name }}!", {"name": "World"})
         # 'Hello World!'
     """
-    return Template(template_string, language=language).render(context or {})
+    key = hash(template_string)
+
+    if cache and key in _CACHE:
+        return _CACHE[key].render(context or {})
+
+    template = Template(template_string)
+
+    if cache:
+        _CACHE[key] = template
+
+    return template.render(context or {})
 
 
 def render_template_iter(
     template_path: str,
     context: dict = None,
     *,
     chunk_size: int = None,
-    language: str = Language.HTML,
+    cache: bool = True,
 ):
     """
     Creates a `FileTemplate` from the given ``template_path`` and renders it using the provided
     ``context``. Returns a generator that yields the rendered output.
 
+    If ``cache`` is ``True``, the template is saved and reused on next calls, even with different
+    contexts.
+
     :param dict context: Dictionary containing the context for the template
     :param int chunk_size: Size of the chunks to be yielded. If ``None``, the generator yields
         the template in chunks sized specifically for the given template
-    :param str language: Language for autoescaping. Defaults to HTML
+    :param bool cache: When ``True``, the template is saved and reused on next calls.
 
     Example::
 
         list(render_template_iter(..., {"name": "World"})) # r"Hello {{ name }}!"
         # ['Hello ', 'World', '!']
 
         list(render_template_iter(..., {"name": "CircuitPython"}, chunk_size=3))
         # ['Hel', 'lo ', 'Cir', 'cui', 'tPy', 'tho', 'n!']
     """
-    return FileTemplate(template_path, language=language).render_iter(
-        context or {}, chunk_size=chunk_size
+    key = hash(template_path)
+
+    if cache and key in _CACHE:
+        return _yield_as_sized_chunks(
+            _CACHE[key].render_iter(context or {}, chunk_size), chunk_size
+        )
+
+    template = FileTemplate(template_path)
+
+    if cache:
+        _CACHE[key] = template
+
+    return _yield_as_sized_chunks(
+        template.render_iter(context or {}, chunk_size=chunk_size), chunk_size
     )
 
 
 def render_template(
     template_path: str,
     context: dict = None,
     *,
-    language: str = Language.HTML,
+    cache: bool = True,
 ):
     """
     Creates a `FileTemplate` from the given ``template_path`` and renders it using the provided
     ``context``. Returns the rendered output as a string.
 
+    If ``cache`` is ``True``, the template is saved and reused on next calls, even with different
+    contexts.
+
     :param dict context: Dictionary containing the context for the template
-    :param str language: Language for autoescaping. Defaults to HTML
+    :param bool cache: When ``True``, the template is saved and reused on next calls.
 
     Example::
 
         render_template(..., {"name": "World"}) # r"Hello {{ name }}!"
         # 'Hello World!'
     """
-    return FileTemplate(template_path, language=language).render(context or {})
+
+    key = hash(template_path)
+
+    if cache and key in _CACHE:
+        return _CACHE[key].render(context or {})
+
+    template = FileTemplate(template_path)
+
+    if cache:
+        _CACHE[key] = template
+
+    return template.render(context or {})
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/docs/_static/favicon.ico` & `adafruit_circuitpython_templateengine-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/docs/conf.py` & `adafruit_circuitpython_templateengine-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/docs/examples.rst` & `adafruit_circuitpython_templateengine-2.0.0/docs/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,36 @@
 This example is printing a basic HTML page with with a dynamic paragraph.
 
 .. literalinclude:: ../examples/templateengine_simpletest.py
     :caption: examples/templateengine_simpletest.py
     :lines: 5-
     :linenos:
 
-Reusing templates
------------------
+Caching/Reusing templates
+-------------------------
 
-The are two main ways of rendering templates:
+The are two ways of rendering templates:
 
+- manually creating a ``Template`` or ``FileTemplate`` object and calling its method
 - using one of ``render_...`` methods
-- manually creating a ``Template`` object and calling its method
 
-While the first method is simpler, it also compiles the template on every call.
-The second method is more efficient when rendering the same template multiple times, as it allows
-to reuse the compiled template, at the cost of more memory usage.
 
-Both methods can be used interchangeably, as they both return the same result.
-It is up to the user to decide which method is more suitable for a given use case.
+By dafault, the ``render_...`` methods cache the template and reuse it on next calls.
+This speeds up the rendering process, but also uses more memory.
 
-**Generally, the first method will be sufficient for most use cases.**
+If for some reason the caching is not desired, you can disable it by passing ``cache=False`` to
+the ``render_...`` method. This will cause the template to be recreated on every call, which is slower,
+but uses less memory. This might be useful when rendering a large number of different templates that
+might not fit in the memory at the same time or are not used often enough to justify caching them.
 
-It is also worth noting that compiling all used templates using the second method might not be possible,
-depending on the project and board used, due to the limited amount of RAM.
 
 .. literalinclude:: ../examples/templateengine_reusing.py
     :caption: examples/templateengine_reusing.py
     :lines: 5-
-    :emphasize-lines: 1,16,20
+    :emphasize-lines: 22,27,34
     :linenos:
 
 Expressions
 -----------
 
 Token ``{{ ... }}`` is used for evaluating expressions.
 
@@ -230,34 +228,25 @@
     :lines: 5-
     :linenos:
 
 Autoescaping unsafe characters
 ------------------------------
 
 Token ``{% autoescape off %} ... {% endautoescape %}`` is used for marking a block of code that should
-be not be autoescaped. Consequently using ``{% autoescape off %} ...`` does the opposite and turns
+be not be autoescaped. Consequently using ``{% autoescape on %} ...`` does the opposite and turns
 the autoescaping back on.
 
 By default the template engine will escape all HTML-unsafe characters in expressions
 (e.g. ``<`` will be replaced with ``&lt;``).
 
 Content outside expressions is not escaped and is rendered as-is.
 
-For escaping XML and Markdown, you can use the ``language=`` parameter, both in ``render_...`` methods
-and in all ``Template`` constructors.
-
 .. literalinclude:: ../examples/autoescape.html
     :caption: examples/autoescape.html
     :lines: 7-
     :language: html
     :linenos:
 
-.. literalinclude:: ../examples/autoescape.md
-    :caption: examples/autoescape.md
-    :lines: 5-
-    :language: markdown
-    :linenos:
-
 .. literalinclude:: ../examples/templateengine_autoescape.py
     :caption: examples/templateengine_autoescape.py
     :lines: 5-
     :linenos:
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/docs/index.rst` & `adafruit_circuitpython_templateengine-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/autoescape.html` & `adafruit_circuitpython_templateengine-2.0.0/examples/autoescape.html`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     This would be a {{ "<b>bold text</b>" }}, but autoescaping is turned on, so all
     unsafe characters are escaped.
 
     {% autoescape off %}
         This is a {{ "<b>bold text</b>" }}, because autoescaping is turned off in this block.
 
         {% autoescape on %}
-            And againg, this is not a {{ "<b>bold text</b>" }},
+            And again, this is not a {{ "<b>bold text</b>" }},
             because in this block autoescaping is turned on again.
         {% endautoescape %}
     {% endautoescape %}
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 This would be a {{ "bboolldd tteexxtt" }}, but autoescaping is turned on, so all unsafe
 characters are escaped. {% autoescape off %} This is a {{ "bboolldd tteexxtt" }},
 because autoescaping is turned off in this block. {% autoescape on %} And
-againg, this is not a {{ "bboolldd tteexxtt" }}, because in this block autoescaping is
+again, this is not a {{ "bboolldd tteexxtt" }}, because in this block autoescaping is
 turned on again. {% endautoescape %} {% endautoescape %}
```

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/comments.html` & `adafruit_circuitpython_templateengine-2.0.0/examples/comments.html`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_exec.py` & `adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_exec.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_expressions.py` & `adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_expressions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_for_loops.py` & `adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_for_loops.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_if_statements.py` & `adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_if_statements.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/examples/templateengine_while_loops.py` & `adafruit_circuitpython_templateengine-2.0.0/examples/templateengine_while_loops.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-templateengine-1.2.0/pyproject.toml` & `adafruit_circuitpython_templateengine-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-templateengine"
 description = "Templating engine to substitute variables into a template string. Templates can also include conditional logic and loops. Often used for web pages."
-version = "1.2.0"
+version = "2.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TemplateEngine"}
 keywords = [
     "adafruit",
@@ -25,15 +25,14 @@
     "micropython",
     "templateengine",
     "template",
     "string",
     "substitution",
     "web",
     "html",
-    "xml",
     "escaping",
     "syntax",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
```

