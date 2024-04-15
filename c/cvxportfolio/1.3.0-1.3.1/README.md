# Comparing `tmp/cvxportfolio-1.3.0.tar.gz` & `tmp/cvxportfolio-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-1.3.0.tar", last modified: Fri Mar 22 07:40:43 2024, max compression
+gzip compressed data, was "cvxportfolio-1.3.1.tar", last modified: Mon Apr 15 19:13:29 2024, max compression
```

## Comparing `cvxportfolio-1.3.0.tar` & `cvxportfolio-1.3.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.094394 cvxportfolio-1.3.0/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-1.3.0/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)    11358 2023-11-28 14:28:59.000000 cvxportfolio-1.3.0/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)    13958 2024-03-22 07:40:43.093699 cvxportfolio-1.3.0/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)    12626 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/README.rst
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.071614 cvxportfolio-1.3.0/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)     1013 2024-03-22 07:17:28.000000 cvxportfolio-1.3.0/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     3088 2024-01-10 13:06:18.000000 cvxportfolio-1.3.0/cvxportfolio/cache.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.075580 cvxportfolio-1.3.0/cvxportfolio/constraints/
--rw-r--r--   0 enzo       (501) staff       (20)     1678 2024-03-22 07:17:27.000000 cvxportfolio-1.3.0/cvxportfolio/constraints/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     5047 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/constraints/base_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    34953 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/constraints/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    42757 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/costs.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.077355 cvxportfolio-1.3.0/cvxportfolio/data/
--rw-r--r--   0 enzo       (501) staff       (20)     1102 2024-03-22 07:17:28.000000 cvxportfolio-1.3.0/cvxportfolio/data/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)    35137 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/data/market_data.py
--rw-r--r--   0 enzo       (501) staff       (20)    50510 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/data/symbol_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     2385 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    29603 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)    48403 2024-03-22 06:53:57.000000 cvxportfolio-1.3.0/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     8001 2024-02-20 17:24:15.000000 cvxportfolio-1.3.0/cvxportfolio/hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    37009 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)    36934 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)    11195 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    20848 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    32432 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.089726 cvxportfolio-1.3.0/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)     4157 2024-03-22 07:17:28.000000 cvxportfolio-1.3.0/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1251 2023-09-29 14:11:40.000000 cvxportfolio-1.3.0/cvxportfolio/tests/__main__.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-1.3.0/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-1.3.0/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)    14777 2024-01-10 13:06:18.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    11394 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    47775 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)    14451 2024-02-20 17:24:15.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)    27074 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     6219 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    26357 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     4771 2023-10-31 19:11:55.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9890 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    49180 2024-03-22 06:51:45.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)     3361 2024-02-20 17:24:15.000000 cvxportfolio-1.3.0/cvxportfolio/tests/test_utils.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-1.3.0/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     6391 2024-02-20 17:24:15.000000 cvxportfolio-1.3.0/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2024-03-22 07:40:43.091443 cvxportfolio-1.3.0/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)    13958 2024-03-22 07:40:43.000000 cvxportfolio-1.3.0/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1303 2024-03-22 07:40:43.000000 cvxportfolio-1.3.0/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2024-03-22 07:40:43.000000 cvxportfolio-1.3.0/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)      227 2024-03-22 07:40:43.000000 cvxportfolio-1.3.0/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2024-03-22 07:40:43.000000 cvxportfolio-1.3.0/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)     2574 2024-03-22 07:17:28.000000 cvxportfolio-1.3.0/pyproject.toml
--rw-r--r--   0 enzo       (501) staff       (20)       38 2024-03-22 07:40:43.094512 cvxportfolio-1.3.0/setup.cfg
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)      199 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/AUTHORS
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    11358 2023-12-13 09:54:59.000000 cvxportfolio-1.3.1/LICENSE
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    13950 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/PKG-INFO
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    12599 2024-04-06 09:38:48.000000 cvxportfolio-1.3.1/README.rst
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1013 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     3174 2024-04-04 19:18:10.000000 cvxportfolio-1.3.1/cvxportfolio/cache.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/constraints/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1678 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     5548 2024-04-02 16:10:25.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/base_constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    35921 2024-04-04 17:26:07.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    42653 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/costs.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/data/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1102 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/data/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    35784 2024-04-06 09:18:10.000000 cvxportfolio-1.3.1/cvxportfolio/data/market_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    51122 2024-04-04 19:45:16.000000 cvxportfolio-1.3.1/cvxportfolio/data/symbol_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     2385 2024-03-16 05:48:22.000000 cvxportfolio-1.3.1/cvxportfolio/errors.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    30419 2024-04-04 17:32:53.000000 cvxportfolio-1.3.1/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    48403 2024-03-22 08:30:04.000000 cvxportfolio-1.3.1/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     7981 2024-04-04 17:24:49.000000 cvxportfolio-1.3.1/cvxportfolio/hyperparameters.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    38894 2024-04-06 07:46:09.000000 cvxportfolio-1.3.1/cvxportfolio/policies.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    37195 2024-04-04 17:33:55.000000 cvxportfolio-1.3.1/cvxportfolio/result.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    11062 2024-04-02 16:10:25.000000 cvxportfolio-1.3.1/cvxportfolio/returns.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    21541 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/risks.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    32701 2024-03-31 17:12:52.000000 cvxportfolio-1.3.1/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/tests/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6099 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1285 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/__main__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   156730 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   149356 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14857 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    12037 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    50193 2024-04-04 19:56:22.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14443 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    27339 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6249 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_hyperparameters.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    31934 2024-04-04 18:04:07.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     9101 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_result.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     4779 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     9985 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    46115 2024-04-04 19:23:59.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     3389 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_utils.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   116620 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6364 2024-04-04 17:26:30.000000 cvxportfolio-1.3.1/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    13950 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1337 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)        1 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)      231 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)       13 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     2753 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/pyproject.toml
+-rw-r--r--   0 enzo      (1000) enzo      (1000)       38 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/setup.cfg
```

### Comparing `cvxportfolio-1.3.0/LICENSE` & `cvxportfolio-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/PKG-INFO` & `cvxportfolio-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 1.3.0
+Version: 1.3.1
 Summary: Portfolio optimization and back-testing.
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Maintainer-email: Enzo Busseti <enzo.busseti@gmail.com>
 License: Apache License (2.0)
 Project-URL: Homepage, https://www.cvxportfolio.com
 Project-URL: Repository, https://github.com/cvxgrp/cvxportfolio
 Description-Content-Type: text/x-rst
@@ -12,14 +12,15 @@
 License-File: AUTHORS
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: requests
 Requires-Dist: cvxpy
 Requires-Dist: multiprocess
+Requires-Dist: scs
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-github-style; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -32,27 +33,27 @@
 Requires-Dist: beautifulsoup4; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: beautifulsoup4; extra == "examples"
 Requires-Dist: lxml; extra == "examples"
 Requires-Dist: clarabel; extra == "examples"
 Requires-Dist: ecos; extra == "examples"
 
-`Cvxportfolio <https://www.cvxportfolio.com>`__
-===============================================
+`Cvxportfolio <https://www.cvxportfolio.com>`_
+==============================================
 
 |CVXportfolio on PyPI| |linting: pylint| |Coverage Status|
 |Documentation Status| |Apache 2.0 License| |Anaconda-Server Badge|
 
 
 Cvxportfolio is an object-oriented library for portfolio optimization
 and back-testing. It implements models described in the `accompanying paper
-<https://cvxportfolio.readthedocs.org/en/master/_static/cvx_portfolio.pdf>`_.
+<https://cvxportfolio.readthedocs.io/en/master/_static/cvx_portfolio.pdf>`_.
 
 The documentation of the library is at
-`www.cvxportfolio.com <https://www.cvxportfolio.com>`__.
+`www.cvxportfolio.com <https://www.cvxportfolio.com>`_.
 
 .. Installation
 
 *News:*
 
    Since end of 2023 we're running daily `example strategies
    <https://github.com/cvxgrp/cvxportfolio/tree/master/examples/strategies>`_
@@ -67,15 +68,15 @@
 environment by simple:
 
 .. code:: bash
 
    pip install -U cvxportfolio
 
 You can see how this works on our `Installation and Hello
-World <https://youtu.be/1ThOKEu371M>`__ youtube video. 
+World <https://youtu.be/1ThOKEu371M>`_ youtube video.
 Anaconda installs 
 `are also supported <https://anaconda.org/conda-forge/cvxportfolio>`_.
 
 Cvxportfolio's main dependencies are `Cvxpy <https://www.cvxpy.org>`_ for
 interfacing with numerical solvers and `Pandas <https://pandas.pydata.org/>`_
 for interfacing with databases. We don't require any specific version of our
 dependencies and test against all recent ones (up to a few years ago).
@@ -139,42 +140,42 @@
 the paper, and default parameters that are typical for the US stock
 market.
 
 Other examples
 --------------
 
 `Many examples 
-<https://www.cvxportfolio.com/en/stable/examples.html>`_
+<https://cvxportfolio.readthedocs.io/en/stable/examples.html>`_
 are shown in the documentation website, along with
 their output and comments.
 
 `Even more example scripts
 <https://github.com/cvxgrp/cvxportfolio/blob/master/examples>`_ 
 are available in the code repository. 
 
 `The original examples from the paper 
 <https://github.com/cvxgrp/cvxportfolio/tree/0.0.X/examples>`_ 
 are visible in a dedicated branch,
 and are being translated to run with the stable versions (``1.0.0`` and above) of the
 library. The translations are visible at `this documentation page
-<https://www.cvxportfolio.com/en/stable/examples/paper_examples.html>`_.
+<https://cvxportfolio.readthedocs.io/en/stable/examples/paper_examples.html>`_.
 
 We show in the example on `user-provided
-forecasters <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/user_provided_forecasters.py>`__
+forecasters <https://cvxportfolio.readthedocs.io/en/stable/examples/user_provided_forecasters.html>`_
 how the user can define custom classes to forecast the expected returns
 and covariances. These provide callbacks that are executed at each point
 in time during the back-test. The system enforces causality and safety
 against numerical errors. We recommend to always include the default
 forecasters that we provide in any analysis you may do, since they are
 very robust and well-tested.
 
 We show in the examples on `DOW30
-components <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/dow30_example.py>`__
+components <https://cvxportfolio.readthedocs.io/en/stable/examples/dow30.html>`_
 and `wide assets-classes
-ETFs <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/etfs_example.py>`__
+ETFs <https://cvxportfolio.readthedocs.io/en/stable/examples/etfs.html>`_
 how a simple sweep over hyper-parameters, taking advantage of our
 sophisticated parallel backtest machinery, quickly provides results on
 the best strategy to apply to any given selection of assets.
 
 Similar projects
 ----------------
 
@@ -212,52 +213,52 @@
 file.
 
 Development
 -----------
 
 To set up a development environment locally you should clone the
 repository (or, `fork on
-Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`__
+Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_
 and then clone your fork)
 
 .. code:: bash
 
    git clone https://github.com/cvxgrp/cvxportfolio.git
    cd cvxportfolio
 
 Then, you should have a look at our
-`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`__
-and possibly change the ``PYTHON`` variable to match your system’s
+`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`_
+and possibly change the ``PYTHON`` variable to match your system's
 python interpreter. Once you have done that,
 
 .. code:: bash
 
    make env
    make test
 
 This will replicate our `development
-environment <https://docs.python.org/3/library/venv.html>`__ and run our
+environment <https://docs.python.org/3/library/venv.html>`_ and run our
 test suite.
 
 You activate the shell environment with one of scripts in ``env/bin``
 (or ``env\Scripts`` on Windows), for example if you use bash on POSIX
 
 .. code:: bash
 
    source env/bin/activate
 
 and from the environment you can run any of the scripts in the examples
 (the cvxportfolio package is installed in `editable
-mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`__).
+mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`_).
 Or, if you don't want to activate the environment, you can just run
 scripts directly using ``env/bin/python`` (or ``env\Scripts\python`` on
 Windows) like we do in the Makefile.
 
 Additionally, to match our CI/CD pipeline, you may set the following
-`git hooks <https://git-scm.com/docs/githooks>`__
+`git hooks <https://git-scm.com/docs/githooks>`_
 
 .. code:: bash
 
    echo "make lint" > .git/hooks/pre-commit
    chmod +x .git/hooks/pre-commit
    echo "make test" > .git/hooks/pre-push
    chmod +x .git/hooks/pre-push
```

### Comparing `cvxportfolio-1.3.0/README.rst` & `cvxportfolio-1.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-`Cvxportfolio <https://www.cvxportfolio.com>`__
-===============================================
+`Cvxportfolio <https://www.cvxportfolio.com>`_
+==============================================
 
 |CVXportfolio on PyPI| |linting: pylint| |Coverage Status|
 |Documentation Status| |Apache 2.0 License| |Anaconda-Server Badge|
 
 
 Cvxportfolio is an object-oriented library for portfolio optimization
 and back-testing. It implements models described in the `accompanying paper
-<https://cvxportfolio.readthedocs.org/en/master/_static/cvx_portfolio.pdf>`_.
+<https://cvxportfolio.readthedocs.io/en/master/_static/cvx_portfolio.pdf>`_.
 
 The documentation of the library is at
-`www.cvxportfolio.com <https://www.cvxportfolio.com>`__.
+`www.cvxportfolio.com <https://www.cvxportfolio.com>`_.
 
 .. Installation
 
 *News:*
 
    Since end of 2023 we're running daily `example strategies
    <https://github.com/cvxgrp/cvxportfolio/tree/master/examples/strategies>`_
@@ -29,15 +29,15 @@
 environment by simple:
 
 .. code:: bash
 
    pip install -U cvxportfolio
 
 You can see how this works on our `Installation and Hello
-World <https://youtu.be/1ThOKEu371M>`__ youtube video. 
+World <https://youtu.be/1ThOKEu371M>`_ youtube video.
 Anaconda installs 
 `are also supported <https://anaconda.org/conda-forge/cvxportfolio>`_.
 
 Cvxportfolio's main dependencies are `Cvxpy <https://www.cvxpy.org>`_ for
 interfacing with numerical solvers and `Pandas <https://pandas.pydata.org/>`_
 for interfacing with databases. We don't require any specific version of our
 dependencies and test against all recent ones (up to a few years ago).
@@ -101,42 +101,42 @@
 the paper, and default parameters that are typical for the US stock
 market.
 
 Other examples
 --------------
 
 `Many examples 
-<https://www.cvxportfolio.com/en/stable/examples.html>`_
+<https://cvxportfolio.readthedocs.io/en/stable/examples.html>`_
 are shown in the documentation website, along with
 their output and comments.
 
 `Even more example scripts
 <https://github.com/cvxgrp/cvxportfolio/blob/master/examples>`_ 
 are available in the code repository. 
 
 `The original examples from the paper 
 <https://github.com/cvxgrp/cvxportfolio/tree/0.0.X/examples>`_ 
 are visible in a dedicated branch,
 and are being translated to run with the stable versions (``1.0.0`` and above) of the
 library. The translations are visible at `this documentation page
-<https://www.cvxportfolio.com/en/stable/examples/paper_examples.html>`_.
+<https://cvxportfolio.readthedocs.io/en/stable/examples/paper_examples.html>`_.
 
 We show in the example on `user-provided
-forecasters <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/user_provided_forecasters.py>`__
+forecasters <https://cvxportfolio.readthedocs.io/en/stable/examples/user_provided_forecasters.html>`_
 how the user can define custom classes to forecast the expected returns
 and covariances. These provide callbacks that are executed at each point
 in time during the back-test. The system enforces causality and safety
 against numerical errors. We recommend to always include the default
 forecasters that we provide in any analysis you may do, since they are
 very robust and well-tested.
 
 We show in the examples on `DOW30
-components <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/dow30_example.py>`__
+components <https://cvxportfolio.readthedocs.io/en/stable/examples/dow30.html>`_
 and `wide assets-classes
-ETFs <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/etfs_example.py>`__
+ETFs <https://cvxportfolio.readthedocs.io/en/stable/examples/etfs.html>`_
 how a simple sweep over hyper-parameters, taking advantage of our
 sophisticated parallel backtest machinery, quickly provides results on
 the best strategy to apply to any given selection of assets.
 
 Similar projects
 ----------------
 
@@ -174,52 +174,52 @@
 file.
 
 Development
 -----------
 
 To set up a development environment locally you should clone the
 repository (or, `fork on
-Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`__
+Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_
 and then clone your fork)
 
 .. code:: bash
 
    git clone https://github.com/cvxgrp/cvxportfolio.git
    cd cvxportfolio
 
 Then, you should have a look at our
-`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`__
-and possibly change the ``PYTHON`` variable to match your system’s
+`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`_
+and possibly change the ``PYTHON`` variable to match your system's
 python interpreter. Once you have done that,
 
 .. code:: bash
 
    make env
    make test
 
 This will replicate our `development
-environment <https://docs.python.org/3/library/venv.html>`__ and run our
+environment <https://docs.python.org/3/library/venv.html>`_ and run our
 test suite.
 
 You activate the shell environment with one of scripts in ``env/bin``
 (or ``env\Scripts`` on Windows), for example if you use bash on POSIX
 
 .. code:: bash
 
    source env/bin/activate
 
 and from the environment you can run any of the scripts in the examples
 (the cvxportfolio package is installed in `editable
-mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`__).
+mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`_).
 Or, if you don't want to activate the environment, you can just run
 scripts directly using ``env/bin/python`` (or ``env\Scripts\python`` on
 Windows) like we do in the Makefile.
 
 Additionally, to match our CI/CD pipeline, you may set the following
-`git hooks <https://git-scm.com/docs/githooks>`__
+`git hooks <https://git-scm.com/docs/githooks>`_
 
 .. code:: bash
 
    echo "make lint" > .git/hooks/pre-commit
    chmod +x .git/hooks/pre-commit
    echo "make test" > .git/hooks/pre-push
    chmod +x .git/hooks/pre-push
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/__init__.py` & `cvxportfolio-1.3.1/cvxportfolio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Cvxportfolio __init__ module.
 
 This module only republishes the api of a selection of cvxportfolio
 modules. The __all__ attribute of each is used.
 """
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 from .constraints import *
 from .costs import *
 from .data import *
 from .hyperparameters import *
 from .policies import *
 from .result import *
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/cache.py` & `cvxportfolio-1.3.1/cvxportfolio/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import os
 import pickle
 
 logger = logging.getLogger(__name__)
 
 def _mp_init(l):
     """Shared lock to disk access for multiprocessing."""
-    global LOCK
+    # pylint: disable=global-variable-undefined
+    global LOCK # pragma: no cover
     LOCK = l # pragma: no cover
 
 # def _hash_universe(universe):
 #     """Hash given universe"""
 #     return hashlib.sha256(bytes(str(tuple(universe)), 'utf-8')).hexdigest()
 
 def cache_name(signature, base_location):
@@ -55,15 +56,15 @@
         with open(name, 'rb') as f:
             res = pickle.load(f)
             logger.info('Loaded cache %s', name)
             return res
     except FileNotFoundError:
         logger.info('Cache not found!')
         return {}
-    except EOFError:
+    except EOFError: # pragma: no cover
         logger.warning(
             'Cache file %s is corrupt! Discarding it.',
                 name) # pragma: no cover
         return {} # pragma: no cover
     finally:
         if 'LOCK' in globals():
             logger.debug( # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/constraints/__init__.py` & `cvxportfolio-1.3.1/cvxportfolio/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/constraints/base_constraints.py` & `cvxportfolio-1.3.1/cvxportfolio/constraints/base_constraints.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 from ..estimator import CvxpyExpressionEstimator, DataEstimator
 
 __all__ = ['Constraint', 'EqualityConstraint', 'InequalityConstraint']
 
 class Constraint(CvxpyExpressionEstimator):
     """Base cvxpy constraint class."""
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Compile constraint to cvxpy.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Reserved for future expansion.
+        :type kwargs: dict
+
         :returns: some cvxpy.constraints object, or list of those
         :rtype: cvxpy.constraints, list
         """
         raise NotImplementedError # pragma: no cover
 
 
 class EqualityConstraint(Constraint):
@@ -46,31 +49,35 @@
     :func:`InequalityConstraint._compile_constr_to_cvxpy` and
     :func:`InequalityConstraint._rhs` methods.
 
     We factor this code in order to streamline the
     design of :class:`SoftConstraint` costs.
     """
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Compile constraint to cvxpy.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Reserved for future expansion.
+        :type kwargs: dict
+
         :returns: Cvxpy constraints object.
         :rtype: cvxpy.constraints
         """
