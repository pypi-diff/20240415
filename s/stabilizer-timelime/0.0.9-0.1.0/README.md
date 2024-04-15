# Comparing `tmp/stabilizer_timelime-0.0.9.tar.gz` & `tmp/stabilizer_timelime-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.0.9.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.1.0.tar", max compression
```

## Comparing `stabilizer_timelime-0.0.9.tar` & `stabilizer_timelime-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,57 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.0.9/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.0.9/README.md
--rw-r--r--   0        0        0      648 2024-04-11 20:16:44.430968 stabilizer_timelime-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 18:41:51.440222 stabilizer_timelime-0.0.9/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0     7378 2024-04-11 20:14:15.355834 stabilizer_timelime-0.0.9/stabilizer_timelime/src/slurpdata.py
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 stabilizer_timelime-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.0/LICENSE
+-rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.0/README.md
+-rw-r--r--   0        0        0      686 2024-04-15 19:09:06.736248 stabilizer_timelime-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.0/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-12 21:50:28.597160 stabilizer_timelime-0.1.0/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.0/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      384 2024-04-15 00:29:52.614447 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1189 2024-04-15 16:24:28.643589 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7269 2024-04-14 16:32:21.771669 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9869 2024-04-15 16:27:20.688465 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10625 2024-04-15 16:28:00.948752 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2524 2024-04-15 16:28:24.052367 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
+-rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
+-rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
+-rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
+-rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
+-rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
+-rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
+-rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
+-rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
+-rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
+-rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
+-rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
+-rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
+-rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
+-rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
+-rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
+-rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
+-rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
+-rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
+-rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
+-rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
+-rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
+-rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
+-rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
+-rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
+-rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     3318 2024-04-15 16:25:23.301999 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11335 2024-04-15 16:26:03.157190 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4214 2024-04-15 16:26:40.773555 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9267 2024-04-15 16:27:04.354020 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     3906 2024-04-15 17:03:28.530047 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8123 2024-04-14 16:32:20.269541 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5316 2024-04-14 16:32:21.621083 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13665 2024-04-14 21:53:27.853119 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     7408 2024-04-14 17:09:44.278177 stabilizer_timelime-0.1.0/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.0/PKG-INFO
```

### Comparing `stabilizer_timelime-0.0.9/LICENSE` & `stabilizer_timelime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.0.9/stabilizer_timelime/src/slurpdata.py` & `stabilizer_timelime-0.1.0/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
+from pathlib import Path
 
 from datetime import timedelta
 from dateutil.relativedelta import relativedelta
-import time
 
 import github
 from github import Github
 from github import Auth
 
 import pandas as pd
 
@@ -128,14 +128,16 @@
     """
     token_ind = 0
 
     repo_list = pd.read_csv(repo_list_csv)
 
     print("Number of projects to slurp:", repo_list.shape[0])
 
+    Path(dest_folder).mkdir(parents=True, exist_ok=True)
+
     if ("organization" not in repo_list.columns) or ("repo" not in repo_list.columns):
         raise Exception("CSV missing column organization or/and repo")
 
     funcs = [get_commits, get_prs, get_issues, get_stargazers]
 
     for _, row in tqdm(repo_list.iterrows()):
```

### Comparing `stabilizer_timelime-0.0.9/PKG-INFO` & `stabilizer_timelime-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.0.9
+Version: 0.1.0
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyGithub (>=2.2.0,<3.0.0)
+Requires-Dist: freediscovery-stabilizer (==1.4.dev0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # STABILIZER + TIMELIME
```

