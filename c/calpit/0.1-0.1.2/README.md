# Comparing `tmp/calpit-0.1.tar.gz` & `tmp/calpit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calpit-0.1.tar", last modified: Sat Apr 13 15:50:11 2024, max compression
+gzip compressed data, was "calpit-0.1.2.tar", last modified: Mon Apr 15 03:04:48 2024, max compression
```

## Comparing `calpit-0.1.tar` & `calpit-0.1.2.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.266517 calpit-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-13 15:50:03.000000 calpit-0.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-13 15:50:03.000000 calpit-0.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 15:50:03.000000 calpit-0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.254517 calpit-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.254517 calpit-0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 15:50:03.000000 calpit-0.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-13 15:50:03.000000 calpit-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-13 15:50:03.000000 calpit-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-13 15:50:03.000000 calpit-0.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-13 15:50:03.000000 calpit-0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 15:50:03.000000 calpit-0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-13 15:50:03.000000 calpit-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-13 15:50:03.000000 calpit-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-13 15:50:03.000000 calpit-0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-13 15:50:03.000000 calpit-0.1/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-13 15:50:03.000000 calpit-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-13 15:50:11.266517 calpit-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-13 15:50:03.000000 calpit-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:03.000000 calpit-0.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-13 15:50:03.000000 calpit-0.1/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 15:50:03.000000 calpit-0.1/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-13 15:50:03.000000 calpit-0.1/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-04-13 15:50:03.000000 calpit-0.1/docker/build_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-13 15:50:03.000000 calpit-0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-13 15:50:03.000000 calpit-0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-13 15:50:03.000000 calpit-0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 15:50:03.000000 calpit-0.1/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-13 15:50:03.000000 calpit-0.1/docs/notebooks/intro_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-13 15:50:03.000000 calpit-0.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 15:50:03.000000 calpit-0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-13 15:50:03.000000 calpit-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:50:11.266517 calpit-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.258517 calpit-0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-13 15:50:03.000000 calpit-0.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/src/calpit/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13033 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/diagnostics_and_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/example_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/src/calpit/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/ispline_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/src/calpit/nn/umnn/
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/umnn/MonotonicNN.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/umnn/NeuralIntegral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/umnn/ParallelNeuralIntegral.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/umnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-13 15:50:03.000000 calpit-0.1/src/calpit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/src/calpit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 15:50:11.000000 calpit-0.1/src/calpit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-04-13 15:50:03.000000 calpit-0.1/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:11.262517 calpit-0.1/tests/calpit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:50:03.000000 calpit-0.1/tests/calpit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 15:50:03.000000 calpit-0.1/tests/calpit/test_example_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.469302 calpit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 03:04:37.000000 calpit-0.1.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 03:04:37.000000 calpit-0.1.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-15 03:04:37.000000 calpit-0.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.457302 calpit-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.457302 calpit-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-15 03:04:37.000000 calpit-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-15 03:04:37.000000 calpit-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-15 03:04:37.000000 calpit-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 03:04:37.000000 calpit-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 03:04:37.000000 calpit-0.1.2/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 03:04:37.000000 calpit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-15 03:04:48.469302 calpit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-15 03:04:37.000000 calpit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:37.000000 calpit-0.1.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-15 03:04:37.000000 calpit-0.1.2/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 03:04:37.000000 calpit-0.1.2/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-15 03:04:37.000000 calpit-0.1.2/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-04-15 03:04:37.000000 calpit-0.1.2/docker/build_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/notebooks/intro_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 03:04:37.000000 calpit-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-15 03:04:37.000000 calpit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:04:48.469302 calpit-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-15 03:04:37.000000 calpit-0.1.2/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.461302 calpit-0.1.2/src/calpit/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/diagnostics_and_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/example_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.465302 calpit-0.1.2/src/calpit/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/ispline_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.465302 calpit-0.1.2/src/calpit/nn/umnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/umnn/MonotonicNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/umnn/NeuralIntegral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/umnn/ParallelNeuralIntegral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/umnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-15 03:04:37.000000 calpit-0.1.2/src/calpit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.465302 calpit-0.1.2/src/calpit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 03:04:48.000000 calpit-0.1.2/src/calpit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.465302 calpit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-04-15 03:04:37.000000 calpit-0.1.2/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:48.465302 calpit-0.1.2/tests/calpit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 03:04:37.000000 calpit-0.1.2/tests/calpit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 03:04:37.000000 calpit-0.1.2/tests/calpit/test_example_module.py
```

### Comparing `calpit-0.1/.copier-answers.yml` & `calpit-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.gitattributes` & `calpit-0.1.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `calpit-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `calpit-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/pull_request_template.md` & `calpit-0.1.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/asv-main.yml` & `calpit-0.1.2/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/asv-nightly.yml` & `calpit-0.1.2/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/asv-pr.yml` & `calpit-0.1.2/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/build-documentation.yml` & `calpit-0.1.2/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/pre-commit-ci.yml` & `calpit-0.1.2/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/publish-benchmarks-pr.yml` & `calpit-0.1.2/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/publish-to-pypi.yml` & `calpit-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/smoke-test.yml` & `calpit-0.1.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.github/workflows/testing-and-coverage.yml` & `calpit-0.1.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.gitignore` & `calpit-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.pre-commit-config.yaml` & `calpit-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `calpit-0.1/.setup_dev.sh` & `calpit-0.1.2/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `calpit-0.1/LICENSE` & `calpit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calpit-0.1/benchmarks/asv.conf.json` & `calpit-0.1.2/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `calpit-0.1/docker/Dockerfile` & `calpit-0.1.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `calpit-0.1/docs/Makefile` & `calpit-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calpit-0.1/docs/conf.py` & `calpit-0.1.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 # -- sphinx-copybutton configuration ----------------------------------------
 extensions.append("sphinx_copybutton")
 ## sets up the expected prompt text from console blocks, and excludes it from
 ## the text that goes into the clipboard.
 copybutton_exclude = ".linenos, .gp"
 copybutton_prompt_text = ">> "
 