-        return self._compile_constr_to_cvxpy(w_plus, z, w_plus_minus_w_bm) ==\
-            self._rhs()
+        return self._compile_constr_to_cvxpy(
+            w_plus=w_plus, z=z, w_plus_minus_w_bm=w_plus_minus_w_bm, **kwargs
+                ) == self._rhs()
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Cvxpy expression of the left-hand side of the constraint."""
         raise NotImplementedError # pragma: no cover
 
     def _rhs(self):
         """Cvxpy expression of the right-hand side of the constraint."""
         raise NotImplementedError # pragma: no cover
 
@@ -83,35 +90,43 @@
     :func:`InequalityConstraint._compile_constr_to_cvxpy` and
     :func:`InequalityConstraint._rhs` methods.
 
     We factor this code in order to streamline the
     design of :class:`SoftConstraint` costs.
     """
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy(
+            self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Compile constraint to cvxpy.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Reserved for future expansion.
+        :type kwargs: dict
+
+        :raises ConvexityError: If the compiled constraint is not convex.
+
         :returns: Cvxpy constraints object.
         :rtype: cvxpy.constraints
         """
-        _ = self._compile_constr_to_cvxpy(w_plus, z, w_plus_minus_w_bm) <=\
-            self._rhs()
+
+        _ = self._compile_constr_to_cvxpy(
+            w_plus=w_plus, z=z, w_plus_minus_w_bm=w_plus_minus_w_bm, **kwargs
+                ) <= self._rhs()
         if not _.is_dcp():
             raise ConvexityError(f"The constraint {self} is not convex!")
         assert _.is_dcp(dpp=True)
         return _
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Cvxpy expression of the left-hand side of the constraint."""
         raise NotImplementedError # pragma: no cover
 
     def _rhs(self):
         """Cvxpy expression of the right-hand side of the constraint."""
         raise NotImplementedError # pragma: no cover
 
@@ -125,16 +140,17 @@
     is a scalar.
     """
 
     def __init__(self, cost, value):
         self.cost = cost
         self.value = DataEstimator(value, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, **kwargs):
         """Compile constraint to cvxpy."""
-        return self.cost.compile_to_cvxpy(w_plus, z, w_plus_minus_w_bm)
+        return self.cost.compile_to_cvxpy(**kwargs)
 
     def _rhs(self):
         return self.value.parameter
 
     def __repr__(self):
         return self.cost.__repr__() + ' <= ' + self.value.__repr__()
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/constraints/constraints.py` & `cvxportfolio-1.3.1/cvxportfolio/constraints/constraints.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 """This module defines user-facing constraints."""
 
 import cvxpy as cp
 import numpy as np
 
 from ..estimator import DataEstimator, Estimator
-from ..forecast import (HistoricalFactorizedCovariance,
-                        project_on_psd_cone_and_factorize)
+from ..forecast import HistoricalFactorizedCovariance
 from ..policies import MarketBenchmark
 from .base_constraints import (Constraint, EqualityConstraint,
                                InequalityConstraint)
 
 __all__ = [
     "LongOnly",
     "LeverageLimit",
@@ -46,15 +45,16 @@
     "TurnoverLimit",
     "MinCashBalance"
 ]
 
 class NoCash(EqualityConstraint):
     """Require that the cash balance is zero at each period."""
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus[-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return 0
 
@@ -120,15 +120,16 @@
         """
 
         factorized_covariance = self.covariance_forecaster.current_value
         bm = self.benchmark.current_value.iloc[:-1]
         self._market_vector.value = np.array(
             factorized_covariance @ (factorized_covariance.T @ bm))
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus[:-1].T @ self._market_vector
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return 0
 
@@ -149,15 +150,16 @@
         :class:`pd.Series` with datetime index.
     :type delta: float or pd.Series
     """
 
     def __init__(self, delta):
         self.delta = DataEstimator(delta, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, z, **kwargs):
         """Compile left hand side of the constraint expression."""
         return .5 * cp.norm1(z[:-1])
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.delta.parameter
 
@@ -174,16 +176,18 @@
     """
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
         self.volumes = DataEstimator(volumes)
         self.max_participation_rate = DataEstimator(
             max_fraction_of_volumes)
         self.portfolio_value = cp.Parameter(nonneg=True)
+        self._parameter = None
 
-    def initialize_estimator(self, universe, **kwargs):
+    def initialize_estimator( # pylint: disable=arguments-differ
+            self, universe, **kwargs):
         """Initialize internal parameter.
 
         :param universe: Current trading universe.
         :type universe: pd.Index
         :param kwargs: Unused arguments to initialize estimator.
         :type kwargs: dict
         """
@@ -199,15 +203,16 @@
         :type kwargs: dict
         """
         self.portfolio_value.value = current_portfolio_value
         self._parameter.value = (
             self.volumes.current_value
                 * self.max_participation_rate.current_value)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, z, **kwargs):
         """Compile left hand side of the constraint expression."""
         return cp.multiply(cp.abs(z[:-1]), self.portfolio_value)
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self._parameter
 
@@ -229,15 +234,16 @@
         also applies to the cash account.
     :type applies_to_cash: bool
     """
 
     def __init__(self, applies_to_cash=False):
         self.applies_to_cash = applies_to_cash
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Return a Cvxpy constraint."""
         return -(w_plus if self.applies_to_cash else w_plus[:-1])
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return 0
 
@@ -288,23 +294,24 @@
         if t in self.periods:
             self._low.value = 0.
             self._high.value = 0.
         else:
             self._low.value = -100.
             self._high.value = +100.
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, z, **kwargs):
         """Compile constraint to cvxpy, return list of two.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Unused arguments to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
+
+
         :returns: Two constraints.
         :rtype: list of cvxpy.constraints
         """
         return [z[self._index] >= self._low,
                 z[self._index] <= self._high]
 
 
@@ -325,15 +332,16 @@
         as a :class:`pd.Series` with datetime index.
     :type limit: float or pd.Series
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return cp.norm(w_plus[:-1], 1)
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.limit.parameter
 
@@ -367,15 +375,16 @@
         :param current_portfolio_value: Current total value of the portfolio.
         :type current_portfolio_value: float
         :param kwargs: Unused arguments passed to :meth:`values_in_time`.
         :type kwargs: dict
         """
         self.rhs.value = self.c_min.current_value/current_portfolio_value
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return -w_plus[-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return -self.rhs
 
@@ -407,15 +416,16 @@
 
         \mathbf{1}^T \max({(w_t + z_t)}_{1:n}, 0) =
             -\mathbf{1}^T \min({(w_t + z_t)}_{1:n}, 0)
 
     which is simply :math:`{(w_t + z_t)}_{n+1} = 1`.
     """
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus[-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return 1
 
@@ -447,15 +457,16 @@
         that are not traded then.
     :type limit: float, pandas.Series, pandas.DataFrame
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.limit.parameter
 
@@ -487,20 +498,22 @@
         that are not traded then.
     :type limit: float, pandas.Series, pandas.DataFrame
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return -w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
+        # pylint: disable=invalid-unary-operand-type
         return -self.limit.parameter
 
 class MaxBenchmarkDeviation(MaxWeights):
     r"""A max limit on post-trade weights minus the benchmark weights.
 
     In our notation, this is
 
@@ -526,15 +539,18 @@
         provide a value for each name that ever appear in a back-test; the
         data will be sliced according to the current trading universe during a
         back-test. It is fine to have missing values at certain times on assets
         that are not traded then.
     :type limit: float, pandas.Series, pandas.DataFrame
     """
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint pragma b/c we inherit from MaxWeights
+            # pylint: disable=arguments-renamed
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus_minus_w_bm[:-1]
 
 
 class MinBenchmarkDeviation(MinWeights):
     r"""A min limit on post-trade weights minus the benchmark weights.
 
@@ -562,15 +578,18 @@
         provide a value for each name that ever appear in a back-test; the
         data will be sliced according to the current trading universe during a
         back-test. It is fine to have missing values at certain times on assets
         that are not traded then.
     :type limit: float, pandas.Series, pandas.DataFrame
     """
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint pragma b/c we inherit from MinWeights
+            # pylint: disable=arguments-renamed
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile left hand side of the constraint expression."""
         return -w_plus_minus_w_bm[:-1]
 
 
 class MinMaxWeightsAtTimes(Estimator):
     """This class abstracts functionalities used by the two below.
 
@@ -637,21 +656,23 @@
     :type base_limit: float
     :param times: Times at which the constraint is active.
     :type times: iterable of pandas.Timestamp
     """
 
     sign = -1.  # used in values_in_time of parent class
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return -w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
-        return -self.limit
+        return -self.limit # pylint: disable=invalid-unary-operand-type
 
 
 class MaxWeightsAtTimes(MinMaxWeightsAtTimes, InequalityConstraint):
     """Require that at certain times the weights are smaller than a constant.
 
     .. note::
         This constraint is experimental and its interface may change, or we
@@ -660,15 +681,17 @@
     :param base_limit: Maximum limit of the weights.
     :type base_limit: float
     :param times: Times at which the constraint is active.
     :type times: iterable of pandas.Timestamp
     """
     sign = 1.  # used in values_in_time of parent class
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.limit
 
@@ -714,15 +737,17 @@
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True,
             ignore_shape_check=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return self.factor_exposure.parameter.T @ w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.limit.parameter
 
@@ -768,20 +793,23 @@
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True,
             ignore_shape_check=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return -self.factor_exposure.parameter.T @ w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
+        # pylint: disable=invalid-unary-operand-type
         return -self.limit.parameter
 
 
 class FactorGrossLimit(InequalityConstraint):
     r"""A gross limit on portfolio-wide factor (e.g. beta) exposure.
 
     It models the term:
@@ -823,15 +851,17 @@
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(
             factor_exposure, non_negative=True, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True,
             ignore_shape_check=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return self.factor_exposure.parameter.T @ cp.abs(w_plus[:-1])
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.limit.parameter
 
@@ -880,15 +910,17 @@
     """
 
     def __init__(self, factor_exposure, target):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.target = DataEstimator(target, compile_parameter=True)
 
-    def _compile_constr_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_constr_to_cvxpy(
+            # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile left hand side of the constraint expression."""
         return self.factor_exposure.parameter.T @ w_plus[:-1]
 
     def _rhs(self):
         """Compile right hand side of the constraint expression."""
         return self.target.parameter
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/costs.py` & `cvxportfolio-1.3.1/cvxportfolio/costs.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,30 +160,29 @@
 
     def __init__(self, left, right):
         self.left = left
         assert isinstance(left, Cost)
         self.right = right
         assert isinstance(right, Cost)
 
-    def compile_to_cvxpy(self, *args, **kwargs):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, **kwargs):
         """Compile cost by iterating over constituent costs.
 
-        :param args: Symbolic variables
-        :type args: tuple
         :param kwargs: Symbolic variables
         :type kwargs: dict
 
         :raises ConvexSpecificationError: If there are issues with the convex
             rules of the combined cost.
 
         :returns: Symbolic expression of the combined cost.
         :rtype: cvxpy.Expression
         """
         s = self.left.compile_to_cvxpy(
-            *args, **kwargs) + self.right.compile_to_cvxpy(*args, **kwargs)
+            **kwargs) + self.right.compile_to_cvxpy(**kwargs)
         if not s.is_dcp():
             raise ConvexSpecificationError(self)
         return s
 
     def __repr__(self):
         """Pretty print."""
         ri = str(self.right)
@@ -212,32 +211,31 @@
 
     def __init__(self, scalar, cost):
         self.scalar = scalar
         assert isinstance(scalar, (Number, HyperParameter))
         self.cost = cost
         assert isinstance(cost, Cost)
 
-    def compile_to_cvxpy(self, *args, **kwargs):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, **kwargs):
         """Compile cost by iterating over constituent costs.
 
-        :param args: Symbolic variables
-        :type args: tuple
         :param kwargs: Symbolic variables
         :type kwargs: dict
 
         :raises ConvexSpecificationError: If there are issues with convexity
             of the combined cost.
 
         :returns: Symbolic expression of the combined cost.
         :rtype: cvxpy.Expression
         """
         mul = _resolve_hyperpar(
-            self.scalar) * self.cost.compile_to_cvxpy(*args, **kwargs)
+            self.scalar) * self.cost.compile_to_cvxpy(**kwargs)
         if not mul.is_dcp():
-            raise ConvexSpecificationError(self) # pragma: no cover
+            raise ConvexSpecificationError(self)
         assert mul.is_dcp(dpp=True)
         return mul
 
     def __repr__(self):
         """Pretty print."""
         add_parenthesis = isinstance(self.cost, SumCost)
         result = '- ' if (self.scalar == -1) else (str(self.scalar) + ' * ')
@@ -270,35 +268,32 @@
     :type constraint: cvxportfolio.constraints.EqualityConstraint or
         cvxportfolio.constraints.InequalityConstraint
     """
 
     def __init__(self, constraint):
         self.constraint = constraint
 
-    def compile_to_cvxpy( # pylint: disable=inconsistent-return-statements
-        self, w_plus, z, w_plus_minus_w_bm):
+    # pylint: disable=inconsistent-return-statements
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, **kwargs):
         """Compile cost to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Symbolic variables.
+        :type kwargs: dict
 
         :raises SyntaxError: If the constraint is not a EqualityConstraint or
              InequalityConstraint.
 
         :return: Cvxpy expression of the soft constraint.
         :rtype: cvxpy.Expression
         """
 
         try:
             expr = (self.constraint._compile_constr_to_cvxpy(
-                w_plus, z, w_plus_minus_w_bm) - self.constraint._rhs())
+                **kwargs) - self.constraint._rhs())
 
         except AttributeError as exc:
             raise SyntaxError(
                 f"{self.__class__.__name__} can only be used with"
                 " EqualityConstraint or InequalityConstraint instances."
                     ) from exc
 
@@ -342,27 +337,37 @@
     :class:`cvxportfolio.estimator.SimulatorEstimator`. Look at the
     code of the cost classes we implement if in doubt. Every operation that
     is different in simulation and in optimization is wrapped in a
     :class:`cvxportfolio.estimator.SimulatorEstimator` which implements
     different :meth:`values_in_time` and :meth:`simulate` respectively.
     """
 
+    def __init__(self):
+        """Define internal variables."""
+        self._set_internal_vars_to_none()
+
+    def _set_internal_vars_to_none(self):
+        """Set internal variables to None, which are CVXPY objects."""
+        self._w_plus = None
+        self._z = None
+        self._w_plus_minus_w_bm = None
+        self._cvxpy_expression = 0.
+
     def initialize_estimator( # pylint: disable=arguments-differ
         self, universe, **kwargs):
         """Initialize cost by compiling its CVXPY expression (if applies).
 
         This must be called by derived classes if you want to use
         an internal CVXPY expression to evaluate the simulator cost.
 
         :param universe: Current trading universe.
         :type universe: pd.Index
         :param kwargs: Other unused arguments to :meth:`initialize_estimator`.
         :type kwargs: dict
         """
-        # pylint: disable=attribute-defined-outside-init
         if hasattr(self, 'compile_to_cvxpy'):
             self._w_plus = cp.Variable(len(universe))
             self._z = cp.Variable(len(universe))
             self._w_plus_minus_w_bm = cp.Variable(len(universe))
             self._cvxpy_expression = self.compile_to_cvxpy(
                 w_plus = self._w_plus, z = self._z,
                 w_plus_minus_w_bm = self._w_plus_minus_w_bm)
@@ -531,14 +536,15 @@
             long_fees)
         self.dividends = None if dividends is None else DataEstimator(
             dividends)
         self.periods_per_year = YearDividedByTradingPeriod(periods_per_year)
         self._short_fees_parameter = None
         self._long_fees_parameter = None
         self._dividends_parameter = None
+        super().__init__()
 
     def initialize_estimator(self, universe, **kwargs):
         """Initialize cvxpy parameters.
 
         We don't use the parameter from
         :class:`cvxportfolio.estimator.DataEstimator` because we need to
         divide the value by periods_per_year.
@@ -591,24 +597,22 @@
                     self.periods_per_year.current_value)
 
         if self.dividends is not None:
             self._dividends_parameter.value =\
                 np.ones(self._dividends_parameter.size
                 ) * self.dividends.current_value
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile cost to cvxpy expression.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark
-            weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Unused arguments to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression.
         :rtype: cvxpy.expression
         """
 
         expression = 0.
 
@@ -806,14 +810,15 @@
         if exponent < 1.:
             raise SyntaxError(
                 'Exponent should be >=1, otherwise the'
                 ' transaction cost model is not convex.')
         self.exponent = exponent
         self._first_term_multiplier = None
         self._second_term_multiplier = None
+        super().__init__()
 
     def initialize_estimator(self, universe, **kwargs):
         """Initialize cvxpy parameters.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param kwargs: Other unused arguments to :meth:`initialize_estimator`.
@@ -845,24 +850,22 @@
         if self.b is not None:
 
             self._second_term_multiplier.value =\
                 (self.b.current_value * self.sigma.current_value
                 ) / ((self.market_volumes.current_value + 1E-8)
                     / current_portfolio_value) ** (self.exponent - 1)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy(  # pylint: disable=arguments-differ
+            self, z, **kwargs):
         """Compile cost to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark
-            weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Unused arguments to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression.
         :rtype: cvxpy.expression
         """
         expression = 0
         if self.a is not None:
             expression += cp.abs(z[:-1]) @ self._first_term_multiplier
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/data/__init__.py` & `cvxportfolio-1.3.1/cvxportfolio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/data/market_data.py` & `cvxportfolio-1.3.1/cvxportfolio/data/market_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 
 import numpy as np
 import pandas as pd
 
 from ..errors import DataError
 from ..utils import (hash_, make_numeric, periods_per_year_from_datetime_index,
                      resample_returns, set_pd_read_only)
-from .symbol_data import *
-from .symbol_data import OLHCV
+from .symbol_data import ( # pylint: disable=unused-import
+    BASE_LOCATION, OLHCV, Fred, SymbolData, YahooFinance, _loader_csv,
+    _loader_pickle, _loader_sqlite, _storer_csv, _storer_pickle,
+    _storer_sqlite)
 
 logger = logging.getLogger(__name__)
 
 __all__ = ['DownloadedMarketData', 'MarketData', 'UserProvidedMarketData']
 
 
 class MarketData:
@@ -129,18 +131,20 @@
     'GBPOUND': 'IUDSOIA', # SONIA
     'JPYEN': 'IRSTCB01JPM156N', # updated monthly
     }
 
 class MarketDataInMemory(MarketData):
     """Market data that is stored in memory when initialized."""
 
+    # pylint: disable=too-many-instance-attributes
+
     # this is overwritten in the derived classes' initializers
     returns = None
 
-    def __init__(
+    def __init__( # pylint: disable=too-many-arguments
         self, trading_frequency, base_location, cash_key, min_history,
         online_usage = False, universe_selection_in_time=None):
         """This must be called by the derived classes."""
         if (self.returns.index[-1] - self.returns.index[0]) < min_history:
             raise DataError(
                 "The provided returns have less history "
                 + f"than the min_history {min_history}")
@@ -208,14 +212,26 @@
         """Full universe, which might not be available for trading.
 
         :returns: Full universe.
         :rtype: pandas.Index
         """
         return self.returns.columns
 
+    def universe_at_time(self, t):
+        """Return trading universe at given time.
+
+        :param t: Trading time. It must be included in the timestamps returned
+            by :meth:`trading_calendar`.
+        :type t: pandas.Timestamp
+
+        :returns: Trading universe at time ``t``.
+        :rtype: pd.Index
+        """
+        return self.full_universe[self._universe_mask_at_time(t)]
+
     def serve(self, t):
         """Serve data for policy and simulator at time :math:`t`.
 
         :param t: Time of execution, *e.g.*, stock market open of a given day.
         :type t: pandas.Timestamp
 
         :returns: (past_returns, current_returns, past_volumes,
@@ -596,15 +612,15 @@
         bad_assets = changes_nan_status[changes_nan_status > 2]
         if len(bad_assets) > 0:
             logger.warning(
                 'In the user-provided returns, assets %s seem to have'
                 ' incorrect missing values structure. For each asset, missing'
                 ' returns should only be at the start and/or at the end.'
                 ' You should use universe_selection_in_time if you wanted to'
-                ' specify changes of universe in time.', bad_assets)
+                ' specify changes of universe in time.', bad_assets.index)
 
 
 class DownloadedMarketData(MarketDataInMemory):
     """Market data that is downloaded.
 
     .. versionadded:: 1.3.0
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/data/symbol_data.py` & `cvxportfolio-1.3.1/cvxportfolio/data/symbol_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines :class:`SymbolData` and derived classes."""
 
+# pylint: disable=too-many-lines
+
 import datetime
 import logging
 import sqlite3
 import warnings
 from pathlib import Path
 from pickle import UnpicklingError
 from urllib.error import URLError
@@ -438,27 +440,27 @@
         #         ['open', 'high', 'close']].min(1))
         # assert np.all(
         #     new_data['high'].fillna(np.inf) >= new_data[
         #         ['open', 'low', 'close']].max(1))
 
         return new_data
 
-    def _fillna_and_message(
+    def _fillna_and_message( # pylint: disable=too-many-arguments
         self, data, col_name, message, filler_arg=None, level='warning'):
         """Fill NaNs in column with chosen method and arg."""
         bad_indexes = data.index[data[col_name].isnull()]
         if len(bad_indexes) > 0:
             getattr(logger, level)(
                 '%s("%s").data["%s"] has NaNs on timestamps: %s,'
                 + ' filling them with %s.', self.__class__.__name__,
                 self.symbol, col_name, bad_indexes, message)
             data[col_name] = data[col_name].fillna(filler_arg)
 
-    def _ffill(self, data, col_name, message, saved_data=None,
-            level='warning'):
+    def _ffill( # pylint: disable=too-many-arguments
+            self, data, col_name, message, saved_data=None, level='warning'):
         """Forward-fill column also using saved data if present."""
         bad_indexes = data.index[data[col_name].isnull()]
         if len(bad_indexes) > 0:
             getattr(logger, level)(
                 '%s("%s").data["%s"] has NaNs on timestamps: %s,'
                 + ' filling them with %s.', self.__class__.__name__,
                 self.symbol, col_name, bad_indexes, message)
@@ -469,15 +471,15 @@
                     [saved_data.loc[
                         # saved_data is already clean, we only need last row
                         # we make 2 for backward compatibility w/ data stored
                         # by Cvxportfolio < 1.2.0
                         saved_data.index < data.index[0], col_name].iloc[-2:],
                     data[col_name]]).ffill().loc[data.index]
 
-    def _nan_anomalous_prices(
+    def _nan_anomalous_prices( # pylint: disable=too-many-arguments
             self, new_data, price_name, threshold, saved_data=None,
                 level='warning'):
         """Set to NaN given price name on its anomalous logrets to close."""
         new_lr_to_close =\
             np.log(new_data['close']) - np.log(new_data[price_name])
 
         # if there is saved data, we use it to compute the logrets
@@ -508,15 +510,15 @@
                 all_lr_to_close, all_lr_to_close, scaler=_median_scale_around,
                 windows=self.FILTERING_WINDOWS)
         self._nan_values(
             new_data, condition = score.loc[new_data.index] > threshold,
             columns_to_nan=price_name, message=f'anomalous {price_name} price',
             level=level)
 
-    def _nan_values(
+    def _nan_values( # pylint: disable=too-many-arguments
             self, data, condition, columns_to_nan, message, level='warning'):
         """Set to NaN in-place for indexing condition and chosen columns."""
 
         bad_indexes = data.index[condition]
         if len(bad_indexes) > 0:
             getattr(logger, level)(
                 '%s("%s") has %s on timestamps: %s,'
@@ -590,17 +592,21 @@
     def _set_infty_to_nan(self, data, level='warning'):
         """Set all +/- infty elements of data to NaN, in-place."""
 
         if np.isinf(data).sum().sum() > 0:
             getattr(logger, level)(
                 '%s("%s") has +/- infinity values, setting those to nan',
                 self.__class__.__name__, self.symbol)
-            data.iloc[:, :] = np.nan_to_num(
-                data.values, copy=True, nan=np.nan, posinf=np.nan,
-                neginf=np.nan)
+            with warnings.catch_warnings(): # op below warns on old pandas
+                if int(pd.__version__.split('.')[0]) < 2:
+                    warnings.filterwarnings( # pragma: no cover
+                        "ignore", category=FutureWarning)
+                data.iloc[:, :] = np.nan_to_num(
+                    data.values, copy=True, nan=np.nan, posinf=np.nan,
+                    neginf=np.nan)
 
     def _warn_on_extreme_logreturns(
             self, logreturns, threshold, what, level='warning'):
         """Log warning if logreturns are extreme."""
         # with this we skip over exact zeros (which we assume come from some
         # cleaning) and would bias the scale down
         logreturns.loc[logreturns == 0] = np.nan
@@ -654,15 +660,15 @@
         US dollar) value of the volume exchanged on the day.
         """
 
         # this is not used currently, but if we implement an interface to a
         # pure OLHCV data source there is no need to store the open-to-open
         # returns, they can be computed here
         if not 'return' in data.columns:
-           data['return'] = data[
+            data['return'] = data[
                 'open'].pct_change().shift(-1) # pragma: no cover
 
         self._quality_check(data)
 
         # NaN intraday data
         if len(data) > 0:
             data.loc[data.index[-1],
@@ -1022,14 +1028,17 @@
         # TODO this could be put at a lower class hierarchy
         if (current is None) or (len(current) < self.UPDATE_OVERLAP):
             updated = self._get_data_yahoo(symbol, **kwargs)
             logger.info('Downloading from the start.')
             result = self._process(updated)
             # we remove first row if it contains NaNs
             if np.any(result.iloc[0].isnull()):
+                logger.info(
+                    '%s(%s) is removing data at %s because there are NaNs',
+                    self, self.symbol, result.index[0])
                 result = result.iloc[1:]
             return result
         if (now_timezoned() - current.index[-1]
                 ) < pd.Timedelta(grace_period):
             logger.info(
                 'Skipping download because stored data is recent enough.')
             return current
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/errors.py` & `cvxportfolio-1.3.1/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/estimator.py` & `cvxportfolio-1.3.1/cvxportfolio/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 subestimator.values_in_time_recursive(**kwargs)
         for subestimator in self.__subestimators__:
             subestimator.values_in_time_recursive(**kwargs)
         if hasattr(self, "values_in_time"):
             # pylint: disable=assignment-from-no-return
             self._current_value = self.values_in_time(**kwargs)
             return self.current_value
-        return None
+        return None # pragma: no cover
 
     def collect_hyperparameters(self):
         """Collect (recursively) all hyperparameters defined in a policy.
 
         :returns: List of :class:`cvxportfolio.hyperparameters.HyperParameter`
             instances.
         :rtype: list
@@ -327,40 +327,53 @@
             self._current_value = self.simulate(**kwargs)
             return self.current_value
         return None # pragma: no cover
 
 class CvxpyExpressionEstimator(Estimator):
     """Base class for estimators that are Cvxpy expressions."""
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm, **kwargs):
         """Compile term to cvxpy expression.
 
         This is called by a Policy class on its terms before the start
         of the backtest to compile its Cvxpy problem. If the Policy
         changes in time this is called at every time step.
 
         It can either return a scalar expression, in the case of
         objective terms, or a list of cvxpy constraints, in the case of
         constraints.
 
         In MultiPeriodOptimization policies this is called separately
         for costs and constraints at different look-ahead steps with the
-        corresponding w_plus and z.
+        corresponding symbolic variable objects.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
         :param z: Trade weights.
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: Reserved for future expansion.
+        :type kwargs: dict
         """
         raise NotImplementedError # pragma: no cover
 
