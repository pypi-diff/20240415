# Comparing `tmp/stabilizer_timelime-0.1.1.tar.gz` & `tmp/stabilizer_timelime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.1.1.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.1.2.tar", max compression
```

## Comparing `stabilizer_timelime-0.1.1.tar` & `stabilizer_timelime-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.1/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.1/README.md
--rw-r--r--   0        0        0      774 2024-04-15 19:15:37.162338 stabilizer_timelime-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.1/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0       34 2024-04-12 21:50:28.597160 stabilizer_timelime-0.1.1/stabilizer_timelime/src/dataslurper/__init__.py
--rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.1/stabilizer_timelime/src/dataslurper/slurpdata.py
--rw-r--r--   0        0        0      384 2024-04-15 00:29:52.614447 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/__init__.py
--rw-r--r--   0        0        0     1189 2024-04-15 16:24:28.643589 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/config.py
--rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/.DS_Store
--rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/CFS.py
--rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
--rw-r--r--   0        0        0     7269 2024-04-14 16:32:21.771669 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/DE.py
--rw-r--r--   0        0        0     9869 2024-04-15 16:27:20.688465 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
--rw-r--r--   0        0        0    10625 2024-04-15 16:28:00.948752 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
--rw-r--r--   0        0        0     2524 2024-04-15 16:28:24.052367 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Stats_files.py
--rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__init__.py
--rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
--rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
--rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
--rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
--rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
--rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
--rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
--rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
--rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
--rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
--rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
--rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
--rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
--rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
--rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
--rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
--rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
--rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
--rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
--rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
--rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
--rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
--rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
--rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
--rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
--rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
--rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     3318 2024-04-15 16:25:23.301999 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
--rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/birch.py
--rw-r--r--   0        0        0    11335 2024-04-15 16:26:03.157190 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
--rw-r--r--   0        0        0     4214 2024-04-15 16:26:40.773555 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
--rw-r--r--   0        0        0     9267 2024-04-15 16:27:04.354020 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
--rw-r--r--   0        0        0     3906 2024-04-15 17:03:28.530047 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
--rw-r--r--   0        0        0     8123 2024-04-14 16:32:20.269541 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/learners.py
--rw-r--r--   0        0        0     5316 2024-04-14 16:32:21.621083 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/optimizer.py
--rw-r--r--   0        0        0    13665 2024-04-14 21:53:27.853119 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
--rw-r--r--   0        0        0     7408 2024-04-14 17:09:44.278177 stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/utils.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.2/LICENSE
+-rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.2/README.md
+-rw-r--r--   0        0        0      774 2024-04-15 19:35:38.007374 stabilizer_timelime-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.2/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-12 21:50:28.597160 stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      438 2024-04-15 19:26:58.504536 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1189 2024-04-15 16:24:28.643589 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10624 2024-04-15 19:30:51.521486 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
+-rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
+-rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
+-rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
+-rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
+-rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
+-rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
+-rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
+-rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
+-rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
+-rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
+-rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
+-rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
+-rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
+-rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
+-rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
+-rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
+-rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
+-rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
+-rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
+-rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
+-rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
+-rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
+-rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
+-rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     3268 2024-04-15 19:27:21.411760 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11349 2024-04-15 19:28:16.647125 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9281 2024-04-15 19:29:17.579849 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     3906 2024-04-15 17:03:28.530047 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13666 2024-04-15 19:31:02.203042 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
+-rw-r--r--   0        0        0     7408 2024-04-14 17:09:44.278177 stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.2/PKG-INFO
```

### Comparing `stabilizer_timelime-0.1.1/LICENSE` & `stabilizer_timelime-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/dataslurper/slurpdata.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/config.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/config.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/.DS_Store` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/CFS.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/CFS_regression.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/CFS_regression.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/DE.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/DE.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import print_function, division
 import random
 import pdb
 import time
 import traceback
-from utils import *
+from .utils import *
 
 # __author__ = 'WeiFu'
 
 class BaseSearch(object):
   def __init__(self, learner, params_distribution, train_data, tune_data,
                objective):
     self.learner = learner
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 import platform
 from os import listdir
 from os.path import isfile, join
 from glob import glob
 from pathlib import Path
 import sys
 import os
-import copy
-import traceback
+
 from pathlib import Path
 
 
-import birch_bellwether_p_CFS as birch_bell
-import birch
-import utils
+from . import birch_bellwether_p_CFS as birch_bell
+from . import birch
+from . import utils
 
 import sys
 import traceback
 import warnings
 warnings.filterwarnings("ignore")
 
 from ..config import Config
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 import os
 import copy
 import traceback
 from pathlib import Path
 
 import traceback
 import matplotlib.pyplot as plt
-import graphviz
 
-import birch
-from predictor_advance_v1 import *
-import utils
+from . import birch
+from .predictor_advance_v1 import *
+from . import utils
 
 import sys
 import traceback
 import warnings
 warnings.filterwarnings("ignore")
 
 from ..config import Config
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/Stats_files.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/Stats_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import math
 import pickle
 import sys
-import utils
+from . import utils
 
 
 from ..config import Config
 
 DEFAULT_CONFIG = Config()
 
 def create_files(path, goal,seed, month):
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/attribute_selector.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/attribute_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import pandas as pd
 import numpy as np
 
-import utils
+from . import utils
 
 import platform
 from os import listdir
 from os.path import isfile, join
 from glob import glob
 from pathlib import Path
 import sys
 import os
-import copy
-import traceback
-import timeit
-import random
 from ..config import Config
 
 DEFAULT_CONFIG = Config()
 
 def calculate_median(repo_pool, path, goal, config):
     feature_selected = []
     repos = []
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/birch.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 import traceback
 import timeit
 import random
 
 
 import matplotlib.pyplot as plt
 
-import birch
+from . import birch
 from predictor_advance_v1 import *
-import utils
+from . import utils
 import CFS_regression as CFS
 
 
 from multiprocessing import Pool, cpu_count
 from threading import Thread
 from multiprocessing import Queue
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pandas as pd
 
-import utils
+from . import utils
 
 from ..config import Config
 
 DEFAULT_CONFIG = Config()
 
 def collect_bellwether(config=DEFAULT_CONFIG):
     month = config.month
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/default_bellwether.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/default_bellwether.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 import sys
 import os
 import timeit
 
 
 import matplotlib.pyplot as plt
 
-import birch
+from . import birch
 from predictor_advance_v1 import *
-import utils
+from . import utils
 
 
 from multiprocessing import  cpu_count
 from threading import Thread
 
 # import metrices
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/init_datafiles.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/init_datafiles.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/learners.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/learners.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.cluster import KMeans
 from sklearn.naive_bayes import GaussianNB
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor
 import traceback
-from utils import *
+from .utils import *
 import pdb
 __author__ = 'Suvodeep'
 
 
 class Learners(object):
   def __init__(self, clf, train_X, train_Y, predict_X, predict_Y, goal):
     """
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/optimizer.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import random
 from sklearn.tree import DecisionTreeRegressor
 from sklearn import tree
 # import matplotlib.pyplot as plt
-from utils import *
+from .utils import *
 
 def de(fun_opt, metrics, bounds, mut=0.5, crossp=0.5, popsize=20, itrs=10):
     dimensions = len(bounds)
     pop = np.random.rand(popsize, dimensions)
     min_b, max_b = np.asarray(bounds)[:,0], np.asarray(bounds)[:,1]
     diff = np.fabs(min_b - max_b)
     print(diff)
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from utils import *
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor
 from optimizer import *
-from predictor_baseline import *
+from .predictor_baseline import *
 import pandas as pd
 
 from learners import SK_DTR, SK_RRF
 from DE import DE_Tune_ML
 import traceback
 
 from ..config import Config
```

### Comparing `stabilizer_timelime-0.1.1/stabilizer_timelime/src/stabilizer/src/utils.py` & `stabilizer_timelime-0.1.2/stabilizer_timelime/src/stabilizer/src/utils.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.1/PKG-INFO` & `stabilizer_timelime-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.1.1
+Version: 0.1.2
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