+# -- sphinxcontrib-bibtex configuration --------------------------------------
+extensions.append("sphinxcontrib.bibtex")
+bibtex_bibfiles = ["refs.bib"]
+bibtex_default_style = "unsrt"
+bibtex_reference_style = "author_year"
+
 ## lets us suppress the copy button on select code blocks.
 copybutton_selector = "div:not(.no-copybutton) > div.highlight > pre"
 
 templates_path = []
 exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 
 # This assumes that sphinx-build is called from the root directory
@@ -52,7 +58,9 @@
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
 autoapi_ignore = ["*/__main__.py", "*/_version.py"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
 html_theme = "sphinx_rtd_theme"
+# Exclude checkpoint and build files from sphinx
+exclude_patterns = ["_build", "**.ipynb_checkpoints"]
```

### Comparing `calpit-0.1/docs/notebooks/intro_notebook.ipynb` & `calpit-0.1.2/docs/notebooks/intro_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `calpit-0.1/pyproject.toml` & `calpit-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,20 @@
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
+"numpy",
+"scipy",
+"prettytable",
+"torch",
+"torchvision",
+"tqdm",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/lee-group-cmu/Cal-PIT"
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
```

### Comparing `calpit-0.1/src/.pylintrc` & `calpit-0.1.2/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/diagnostics_and_calibration.py` & `calpit-0.1.2/src/calpit/diagnostics_and_calibration.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/metrics.py` & `calpit-0.1.2/src/calpit/metrics.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/ispline_nn.py` & `calpit-0.1.2/src/calpit/nn/ispline_nn.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/models.py` & `calpit-0.1.2/src/calpit/nn/models.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/umnn/MonotonicNN.py` & `calpit-0.1.2/src/calpit/nn/umnn/MonotonicNN.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/umnn/NeuralIntegral.py` & `calpit-0.1.2/src/calpit/nn/umnn/NeuralIntegral.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/umnn/ParallelNeuralIntegral.py` & `calpit-0.1.2/src/calpit/nn/umnn/ParallelNeuralIntegral.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/nn/utils.py` & `calpit-0.1.2/src/calpit/nn/utils.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit/utils.py` & `calpit-0.1.2/src/calpit/utils.py`

 * *Files identical despite different names*

### Comparing `calpit-0.1/src/calpit.egg-info/SOURCES.txt` & `calpit-0.1.2/src/calpit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 benchmarks/benchmarks.py
 docker/Dockerfile
 docker/build_image.sh
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
+docs/refs.bib
 docs/requirements.txt
 docs/notebooks/README.md
 docs/notebooks/intro_notebook.ipynb
 src/.pylintrc
 src/calpit/__init__.py
 src/calpit/_version.py
 src/calpit/datasets.py
```

### Comparing `calpit-0.1/tests/.pylintrc` & `calpit-0.1.2/tests/.pylintrc`

 * *Files identical despite different names*