-# pylint: disable=too-many-arguments
+    def finalize_estimator(self, **kwargs):
+        """Delete references to internal CVXPY objects.
+
+        :param kwargs: Unused arguments to :meth:`finalize_estimator`.
+        :type kwargs: dict
+        """
+        for k, obj in self.__dict__.items():
+            if isinstance(obj, (cp.Parameter, cp.Variable, cp.Expression)):
+                setattr(self, k, None)
+
+
+# pylint: disable=too-many-arguments,too-many-instance-attributes
 class DataEstimator(SimulatorEstimator):
     """Estimator of point-in-time values from internal data.
 
     It also implements logic to check that no ``nan`` are returned
     by its ``values_in_time_recursive`` method, which is the way Cvxportfolio
     objects use this class to get data, to compile and update a Cvxpy
     parameter, and to slice the data with the current trading universe.
@@ -419,14 +432,22 @@
         self._non_negative = non_negative
         self._positive_semi_definite = positive_semi_definite
         self._universe_maybe_noncash = None
         self._data_includes_cash = data_includes_cash
         self._ignore_shape_check = ignore_shape_check
         self.parameter = None
 
+    def finalize_estimator(self, **kwargs):
+        """Delete references to internal CVXPY objects.
+
+        :param kwargs: Unused arguments to :meth:`finalize_estimator`.
+        :type kwargs: dict
+        """
+        self.parameter = None
+
     def initialize_estimator(self, universe, trading_calendar, **kwargs):
         """Initialize with current universe.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param trading_calendar: Future (including current) trading calendar.
         :type trading_calendar: pandas.DatetimeIndex
@@ -475,14 +496,15 @@
             # we pass a copy because it can be accidentally overwritten
             return np.array(result)
 
         raise DataError(
             f"{self.__class__.__name__}.values_in_time_recursive result"
             + " is not a scalar or array.")
 
+    # pylint: disable=too-many-return-statements
     def _universe_subselect(self, data):
         """This function subselects from ``data`` the relevant universe.
 
         See github issue #106.
 
         If data is a pandas Series we subselect its index. If we fail we
         throw an error. If data is a pandas DataFrame (covariance,
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/forecast.py` & `cvxportfolio-1.3.1/cvxportfolio/forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/hyperparameters.py` & `cvxportfolio-1.3.1/cvxportfolio/hyperparameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
     You can sum and multiply HPs between themselves and with scalars,
     and divide by a scalar. Arbitrary algebraic combination of these
     operations are supported.
     """
 
     def __mul__(self, other):
-        if np.isscalar(other) or isinstance(other, HyperParameter) \
-                or isinstance(other, pd.Timedelta):
+        if np.isscalar(other) or isinstance(
+                other, (HyperParameter, pd.Timedelta)):
             return CombinedHyperParameter([self], [other])
         return NotImplemented
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __div__(self, other):
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/policies.py` & `cvxportfolio-1.3.1/cvxportfolio/policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,19 +168,19 @@
         :rtype: pandas.Series
         """
         result = pd.Series(0., past_returns.columns)
         result.iloc[-1] = 1.
         return result
 
 class MarketBenchmark(Policy):
-    """Allocation weighted by last year's average market traded volumes.
+    """Allocation weighted by average market traded volumes.
 
     This policy provides an approximation of a market capitalization-weighted
     allocation, by using the average of traded volumes in units of value (e.g.,
-    USDOLLAR) over the previous year as proxy.
+    USDOLLAR) over the previous year (by default, can be changed) as proxy.
 
     .. versionadded:: 1.2.0
 
         We added the ``mean_volume_forecast`` parameter.
 
     :param mean_volume_forecast: Forecaster class that computes the average
         of historical volumes. You can also pass a DataFrame containing
@@ -295,14 +295,16 @@
 
     :param targets: time-indexed DataFrame of target weight vectors at
         given points in time (e.g., start of each month).
     :type targets: pandas.DataFrame
     """
 
     def __init__(self, targets):
+        assert isinstance(targets, pd.DataFrame)
+        assert isinstance(targets.index, pd.DatetimeIndex)
         self.targets = targets
         self.trading_days = None
 
     def initialize_estimator( # pylint: disable=arguments-differ
             self, trading_calendar, **kwargs):
         """Initialize policy instance with updated trading_calendar.
 
@@ -351,15 +353,15 @@
     """Sell all assets to cash.
 
     Alias of :class:`AllCash`.
     """
 
 
 class FixedTrades(Policy):
-    """Each day trade the provided trade weights vector.
+    """Each day trade the provided *trade weights* vector.
 
     If there are no weights defined for the given day, default to no
     trades.
 
     :param trades_weights: target trade weights :math:`z_t` to trade at each
         period. If constant in time use a pandas Series indexed by the assets'
         names, including the cash account name (``cash_key`` option to
@@ -403,15 +405,15 @@
                 self.__class__.__name__, t)
             result = current_weights
         self._current_value = result
         return result
 
 
 class FixedWeights(Policy):
-    """Each day trade to the provided trade weights vector.
+    """Each day trade to the provided *weights* vector.
 
     If there are no weights defined for the given day, default to no
     trades.
 
     :param target_weights: target weights :math:`w_t^+` to trade to at each
         period. If constant in time use a pandas Series indexed by the assets'
         names, including the cash account name (``cash_key`` option
@@ -458,15 +460,16 @@
         self._current_value = result
         return result
 
 
 class Uniform(FixedWeights):
     """Uniform allocation on non-cash assets.
 
-    :param leverage: Leverage of the allocation.
+    :param leverage: Leverage of the allocation. Default is 1, corresponding to
+        the classic :math:`1/n` allocation.
     :type leverage: float
     """
 
     # pylint: disable=super-init-not-called
     def __init__(self, leverage=1.):
         self.leverage = leverage
         # then we re-define the target weights for each universe in the method
@@ -532,16 +535,18 @@
     We use the 2-norm as trigger for rebalance. You may want to
     calibrate ``tracking_error`` for your application
     by backtesting this policy, *e.g.*, to get your desired turnover.
 
     :param target: target weights to rebalance to.
         It is assumed a constant if it is a Series. If it varies in
         time (you must specify it for every trading day) pass a
-        DataFrame indexed by time.
-    :type target: pd.Series or pd.DataFrame
+        DataFrame indexed by time. You can also pass a policy object instance
+        and its resulting weights will be used as targets, at each point in
+        time.
+    :type target: pd.Series or pd.DataFrame or cvx.policy.Policy instance
     :param tracking_error: we trade to match the target
         weights whenever the 2-norm of our weights minus the
         target is larger than this. Pass a Series if you want to vary it in
         time.
     :type tracking_error: pd.Series or pd.DataFrame
     """
 
@@ -664,48 +669,51 @@
             self.benchmark = DataEstimator(benchmark, data_includes_cash=True)
         else:
             self.benchmark = benchmark() if isinstance(benchmark, type
                 ) else benchmark
 
         self.cvxpy_kwargs = kwargs
 
-        # redefined below
+        self._set_internal_vars_to_none()
+
+        # for recursive evaluation
+        self.__subestimators__ = tuple(
+            [self.benchmark] + self.objective + sum(
+                [list(con_at_lag) for con_at_lag in self.constraints], []))
+
+    def _set_internal_vars_to_none(self):
+        """Set internal variables to None, includes CVXPY objects."""
         self._cvxpy_objective = 0
         self._cvxpy_constraints = []
         self._problem = None
         self._w_bm = None
         self._w_current = None
         self._z_at_lags = None
         self._w_plus_at_lags = None
         self._w_plus_minus_w_bm_at_lags = None
         self._cache = {}
 
-        # for recursive evaluation
-        self.__subestimators__ = tuple(
-            [self.benchmark] + self.objective + sum(
-                [list(con_at_lag) for con_at_lag in self.constraints], []))
-
     def _compile_to_cvxpy(self):
         """Compile all cvxpy expressions and the problem."""
         self._cvxpy_objective = [
             el.compile_to_cvxpy(
-                self._w_plus_at_lags[i], self._z_at_lags[i],
-                self._w_plus_minus_w_bm_at_lags[i])
+                w_plus=self._w_plus_at_lags[i], z=self._z_at_lags[i],
+                w_plus_minus_w_bm=self._w_plus_minus_w_bm_at_lags[i])
             for i, el in enumerate(self.objective)]
         for el, term in zip(self.objective, self._cvxpy_objective):
             if not term.is_dcp():
                 raise ConvexSpecificationError(el)
             if not term.is_concave():
                 raise ConvexityError(el)
         self._cvxpy_objective = sum(self._cvxpy_objective)
 
         def _compile_and_check_constraint(constr, i):
             result = constr.compile_to_cvxpy(
-                self._w_plus_at_lags[i], self._z_at_lags[i],
-                self._w_plus_minus_w_bm_at_lags[i])
+                w_plus=self._w_plus_at_lags[i], z=self._z_at_lags[i],
+                w_plus_minus_w_bm=self._w_plus_minus_w_bm_at_lags[i])
             for el in (result if hasattr(result, '__iter__') else [result]):
                 if not el.is_dcp():
                     raise ConvexSpecificationError(constr)
             return result
 
         self._cvxpy_constraints = [
             flatten_heterogeneous_list([
@@ -722,37 +730,32 @@
                 self._w_plus_at_lags[i] - self._w_bm == \
                     self._w_plus_minus_w_bm_at_lags[i])
             w = self._w_plus_at_lags[i]
         if not self.terminal_constraint is None:
             self._cvxpy_constraints.append(w == self.terminal_constraint)
         self._problem = cp.Problem(cp.Maximize(
             self._cvxpy_objective), self._cvxpy_constraints)
-        if not self._problem.is_dcp():  # dpp=True)
-            raise SyntaxError(
+        if not self._problem.is_dcp(): # this one can't be triggered, I think
+            raise SyntaxError( # pragma: no cover
               f"The optimization problem compiled by {self.__class__.__name__}"
                 + " does not follow the convex optimization rules."
                 + " This should not happen if you're using the default "
                 + " cvxportfolio terms and is probably due to a"
                 + " mis-specified custom term.")
 
-    def initialize_estimator_recursive( # pylint: disable=arguments-differ
+    def initialize_estimator( # pylint: disable=arguments-differ
             self, universe, **kwargs):
-        """Initialize the policy object with the trading universe.
-
-        We redefine the recursive version of :meth:`initialize_estimator`
-        because we initialize all objective and constraint objects.
+        """Initialize the policy object by defining all CVXPY terms.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param kwargs: Arguments to :meth:`initialize_estimator`.
         :type kwargs: dict
         """
 
-        super().initialize_estimator_recursive(universe=universe, **kwargs)
-
         self._w_bm = cp.Parameter(len(universe))
 
         self._w_current = cp.Parameter(len(universe))
         self._z_at_lags = [cp.Variable(len(universe))
                           for i in range(self._planning_horizon)]
         self._w_plus_at_lags = [cp.Variable(
             len(universe)) for i in range(self._planning_horizon)]
@@ -760,20 +763,31 @@
             len(universe)) for i in range(self._planning_horizon)]
 
         # simulator will overwrite this with cache loaded from disk
         self._cache = {}
 
         self._compile_to_cvxpy()
 
+    def finalize_estimator(self, **kwargs):
+        """Finalize the policy, delete CVXPY objects.
+
+        :param kwargs: Unused arguments to :meth:`finalize_estimator`.
+        :type kwargs: dict
+        """
+
+        self._set_internal_vars_to_none()
+
     def values_in_time_recursive( # pylint: disable=arguments-differ
             self, t, current_weights, current_portfolio_value, **kwargs):
         """Update all cvxpy parameters, solve, and return allocation weights.
 
         We redefine the recursive version of :meth:`values_in_time`
-        because we evaluate all objective and constraint objects.
+        because we change the variables that are passed down the tree:
+        we add ``cache`` and ``mpo_step``, and the latter is changed for the
+        different MPO steps.
 
         :param t: Current time.
         :type t: pandas.Timestamp
         :param current_weights: Current allocation weights.
         :type current_weights: pandas.Series
         :param current_portfolio_value: Current total value of the portfolio.
         :type current_portfolio_value: float
@@ -817,27 +831,47 @@
             **kwargs)
 
         self._w_bm.value = np.array(self.benchmark.current_value.values)\
              if hasattr(self.benchmark.current_value, 'values'
             ) else np.array(self.benchmark.current_value)
         self._w_current.value = current_weights.values
 
-        try:
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    "ignore", message='Solution may be inaccurate')
-                # suppress cvxpy 1.4 ECOS deprecation warnings
-                if cp.__version__[:3] == '1.4':
-                    warnings.filterwarnings("ignore", category=FutureWarning)
+        with warnings.catch_warnings():
+            # these warnings are thrown on numerical inaccuracies reported by
+            # the solver and accounted for by cvxpy; we expect expert users
+            # to set the solver options explicitely and/or setting verbose=True
+            # in the cvxpy_kwargs
+            warnings.filterwarnings(
+                "ignore", category=UserWarning,
+                message='Solution may be inaccurate')
+            # cvxpy 1.4 FutureWarnings
+            if cp.__version__[:3] == '1.4':
+                warnings.filterwarnings("ignore", category=FutureWarning)
+            try:
                 self._problem.solve(**self.cvxpy_kwargs)
-        except cp.SolverError as exc:
-            raise PortfolioOptimizationError(
-                f"Numerical solver for policy {self.__class__.__name__} at"
-                + f" time {t} failed; try changing it, relaxing some"
-                + " constraints, or removing costs.") from exc
+            except cp.SolverError as exc:
+                # try to solve with SCS; it's the most robust
+                logger.error(
+                    'CVXPY with settings %s reported numerical solver failure'
+                    ' at time %s;'
+                    ' re-trying by using SCS with basic options.',
+                    self.cvxpy_kwargs, t)
+                # we could refactor code to handle solve errors also here
+                try:
+                    self._problem.solve(ignore_dpp=True, solver='SCS')
+                # old cvxpy had no ignore_dpp
+                except TypeError: # pragma: no cover
+                    self._problem.solve(solver='SCS') # pragma: no cover
+                if self._problem.status in ['optimal', 'optimal_inaccurate']:
+                    logger.warning('Fallback solution with SCS worked!')
+                else: # pragma: no cover
+                    raise PortfolioOptimizationError( # pragma: no cover
+                      f"Numerical solver for policy {self.__class__.__name__}"
+                      + f" at time {t} failed; try changing it, relaxing some"
+                      + " constraints, or removing costs.") from exc
 
         if self._problem.status in ["unbounded", "unbounded_inaccurate"]:
             raise PortfolioOptimizationError(
                 f"Policy {self.__class__.__name__} at time "
                 + f"{t} resulted in an unbounded problem.")
 
         if self._problem.status in ["infeasible", 'infeasible_inaccurate']:
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/result.py` & `cvxportfolio-1.3.1/cvxportfolio/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 .. versionadded:: 1.1.0
     The :attr:`BacktestResult.log` property, which returns the logs produced
     during the back-test, at level ``INFO`` or higher. It works also for
     back-tests run in parallel!
 """
 
+# pylint: disable=too-many-lines
 
 from __future__ import annotations, print_function
 
 import collections
 import logging
 import time
 from io import StringIO
@@ -44,27 +45,29 @@
 
 from .utils import periods_per_year_from_datetime_index
 
 __all__ = ['BacktestResult']
 
 # Module level constants, should be exposed to user (move to configuration.py?)
 RECORD_LOGS = 'INFO'
-LOG_FORMAT = '| %(asctime)s | %(levelname)s | process:%(process)d | %(pathname)s:%(lineno)s | %(message)s '
+LOG_FORMAT = (
+    '| %(asctime)s | %(levelname)s | process:%(process)d |'
+    + ' %(pathname)s:%(lineno)s | %(message)s ')
 
 
 logger = logging.getLogger(__name__)
 
 # def getFiscalQuarter(dt):
 #     """Convert a time to a fiscal quarter."""
 #     year = dt.year
 #     quarter = (dt.month - 1) // 3 + 1
 #     return "Q%i %s" % (quarter, year)
 
 
-# pylint: disable=too-many-public-methods
+# pylint: disable=too-many-public-methods,too-many-instance-attributes
 class BacktestResult:
     """Store the data from a back-test and produce metrics and plots.
 
     Additionally, record all logs produced by the simulator, market data
     server, and policy object during the back-test. These are stored in the
     ``logs`` attribute as a newline separated string. This is done in a
     multi-process safe manner, so that if you run parallel back-tests with
@@ -85,14 +88,17 @@
         The initializer of this class is still experimental, we might still
         change its signature without the guarantee of semantic versioning.
     """
 
     def __init__(self, universe, trading_calendar, costs):
         """Initialization of back-test result."""
         timer = time.time()
+        assert isinstance(trading_calendar, pd.DatetimeIndex)
+        # trading calendar must be monotonous increasing
+        assert np.all(trading_calendar[1:] > trading_calendar[:-1])
         self._h = pd.DataFrame(index=trading_calendar,
                               columns=universe, dtype=float)
         self._u = pd.DataFrame(index=trading_calendar,
                               columns=universe, dtype=float)
         self._z = pd.DataFrame(index=trading_calendar,
                               columns=universe, dtype=float)
         self.costs = {cost.__class__.__name__: pd.Series(
@@ -107,22 +113,22 @@
             index=trading_calendar, dtype=float)
         self._cash_returns = pd.Series(index=trading_calendar, dtype=float)
         self._benchmark_returns = pd.Series(
             index=trading_calendar, dtype=float)
         self._current_universe = pd.Index(universe)
         self._indexer = np.arange(len(universe), dtype=int)
         self._init_timer = time.time() - timer
+        self._log = ''
 
     def __enter__(self):
         """Set up logging context to record back-test logs."""
         # we do this because you can also use the class without logging
         # pylint: disable=attribute-defined-outside-init
 
         # record logs
-        self._log = ''
         self._root_logger = logging.getLogger()
 
         # We modify the root logger to filter at our chosen level (or lower
         # if its was lower) and pre-existing handlers (notably the
         # stderr one) to filter at the level of the original logger, or theirs
         # if higher. We put them back to their initial state at the end.
         self._orig_rootlogger_level = self._root_logger.level
@@ -1067,16 +1073,16 @@
             "Avg. turnover": f"{self.turnover.mean() * 100:.1f}%",
             "Max. turnover": f"{self.turnover.max() * 100:.1f}%",
             ' '*9: '',
             "Avg. policy time": f"{self.policy_times.mean():.3f}s",
             "Avg. simulator time": f"{self.simulator_times.mean():.3f}s",
             "    Of which: market data":
                 f"{self.market_data_times.mean():.3f}s",
-            # "    Of which: result":
-            #     f"{self.result_times.mean():.3f}s",
+            "    Of which: result":
+                f"{self.result_times.mean():.3f}s",
             "Total time":
                 f"{self.simulator_times.sum() + self.policy_times.sum():.3f}s",
             }))
 
         if np.all(np.isnan(self.active_returns)):
             del stats["Avg. active return (annualized)"]
             del stats["Active volatility (annualized)"]
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/returns.py` & `cvxportfolio-1.3.1/cvxportfolio/returns.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,22 @@
         :type past_returns: pandas.DataFrame
         :param kwargs: All other parameters to :meth:`values_in_time`.
         :type kwargs: dict
         """
         if self.cash_returns is None:
             self._cash_return_parameter.value = past_returns.iloc[-1, -1]
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile to cvxpy expression.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark
-            weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         return w_plus[-1] * self._cash_return_parameter
 
 
@@ -198,24 +196,22 @@
         :param kwargs: All other parameters to :meth:`values_in_time`.
         :type kwargs: dict
         """
         self._r_hat_parameter.value = \
             np.ones(self._r_hat_parameter.size) * \
             self.r_hat.current_value * self.decay**(mpo_step)
 
-    def compile_to_cvxpy(self,  w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus, **kwargs):
         """Compile to cvxpy expression.
 
         :param w_plus: Post-trade weights.
         :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark
-            weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         return w_plus[:-1].T @ self._r_hat_parameter
 
 
@@ -266,24 +262,23 @@
         """Update returns forecast error parameters.
 
         :param kwargs: All arguments to :meth:`values_in_time`.
         :type kwargs: dict
         """
         self._deltas_parameter.value = self.deltas.current_value
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         _ = cp.abs(w_plus_minus_w_bm[:-1]).T @ self._deltas_parameter
         assert _.is_dcp(dpp=True)
         assert _.is_convex()
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/risks.py` & `cvxportfolio-1.3.1/cvxportfolio/risks.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,24 +103,23 @@
         """
         if self._alreadyfactorized:
             self._sigma_sqrt.value = self.Sigma.current_value
         else:
             self._sigma_sqrt.value = project_on_psd_cone_and_factorize(
                 self.Sigma.current_value)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile risk term to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         cvxpy_expression = cp.sum_squares(
             self._sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
         assert cvxpy_expression.is_dcp(dpp=True)
@@ -148,54 +147,54 @@
 
     def __init__(self, sigma_squares=HistoricalVariance):
 
         if isinstance(sigma_squares, type):
             sigma_squares = sigma_squares()
 
         self.sigma_squares = DataEstimator(sigma_squares)
+        self._sigmas_parameter = None
 
     def initialize_estimator( # pylint: disable=arguments-differ
             self, universe, **kwargs):
         """Initialize risk model with universe and trading times.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param kwargs: Other unused arguments to :meth:`initialize_estimator`.
         :type kwargs: dict
         """
-        self.sigmas_parameter = cp.Parameter(
+        self._sigmas_parameter = cp.Parameter(
             len(universe)-1, nonneg=True)  # +self.kelly))
 
     def values_in_time( # pylint: disable=arguments-differ
             self, **kwargs):
         """Update parameters of risk model.
 
         :param kwargs: All parameters to :meth:`values_in_time`.
         :type kwargs: dict
         """
         sigma_squares = self.sigma_squares.current_value
 
-        self.sigmas_parameter.value = np.sqrt(sigma_squares)
+        self._sigmas_parameter.value = np.sqrt(sigma_squares)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile risk term to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         cvxpy_expression = cp.square(
-            cp.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
+            cp.abs(w_plus_minus_w_bm[:-1]).T @ self._sigmas_parameter)
         assert cvxpy_expression.is_dcp(dpp=True)
         assert cvxpy_expression.is_convex()
         return cvxpy_expression
 
 
 class DiagonalCovariance(Cost):
     r"""Diagonal covariance matrix, user-provided or fit from data.
@@ -222,65 +221,67 @@
     """
 
     def __init__(self, sigma_squares=HistoricalVariance):
 
         if isinstance(sigma_squares, type):
             sigma_squares = sigma_squares()
         self.sigma_squares = DataEstimator(sigma_squares)
+        self._sigmas_parameter = None
 
     def initialize_estimator( # pylint: disable=arguments-differ
             self, universe, **kwargs):
         """Initialize risk model with universe and trading times.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param kwargs: Other unused arguments to :meth:`initialize_estimator`.
         :type kwargs: dict
         """
-        self.sigmas_parameter = cp.Parameter(len(universe)-1)
+        self._sigmas_parameter = cp.Parameter(len(universe)-1)
 
     def values_in_time( # pylint: disable=arguments-differ
             self, **kwargs):
         """Update parameters of risk model.
 
         :param kwargs: All parameters to :meth:`values_in_time`.
         :type kwargs: dict
         """
         sigma_squares = self.sigma_squares.current_value
-        self.sigmas_parameter.value = np.sqrt(sigma_squares)
+        self._sigmas_parameter.value = np.sqrt(sigma_squares)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile risk term to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         cvxpy_expression = cp.sum_squares(cp.multiply(w_plus_minus_w_bm[:-1],
-            self.sigmas_parameter))
+            self._sigmas_parameter))
         assert cvxpy_expression.is_dcp(dpp=True)
         assert cvxpy_expression.is_convex()
         return cvxpy_expression
 
 
 class FactorModelCovariance(Cost):
+    # pylint: disable=too-many-instance-attributes
     r"""Factor model covariance, either user-provided or fitted from the data.
 
     It represents the objective term:
 
     .. math::
 
-        {(w^+_t - w^\text{b}_t )}^T (F \Sigma_{F} F^T + \mathbf{diag}(d)) (w^+_t - w^\text{b}_t)
+        {(w^+_t - w^\text{b}_t )}^T (F \Sigma_{F} F^T
+            + \mathbf{diag}(d)) (w^+_t - w^\text{b}_t)
 
     where the factors exposure :math:`F` has as many rows as the number of
     assets and as many columns as the number of factors,
     the factors covariance matrix :math:`\Sigma_{F}` is positive semi-definite,
     and the idyosyncratic variances vector :math:`d` is non-negative.
 
     The advantage of this risk model over the standard :class:`FullCovariance`
@@ -332,15 +333,17 @@
         None. Forecaster that at each point in time produces estimate of F and
         d. By default we use a SVD-based forecaster that is equivalent to
         :class:`cvxportfolio.forecast.HistoricalFactorizedCovariance` if there
         are no missing values. If you pass a class, it will be instantiated
         with ``num_factors``.
     :type F_and_d_Forecaster: cvxportfolio.forecast.BaseForecast
     """
-
+    # we use the first pylint pragma because Sigma_F and F_and_d_Forecaster are
+    # not PEP8 compliant; that was a bad naming choice
+    # pylint: disable=invalid-name,too-many-arguments
     def __init__(self, F=None, d=None, Sigma_F=None, num_factors=1,
             Sigma=HistoricalFactorizedCovariance,
             F_and_d_Forecaster=HistoricalLowRankCovarianceSVD):
         self.F = F if F is None else DataEstimator(F, compile_parameter=True)
         self.d = d if d is None else DataEstimator(d)
         self.Sigma_F = Sigma_F if Sigma_F is None else DataEstimator(
             Sigma_F, ignore_shape_check=True)
@@ -356,87 +359,93 @@
                     Sigma = Sigma()
                 self._alreadyfactorized = hasattr(Sigma, 'FACTORIZED')\
                     and Sigma.FACTORIZED
                 self.Sigma = DataEstimator(Sigma)
             self.num_factors = num_factors
         else:
             self._fit = False
-        self.idyosync_sqrt_parameter = None
+        self._idyosync_sqrt_parameter = None
+        self._factor_exposures_parameter = None
 
     def initialize_estimator( # pylint: disable=arguments-differ
             self, universe, **kwargs):
         """Initialize risk model with universe and trading times.
 
         :param universe: Trading universe, including cash.
         :type universe: pandas.Index
         :param kwargs: Other unused arguments to :meth:`initialize_estimator`.
         :type kwargs: dict
         """
-        self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
+        self._idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
         if self._fit:
             effective_num_factors = min(self.num_factors, len(universe)-1)
-            self.factor_exposures_parameter = cp.Parameter(
+            self._factor_exposures_parameter = cp.Parameter(
                 (effective_num_factors, len(universe)-1))
         else:
             if self.Sigma_F is None:
-                self.factor_exposures_parameter = self.F.parameter
+                self._factor_exposures_parameter = self.F.parameter
             else:
                 # we could refactor the code here
                 # so we don't create duplicate parameters
-                self.factor_exposures_parameter = cp.Parameter(
+                self._factor_exposures_parameter = cp.Parameter(
                     self.F.parameter.shape)
 
     def values_in_time( # pylint: disable=arguments-differ
             self, **kwargs):
         """Update internal parameters.
 
         :param kwargs: All parameters to :meth:`values_in_time`.
         :type kwargs: dict
         """
         if self._fit:
             if hasattr(self, 'F_and_d_Forecaster'):
-                self.factor_exposures_parameter.value, d = \
+                self._factor_exposures_parameter.value, d = \
                     self.F_and_d_Forecaster.current_value
             else:
                 sigma_sqrt = self.Sigma.current_value \
                     if self._alreadyfactorized \
                     else project_on_psd_cone_and_factorize(
                         self.Sigma.current_value)
                 # numpy eigendecomposition has largest eigenvalues last
-                self.factor_exposures_parameter.value = sigma_sqrt[
+                self._factor_exposures_parameter.value = sigma_sqrt[
                     :, -self.num_factors:].T
                 d = np.sum(sigma_sqrt[:, :-self.num_factors]**2, axis=1)
         else:
             d = self.d.current_value
             if not self.Sigma_F is None:
-                self.factor_exposures_parameter.value = (
-                    self.F.parameter.value.T @ np.linalg.cholesky(
-                        self.Sigma_F.current_value)).T
+                # we were originally using Cholesky here, but if the user
+                # provides factor Sigmas with zero eigenvalues (some vendors
+                # give such) that would break; eigh is more robust
+                # sigma_F_factorized = np.linalg.cholesky(
+                #     self.Sigma_F.current_value)
+                sigma_F_factorized = project_on_psd_cone_and_factorize(
+                    self.Sigma_F.current_value)
+                self._factor_exposures_parameter.value = (
+                    self.F.parameter.value.T @ sigma_F_factorized).T
 
-        self.idyosync_sqrt_parameter.value = np.sqrt(d)
+        self._idyosync_sqrt_parameter.value = np.sqrt(d)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, w_plus_minus_w_bm, **kwargs):
         """Compile risk term to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: Post-trade weights minus benchmark
             weights.
         :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All other parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         cvxpy_expression = cp.sum_squares(cp.multiply(
-            self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
+            self._idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert cvxpy_expression.is_dcp(dpp=True)
 
-        cvxpy_expression += cp.sum_squares(self.factor_exposures_parameter @
+        cvxpy_expression += cp.sum_squares(self._factor_exposures_parameter @
                                           w_plus_minus_w_bm[:-1])
         assert cvxpy_expression.is_dcp(dpp=True)
         assert cvxpy_expression.is_convex()
         return cvxpy_expression
 
 
 class WorstCaseRisk(Cost):
@@ -458,31 +467,29 @@
     :type riskmodels: list
     """
 
     def __init__(self, riskmodels):
         self.riskmodels = riskmodels
         self.__subestimators__ = self.riskmodels
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        """Compile risk term to cvxpy expression.
+    def compile_to_cvxpy( # pylint: disable=arguments-differ
+            self, **kwargs):
+        """Compile worst case risk term to cvxpy expression.
 
-        :param w_plus: Post-trade weights.
-        :type w_plus: cvxpy.Variable
-        :param z: Trade weights.
-        :type z: cvxpy.Variable
-        :param w_plus_minus_w_bm: Post-trade weights minus benchmark
-            weights.
-        :type w_plus_minus_w_bm: cvxpy.Variable
+        :param kwargs: All parameters to :meth:`compile_to_cvxpy`.
+        :type kwargs: dict
+
+        :raises ConvexityError: If the compiled risk is not convex.
 
         :returns: Cvxpy expression representing the risk model.
         :rtype: cvxpy.expression
         """
         risks = []
         for risk in self.riskmodels:
-            _ = risk.compile_to_cvxpy(w_plus, z, w_plus_minus_w_bm)
+            _ = risk.compile_to_cvxpy(**kwargs)
             assert _.is_dcp(dpp=True)
             if not _.is_convex():
                 raise ConvexityError(f"The risk term {risk} is not convex!")
             risks.append(_)
 
         cvxpy_expression = cp.max(cp.hstack(risks))
         assert cvxpy_expression.is_dcp(dpp=True)
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/simulator.py` & `cvxportfolio-1.3.1/cvxportfolio/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,52 +284,57 @@
         assert not np.any(current_returns.isnull())
         h_next *= (1 + current_returns)
 
         return h_next, z, u, realized_costs, policy_time
 
     def _get_initialized_policy(self, orig_policy, universe, trading_calendar):
 
-        policy = copy.deepcopy(orig_policy)
+        # TODO: more testing to make sure we don't need this any more
+        # policy = copy.deepcopy(orig_policy)
+        policy = orig_policy
 
         # caching will be handled here
         policy.initialize_estimator_recursive(
             universe=universe, trading_calendar=trading_calendar)
 
         # we also initialize cost objects
         for cost in self.costs:
             if hasattr(cost, 'initialize_estimator_recursive'):
                 # to support interface before 1.2.0
                 cost.initialize_estimator_recursive(
                     universe=universe, trading_calendar=trading_calendar)
 
+        # TODO: this will be handled by initialize_estimator of the forecasters
         # if policy uses a cache load it from disk
         if hasattr(policy, '_cache'):
             logger.info('Trying to load cache from disk...')
             policy._cache = _load_cache(
               signature=self.market_data.partial_universe_signature(universe),
               base_location=self.base_location)
 
         return policy
 
     def _finalize_policy(self, policy, universe):
 
-        policy.finalize_estimator_recursive() # currently unused
-
-        for cost in self.costs:
-            if hasattr(cost, 'finalize_estimator_recursive'):
-                # to support interface before 1.2.0
-                cost.finalize_estimator_recursive() # currently unused
-
+        # TODO: this will be handled by finalize_estimator of the forecasters
+        # save cache to disk
         if hasattr(policy, '_cache'):
             logger.info('Storing cache from policy to disk...')
             _store_cache(
               cache=policy._cache,
               signature=self.market_data.partial_universe_signature(universe),
               base_location=self.base_location)
 
+        policy.finalize_estimator_recursive()
+
+        for cost in self.costs:
+            if hasattr(cost, 'finalize_estimator_recursive'):
+                # to support interface before 1.2.0
+                cost.finalize_estimator_recursive() # currently unused
+
     def _backtest(self, policy, start_time, end_time, h):
         """Run a backtest with changing universe."""
 
         timer = time.time()
 
         trading_calendar = self.market_data.trading_calendar(
             start_time, end_time, include_end=True)
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/__main__.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from .test_constraints import TestConstraints
 from .test_costs import TestCosts
 from .test_data import TestData, TestMarketData
 from .test_estimator import TestEstimator
 from .test_forecast import TestForecast
 from .test_hyperparameters import TestHyperparameters
 from .test_policies import TestPolicies
+from .test_result import TestResult
 from .test_returns import TestReturns
 from .test_risks import TestRisks
 from .test_simulator import TestSimulator
 from .test_utils import TestUtils
 
 if __name__ == '__main__':
 
-    unittest.main()#warnings='error')
+    unittest.main(warnings='error')
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/returns.csv` & `cvxportfolio-1.3.1/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-1.3.1/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     """Test Cvxportfolio constraint objects."""
 
     def _build_constraint(self, constraint, t=None):
         """Initialize constraint, build expression, and point it to time."""
         constraint.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
         cvxpy_expression = constraint.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         constraint.values_in_time_recursive(
             t=pd.Timestamp("2020-01-01") if t is None else t,
             current_portfolio_value=1000,
             **VALUES_IN_TIME_DUMMY_KWARGS
             )
         return cvxpy_expression
 
@@ -408,17 +409,18 @@
         value = 1e6
         model = cvx.ParticipationRateLimit(
             self.volumes, max_fraction_of_volumes=0.1)
         model.initialize_estimator_recursive(
             universe=self.returns.columns,
             trading_calendar=self.returns.index)
         cons = model.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         model.values_in_time_recursive(t=t, current_portfolio_value=value)
-        print(model.portfolio_value.value)
+        # print(model.portfolio_value.value)
         # cons = model.weight_expr(t, None, z, value)[0]
         tmp = np.zeros(self.N)
         tmp[:-1] = self.volumes.loc[t].values / value * 0.05
         self.z.value = tmp
         self.assertTrue(cons.value())
         self.z.value = -100 * self.z.value  # -100*np.ones(n)
         self.assertFalse(cons.value())
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_costs.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_costs.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,49 +38,57 @@
             self.returns.iloc[:, :-1].T @ self.returns.iloc[:, :-1]
                 / len(self.returns))
         cost3 = cost1 + cost2
 
         cost3.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
         expr3 = cost3.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         expr1 = cost1.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         expr2 = cost2.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         cost3.values_in_time_recursive(
             t=t, past_returns=self.returns.loc[self.returns.index < t],
             current_weights=None, current_portfolio_value=None,
             past_volumes=None, current_prices=None)
         self.assertTrue(expr3.value == expr1.value + expr2.value)
 
         cost4 = cost1 * 2
         expr4 = cost4.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         self.assertTrue(expr4.value == expr1.value * 2)
 
         cost3 = cost1 + 3 * cost2
         expr3 = cost3.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         self.assertTrue(expr3.value == expr1.value + 3 * expr2.value)
 
         cost3 = 3 * cost1 + 2 * cost2
         expr3 = cost3.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         self.assertTrue(expr3.value == 3 * expr1.value + 2 * expr2.value)
 
         cost3 = .1 * cost1 + 2 * (cost2 + cost1)
         expr3 = cost3.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         self.assertTrue(np.isclose(expr3.value, .1 * expr1.value +
                         2 * (expr2.value + expr1.value)))
 
         cost3 = cost1 + 5 * (cost2 + cost1)
         expr3 = cost3.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         self.assertTrue(np.isclose(expr3.value, expr1.value +
                         5 * (expr2.value + expr1.value)))
 
     def test_extra_cost_algebra(self):
         """Test code of cost algebra that is not tested above."""
 
         cost = cvx.ReturnsForecast()
@@ -119,23 +127,24 @@
             123],
         ]:
 
             hcost.initialize_estimator_recursive(
                 universe=self.returns.columns,
                 trading_calendar=self.returns.index)
             expression = hcost.compile_to_cvxpy(
-                self.w_plus, self.z, self.w_plus_minus_w_bm)
+                w_plus=self.w_plus, z=self.z,
+                w_plus_minus_w_bm=self.w_plus_minus_w_bm)
             hcost.values_in_time_recursive(
                 t=self.returns.index[t], past_returns=self.returns.iloc[:t])
 
             for _ in range(10):
                 self.w_plus.value = np.random.randn(self.N)
                 self.w_plus.value[-1] = 1 - np.sum(self.w_plus.value[:-1])
 
-                print(expression.value)
+                # print(expression.value)
 
                 self.assertTrue(
                     np.isclose(expression.value,
                         # short fees
                         - np.sum(np.minimum(
                         self.w_plus.value[:-1], 0.))
                         * (np.exp(np.log(1.05)/252) - 1)
@@ -153,51 +162,54 @@
             asset='AAPL', periods=[pd.Timestamp.today()])
         bad_soft_constraint = cvx.SoftConstraint(bad_constraint)
         bad_soft_constraint.initialize_estimator_recursive(
             universe=['AAPL'], trading_calendar=[pd.Timestamp.today()])
 
         with self.assertRaises(SyntaxError):
             bad_soft_constraint.compile_to_cvxpy(
-                self.w_plus, self.z, self.w_plus_minus_w_bm)
+                w_plus=self.w_plus, z=self.z,
+                w_plus_minus_w_bm=self.w_plus_minus_w_bm)
 
     def test_tcost(self):
         """Test tcost model."""
         value = 1e6
 
         pershare_cost = pd.Series(
             [0., 0.005, 0.],
             [self.returns.index[12], self.returns.index[23],
                 self.returns.index[34]])
         b = pd.Series([0., 0., 1.], [self.returns.index[12],
                       self.returns.index[23], self.returns.index[34]])
 
-        tcost = cvx.StocksTransactionCost(
-            a=0.001/2, pershare_cost=pershare_cost,
-            b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
+        with self.assertWarns(DeprecationWarning):
+            tcost = cvx.StocksTransactionCost(
+                a=0.001/2, pershare_cost=pershare_cost,
+                b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
 
         tcost.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
         expression = tcost.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
 
         # only spread
 
         tcost.values_in_time_recursive(
             t=self.returns.index[12], current_portfolio_value=value,
             past_returns=self.returns.iloc[:12],
             past_volumes=self.volumes.iloc[:12],
             current_prices=pd.Series(np.ones(self.returns.shape[1]-1),
                 self.returns.columns[:-1]))
 
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
 
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
-        print(est_tcost_lin)
-        print(expression.value)
+        # print(est_tcost_lin)
+        # print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
 
         # spread and fixed cost
 
         prices = pd.Series(np.random.uniform(
             1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1])
 
@@ -208,16 +220,16 @@
                                         current_prices=prices)
 
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
 
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         est_tcost_lin += np.abs(self.z.value[:-1]) @ (0.005 / prices)
-        print(est_tcost_lin)
-        print(expression.value)
+        # print(est_tcost_lin)
+        # print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
 
         # spread and nonlin cost
 
         tcost.values_in_time_recursive(
             t=self.returns.index[34],
             current_portfolio_value=value,
@@ -231,29 +243,31 @@
 
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         volumes_est = self.volumes.iloc[:34].mean().values
         sigmas_est = np.sqrt((self.returns.iloc[:34, :-1]**2).mean()).values
         est_tcost_nonnlin = (
             np.abs(self.z.value[:-1])**(3/2)) @ (
                 sigmas_est * np.sqrt(value / volumes_est))
-        print(est_tcost_lin)
-        print(est_tcost_nonnlin)
-        print(expression.value)
+        # print(est_tcost_lin)
+        # print(est_tcost_nonnlin)
+        # print(expression.value)
         self.assertTrue(np.isclose(expression.value,
                         est_tcost_lin+est_tcost_nonnlin))
 
         # also c
-        tcost = cvx.StocksTransactionCost(
-            a=0.001/2, pershare_cost=pershare_cost,
-            b=b, window_sigma_est=250, window_volume_est=250, c=0.001,
-             exponent=1.5)
+        with self.assertWarns(DeprecationWarning):
+            tcost = cvx.StocksTransactionCost(
+                a=0.001/2, pershare_cost=pershare_cost,
+                b=b, window_sigma_est=250, window_volume_est=250, c=0.001,
+                exponent=1.5)
         tcost.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
         expression = tcost.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
 
         tcost.values_in_time_recursive(
             t=self.returns.index[34],
             current_portfolio_value=value,
             past_returns=self.returns.iloc[:34],
             past_volumes=self.volumes.iloc[:34],
             current_prices=pd.Series(np.ones(self.returns.shape[1]-1),
@@ -265,17 +279,17 @@
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         volumes_est = self.volumes.iloc[:34].mean().values
         sigmas_est = np.sqrt((self.returns.iloc[:34, :-1]**2).mean()).values
         est_tcost_nonnlin = (
             np.abs(self.z.value[:-1])**(3/2)) @ (
                 sigmas_est * np.sqrt(value / volumes_est))
         est_tcost_c = np.sum(self.z.value[:-1] * 0.001)
-        print(est_tcost_lin)
-        print(est_tcost_nonnlin)
-        print(expression.value)
+        # print(est_tcost_lin)
+        # print(est_tcost_nonnlin)
+        # print(expression.value)
         self.assertTrue(np.isclose(expression.value,
                         est_tcost_lin+est_tcost_nonnlin+est_tcost_c))
 
 
 if __name__ == '__main__':
 
-    unittest.main() # pragma: no cover
+    unittest.main(warnings='error') # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_data.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,14 @@
 class TestData(CvxportfolioTest):
     """Test SymbolData methods and interface."""
 
     def test_yfinance_download(self):
         """Test YfinanceBase."""
 
         storer = YahooFinance('AAPL', base_location=self.datadir)
-
-        # pylint: disable=protected-access
         data = storer._download("AAPL", start="2023-04-01", end="2023-04-15")
 
         self.assertTrue(np.isclose(
             data.loc["2023-04-10 13:30:00+00:00", "return"],
             data.loc["2023-04-11 13:30:00+00:00", "open"] /
             data.loc["2023-04-10 13:30:00+00:00", "open"] - 1,
             rtol=1e-04, atol=1e-07,
@@ -87,24 +85,23 @@
     def test_fred(self):
         """Test basic Fred usage."""
 
         store = Fred(
             symbol="DFF", storage_backend='pickle',
             base_location=self.datadir)
 
-        print(store.data)
+        # print(store.data)
         data = store.data
         self.assertTrue(np.isclose(data["2023-04-10"], 4.83))
         self.assertTrue(data.index[0] ==
             pd.Timestamp("1954-07-01 00:00:00+00:00"))
 
         # test update
         olddata = pd.Series(data.iloc[:-123], copy=True)
         olddata.index = olddata.index.tz_localize(None)
-        # pylint: disable=protected-access
         newdata = store._preload(store._download("DFF", olddata))
         self.assertTrue(np.all(store.data == newdata))
 
         # test not re-downloading
         _ = Fred(
             symbol="DFF", grace_period=pd.Timedelta('10d'),
             base_location=self.datadir)
@@ -310,23 +307,23 @@
         # second level is timestamp
         timeindex = pd.date_range("2022-01-01", "2022-01-30", tz='UTC')
         second_level = pd.date_range("2022-01-01", "2022-01-03", tz='UTC')
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 3), index=index)
         data.columns = ["a", "b", "c"]
 
-        #print(data.index)
+        ## print(data.index)
         # print(data)
         # print(data.index.dtypes)
         # print(data.dtypes)
 
         storer("example", data, self.datadir)
         data1 = loader("example", self.datadir)
 
-        #print(data1.index)
+        ## print(data1.index)
         # print(data1)
         # print(data1.index.dtypes)
         # print(data1.dtypes)
 
         self.assertTrue(all(data == data1))
         self.assertTrue(all(data.index == data1.index))
         self.assertTrue(all(data.index.dtypes == data1.index.dtypes))
@@ -335,15 +332,14 @@
     def test_download_errors(self):
         """Test single-symbol download error."""
 
         storer = YahooFinance(
             'AAPL', grace_period=self.data_grace_period,
             base_location=self.datadir)
         # with self.assertRaises(SyntaxError):
-        #     # pylint: disable=protected-access
         #     storer._download('AAPL', overlap=1)
 
         class YahooFinanceErroneous(YahooFinance):
             """Modified YF that nans last open price."""
             def _download(
                     self, symbol, current=None, grace_period='5d', **kwargs):
                 """Modified download method."""
@@ -423,15 +419,14 @@
         """Test simple errors with Yahoo Finance."""
 
         with self.assertRaises(DataError):
             YahooFinance("DOESNTEXIST", base_location=self.datadir)
 
     def test_yahoo_finance_update(self):
         """Test specific issues when updating already stored data."""
-        # pylint: disable=protected-access
 
         raw_data = pd.DataFrame(
             # skip last day because there might actually be issues
             # that invalidate the tests assumptions
             cvx.YahooFinance._get_data_yahoo('AAPL'), copy=True).iloc[:-1]
 
         # make sure last open is different from close of day before
@@ -446,15 +441,16 @@
         class YahooFinanceUpdaterTest(cvx.YahooFinance):
             """Tester of issues with update."""
 
             def _get_data_yahoo(
                     self, symbol, start=None, *args, **kwargs):
                 return pd.DataFrame(
                     self.mock_data if start is None else
-                    self.mock_data.loc[self.mock_data.index >= start], copy=True)
+                    self.mock_data.loc[self.mock_data.index >= start],
+                    copy=True)
 
             @classmethod
             def _set_mock_data(cls, mock_data):
                 cls.mock_data = mock_data
 
             def _delete_recent_stored(self, how_many):
                 raw_stored = self._load_raw()
@@ -475,15 +471,15 @@
             grace_period=pd.Timedelta('0d')).data
         self.assertTrue(np.allclose(initial, updated, equal_nan=True))
         obj._delete_recent_stored(10)
         re_updated = YahooFinanceUpdaterTest(
             'AAPL', base_location=self.datadir,
             grace_period=pd.Timedelta('0d')).data
         self.assertTrue(np.allclose(initial, re_updated, equal_nan=True))
-        print(initial)
+        # print(initial)
 
         # change intraday data keeping it valid, nothing happens
         raw_data_intraday_changed = pd.DataFrame(raw_data, copy=True)
         raw_data_intraday_changed.iloc[-1, 1] *= .9 # low
         raw_data_intraday_changed.iloc[-1, 2] *= 1.1 # high
         raw_data_intraday_changed.iloc[-1, 3] *= 1.05 # close
         raw_data_intraday_changed.iloc[-1, 4] *= 1.05 # adjclose
@@ -584,15 +580,15 @@
         with self.assertLogs(level='INFO') as _:
             re_updated = YahooFinanceUpdaterTest(
                 'AAPL', base_location=self.datadir,
                 grace_period=pd.Timedelta('0d')).data
             self.assertTrue(np.any(
                 ['not append-only' in el for el in _.output]))
             # for el in _.output:
-            #     print(el)
+            #     # print(el)
         # print(re_updated)
         self.assertTrue(re_updated.iloc[-2, 0] == re_updated.iloc[-1, 0])
         self.assertFalse(np.allclose(initial, re_updated, equal_nan=True))
 
         # reset to init
         obj._delete_recent_stored(20)
         YahooFinanceUpdaterTest._set_mock_data(raw_data)
@@ -606,15 +602,15 @@
         YahooFinanceUpdaterTest._set_mock_data(
             raw_data_recent_invalid)
         with self.assertLogs(level='INFO') as _:
             re_updated = YahooFinanceUpdaterTest(
                 'AAPL', base_location=self.datadir,
                 grace_period=pd.Timedelta('0d')).data
             # for el in _.output:
-            #     print(el)
+            #     # print(el)
             self.assertTrue(np.any(
                 ['is eliminating data' in el for el in _.output]))
 
         # print(re_updated)
         self.assertTrue(np.allclose(initial, re_updated, equal_nan=True))
 
         # reset to init
@@ -637,15 +633,15 @@
                 'AAPL', base_location=self.datadir,
                 grace_period=pd.Timedelta('0d')).data
             self.assertTrue(np.any(
                 ['is eliminating data' in el for el in _.output]))
             self.assertTrue(np.any(
                 ['re-downloading from the start' in el for el in _.output]))
             # for el in _.output:
-            #     print(el)
+            #     # print(el)
         # print(re_updated)
         # last open hasn't changed (re-download is with same bad data, but
         # ffill will work on fresh re-download)
         self.assertTrue(initial.iloc[-1, 0] == re_updated.iloc[-1, 0])
 
     def test_yahoo_finance_cleaning(self):
         """Test our logic to clean Yahoo Finance data."""
@@ -664,26 +660,24 @@
         data = YahooFinance('GME', base_location=self.datadir).data
         self.assertGreater(data['return'].min(), -0.75)
         self.assertGreater(data['return'].max(), 3)
 
     def test_yahoo_finance_preload_warnings(self):
         """Test warnings on _preload if data has issues."""
 
-        # pylint: disable=protected-access
-
         raw_data = YahooFinance._get_data_yahoo('ZM')
         empty_instance = YahooFinance.__new__(YahooFinance)
         empty_instance._symbol = 'ZM' # because the warnings use the symbol
         cleaned = empty_instance._process(raw_data, None)
 
         def _test_warning(
                 data_transformation, part_of_message, level='WARNING'):
             """Test that warning is raised w/ message containing some word."""
             data = pd.DataFrame(cleaned, copy=True)
-            exec(data_transformation) # pylint: disable=exec-used
+            exec(data_transformation)
             # print(data)
             with self.assertLogs(level=level) as _:
                 empty_instance._preload(data)
                 # print(_)
                 self.assertTrue(part_of_message in _.output[0])
 
         # columns are: open low high close volume return
@@ -752,25 +746,24 @@
             YahooFinance('BA.L', base_location=self.datadir)
             self.assertFalse(np.any([
                     'anomalous adjclose prices' in el for el in _.output]))
 
     def test_yahoo_finance_cleaning_granular(self):
         """Test each step of cleaning."""
 
-        # pylint: disable=protected-access
         raw_data = YahooFinance._get_data_yahoo('ZM')
         # print(raw_data)
         empty_instance = YahooFinance.__new__(YahooFinance)
         empty_instance._symbol = 'ZM' # because the warnings use the symbol
 
         def _test_warning(
                 data_transformation, part_of_message, level='WARNING'):
             """Test that warning is raised w/ message containing some word."""
             data = pd.DataFrame(raw_data, copy=True)
-            exec(data_transformation) # pylint: disable=exec-used
+            exec(data_transformation)
             with self.assertLogs(level=level) as _:
                 _cleaned = empty_instance._process(data, None)
                 self.assertTrue(
                     np.any([part_of_message in el for el in _.output]))
                 # check all NaNs have been filled
                 self.assertTrue(_cleaned.iloc[:-1].isnull().sum().sum() == 0)
 
@@ -778,15 +771,15 @@
                 data_transformation, part_of_message, level='WARNING'):
             """Test that warning is raised w/ message containing some word."""
             new_data = pd.DataFrame(raw_data.iloc[-20:], copy=True)
             saved_data = pd.DataFrame(raw_data.iloc[:-15], copy=True)
             # no need to make it precise
             saved_data['return'] = np.log(saved_data.adjclose).diff()
             del saved_data['adjclose']
-            exec(data_transformation) # pylint: disable=exec-used
+            exec(data_transformation)
             with self.assertLogs(level=level) as _:
                 _cleaned = empty_instance._process(new_data, saved_data)
                 self.assertTrue(
                     np.any([part_of_message in el for el in _.output]))
                 # check all NaNs have been filled
                 self.assertTrue(_cleaned.iloc[:-1].isnull().sum().sum() == 0)
 
@@ -895,14 +888,38 @@
             + 'new_data.iloc[-1,2] = new_data.iloc[-1,0]',
             'anomalous open price', level='INFO')
         _test_warning_update(
             'new_data.iloc[-1,0] = new_data.iloc[-1,0] *  0.5;'
             + 'new_data.iloc[-1,1] = new_data.iloc[-1,0]',
             'anomalous open price', level='INFO')
 
+    def test_yahoo_finance_delete_first_line(self):
+        """Test that the first line is deleted if there are NaNs."""
+
+        class YahooFinanceNanInFirstLine(YahooFinance):
+            # pylint: disable=all
+
+            @staticmethod
+            def _get_data_yahoo(
+                ticker, start='1900-01-01', end='2100-01-01'):
+                """Modified download method."""
+                index = pd.date_range('2020-01-01', '2021-01-01', 10)
+                index = pd.DatetimeIndex(index).tz_localize('UTC')
+                columns = [
+                    'open', 'low', 'high', 'close', 'adjclose', 'volume']
+                data = np.ones((10, 6))
+                result = pd.DataFrame(data, index=index, columns=columns)
+                result.iloc[0, 0] = np.nan
+                return result
+
+        with self.assertLogs(level='INFO') as logs:
+            YahooFinanceNanInFirstLine('XXX', base_location=self.datadir)
+            self.assertTrue(
+                np.any(['is removing data at' in el for el in logs.output]))
+
     # def test_yahoo_finance_wrong_last_time(self):
     #     """Test that we correct last time if intraday."""
     #
     #     class YahooFinanceErroneous4(YahooFinance):
     #         """Modified YF that sets last time wrong."""
     #         counter = 0
     #
@@ -912,26 +929,60 @@
     #             """Modified download method."""
     #             res = YahooFinance._get_data_yahoo(
     #                 ticker, start=start, end=end)
     #             if self.counter > 0:
     #                 res.index = list(res.index)[:-1] + [
     #                     res.index[-1] - pd.Timedelta('3h')]
     #             self.counter += 1
-    #             print(res)
+    #             # print(res)
     #             return res
     #
     #     storer = YahooFinanceErroneous4('GOOGL', base_location=self.datadir)
-    #     print(storer.data)
+    #     # print(storer.data)
     #     #storer.update(pd.Timedelta('0d'))
-    #     #print(storer.data)
+    #     ## print(storer.data)
 
 
 class TestMarketData(CvxportfolioTest):
     """Test MarketData methods and interface."""
 
+    def test_prepare_data(self):
+        """Test that (Downloaded)MarketData is created correctly."""
+        market_data = cvx.DownloadedMarketData(
+            ['ZM', 'META'], grace_period = self.data_grace_period,
+            base_location=self.datadir, datasource=YahooFinance)
+        self.assertTrue(market_data.returns.shape[1] == 3)
+        self.assertTrue(market_data.prices.shape[1] == 2)
+        self.assertTrue(market_data.volumes.shape[1] == 2)
+        # self.assertTrue( simulator.sigma_estimate.data.shape[1] == 2)
+        self.assertTrue(np.isnan(market_data.returns.iloc[-1, 0]))
+        self.assertTrue(np.isnan(market_data.volumes.iloc[-1, 1]))
+        self.assertTrue(not np.isnan(market_data.prices.iloc[-1, 0]))
+        self.assertTrue(
+            market_data.returns.index[-1] == market_data.volumes.index[-1])
+        self.assertTrue(
+            market_data.returns.index[-1] == market_data.prices.index[-1])
+
+    def test_market_data_remove_missing_recent(self):
+        """Test DownloadedMarketData logic to handle recent missing data."""
+
+        class YahooFinanceDelisted(YahooFinance): # pylint: disable-all
+            """Fake delistings of stocks."""
+
+            def _preload(self, raw):
+                if self.symbol == 'ZM':
+                    return super()._preload(
+                        pd.DataFrame(raw.iloc[:-2], copy=True))
+                else:
+                    return super()._preload(raw)
+        with self.assertLogs(level='WARNING'):
+            cvx.DownloadedMarketData(
+                ['ZM', 'META'], grace_period = self.data_grace_period,
+                base_location=self.datadir, datasource=YahooFinanceDelisted)
+
     def test_market_data_downsample(self):
         """Test downsampling of market data."""
         md = DownloadedMarketData(
             ['AAPL', 'GOOG'], grace_period=self.data_grace_period,
             base_location=self.datadir)
 
         # TODO: better to rewrite this test
@@ -949,26 +1000,26 @@
 
         for i, freq in enumerate(freqs):
 
             new_md = deepcopy(md)
 
             # pylint: disable=protected-access
             new_md._downsample(freq)
-            print(new_md.returns)
+            # print(new_md.returns)
             self.assertTrue(np.isnan(new_md.returns.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.volumes.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.prices.GOOG.iloc[0]))
 
             if freq == 'weekly':
-                print((new_md.returns.index.weekday < 2).mean())
+                # print((new_md.returns.index.weekday < 2).mean())
                 self.assertTrue(
                     (new_md.returns.index.weekday < 2).mean() > .95)
 
             if freq == 'monthly':
-                print((new_md.returns.index.day < 5).mean())
+                # print((new_md.returns.index.day < 5).mean())
                 self.assertTrue((new_md.returns.index.day < 5).mean() > .95)
 
             self.assertTrue(
                 all(md.prices.loc[testdays[i]] ==
                     new_md.prices.loc[testdays[i]]))
             self.assertTrue(np.allclose(
                 md.volumes.loc[periods[i]].sum(),
@@ -1179,12 +1230,12 @@
         self.assertTrue(sig3 == sig2)
 
         md = DownloadedMarketData(['WM2NS'],
             datasource='Fred',
             grace_period=self.data_grace_period,
             base_location=self.datadir)
 
-        print(md.partial_universe_signature(md.full_universe))
+        # print(md.partial_universe_signature(md.full_universe))
 
 if __name__ == '__main__':
 
     unittest.main(warnings='error') # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,19 @@
         estimator = DataEstimator(data)
         self.assertTrue(
             np.all(estimator.values_in_time_recursive(t=time) == data.values))
 
     def test_series_timeindex(self):
         """Test DataEstimator with time-indexed series."""
         index = pd.date_range("2022-01-01", "2022-01-30")
-        print(index)
+        # print(index)
         data = pd.Series(np.arange(len(index)), index)
         estimator = DataEstimator(data)
 
-        print(estimator.values_in_time_recursive(t="2022-01-05"))
+        # print(estimator.values_in_time_recursive(t="2022-01-05"))
         self.assertTrue(estimator.values_in_time_recursive(
             t="2022-01-05") == data.loc["2022-01-05"])
 
         with self.assertRaises(MissingTimesError):
             estimator.values_in_time_recursive(t="2022-02-05")
 
         estimator = DataEstimator(data, use_last_available_time=True)
@@ -143,15 +143,15 @@
 
     def test_dataframe_timeindex(self):
         """Test DataEstimator with time-indexed dataframe."""
         index = pd.date_range("2022-01-01", "2022-01-30")
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         estimator = DataEstimator(data)
 
-        print(estimator.values_in_time_recursive(t="2022-01-05"))
+        # print(estimator.values_in_time_recursive(t="2022-01-05"))
         self.assertTrue(np.all(estimator.values_in_time_recursive(
             t="2022-01-05") == data.loc["2022-01-05"]))
 
         with self.assertRaises(MissingTimesError):
             estimator.values_in_time_recursive(t="2021-01-05")
 
         estimator = DataEstimator(data, use_last_available_time=True)
@@ -247,15 +247,15 @@
 
         We also check that _universe_subselect works fine.
         """
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
-        print(data.index)
+        # print(data.index)
         estimator = DataEstimator(data)
         self.assertTrue(np.all(estimator.values_in_time_recursive(
             t="2022-01-05") == data.loc["2022-01-05"]))
 
         # use_last_avalaible_time
         estimator = DataEstimator(data, use_last_available_time=True)
         self.assertTrue(np.all(estimator.values_in_time_recursive(
@@ -324,24 +324,24 @@
         self.assertTrue(estimator.parameter is not None)
         estimator.values_in_time_recursive(t="2022-01-05")
         self.assertTrue(
             np.all(estimator.parameter.value == data.loc["2022-01-05"]))
 
     def test_repr_dataestimator(self):
         """Test __repr__ magic method of DataEstimator."""
-        print(DataEstimator(3))
-        print(DataEstimator(np.array([1, 2, 3])))
-        print(DataEstimator(pd.Series([1, 2, 3])))
-        print(DataEstimator(pd.DataFrame([1, 2, 3])))
+        str(DataEstimator(3))
+        str(DataEstimator(np.array([1, 2, 3])))
+        str(DataEstimator(pd.Series([1, 2, 3])))
+        str(DataEstimator(pd.DataFrame([1, 2, 3])))
 
     def test_repr(self):
         """Test other assorted __repr__ methods of derived objects."""
-        print(cvx.FactorModelCovariance(num_factors=10))
-        print(cvx.ReturnsForecast() - .5 * cvx.FullCovariance())
-        print(cvx.SinglePeriodOptimization(cvx.ReturnsForecast(),
+        str(cvx.FactorModelCovariance(num_factors=10))
+        str(cvx.ReturnsForecast() - .5 * cvx.FullCovariance())
+        str(cvx.SinglePeriodOptimization(cvx.ReturnsForecast(),
                                            [cvx.LongOnly()]))
-        print(cvx.LeverageLimit(3))
+        str(cvx.LeverageLimit(3))
 
 
 if __name__ == '__main__':
 
     unittest.main() # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_forecast.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                                    HistoricalMeanVolume,
                                    HistoricalStandardDeviation,
                                    HistoricalVariance, RegressionMeanReturn)
 from cvxportfolio.tests import CvxportfolioTest
 from cvxportfolio.utils import set_pd_read_only
 
 
-class TestForecast(CvxportfolioTest):
+class TestForecast(CvxportfolioTest): # pylint: disable=too-many-public-methods
     """Test forecast estimators and their caching.
 
     In most cases we test against the relevant pandas function as reference.
     """
 
     def test_estimate(self):
         """Test estimate method of a forecaster."""
@@ -59,15 +59,15 @@
                 market_data=self.market_data,
                 t = self.market_data.returns.index[-1] + pd.Timedelta('300d'))
 
     def test_nested_cached_eval(self):
         """Test nested evaluation with caching."""
 
         forecaster = HistoricalVariance(kelly=False)
-        forecaster._CACHED = True
+        forecaster._CACHED = True # pylint: disable=protected-access
         md = self.market_data
         returns = md.returns
         cache = {}
         for tidx in [-30, -29, -25, -24, -23, -30, -29]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index < t]
 
@@ -75,44 +75,44 @@
                     past_returns=past_returns, t=t, cache=cache)
 
             self.assertTrue(
                 np.allclose(result, past_returns.iloc[:, :-1].var(ddof=0)))
         self.assertEqual(len(cache), 1)
         self.assertEqual(len(list(cache.values())[0]), 5)
 
-    def test_regression_mean_return(self):
+    def test_regression_mean_return(self): # pylint: disable=too-many-locals
         """Test historical mean return with regression."""
 
         # will be refactored
         # vix = cvx.YahooFinance('^VIX').data.open
         # vix.name = 'VIX'
 
         md = copy.deepcopy(self.market_data)
         rets = pd.DataFrame(self.market_data.returns, copy=True)
-        rets.loc[rets.index <= rets.index[10], 'AAPL'] = np.nan
+        rets.loc[rets.index <= rets.index[6], 'AAPL'] = np.nan
         rets.loc[rets.index <= rets.index[5], 'WMT'] = np.nan
         assert rets.iloc[0].isnull().sum() > 0
         md.returns = set_pd_read_only(rets)
 
         np.random.seed(0)
         vix = pd.Series(np.random.uniform(len(md.returns)), md.returns.index)
         vix.name = 'VIX'
         regr_mean_ret = RegressionMeanReturn(regressors=[vix])
         regr_mean_ret.initialize_estimator_recursive(
             universe=self.market_data.returns.columns,
             trading_calendar=self.market_data.returns.index)
-        regr_mean_ret._CACHED = True
+        regr_mean_ret._CACHED = True # pylint: disable=protected-access
         returns = md.returns
 
         # ValueError thrown by UserProvidedRegressor (not enough history)
         with self.assertRaises(ValueError):
             t = returns.index[9]
             past_returns = returns.loc[returns.index < t]
             regr_mean_ret.values_in_time_recursive(
-                    past_returns=past_returns, t=t)
+                past_returns=past_returns, t=t)
 
         for tidx in [-30, -29, -25, -24, -23]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index < t]
 
             result  = \
                 regr_mean_ret.values_in_time_recursive(
@@ -129,14 +129,17 @@
                 x_last = pd.Series(1., index=['intercept'])
                 x_last['VIX'] = vix[vix.index < t].iloc[-1]
                 local_result = x_last @ beta
                 # print(local_result)
                 # print(result[asset])
                 self.assertTrue(np.isclose(local_result, result[asset]))
 
+        # so it also calls finalize_estimator
+        regr_mean_ret.estimate(market_data=md, t=md.returns.index[30])
+
     def test_historical_mean_volume(self):
         """Test mean volume forecaster."""
 
         forecaster = HistoricalMeanVolume()
         for tidx in [20, 21, 22, 25, 26, 27]:
             cvx_val = forecaster.values_in_time_recursive(
                 t=self.volumes.index[tidx],
@@ -349,16 +352,16 @@
 
         self._base_test_moving_window_vector_update(
             HistoricalCovariance, {'kelly': False}, 'cov', {'ddof': 0},
             with_nans=False)
 
     def _base_test_exponential_moving_window_vector_update(
             self, forecaster, fc_kwargs, df_callable=None, with_nans=True):
-        """Base test for vector quantities using an exponential moving window,
-        and an exponential moving window in combination with a moving window."""
+        """Base test for vector quantities w/ exponential moving window,
+        and exponential moving window + moving window."""
         half_life = pd.Timedelta('20d')
         inst_forecaster = forecaster(**fc_kwargs, half_life=half_life)
         returns = pd.DataFrame(self.returns, copy=True)
         if with_nans:
             returns.iloc[:40, 3:10] = np.nan
 
         for tidx in [50, 51, 52, 55, 56, 57, 58, 59, 60]:
@@ -454,17 +457,17 @@
 
         # pylint: disable=protected-access
         count_matrix = forecaster._compute_denominator(
             returns.iloc[:, :-1], None)
 
         for indexes in [(1, 2), (4, 5), (1, 5), (7, 18),
                 (7, 24), (1, 15), (13, 22)]:
-            print(count_matrix.iloc[indexes[0], indexes[1]])
-            print(len((returns.iloc[:, indexes[0]] *
-                  returns.iloc[:, indexes[1]]).dropna()))
+            # print(count_matrix.iloc[indexes[0], indexes[1]])
+            # print(len((returns.iloc[:, indexes[0]] *
+            #       returns.iloc[:, indexes[1]]).dropna()))
             self.assertTrue(
                 np.isclose(count_matrix.iloc[indexes[0], indexes[1]],
                     len((returns.iloc[:, indexes[0]]
                          * returns.iloc[:, indexes[1]]).dropna())))
 
     def test_sum_matrix(self):
         """Test internal method(s) of HistoricalFactorizedCovariance."""
@@ -477,18 +480,18 @@
             t=pd.Timestamp('2022-01-01'), past_returns=returns)
 
         # pylint: disable=protected-access
         sum_matrix = forecaster._numerator
 
         for indexes in [(1, 2), (4, 5), (1, 5), (7, 18),
                 (7, 24), (1, 15), (13, 22)]:
-            print()
-            print(sum_matrix.iloc[indexes[0], indexes[1]])
-            print((returns.iloc[:, indexes[0]] *
-                  returns.iloc[:, indexes[1]]).sum())
+            # print()
+            # print(sum_matrix.iloc[indexes[0], indexes[1]])
+            # print((returns.iloc[:, indexes[0]] *
+            #       returns.iloc[:, indexes[1]]).sum())
             self.assertTrue(np.isclose(
                 sum_matrix.iloc[indexes[0], indexes[1]],
                 (returns.iloc[:, indexes[0]] *
                  returns.iloc[:, indexes[1]]).sum()
             ))
 
     def test_covariance_update_withnans(self):
@@ -545,15 +548,15 @@
         def _cov_ij(i, j, rets):
             i_nanmasker = np.zeros(len(rets))
             i_nanmasker[rets.iloc[:, i].isnull()] = np.nan
             i_nanmasker[~(rets.iloc[:, i].isnull())] = 1.
             j_nanmasker = np.zeros(len(rets))
             j_nanmasker[rets.iloc[:, j].isnull()] = np.nan
             j_nanmasker[~(rets.iloc[:, j].isnull())] = 1.
-            print(i_nanmasker, j_nanmasker)
+            # print(i_nanmasker, j_nanmasker)
             return np.nanmean(rets.iloc[:, i] * rets.iloc[:, j]
                 ) - np.nanmean(rets.iloc[:, i] * j_nanmasker
                     ) * np.nanmean(rets.iloc[:, j] * i_nanmasker)
 
         def _compute_covariance(rets):
             res = np.zeros((3, 3))
             res[0, 0] = _cov_ij(0, 0, rets)
@@ -611,20 +614,20 @@
             sigma_fact = forecaster2.values_in_time_recursive(
                 t=t, past_returns=returns)
 
             sigma_svd = F.T @ F + np.diag(d)
             sigma_eigh = (
                 sigma_fact[:, -num_factors:] @ sigma_fact[:, -num_factors:].T
                 + np.diag((sigma_fact[:, :-num_factors]**2).sum(1)))
-            print(sigma_svd)
-            print(sigma_eigh)
-            print(np.linalg.norm(sigma_svd),
-                  np.linalg.norm(sigma_eigh),
-                  np.linalg.norm(sigma_eigh-sigma_svd)
-                  )
+            # print(sigma_svd)
+            # print(sigma_eigh)
+            # print(np.linalg.norm(sigma_svd),
+            #      np.linalg.norm(sigma_eigh),
+            #      np.linalg.norm(sigma_eigh-sigma_svd)
+            #      )
 
             forecaster3 = HistoricalLowRankCovarianceSVD(num_factors=1,
                 svd='scipy')
 
             with self.assertRaises(SyntaxError):
                 forecaster3.values_in_time_recursive(t=t, past_returns=returns)
 
@@ -642,39 +645,39 @@
         diff2 = _compare_with_eigh(returns)
         self.assertTrue(diff1 < diff2)
 
         returns.iloc[25:40, 2] = np.nan
         diff3 = _compare_with_eigh(returns)
         self.assertTrue(diff2 < diff3)
 
-        print(returns.isnull().mean())
+        # print(returns.isnull().mean())
         returns.iloc[4:-3, -2] = np.nan
-        print(returns.isnull().mean())
+        # print(returns.isnull().mean())
         diff4 = _compare_with_eigh(returns)
         self.assertTrue(diff3 < diff4)
 
         returns.iloc[:50, 0] = np.nan
         returns.iloc[50:, 1] = np.nan
-        print(returns.isnull().mean())
+        # print(returns.isnull().mean())
 
         with self.assertRaises(ForecastError):
             forecaster2.values_in_time_recursive(t=t, past_returns=returns)
 
         # this one is even more robust!
         forecaster.values_in_time_recursive(
             t=t, past_returns=returns)
 
         returns.iloc[56:, 0] = np.nan
-        print(returns.isnull().mean())
+        # print(returns.isnull().mean())
 
         forecaster.values_in_time_recursive(
             t=t, past_returns=returns)
 
         returns.iloc[:70, 1] = np.nan
-        print(returns.isnull().mean())
+        # print(returns.isnull().mean())
 
         with self.assertRaises(ForecastError):
             forecaster.values_in_time_recursive(
                 t=t, past_returns=returns)
 
 
 if __name__ == '__main__':
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_hyperparameters.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_hyperparameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """Unit tests for the hyper-parameters interface."""
 
 import unittest
 
 import cvxportfolio as cvx
 from cvxportfolio.tests import CvxportfolioTest
 
-GAMMA_RISK_RANGE = [.5, 1., 2., 5., 10.]
-GAMMA_COST_RANGE = [0., .1, .2, .5, 1., 2., 5., 10.]
+GAMMA_RISK_RANGE = (.5, 1., 2., 5., 10.)
+GAMMA_COST_RANGE = (0., .1, .2, .5, 1., 2., 5., 10.)
 
 class GammaRisk(cvx.RangeHyperParameter):
     """Multiplier of a risk term."""
 
     def __init__(self, values_range=GAMMA_RISK_RANGE, current_value=1.):
         super().__init__(values_range, current_value)
 
@@ -54,44 +54,44 @@
         self.assertEqual(len(set(hps)), 2)
 
     def test_repr(self):
         """Test the repr method."""
         obj = cvx.ReturnsForecast() - cvx.Gamma() * cvx.FullCovariance()\
             - cvx.Gamma() * cvx.StocksTransactionCost()
 
-        print(obj)
+        str(obj)
 
         ref = ('ReturnsForecast(r_hat=HistoricalMeanReturn(half_life=inf,'
             + ' rolling=inf), decay=1.0)'
             + ' - Gamma(current_value=1.0) * FullCovariance('
             + 'Sigma=HistoricalFactorizedCovariance(half_life=inf,'
             + ' rolling=inf, kelly=True))'
             + ' - Gamma(current_value=1.0) * StocksTransactionCost(a=0.0, '
             + 'b=1.0, market_volumes=VolumeHatOrRealized('
             + 'volume_hat=HistoricalMeanVolume(half_life=inf, '
             + "rolling=Timedelta('365 days 05:45:36'))), "
             + "sigma=HistoricalStandardDeviation(half_life=inf, "
             + "rolling=Timedelta('365 days 05:45:36'), kelly=True), "
             + 'exponent=1.5, pershare_cost=0.005)')
 
-        print(ref)
+        # print(ref)
 
         self.assertTrue(str(obj) == ref)
 
-        print(cvx.Gamma() * cvx.Gamma())
-        print(cvx.Gamma() - cvx.Gamma())
-        print(cvx.Gamma() - (2 * cvx.Gamma()))
-        print(cvx.Gamma() - (-2 * cvx.Gamma()))
-        print(cvx.Gamma() - (cvx.Gamma() * -2))
-        print(cvx.Gamma() - (cvx.Gamma() * -2))
-        print(cvx.Gamma() * -1 * (cvx.Gamma() * -2))
-        print(2 * cvx.Gamma() - 3 * cvx.Gamma())
-        print(2 * cvx.Gamma() * ( cvx.ReturnsForecast()
+        str(cvx.Gamma() * cvx.Gamma())
+        str(cvx.Gamma() - cvx.Gamma())
+        str(cvx.Gamma() - (2 * cvx.Gamma()))
+        str(cvx.Gamma() - (-2 * cvx.Gamma()))
+        str(cvx.Gamma() - (cvx.Gamma() * -2))
+        str(cvx.Gamma() - (cvx.Gamma() * -2))
+        str(cvx.Gamma() * -1 * (cvx.Gamma() * -2))
+        str(2 * cvx.Gamma() - 3 * cvx.Gamma())
+        str(2 * cvx.Gamma() * ( cvx.ReturnsForecast()
             - 3 * cvx.Gamma() * cvx.FullCovariance()))
-        print(cvx.Gamma() * 2 * ( cvx.ReturnsForecast()
+        str(cvx.Gamma() * 2 * ( cvx.ReturnsForecast()
             - cvx.Gamma() * (-3) *  cvx.FullCovariance()))
 
     def test_basic_hyper_parameters(self):
         """Test simple syntax and errors."""
         gamma = GammaRisk(current_value=1)
 
         self.assertTrue((-gamma).current_value == -1)
@@ -105,14 +105,16 @@
             cvx.SinglePeriodOptimization(GammaRisk * cvx.FullCovariance())
 
         cvx.SinglePeriodOptimization(-GammaRisk() * cvx.FullCovariance())
 
     def test_range_hyper_parameter(self):
         """Test range hyperparameter."""
 
+        # pylint: disable=protected-access
+
         gamma = GammaRisk(current_value=1)
         self.assertTrue((gamma).current_value == 1)
         gamma._decrement()
         self.assertTrue((gamma).current_value == .5)
         with self.assertRaises(IndexError):
             gamma._decrement()
 
@@ -137,30 +139,30 @@
 
     def test_collect_hyper_parameters(self):
         """Test collect hyperparameters."""
 
         pol = cvx.SinglePeriodOptimization(GammaRisk() * cvx.FullCovariance())
 
         res = pol.collect_hyperparameters()
-        print(res)
+        # print(res)
         self.assertTrue(len(res) == 1)
 
         pol = cvx.SinglePeriodOptimization(
             - GammaRisk() * cvx.FullCovariance()
             - GammaTrade() * cvx.TransactionCost())
 
         res = pol.collect_hyperparameters()
-        print(res)
+        # print(res)
         self.assertTrue(len(res) == 2)
 
         pol = cvx.SinglePeriodOptimization(
             -(GammaRisk() + .5 * GammaRisk()) * cvx.FullCovariance()
             - GammaTrade() * cvx.TransactionCost())
 
         res = pol.collect_hyperparameters()
-        print(res)
+        # print(res)
         self.assertTrue(len(res) == 3)
 
 
 if __name__ == '__main__':
 
     unittest.main() # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_policies.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_policies.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,14 +93,27 @@
         self.assertTrue(wplus["AAPL"] == 0)
         self.assertTrue(wplus["TSLA"] == -wplus["GOOGL"])
         self.assertTrue(np.abs(wplus[:-1]).sum() == 3)
 
     def test_proportional_trade(self):
         """Test proportional trade policy."""
 
+        # targets do not sum to 1
+        wrong_targets = pd.Series(0, self.returns.columns)
+        wrong_targets = pd.DataFrame(
+            {self.returns.index[3]: wrong_targets,
+            self.returns.index[15]: wrong_targets}).T
+        with self.assertRaises(ValueError):
+            policy = cvx.ProportionalTradeToTargets(wrong_targets)
+            valid_start = pd.Series(0, self.returns.columns)
+            valid_start['cash'] = 1.
+            policy.execute(
+                market_data=self.market_data, h=valid_start,
+                t=self.returns.index[7])
+
         a = pd.Series(1., self.returns.columns)
         a.iloc[-1] = 1 - sum(a.iloc[:-1])
         b = pd.Series(-1., self.returns.columns)
         b.iloc[-1] = 1 - sum(b.iloc[:-1])
 
         targets = pd.DataFrame({self.returns.index[3]: a,
                                 self.returns.index[15]: b
@@ -111,25 +124,25 @@
             universe=self.returns.columns, trading_calendar=self.returns.index)
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
             self.returns.columns)
         start_portfolio.iloc[-1] = 1 - sum(start_portfolio.iloc[:-1])
         for t in self.returns.index[:17]:
-            print(t)
-            print(start_portfolio)
+            # print(t)
+            # print(start_portfolio)
 
             wplus = policy.values_in_time_recursive(
                 t=t, current_weights=start_portfolio)
             trade = wplus - start_portfolio.values
             start_portfolio = pd.Series(wplus, copy=True)
 
             if t in targets.index:
                 self.assertTrue(np.all(start_portfolio == targets.loc[t]))
-        print('trade', trade)
+        # print('trade', trade)
         self.assertTrue(np.allclose(trade, 0.))
 
     def test_sell_all(self):
         """Test sell-all policy."""
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
@@ -266,15 +279,15 @@
         wplus = policy.values_in_time_recursive(
             t=self.returns.index[1], current_weights=init)
         trade = wplus - init
         wplus2 = policy.values_in_time_recursive(
             t=self.returns.index[2], current_weights=wplus)
         trade2 = wplus2 - wplus
         self.assertTrue(np.allclose(trade, trade2))
-        print(trade + trade2 + init, target)
+        # print(trade + trade2 + init, target)
         self.assertTrue(np.allclose(trade + trade2 + init, target))
 
     def test_adaptive_rebalance(self):
         """Test adaptive rebalance policy."""
         np.random.seed(0)
         target = pd.Series(
             np.random.uniform(
@@ -319,15 +332,14 @@
                 cvx.LongOnly(applies_to_cash=False), cvx.LeverageLimit(1)],
             include_cash_return=False,
             # verbose=True,
             solver=self.default_socp_solver)
 
         policy.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
-        # policy.compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         result = policy.values_in_time_recursive(
             t=self.returns.index[121],
             current_weights=pd.Series(
@@ -336,15 +348,15 @@
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:121],
             past_volumes=self.volumes.iloc[:121],
             current_prices=pd.Series(1., self.volumes.columns))
 
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
-        print(cvxportfolio_result)
+        # print(cvxportfolio_result)
 
         # print(np.linalg.eigh(self.returns.iloc[:121, :-1].cov().values)[0])
 
         # REPLICATE WITH CVXPY
 
         covariance = self.returns.iloc[:121, :-1].cov(ddof=0).values
         w = cp.Variable(self.N)
@@ -352,17 +364,17 @@
             cp.Maximize(w[:-1].T @ self.returns.iloc[:121, :-1].mean().values -
             2 * cp.quad_form(w[:-1], covariance) -
             5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])),
             [w >= 0, w <= 1, sum(w) == 1]).solve(solver='ECOS')
 
         cvxpy_result = pd.Series(w.value, self.returns.columns)
 
-        print(cvxpy_result)
+        # print(cvxpy_result)
 
-        print(cvxportfolio_result - cvxpy_result)
+        # print(cvxportfolio_result - cvxpy_result)
         self.assertTrue(np.allclose(
             cvxportfolio_result - cvxpy_result, 0., atol=1e-5))
 
     def test_single_period_optimization_solve_twice(self):
         """Test resolve of SPO policy with Cvxpy parameters."""
 
         return_forecast = cvx.ReturnsForecast()
@@ -374,15 +386,14 @@
             - cvx.TransactionCost(a=5 * 1E-4, b=0.),
             constraints=[cvx.LongOnly(), cvx.LeverageLimit(1)],
             # verbose=True,
             solver=self.default_socp_solver)
 
         policy.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
-        # policy.compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         result = policy.values_in_time_recursive(
             t=self.returns.index[134],
             current_weights=pd.Series(
@@ -421,15 +432,14 @@
             constraints=[cvx.LongOnly(), cvx.LeverageLimit(1),
                 cvx.MaxWeights(-1)],
             # verbose=True,
             solver=self.default_socp_solver)
 
         policy.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
-        # policy.compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
             policy.values_in_time_recursive(
                 t=self.returns.index[134],
@@ -449,15 +459,14 @@
             return_forecast,
             constraints=[cvx.LongOnly(applies_to_cash=False)],
             # verbose=True,
             solver=self.default_socp_solver)
 
         policy.initialize_estimator_recursive(
             universe=self.returns.columns, trading_calendar=self.returns.index)
-        # policy.compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
             policy.values_in_time_recursive(
                 t=self.returns.index[134],
@@ -487,15 +496,14 @@
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver=self.default_socp_solver)
 
             policy.initialize_estimator_recursive(
                 universe=self.returns.columns,
                 trading_calendar=self.returns.index)
-            # policy.compile_to_cvxpy()
 
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             results.append(policy.values_in_time_recursive(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
@@ -525,15 +533,14 @@
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver=self.default_socp_solver)
 
             policy.initialize_estimator_recursive(
                 universe=self.returns.columns,
                 trading_calendar=self.returns.index)
-            # policy.compile_to_cvxpy()
 
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             results.append(policy.values_in_time_recursive(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
@@ -582,15 +589,14 @@
                 terminal_constraint=benchmark,
                 planning_horizon=planning_horizon,
                 solver=self.default_socp_solver)
 
             policy.initialize_estimator_recursive(
                 universe=self.returns.columns,
                 trading_calendar=self.returns.index)
-            # policy.compile_to_cvxpy()
 
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             diff_to_benchmarks.append(policy.values_in_time_recursive(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
@@ -604,22 +610,114 @@
 
         self.assertTrue(np.isclose(np.linalg.norm(diff_to_benchmarks[0]), 0.))
         self.assertTrue(np.linalg.norm(
             diff_to_benchmarks[0]) < np.linalg.norm(diff_to_benchmarks[1]))
         self.assertTrue(np.linalg.norm(
             diff_to_benchmarks[1]) < np.linalg.norm(diff_to_benchmarks[2]))
 
+    def test_dcp_check_MPO(self):
+        """Test DCP checks in S/MPO."""
+
+        t = self.market_data.returns.index[50]
+        h = pd.Series(0., self.market_data.universe_at_time(t))
+        h[self.market_data.cash_key] = 1.
+
+        class _NonDCP(cvx.costs.Cost): # pylint: disable=all
+            """Non DCP cost."""
+            def compile_to_cvxpy(self, w_plus, **kwargs):
+                """Making it convex to trigger specific check."""
+                return -w_plus[:-1] @ w_plus[:-1]
+
+        non_dcp_obj = cvx.SinglePeriodOptimization(
+            _NonDCP(), include_cash_return=False)
+
+        with self.assertRaises(cvx.errors.ConvexSpecificationError):
+            non_dcp_obj.execute(market_data=self.market_data, h=h)
+
+        # try with constraint; this one triggers a line in costs.py
+        non_dcp_constr = cvx.SinglePeriodOptimization(
+            cvx.ReturnsForecast(), [_NonDCP() >= 0.])
+        with self.assertRaises(cvx.errors.ConvexSpecificationError):
+            non_dcp_constr.execute(market_data=self.market_data, h=h)
+
+        class _NonDCPConstr(cvx.constraints.Constraint):
+            # pylint: disable=all
+            """Non DCP, but convex, constraint."""
+            def compile_to_cvxpy(self, w_plus, **kwargs):
+                return w_plus[:-1] @ w_plus[:-1] <= 0
+
+        non_dcp_constr1 = cvx.SinglePeriodOptimization(
+            cvx.ReturnsForecast(), [_NonDCPConstr()])
+        with self.assertRaises(cvx.errors.ConvexSpecificationError):
+            non_dcp_constr1.execute(market_data=self.market_data, h=h)
+
+    def test_MPO_difficult_errors(self):
+        """Test some error checks of MPO that are difficult to trigger."""
+
+        t = self.market_data.returns.index[50]
+        h = pd.Series(0., self.market_data.universe_at_time(t))
+        h[self.market_data.cash_key] = 1.
+
+        # check inside MultiPeriodOpt.values_in_time_recursive that
+        # the current value is positive; this check should be impossible
+        # to trigger by using the public interfaces
+        pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast())
+        pol.initialize_estimator_recursive(
+            universe=self.market_data.universe_at_time(t),
+            trading_calendar=self.market_data.trading_calendar())
+        with self.assertRaises(ValueError):
+            pol.values_in_time_recursive(
+                t, current_weights=h, current_portfolio_value=-1)
+
+        # numerical solver errors; these are known to happen with bad
+        # conditioning of the self-dual embedding matrix, but it's all
+        # solver-specific and hard to simulate; we simulate it by
+        # setting an extremely low maximum number of solver iterates;
+        # the fallback solver will work fine
+
+        pol = cvx.SinglePeriodOptimization(
+            cvx.ReturnsForecast() - cvx.FullCovariance(),
+            solver=self.default_qp_solver, max_iter=10)
+        with self.assertLogs(level='WARNING'):
+            pol.execute(market_data=self.market_data, h=h, t=t)
+
+        # then, we create a problem that also breaks the fallback solver
+
+        np.random.seed(0)
+        N = len(self.market_data.universe_at_time(t))-1
+        Sigma = np.random.randn(N, N)
+        Sigma = Sigma.T @ Sigma
+        eival, eivec = np.linalg.eigh(Sigma)
+        eival **= 10
+        Sigma = eivec @ np.diag(eival) @ eivec.T
+
+        randmu = np.random.randn(N)
+        randlim = np.random.randn(N)*100
+
+        pol = cvx.SinglePeriodOptimization(
+            cvx.ReturnsForecast(randmu) - cvx.FullCovariance(Sigma),
+            [cvx.MinWeights(randlim-1), cvx.MaxWeights(randlim+1)],
+            solver=self.default_qp_solver, max_iter=1)
+
+        with self.assertLogs(level='ERROR') as logs:
+            with self.assertRaises(cvx.errors.PortfolioOptimizationError):
+                pol.execute(market_data=self.market_data, h=h, t=t)
+
+                # on some combinations of platform and version,
+                # the fallback solver solves this problem
+                raise cvx.errors.PortfolioOptimizationError # pragma: no cover
+
     def test_execute(self):
         """Test the ``execute`` method."""
 
         policy = cvx.Uniform()
         h = pd.Series(0., self.returns.columns)
         h.iloc[-1] = 10000
         u, t, shares_traded = policy.execute(market_data=self.market_data, h=h)
-        print(t, u, shares_traded)
+        # print(t, u, shares_traded)
         self.assertTrue(np.isclose(u.sum(), 0.))
         self.assertTrue(t == self.returns.index[-1])
         self.assertTrue(len(set(u.iloc[:-1])) == 1)
 
         policy = cvx.SinglePeriodOptimization(
             cvx.ReturnsForecast() - 5 * cvx.FullCovariance(),
             [cvx.LongOnly(applies_to_cash=True)],
@@ -627,15 +725,15 @@
 
         market_data = cvx.UserProvidedMarketData(
                     returns=self.returns, volumes=self.volumes,
                     cash_key='cash', base_location=self.datadir,
                     min_history=pd.Timedelta('0d'))
 
         execution = policy.execute(market_data=market_data, h=h)
-        print(execution)
+        # print(execution)
         u, t, shares_traded = execution
         self.assertTrue(shares_traded is None)
         self.assertTrue(np.isclose(u.sum(), 0.))
         self.assertTrue(t == self.returns.index[-1])
         self.assertTrue(u['CSCO'] >= .9)
 
         # wrong time
@@ -676,11 +774,39 @@
                     cash_key='cash', base_location=self.datadir,
                     min_history=pd.Timedelta('0d'),
                     online_usage=True)
 
         execution_online = policy.execute(market_data=market_data, h=h)
         self.assertTrue(np.all(execution[0] == execution_online[0]))
 
+    def test_policy_reuse(self): # pylint: disable=too-many-locals
+        """Test policy re-used by execute.
+
+        Checks no memory issues, because we allocate/deallocate many structs
+        from extension modules. Also checks results are close (some CVXPY
+        interfaced solvers have built-in randomness).
+        """
+
+        sim, t_s, t_e, policies = self._difficult_simulator_and_policies()
+
+        all_times = sim.market_data.trading_calendar()
+        valid_times = all_times[(all_times >= t_s) & (all_times <= t_e)]
+
+        results_1, results_2 = {}, {}
+
+        for result in (results_1, results_2):
+            for policy in policies:
+                for t in valid_times:
+                    uni = sim.market_data.universe_at_time(t)
+                    h_init = pd.Series(0., uni)
+                    h_init[sim.market_data.cash_key] = 1E6
+                    # print(f'executing {policy} at time {t}')
+                    u, _, _ = policy.execute(
+                        h=h_init, market_data=sim.market_data, t=t)
+                    result[(str(policy), t)] = u
+
+        for k, v in results_1.items():
+            self.assertTrue(np.allclose(v, results_2[k]))
 
 if __name__ == '__main__':
 
     unittest.main(warnings='error') # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_returns.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_returns.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     def test_returns_forecast(self):
         """Test ReturnsForecast object with provided assets' returns."""
         alpha_model = ReturnsForecast(self.returns.iloc[:, :-1])
         cvxpy_expression = self.boilerplate(alpha_model)
         alpha_model.values_in_time_recursive(
             t=self.returns.index[123], past_returns=None)
         self.w_plus.value = np.random.randn(self.N)
-        print(cvxpy_expression.value)
-        print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1])
+        # print(cvxpy_expression.value)
+        # print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1])
         self.assertTrue(np.isclose(cvxpy_expression.value,
                         self.w_plus[:-1].value @ self.returns.iloc[123][:-1]))
 
     def test_full_returns_forecast(self):
         """Test ReturnsForecast object with historical mean forecasts."""
         alpha_model = ReturnsForecast()
         cvxpy_expression = self.boilerplate(alpha_model)
@@ -92,16 +92,16 @@
         error_risk = ReturnsForecastError()
         cvxpy_expression = self.boilerplate(error_risk)
         t = self.returns.index[123]
         past_returns = self.returns.loc[self.returns.index < t]
         error_risk.values_in_time_recursive(t=t, past_returns=past_returns)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         delta = past_returns.std(ddof=0) / np.sqrt(past_returns.count())
-        print(cvxpy_expression.value)
-        print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
+        # print(cvxpy_expression.value)
+        # print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(
             self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
 
 
 if __name__ == '__main__':
 
     unittest.main() # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_risks.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_risks.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
         should_be = past.iloc[:, :-1].T @ past.iloc[:, :-1] / len(past)
 
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model.values_in_time_recursive(t=t, past_returns=past)
-        print(cvxpy_expression.value)
+        # print(cvxpy_expression.value)
 
-        print(self.w_plus_minus_w_bm.value[:-1] @
-              should_be @ self.w_plus_minus_w_bm.value[:-1])
+        # print(self.w_plus_minus_w_bm.value[:-1] @
+        #      should_be @ self.w_plus_minus_w_bm.value[:-1])
 
         self.assertTrue(
             np.isclose(cvxpy_expression.value,
             self.w_plus_minus_w_bm.value[:-1] @ should_be
                 @ self.w_plus_minus_w_bm.value[:-1]))
 
     def test_diagonal_covariance(self):
@@ -122,18 +122,18 @@
 
         t = historical_variances.index[123]
 
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model.values_in_time_recursive(t=t, past_returns='hello')
 
-        print(cvxpy_expression.value)
-        print((np.abs(
-            self.w_plus_minus_w_bm.value[:-1])
-                @ np.sqrt(historical_variances.loc[t]))**2)
+        # print(cvxpy_expression.value)
+        # print((np.abs(
+        #    self.w_plus_minus_w_bm.value[:-1])
+        #        @ np.sqrt(historical_variances.loc[t]))**2)
         self.assertTrue(
             np.isclose(cvxpy_expression.value,
             (np.abs(self.w_plus_minus_w_bm.value[:-1])
                 @ np.sqrt(historical_variances.loc[t]))**2))
 
     def test_full_forecast_error(self):
         """Test RiskForecastError term estimated internally."""
@@ -237,30 +237,32 @@
         worst_case = cvx.WorstCaseRisk([risk_model0, risk_model1])
 
         cvxpy_expression = self.boilerplate(worst_case)
 
         assert cvxpy_expression.is_convex()
 
         cvxpy_expression0 = risk_model0.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
         cvxpy_expression1 = risk_model1.compile_to_cvxpy(
-            self.w_plus, self.z, self.w_plus_minus_w_bm)
+            w_plus=self.w_plus, z=self.z,
+            w_plus_minus_w_bm=self.w_plus_minus_w_bm)
 
         self.w_plus_minus_w_bm.value = np.ones(self.N)
 
         t = pd.Timestamp('2014-06-02')
 
         worst_case.values_in_time_recursive(
             t=t, past_returns=self.returns.loc[self.returns.index < t],
             current_weights=None, current_portfolio_value=None,
             past_volumes=None, current_prices=None)
 
-        print(cvxpy_expression.value)
-        print(cvxpy_expression0.value)
-        print(cvxpy_expression1.value)
+        # print(cvxpy_expression.value)
+        # print(cvxpy_expression0.value)
+        # print(cvxpy_expression1.value)
         self.assertTrue(cvxpy_expression.value == cvxpy_expression0.value)
         self.assertTrue(cvxpy_expression.value > cvxpy_expression1.value)
 
 
 if __name__ == '__main__':
 
     unittest.main() # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for the market simulator and its backtest methods."""
 
+# pylint: disable=too-many-lines
+
 import copy
+import datetime
 import multiprocessing
+import re
 import time
 import unittest
 
 import numpy as np
 import pandas as pd
 
 import cvxportfolio as cvx
 from cvxportfolio.errors import ConvexityError, ConvexSpecificationError
 from cvxportfolio.simulator import MarketSimulator, StockMarketSimulator
 from cvxportfolio.tests import CvxportfolioTest
 
 
+# pylint: disable=too-many-public-methods
 class TestSimulator(CvxportfolioTest):
     """Test MarketSimulator and assorted end-to-end tests."""
 
     @classmethod
     def setUpClass(cls):
         """Also define some MarketData objects to share.
 
@@ -79,21 +84,26 @@
 
         :param years: How many years.
         :type years: int
         :param assets: How many assets (max 28).
         :type assets: int
         :param nan_frac: Fraction of NaNs (approximate).
         :type nan_frac: float
+
+        :returns: Market data object.
+        :rtype: cvx.UserProvidedMarketData
         """
         rng = np.random.default_rng(seed=0)
         bs_index = rng.choice(cls.returns.index, size=len(cls.returns)*years)
-        rets = cls.returns.iloc[:, -assets-1:].loc[bs_index]
-        vols = cls.volumes.iloc[:, -assets:].loc[bs_index]
+        rets = pd.DataFrame(
+            cls.returns.iloc[:, -assets-1:].loc[bs_index], copy=True)
+        vols = pd.DataFrame(
+            cls.volumes.iloc[:, -assets:].loc[bs_index], copy=True)
         index = pd.date_range(
-            freq='1b', periods=len(rets), end=pd.Timestamp.utcnow().date())
+            freq='1b', periods=len(rets), end=datetime.date(2024, 4, 1))
         rets.index = index
         vols.index = index
         rets.iloc[-1] = np.nan
         vols.iloc[-1] = np.nan
         np.random.seed(0)
         rets *= np.random.randn(*rets.shape)*0.01 + 1
         vols *= np.random.randn(*vols.shape)*0.1 + 1
@@ -148,160 +158,14 @@
         with self.assertRaises(SyntaxError):
             MarketSimulator(returns=pd.DataFrame(
                 [[0., 0.]], index=[pd.Timestamp.today()],
                 columns=['X', 'USDOLLAR']),
                 volumes=pd.DataFrame([[0.]]),
                 min_history = pd.Timedelta('0d'))
 
-    def test_backtest_with_time_changing_universe(self):
-        """Test back-test with user-defined time-varying universe."""
-        rets = pd.DataFrame(self.returns.iloc[:, -10:], copy=True)
-        volumes = pd.DataFrame(self.volumes.iloc[:, -9:], copy=True)
-        prices = pd.DataFrame(self.prices.iloc[:, -9:], copy=True)
-
-        universe_selection = pd.DataFrame(
-            True, index=rets.index, columns=rets.columns[:-1])
-        universe_selection.iloc[14:25, 1:3] = False
-        universe_selection.iloc[9:17, 3:5] = False
-        universe_selection.iloc[8:15, 5:7] = False
-        universe_selection.iloc[16:29, 7:8] = False
-        print(universe_selection.iloc[10:20])
-
-        modified_market_data = cvx.UserProvidedMarketData(
-            returns=rets, volumes=volumes, prices=prices,
-            cash_key='cash',
-            min_history=pd.Timedelta('0d'),
-            universe_selection_in_time=universe_selection)
-
-        simulator = cvx.StockMarketSimulator(market_data=modified_market_data)
-
-        policy = cvx.SinglePeriodOptimization(
-            cvx.ReturnsForecast() - 10 * cvx.FullCovariance(),
-            [cvx.LongOnly(), cvx.LeverageLimit(1)],
-            solver=self.default_qp_solver)
-
-        # with self.assertRaises(ValueError):
-        #     simulator.backtest(policy, start_time = rets.index[10],
-        #     end_time = rets.index[9])
-
-        bt_result = simulator.backtest(policy, start_time = rets.index[10],
-            end_time = rets.index[20])
-
-        print(bt_result.w)
-
-        self.assertTrue(set(bt_result.w.columns) == set(rets.columns))
-        self.assertTrue(
-            np.all(bt_result.w.iloc[:-1, :-1].isnull()
-                == ~universe_selection.iloc[10:20]))
-
-        # try without repeating the uni
-        reduced = pd.DataFrame(universe_selection.iloc[10:20], copy=True)
-        reduced = pd.DataFrame(reduced.iloc[[0, 4, 5, 6, 7]], copy=True)
-        print(reduced)
-
-        modified_market_data = cvx.UserProvidedMarketData(
-            returns=rets, volumes=volumes, prices=prices,
-            cash_key='cash',
-            min_history=pd.Timedelta('0d'),
-            universe_selection_in_time=reduced)
-
-        simulator = cvx.StockMarketSimulator(market_data=modified_market_data)
-
-        bt_result1 = simulator.backtest(policy, start_time = rets.index[10],
-            end_time = rets.index[20])
-
-        self.assertTrue(bt_result.sharpe_ratio == bt_result1.sharpe_ratio)
-
-    def test_backtest_with_ipos_and_delistings(self):
-        """Test back-test with assets that both enter and exit."""
-        rets = pd.DataFrame(self.returns.iloc[:, -10:], copy=True)
-        volumes = pd.DataFrame(self.volumes.iloc[:, -9:], copy=True)
-        prices = pd.DataFrame(self.prices.iloc[:, -9:], copy=True)
-        rets.iloc[14:25, 1:3] = np.nan
-        rets.iloc[9:17, 3:5] = np.nan
-        rets.iloc[8:15, 5:7] = np.nan
-        rets.iloc[16:29, 7:8] = np.nan
-        print(rets.iloc[10:20])
-
-        modified_market_data = cvx.UserProvidedMarketData(
-            returns=rets, volumes=volumes, prices=prices,
-            cash_key='cash',
-            min_history=pd.Timedelta('0d'))
-
-        simulator = cvx.StockMarketSimulator(market_data=modified_market_data)
-
-        policy = cvx.SinglePeriodOptimization(
-            cvx.ReturnsForecast() - 10 * cvx.FullCovariance(),
-            [cvx.LongOnly(), cvx.LeverageLimit(1)],
-            solver=self.default_qp_solver)
-
-        with self.assertRaises(ValueError):
-            simulator.backtest(policy, start_time = rets.index[10],
-            end_time = rets.index[9])
-
-        bt_result = simulator.backtest(policy, start_time = rets.index[10],
-            end_time = rets.index[20])
-
-        print(bt_result.w)
-
-        self.assertTrue(set(bt_result.w.columns) == set(rets.columns))
-        self.assertTrue(
-            np.all(bt_result.w.iloc[:-1].isnull() == rets.iloc[
-                10:20].isnull()))
-
-    def test_backtest_with_difficult_universe_changes(self):
-        """Test back-test with assets that both enter and exit at same time."""
-        rets = pd.DataFrame(self.returns.iloc[:, -10:], copy=True)
-        volumes = pd.DataFrame(self.volumes.iloc[:, -9:], copy=True)
-        prices = pd.DataFrame(self.prices.iloc[:, -9:], copy=True)
-        rets.iloc[15:25, 1:3] = np.nan
-        rets.iloc[9:17, 3:5] = np.nan
-        rets.iloc[8:15, 5:7] = np.nan
-        rets.iloc[17:29, 7:8] = np.nan
-        print(rets.iloc[10:20])
-
-        modified_market_data = cvx.UserProvidedMarketData(
-            returns=rets, volumes=volumes, prices=prices,
-            cash_key='cash',
-            min_history=pd.Timedelta('0d'))
-
-        simulator = cvx.StockMarketSimulator(market_data=modified_market_data)
-
-        policy = cvx.SinglePeriodOptimization(
-            cvx.ReturnsForecast() - 10 * cvx.FullSigma(),
-            [cvx.LongOnly(), cvx.LeverageLimit(1)],
-            solver=self.default_qp_solver)
-
-        bt_result = simulator.run_backtest(policy, start_time = rets.index[10],
-            end_time = rets.index[20])
-
-        print(bt_result.w)
-
-        self.assertTrue(set(bt_result.w.columns) == set(rets.columns))
-        self.assertTrue(
-            np.all(bt_result.w.iloc[:-1].isnull() == rets.iloc[
-                10:20].isnull()))
-
-    def test_prepare_data(self):
-        """Test that (Downloaded)MarketData is created correctly."""
-        market_data = cvx.DownloadedMarketData(
-            ['ZM', 'META'], grace_period = self.data_grace_period,
-            base_location=self.datadir)
-        self.assertTrue(market_data.returns.shape[1] == 3)
-        self.assertTrue(market_data.prices.shape[1] == 2)
-        self.assertTrue(market_data.volumes.shape[1] == 2)
-        # self.assertTrue( simulator.sigma_estimate.data.shape[1] == 2)
-        self.assertTrue(np.isnan(market_data.returns.iloc[-1, 0]))
-        self.assertTrue(np.isnan(market_data.volumes.iloc[-1, 1]))
-        self.assertTrue(not np.isnan(market_data.prices.iloc[-1, 0]))
-        self.assertTrue(
-            market_data.returns.index[-1] == market_data.volumes.index[-1])
-        self.assertTrue(
-            market_data.returns.index[-1] == market_data.prices.index[-1])
-
     def test_holding_cost(self):
         """Test the simulator interface of cvx.HoldingCost."""
 
         t = self.returns.index[-20]
 
         # stock holding cost
         for i in range(10):
@@ -328,15 +192,15 @@
                 current_prices=None,
                 current_portfolio_value=sum(h_plus),
                 current_weights=None)
 
             hcost = -(np.exp(np.log(1.05)/365.24)-1) * sum(
                 -np.minimum(h_plus, 0.)[:-1])
             hcost += dividends @ h_plus[:-1]
-            print(hcost, -sim_hcost)
+            # print(hcost, -sim_hcost)
             self.assertTrue(np.isclose(hcost, -sim_hcost))
 
     def test_transaction_cost_syntax(self):
         """Test syntax checks of (Stocks)TransactionCost."""
 
         t = self.returns.index[-20]
 
@@ -376,15 +240,28 @@
         with self.assertRaises(SyntaxError):
             tcost.simulate_recursive(t=t, u=u, current_prices=current_prices,
                             past_returns=past_returns,
                             current_returns=current_returns,
                             past_volumes=None,
                             current_volumes=None,
                             current_portfolio_value=None,
-                            current_weights=None,)
+                            current_weights=None)
+
+        tcost = cvx.TransactionCost(b=0., volume_hat=1.)
+        tcost.initialize_estimator_recursive(
+                universe=current_returns.index, trading_calendar=[t])
+        with self.assertRaises(SyntaxError):
+            tcost.simulate_recursive(t=t, u=u, current_prices=None,
+                        t_next=None, h_plus=pd.Series(1., u.index),
+                        past_returns=past_returns,
+                        current_returns=current_returns,
+                        past_volumes=past_volumes,
+                        current_volumes=current_volumes,
+                        current_portfolio_value=1000,
+                        current_weights=None,)
 
         with self.assertWarns(DeprecationWarning):
             tcost = cvx.StocksTransactionCost(window_volume_est=252)
         with self.assertRaises(SyntaxError):
             tcost.values_in_time_recursive(t=t,
                 current_prices=current_prices,
                 past_returns=past_returns,
@@ -447,15 +324,15 @@
             shares = sum(np.abs(u[:-1] / current_prices))
             tcost = -0.005 * shares
             # print(tcost, sim_cost)
             tcost -= np.abs(u.iloc[:-1]) @ spreads / 2
             tcost -= sum((np.abs(u.iloc[:-1])**1.5
                 ) * self.returns.loc[self.returns.index <=
                 t].iloc[-252:, :-1].std(ddof=0) / np.sqrt(self.volumes.loc[t]))
-            print(tcost, sim_cost)
+            # print(tcost, sim_cost)
             self.assertTrue(np.isclose(tcost, -sim_cost))
 
     def test_methods(self):
         """Test some methods of MarketSimulator."""
         simulator = MarketSimulator(
             # because we modify it
             market_data=copy.deepcopy(self.md_3assets),
@@ -478,17 +355,54 @@
                 rounded = simulator._round_trade_vector(
                     u, simulator.market_data.prices.loc[t])
                 self.assertTrue(np.isclose(sum(rounded), 0))
                 self.assertTrue(
                     np.linalg.norm(rounded[:-1] - u[:-1])
                     < np.linalg.norm(simulator.market_data.prices.loc[t]/2))
 
-                print(u)
+                # print(u)
+
+    def test_backtest_cache(self):
+        """Test methods of cache.py, which stores factorized covariances.
+
+        This is scheduled for refactoring, but currently only works with
+        downloaded data, so we have to use that.
+        """
+        simulator = StockMarketSimulator(
+            market_data = cvx.DownloadedMarketData(
+                ['META', 'AAPL'],
+                grace_period=self.data_grace_period,
+                base_location=self.datadir),
+                base_location=self.datadir) # need to specify for cache loc
+
+        policy = cvx.SinglePeriodOptimization(
+            cvx.ReturnsForecast() - .5 * cvx.FullCovariance(),
+            [cvx.LongOnly(applies_to_cash=True)])
+
+        self.assertFalse((self.datadir / 'backtest_cache').exists())
+
+        result_fresh = simulator.backtest(
+            policy, start_time='2024-01-01', end_time='2024-02-01')
+
+        self.assertTrue((self.datadir / 'backtest_cache').exists())
+        self.assertTrue((self.datadir / 'backtest_cache').is_dir())
+        caches = list((self.datadir / 'backtest_cache').iterdir())
+        self.assertEqual(len(caches), 1)
+        self.assertEqual('.pkl', str(caches[0])[-4:])
+
+        result_w_cache = simulator.backtest(
+            policy, start_time='2024-01-01', end_time='2024-02-01')
 
-    def test_simulate_policy(self):
+        self.assertTrue(np.allclose(result_fresh.w, result_w_cache.w))
+
+        caches_same = list((self.datadir / 'backtest_cache').iterdir())
+        self.assertEqual(len(caches_same), 1)
+        self.assertEqual(str(caches_same[0]), str(caches[0]))
+
+    def test_simulate_policy(self): # pylint: disable=too-many-locals
         """Test basic policy simulation."""
         simulator = StockMarketSimulator(
             # because we modify it
             # market_data=copy.deepcopy(self.market_data_3),
             # base_location=self.datadir)
             market_data = cvx.DownloadedMarketData(
                 ['META', 'AAPL'],
@@ -581,15 +495,15 @@
                 h, _, _, costs, _ = simulator.simulate(
                     t=t, h=h, policy=policy, t_next=t_next,
                     past_returns=past_returns, current_returns=current_returns,
                     past_volumes=past_volumes, current_volumes=current_volumes,
                     current_prices=current_prices)
                 tcost, hcost = costs['StocksTransactionCost'
                     ], costs['StocksHoldingCost']
-                print(h)
+                # print(h)
                 # print(tcost, stock_hcost, cash_hcost)
 
             self.assertTrue(
                 np.all(np.abs(h[:-1])
                     < simulator.market_data.prices.loc[end_time]))
 
     def test_backtest(self):
@@ -602,16 +516,15 @@
             [cvx.LeverageLimit(1)], # verbose=True,
             solver=self.default_socp_solver)
         sim = cvx.MarketSimulator(
             market_data=self.md_3assets, base_location=self.datadir)
         # print(self.md_3assets.returns)
         result = sim.backtest(pol, pd.Timestamp(
             '2014-06-01'), pd.Timestamp('2014-08-20'))
-
-        print(result)
+        str(result)
 
     def test_wrong_worstcase(self):
         """Test wrong worst-case convexity."""
         pol = cvx.SinglePeriodOptimization(
             cvx.ReturnsForecast() - cvx.ReturnsForecastError()
             - .5 * cvx.WorstCaseRisk(
                 [-cvx.FullCovariance(),
@@ -629,15 +542,15 @@
         """Test back-test with changing universe.
 
         Second asset is out of the universe initially.
         """
 
         sim = cvx.MarketSimulator(
             market_data=self.md_2assets_nan, base_location=self.datadir)
-        print(sim.market_data.returns)
+        # print(sim.market_data.returns)
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
                                            cvx.ReturnsForecastError() -
                                            .5 * cvx.FullCovariance(),
                                            [  # cvx.LongOnly(),
             cvx.LeverageLimit(1)], # verbose=True,
             solver=self.default_qp_solver)
 
@@ -649,17 +562,17 @@
             result.w[sim.market_data.returns.columns[1]].isnull().sum() > 5)
         self.assertTrue(
             result.w[sim.market_data.returns.columns[0]].isnull().sum() < 2)
         self.assertTrue(len(ridx) == len(set(ridx)))
         self.assertTrue(len(ridx) == len(sim.market_data.returns.loc[
             (sim.market_data.returns.index >= ridx[0]) & (
             sim.market_data.returns.index <= ridx[-1])]))
-        print(result)
+        # print(result)
 
-    def test_multiple_backtest(self):
+    def test_multiple_backtest(self): # pylint: disable=too-many-locals
         """Test multiple back-tests (in parallel)."""
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
                                            cvx.ReturnsForecastError() -
                                            .5 * cvx.FullCovariance(),
                                            [  # cvx.LongOnly(),
             cvx.LeverageLimit(1)], # verbose=True,
             solver=self.default_qp_solver)
@@ -756,17 +669,17 @@
 
             cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
             ) - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)],
                 benchmark=cvx.MarketBenchmark, solver=self.default_qp_solver),
         ]
         results = sim.backtest_many(pols, pd.Timestamp(
             start), pd.Timestamp(end), parallel=True)
-        print(np.linalg.norm(results[0].w.sum()[:2] - .5))
-        print(np.linalg.norm(results[1].w.sum()[:2] - .5))
-        print(np.linalg.norm(results[2].w.sum()[:2] - .5))
+        # print(np.linalg.norm(results[0].w.sum()[:2] - .5))
+        # print(np.linalg.norm(results[1].w.sum()[:2] - .5))
+        # print(np.linalg.norm(results[2].w.sum()[:2] - .5))
         self.assertTrue(np.linalg.norm(results[1].w.sum()[
                         :2] - .5) < np.linalg.norm(
                         results[0].w.sum()[:2] - .5))
         self.assertTrue(np.linalg.norm(results[1].w.sum()[
                         :2] - .5) < np.linalg.norm(
                         results[2].w.sum()[:2] - .5))
 
@@ -787,15 +700,15 @@
                 market_data=market_data,
                 base_location=self.datadir)
             pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
             ) - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5),
             [cvx.LeverageLimit(1)], solver=self.default_socp_solver)
             s = time.time()
             results_first.append(sim.backtest(pol, pd.Timestamp('2020-12-01')))
-            print(results_first[-1])
+            # print(results_first[-1])
             time_first += time.time() - s
 
         with self.assertRaises(SyntaxError):
             _ = cvx.UserProvidedMarketData(
                 returns=self.returns,
                 prices=self.prices,
                 volumes=self.volumes,
@@ -821,38 +734,26 @@
             pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
             ) - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5),
             [cvx.LeverageLimit(1)],
             solver=self.default_socp_solver)
             s = time.time()
             results_second.append(sim.backtest(
                 pol, pd.Timestamp('2020-12-01')))
-            print(results_second[-1])
+            # print(results_second[-1])
             time_second += time.time() - s
 
         # example is too small to see speed difference w/ cache
         # sadly we have to drop this test element (also cache is not enabled
         # with user-provided data, currently)
         # self.assertTrue(time_second < time_first)
-        print(time_second, time_first)
+        # print(time_second, time_first)
         for i, _ in enumerate(results_first):
             self.assertTrue(
                 np.isclose(_.sharpe_ratio, results_second[i].sharpe_ratio))
 
-    def test_result(self):
-        """Test methods and properties of result."""
-        sim = cvx.MarketSimulator(
-            market_data = self.md_2assets_nan, base_location=self.datadir)
-        result = sim.backtest(cvx.Uniform(), pd.Timestamp(
-            '2014-05-01'))
-        result.plot(show=False)
-        result.times_plot(show=False)
-        print(result)
-        for attribute in dir(result):
-            print(attribute, getattr(result, attribute))
-
     def test_spo_benchmark(self):
         """Test the effect of benchmark on SPO policies."""
 
         sim = cvx.MarketSimulator(
             market_data=self.md_5assets, base_location=self.datadir)
 
         objective = cvx.ReturnsForecast() - 20 * (
@@ -861,15 +762,15 @@
 
         myunif = pd.Series(0.2, sim.market_data.returns.columns[:-1])
         myunif[sim.market_data.cash_key] = 0.
 
         policies = [
             cvx.SinglePeriodOptimization(
                 objective, constraints, benchmark=bm,
-                solver=self.default_qp_solver)
+                solver=self.default_socp_solver)
             for bm in
                 [cvx.AllCash(), cvx.Uniform(), cvx.MarketBenchmark(), myunif]]
 
         results = sim.backtest_many(
             policies, #start_time='2014-02-01',
             parallel=False)  # important for test coverage!!
 
@@ -884,94 +785,101 @@
                         results[2].w[sim.market_data.cash_key].mean())
 
         # check that uniform bm sol is closer
         # to uniform alloc than market bm sol
         norm_smaller = (
             (results[1].w.iloc[:, :-1] - 0.2)
               ** 2).mean(1) < ((results[2].w.iloc[:, :-1] - 0.2)**2).mean(1)
-        print(norm_smaller.describe())
+        # print(norm_smaller.describe())
         self.assertTrue(norm_smaller.mean() > .5)
 
     def test_market_neutral(self):
         """Test SPO with market neutral constraint."""
-        market_data = cvx.DownloadedMarketData(
-            ['AAPL', 'MSFT', 'GE', 'GOOG', 'META', 'GLD'],
-            base_location=self.datadir,
-            grace_period=self.data_grace_period,
-            trading_frequency='monthly')
+        market_data = self.generate_market_data(nan_frac=.2)
         sim = cvx.MarketSimulator(
             market_data=market_data, base_location=self.datadir)
 
         objective = cvx.ReturnsForecast() - 2 * cvx.FullCovariance()
 
         policies = [cvx.SinglePeriodOptimization(objective, co,
             solver=self.default_qp_solver) for co in [
             [], [cvx.MarketNeutral()], [cvx.DollarNeutral()]]]
 
         results = sim.backtest_many(
-            policies, start_time='2023-01-01',
+            policies, start_time='2023-01-01', end_time='2023-02-01',
             parallel=False)  # important for test coverage
 
-        print(results)
+        # print(results)
 
-        # check that market neutral sol is closer to
         dists_from_dollar_neutral = [
             np.abs(result.w.iloc[:, -1] - 1).mean() for result in results]
-        print('dists_from_dollar_neutral')
-        print(dists_from_dollar_neutral)
+        # print('dists_from_dollar_neutral')
+        # print(dists_from_dollar_neutral)
         self.assertTrue(
             dists_from_dollar_neutral[2] < dists_from_dollar_neutral[1])
         self.assertTrue(
             dists_from_dollar_neutral[1] < dists_from_dollar_neutral[0])
 
     def test_timed_constraints(self):
         """Test some constraints that depend on time."""
 
-        market_data = cvx.DownloadedMarketData(
-            ['AAPL', 'MSFT', 'GE', 'ZM', 'META'],
-            base_location=self.datadir,
-            grace_period=self.data_grace_period,
-            trading_frequency='monthly')
+        # market_data = cvx.DownloadedMarketData(
+        #     ['AAPL', 'MSFT', 'GE', 'ZM', 'META'],
+        #     base_location=self.datadir,
+        #     grace_period=self.data_grace_period,
+        #     trading_frequency='monthly')
+        # stock = 'AAPL'
+
+        market_data = self.generate_market_data(assets=5, nan_frac=0.1)
+        stock = market_data.returns.columns[0]
 
         sim = cvx.StockMarketSimulator(
             market_data=market_data, base_location=self.datadir)
 
         # cvx.NoTrade
         objective = cvx.ReturnsForecast() - 2 * cvx.FullCovariance()
 
-        no_trade_ts = [sim.market_data.returns.index[-2],
-                       sim.market_data.returns.index[-6]]
+        base_idx = market_data.returns.index.get_loc('2023-01-02')
+        no_trade_idx = [base_idx + 7, base_idx + 17]
+        no_trade_ts = [market_data.returns.index[idx] for idx in no_trade_idx]
 
         policy = cvx.SinglePeriodOptimization(
-            objective, [cvx.NoTrade('AAPL', no_trade_ts)],
+            objective, [cvx.NoTrade(stock, no_trade_ts)],
             solver=self.default_qp_solver)
 
-        result = sim.backtest(policy, start_time='2023-01-01')
-        print(result.z)
+        result = sim.backtest(
+            policy, start_time='2023-01-01', end_time='2023-04-01')
+        str(result)
+        # print(result.z)
         for t in no_trade_ts:
-            self.assertTrue(np.isclose(result.z['AAPL'].loc[t], 0., atol=1E-3))
+            self.assertTrue(np.isclose(result.z[stock].loc[t], 0., atol=1E-3))
 
         # cvx.MinWeightsAtTimes, cvx.MaxWeightsAtTimes
         policies = [cvx.MultiPeriodOpt(
             objective - cvx.StocksTransactionCost(),
             [cvx.MinWeightsAtTimes(0., no_trade_ts),
-            cvx.MaxWeightsAtTimes(0., no_trade_ts)],
+            cvx.MaxWeightsAtTimes(0., no_trade_ts),
+            cvx.LeverageLimit(5)],
             planning_horizon=p,
             solver=self.default_socp_solver) for p in [1, 3, 5]]
 
         results = sim.backtest_many(
-            policies, start_time='2023-01-01', initial_value=1E6,
-            parallel=False)  # important for test coverage
-        print(results)
+            policies, start_time='2023-01-01', end_time='2023-02-01',
+            initial_value=1E7, parallel=False)  # important for test coverage
+        # print(results)
+
+        # check that the more planning horizon, the less steep the change
+        # in the stock with the timed constraint
+
+        how_fast_trades = [
+            np.abs(result.w[stock].diff()).mean() / result.w[stock].mean()
+                for result in results]
 
-        total_tcosts = [result.costs['StocksTransactionCost'].sum()
-                        for result in results]
-        print(total_tcosts)
-        self.assertTrue(total_tcosts[0] > total_tcosts[1])
-        self.assertTrue(total_tcosts[1] > total_tcosts[2])
+        self.assertGreater(how_fast_trades[0], how_fast_trades[1])
+        self.assertGreater(how_fast_trades[1], how_fast_trades[2])
 
     def test_eq_soft_constraints(self):
         """We check that soft DollarNeutral penalizes non-dollar-neutrality."""
 
         sim = cvx.MarketSimulator(
             market_data=self.md_5assets, base_location=self.datadir)
 
@@ -981,17 +889,17 @@
             objective - cvx.SoftConstraint(cvx.DollarNeutral()) * gamma)
             for gamma in [.0001, .001, .01]]
         policies.append(cvx.SinglePeriodOptimization(
             objective, [cvx.DollarNeutral()]))
         results = sim.backtest_many(
             policies, start_time='2014-06-01',
             parallel=False)  # important for test coverage
-        print(results)
+        # print(results)
         allcashpos = [((res.w.iloc[:, -1]-1)**2).mean() for res in results]
-        print(allcashpos)
+        # print(allcashpos)
         self.assertTrue(allcashpos[0] > allcashpos[1])
         self.assertTrue(allcashpos[1] > allcashpos[2])
         self.assertTrue(allcashpos[2] > allcashpos[3])
 
     def test_ineq_soft_constraints(self):
         """We check that soft LongOnly penalizes shorts."""
 
@@ -1006,18 +914,18 @@
             solver=self.default_socp_solver) for gamma in [.0001, .001]]
         policies.append(cvx.SinglePeriodOptimization(
             objective, [cvx.LongOnly(), cvx.MarketNeutral()],
             solver=self.default_socp_solver))
         results = sim.backtest_many(
             policies, start_time='2014-10-01',
             parallel=False)  # important for test coverage
-        print(results)
+        # print(results)
         allshorts = [np.minimum(res.w.iloc[:, :-1], 0.).sum().sum()
                      for res in results]
-        print(allshorts)
+        # print(allshorts)
         self.assertTrue(allshorts[0] < allshorts[1])
         self.assertTrue(allshorts[1] < allshorts[2])
 
     def test_cost_constraints(self):
         """We check that cost constraints work as expected."""
 
         sim = cvx.MarketSimulator(
@@ -1029,15 +937,15 @@
                 solver=self.default_socp_solver)
             for el in [0.01, .02, .05, .1]]
 
         results = sim.backtest_many(
             policies, start_time='2014-11-01',
             parallel=False)  # important for test coverage
 
-        print(results)
+        # print(results)
 
         self.assertTrue(results[0].volatility < results[1].volatility)
         self.assertTrue(results[1].volatility < results[2].volatility)
         self.assertTrue(results[2].volatility < results[3].volatility)
 
     def test_dcp_convex_raises(self):
         """Test that some errors are thrown at wrong problem specifications."""
@@ -1081,97 +989,93 @@
         self.assertTrue(gamma_risk.current_value == 1.)
         self.assertTrue(gamma_trade.current_value == 1.)
 
         init_sharpe = simulator.backtest(
             policy, start_time='2014-11-01').sharpe_ratio
 
         simulator.optimize_hyperparameters(
-            policy, start_time='2014-11-01')#, end_time='2023-10-01')
+            policy, start_time='2014-11-01') #, end_time='2023-10-01')
 
         opt_sharpe = simulator.backtest(
             policy, start_time='2014-11-01').sharpe_ratio
 
         self.assertTrue(opt_sharpe >= init_sharpe)
 
-        print(gamma_risk.current_value)
-        print(gamma_trade.current_value)
+        # print(gamma_risk.current_value)
+        # print(gamma_trade.current_value)
         # self.assertTrue(np.isclose(gamma_risk.current_value, 1.1))
         # self.assertTrue(np.isclose(gamma_trade.current_value, 1.61051))
 
     def test_cancel_trades(self):
         """Test trade cancellation."""
 
-        market_data = cvx.DownloadedMarketData(
-            ['AAPL', 'ZM'],
-            base_location=self.datadir,
-            grace_period=self.data_grace_period,
-            trading_frequency='monthly')
+        vols = pd.DataFrame(self.volumes, copy=True)
+        vols['AAPL'] = 0.
+        market_data = cvx.UserProvidedMarketData(
+            returns=pd.DataFrame(self.returns, copy=True), volumes=vols,
+            prices=pd.DataFrame(self.prices, copy=True), cash_key='cash',
+            min_history=pd.Timedelta('0d'))
+
         sim = cvx.MarketSimulator(
             market_data=market_data, base_location=self.datadir)
 
-        sim.market_data.volumes['ZM'] = 0.
-
         objective = cvx.ReturnsForecast() - 5 * cvx.FullCovariance()
         policy = cvx.SinglePeriodOptimization(
             objective, [cvx.LongOnly(), cvx.LeverageLimit(1)])
 
-        sim.backtest(policy, start_time='2023-01-01')
+        result = sim.backtest(
+            policy, start_time='2014-12-01', end_time='2014-12-31')
+
+        self.assertEqual( # every day there's this log line
+            len(re.findall(
+                'the simulator canceled trades.*AAPL', result.logs)), 21)
 
     def test_svd_covariance_forecaster(self):
         """Test SVD covariance forecaster in simulation."""
 
-        market_data = cvx.DownloadedMarketData(
-            ['AAPL', 'MSFT', 'GE', 'ZM', 'META', 'GOOG', 'GLD'],
-            base_location=self.datadir,
-            grace_period=self.data_grace_period,
-            trading_frequency='quarterly')
+        market_data = self.generate_market_data(nan_frac=.3)
         sim = cvx.StockMarketSimulator(
             market_data=market_data, base_location=self.datadir)
 
         objective = cvx.ReturnsForecast() - 5 * cvx.FactorModel(
             num_factors=2, Sigma=None)
         policy = cvx.SinglePeriodOpt(
             objective, [cvx.LongOnly(), cvx.LeverageLimit(1)],
             solver=self.default_qp_solver)
 
-        result_svd = sim.backtest(policy, start_time='2020-01-01',
-            end_time='2023-09-01')
+        result_svd = sim.backtest(
+            policy, start_time='2020-01-01', end_time='2020-03-01')
 
         objective = cvx.ReturnsForecast() - 5 * cvx.FactorModelCovariance(
             num_factors=2)
         policy = cvx.SinglePeriodOptimization(
             objective, [cvx.LongOnly(), cvx.LeverageLimit(1)],
             solver=self.default_qp_solver)
 
-        result_eig = sim.backtest(policy, start_time='2020-01-01',
-            end_time='2023-09-01')
+        result_eig = sim.backtest(
+            policy, start_time='2020-01-01', end_time='2020-03-01')
 
         self.assertTrue(result_svd.sharpe_ratio > result_eig.sharpe_ratio)
 
-        print(result_svd)
-        print(result_eig)
+        # print(result_svd)
+        # print(result_eig)
 
     def test_bankruptcy(self):
         """Test policy bankruptcy."""
 
-        market_data = cvx.DownloadedMarketData(
-            ['SPY', 'QQQ'],
-            base_location=self.datadir,
-            grace_period=self.data_grace_period)
         sim = cvx.StockMarketSimulator(
-            market_data=market_data, base_location=self.datadir)
+            market_data=self.market_data, base_location=self.datadir)
 
         policy = cvx.SinglePeriodOptimization(
-            cvx.ReturnsForecast(), [cvx.LeverageLimit(20)],
+            cvx.ReturnsForecast(), [cvx.LeverageLimit(30)],
             solver=self.default_qp_solver)
         with self.assertLogs(level='WARNING') as _:
             result = sim.backtest(policy,
-                start_time='2020-02-15', end_time='2020-04-15')
-        # print(result)
-        print(result.h)
+                start_time='2014-12-01', end_time='2020-12-31')
+        # print(result.h)
         self.assertTrue(result.h.shape[0] < 20)
         self.assertTrue(result.final_value < 0)
 
     def test_cache_missing_signature(self):
         """Test backtest with missing market data signature."""
         md = cvx.UserProvidedMarketData(
             returns=self.returns, volumes=self.volumes,
@@ -1188,10 +1092,32 @@
             [cvx.LongOnly(applies_to_cash=True)])
 
         simulator.backtest(
             policy, start_time = self.returns.index[10],
             end_time = self.returns.index[20],
             )
 
+    def test_market_simulator_reuse(self):
+        """Test re-use of MarketSimulator."""
+
+        sim, t_s, t_e, policies = self._difficult_simulator_and_policies()
+
+        results_mp = sim.backtest_many(
+            policies, start_time=t_s, end_time=t_e, parallel=True)
+
+        results_seq = [
+            sim.backtest(pol, start_time=t_s, end_time=t_e)
+                for pol in policies]
+
+        for first_result, second_result in zip(results_mp, results_seq):
+            self.assertTrue(
+                np.allclose(first_result.w, second_result.w, equal_nan=True))
+
+        for first_result, second_result in zip(results_mp, results_seq):
+            self.assertTrue(
+                np.isclose(
+                    first_result.sharpe_ratio, second_result.sharpe_ratio))
+
+
 if __name__ == '__main__':
 
     unittest.main(warnings='error') # pragma: no cover
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/test_utils.py` & `cvxportfolio-1.3.1/cvxportfolio/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,59 +24,60 @@
 class TestUtils(unittest.TestCase):
     """Test functions in the cvxportfolio.utils module."""
 
     def test_hasher(self):
         """Test hashing function."""
         a = np.array([1, 2, 3])
         re = repr_numpy_pandas(a)
-        print(re)
+        # print(re)
         b = np.array([[1, 2, 3]])
         re1 = repr_numpy_pandas(b)
-        print(re1)
+        # print(re1)
         self.assertTrue(re == re1)
 
         with self.assertRaises(NotImplementedError):
             repr_numpy_pandas('Hello!')
 
         a = pd.Series([1, 2, 3], ['2020-01-01', '2021-01-01', '2022-01-01'])
         re = repr_numpy_pandas(a)
-        print(re)
+        # print(re)
         b = pd.Series(a.values, a.index)
         re1 = repr_numpy_pandas(b)
-        print(re1)
+        # print(re1)
         self.assertTrue(re == re1)
 
         # multiindexed df
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         data.columns = ["one", "two", "tre", "quattro",
                         "cinque", "sei", "sette", "otto", "nove", "dieci"]
 
         re = repr_numpy_pandas(data)
-        print(re)
+        # print(re)
 
         data1 = pd.DataFrame(data.values,
                              index=data.index, columns=data.columns)
 
         re1 = repr_numpy_pandas(data1)
-        print(re1)
+        # print(re1)
         self.assertTrue(re == re1)
 
     def test_make_numeric(self):
         """Test make_numeric function for user-provided data."""
 
         for data in [
                 2., np.array([1, 2]), pd.Series([1, 2, 3]),
                 pd.DataFrame([[1, 2., 3], [4, 5., 6]])]:
             self.assertTrue(make_numeric(data) is data)
 
         for data in [
-                np.array([1, 2], dtype=object), pd.Series([1, 2, 3], dtype=object),
+                np.array([1, 2], dtype=object),
+                pd.Series([1, 2, 3], dtype=object),
                 pd.DataFrame([[1, 2., 3], [4, 5., 6]], dtype=object)]:
             self.assertTrue(np.all(make_numeric(data) == data))
 
         for data in [
                 np.array(['1', 2], dtype=object),
                 pd.Series([1, '2', 3], dtype=object),
                 pd.DataFrame([[1, '2.', 3], [4, '5.', 6]], dtype=object)]:
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio/tests/volumes.csv` & `cvxportfolio-1.3.1/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.0/cvxportfolio/utils.py` & `cvxportfolio-1.3.1/cvxportfolio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module contains miscellaneous functions."""
 
 import hashlib
-from numbers import Number
 
 import numpy as np
 import pandas as pd
 
 from .errors import DataError
 
 TRUNCATE_REPR_HASH = 10  # probability of conflict is 1e-16
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-1.3.1/cvxportfolio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 1.3.0
+Version: 1.3.1
 Summary: Portfolio optimization and back-testing.
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Maintainer-email: Enzo Busseti <enzo.busseti@gmail.com>
 License: Apache License (2.0)
 Project-URL: Homepage, https://www.cvxportfolio.com
 Project-URL: Repository, https://github.com/cvxgrp/cvxportfolio
 Description-Content-Type: text/x-rst
@@ -12,14 +12,15 @@
 License-File: AUTHORS
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: requests
 Requires-Dist: cvxpy
 Requires-Dist: multiprocess
+Requires-Dist: scs
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-github-style; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
@@ -32,27 +33,27 @@
 Requires-Dist: beautifulsoup4; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: beautifulsoup4; extra == "examples"
 Requires-Dist: lxml; extra == "examples"
 Requires-Dist: clarabel; extra == "examples"
 Requires-Dist: ecos; extra == "examples"
 
-`Cvxportfolio <https://www.cvxportfolio.com>`__
-===============================================
+`Cvxportfolio <https://www.cvxportfolio.com>`_
+==============================================
 
 |CVXportfolio on PyPI| |linting: pylint| |Coverage Status|
 |Documentation Status| |Apache 2.0 License| |Anaconda-Server Badge|
 
 
 Cvxportfolio is an object-oriented library for portfolio optimization
 and back-testing. It implements models described in the `accompanying paper
-<https://cvxportfolio.readthedocs.org/en/master/_static/cvx_portfolio.pdf>`_.
+<https://cvxportfolio.readthedocs.io/en/master/_static/cvx_portfolio.pdf>`_.
 
 The documentation of the library is at
-`www.cvxportfolio.com <https://www.cvxportfolio.com>`__.
+`www.cvxportfolio.com <https://www.cvxportfolio.com>`_.
 
 .. Installation
 
 *News:*
 
    Since end of 2023 we're running daily `example strategies
    <https://github.com/cvxgrp/cvxportfolio/tree/master/examples/strategies>`_
@@ -67,15 +68,15 @@
 environment by simple:
 
 .. code:: bash
 
    pip install -U cvxportfolio
 
 You can see how this works on our `Installation and Hello
-World <https://youtu.be/1ThOKEu371M>`__ youtube video. 
+World <https://youtu.be/1ThOKEu371M>`_ youtube video.
 Anaconda installs 
 `are also supported <https://anaconda.org/conda-forge/cvxportfolio>`_.
 
 Cvxportfolio's main dependencies are `Cvxpy <https://www.cvxpy.org>`_ for
 interfacing with numerical solvers and `Pandas <https://pandas.pydata.org/>`_
 for interfacing with databases. We don't require any specific version of our
 dependencies and test against all recent ones (up to a few years ago).
@@ -139,42 +140,42 @@
 the paper, and default parameters that are typical for the US stock
 market.
 
 Other examples
 --------------
 
 `Many examples 
-<https://www.cvxportfolio.com/en/stable/examples.html>`_
+<https://cvxportfolio.readthedocs.io/en/stable/examples.html>`_
 are shown in the documentation website, along with
 their output and comments.
 
 `Even more example scripts
 <https://github.com/cvxgrp/cvxportfolio/blob/master/examples>`_ 
 are available in the code repository. 
 
 `The original examples from the paper 
 <https://github.com/cvxgrp/cvxportfolio/tree/0.0.X/examples>`_ 
 are visible in a dedicated branch,
 and are being translated to run with the stable versions (``1.0.0`` and above) of the
 library. The translations are visible at `this documentation page
-<https://www.cvxportfolio.com/en/stable/examples/paper_examples.html>`_.
+<https://cvxportfolio.readthedocs.io/en/stable/examples/paper_examples.html>`_.
 
 We show in the example on `user-provided
-forecasters <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/user_provided_forecasters.py>`__
+forecasters <https://cvxportfolio.readthedocs.io/en/stable/examples/user_provided_forecasters.html>`_
 how the user can define custom classes to forecast the expected returns
 and covariances. These provide callbacks that are executed at each point
 in time during the back-test. The system enforces causality and safety
 against numerical errors. We recommend to always include the default
 forecasters that we provide in any analysis you may do, since they are
 very robust and well-tested.
 
 We show in the examples on `DOW30
-components <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/dow30_example.py>`__
+components <https://cvxportfolio.readthedocs.io/en/stable/examples/dow30.html>`_
 and `wide assets-classes
-ETFs <https://github.com/cvxgrp/cvxportfolio/blob/master/examples/etfs_example.py>`__
+ETFs <https://cvxportfolio.readthedocs.io/en/stable/examples/etfs.html>`_
 how a simple sweep over hyper-parameters, taking advantage of our
 sophisticated parallel backtest machinery, quickly provides results on
 the best strategy to apply to any given selection of assets.
 
 Similar projects
 ----------------
 
@@ -212,52 +213,52 @@
 file.
 
 Development
 -----------
 
 To set up a development environment locally you should clone the
 repository (or, `fork on
-Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`__
+Github <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_
 and then clone your fork)
 
 .. code:: bash
 
    git clone https://github.com/cvxgrp/cvxportfolio.git
    cd cvxportfolio
 
 Then, you should have a look at our
-`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`__
-and possibly change the ``PYTHON`` variable to match your system’s
+`Makefile <https://www.gnu.org/software/make/manual/make.html#Introduction>`_
+and possibly change the ``PYTHON`` variable to match your system's
 python interpreter. Once you have done that,
 
 .. code:: bash
 
    make env
    make test
 
 This will replicate our `development
-environment <https://docs.python.org/3/library/venv.html>`__ and run our
+environment <https://docs.python.org/3/library/venv.html>`_ and run our
 test suite.
 
 You activate the shell environment with one of scripts in ``env/bin``
 (or ``env\Scripts`` on Windows), for example if you use bash on POSIX
 
 .. code:: bash
 
    source env/bin/activate
 
 and from the environment you can run any of the scripts in the examples
 (the cvxportfolio package is installed in `editable
-mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`__).
+mode <https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`_).
 Or, if you don't want to activate the environment, you can just run
 scripts directly using ``env/bin/python`` (or ``env\Scripts\python`` on
 Windows) like we do in the Makefile.
 
 Additionally, to match our CI/CD pipeline, you may set the following
-`git hooks <https://git-scm.com/docs/githooks>`__
+`git hooks <https://git-scm.com/docs/githooks>`_
 
 .. code:: bash
 
    echo "make lint" > .git/hooks/pre-commit
    chmod +x .git/hooks/pre-commit
    echo "make test" > .git/hooks/pre-push
    chmod +x .git/hooks/pre-push
```

### Comparing `cvxportfolio-1.3.0/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-1.3.1/cvxportfolio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 cvxportfolio/tests/test_constraints.py
 cvxportfolio/tests/test_costs.py
 cvxportfolio/tests/test_data.py
 cvxportfolio/tests/test_estimator.py
 cvxportfolio/tests/test_forecast.py
 cvxportfolio/tests/test_hyperparameters.py
 cvxportfolio/tests/test_policies.py
+cvxportfolio/tests/test_result.py
 cvxportfolio/tests/test_returns.py
 cvxportfolio/tests/test_risks.py
 cvxportfolio/tests/test_simulator.py
 cvxportfolio/tests/test_utils.py
 cvxportfolio/tests/volumes.csv
```

### Comparing `cvxportfolio-1.3.0/pyproject.toml` & `cvxportfolio-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [project]
 name = "cvxportfolio"
-version = "1.3.0"
+version = "1.3.1"
 description = "Portfolio optimization and back-testing."
 readme = "README.rst"
 license = {text = "Apache License (2.0)"}
 authors = [{name = "Enzo Busseti"}, {name = "Stephen Boyd"},
     {name = "Steven Diamond"}, {name = "BlackRock Inc."}]
 maintainers = [{name = "Enzo Busseti", email = "enzo.busseti@gmail.com"}]
 dependencies = ["pandas", "numpy", "matplotlib", "requests", "cvxpy",
-    "multiprocess"]
+    "multiprocess", # robustifies usage w/ 3rd party modules
+    "scs" # it's hardcoded as fallback solver if numerical errors
+    ]
 
 [project.optional-dependencies]
 docs = ["sphinx", "furo", "sphinx-github-style"]
 dev = ["build", "twine", "coverage", "diff_cover", "pylint", "isort",
     "autopep8", "docformatter", "beautifulsoup4"]
 examples = ['beautifulsoup4', 'lxml', 'clarabel', 'ecos']
 
@@ -28,22 +30,23 @@
 packages = ["cvxportfolio", "cvxportfolio.data", "cvxportfolio.constraints",
     "cvxportfolio.tests"]
 
 [tool.setuptools.package-data]
 "cvxportfolio.tests" = ["*.csv"]
 
 [tool.pylint.main]
-fail-under = 9.5
+fail-under = 9.75
 jobs = 0 # multiprocessing pylint
 max-line-length = 79 # PEP8 default
 load-plugins =["pylint.extensions.docparams", "pylint.extensions.docstyle"]
 
 [tool.pylint.basic]
 # These variable names are defined in the paper.
 good-names = ["t", "u", "v", "w", "h", "z", "F", "d", "Sigma"]
+disable = ['fixme'] # We are using TODOs in code comments
 
 [tool.pylint.variables]
 # These are sometimes ignored, we might instead use dataclasses for
 # sharing data between elements of a policy's DAG
 ignored-argument-names = "args|kwargs"
 
 [tool.pylint.parameter_documentation]
@@ -70,14 +73,14 @@
 [tool.diff_quality]
 # this will be superflous once we push pylint score to 10
 compare_branch = "origin/master"
 fail_under = 99
 
 [tool.autopep8]
 # these have been selected by hand, whitespaces and empty lines
-select = ["W291","W293","W391","E231","E225","E303"]
+select = ["W291","W292","W293","W391","E231","E225","E303"]
 
 [tool.docformatter]
 # tweaked to remove whitespaces and other simple fixes 
 wrap-summaries = 0
 wrap-descriptions = 0
 tab-width = 4
```

