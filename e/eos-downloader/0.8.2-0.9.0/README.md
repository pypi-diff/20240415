# Comparing `tmp/eos_downloader-0.8.2.tar.gz` & `tmp/eos_downloader-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eos_downloader-0.8.2.tar", last modified: Tue Aug 29 08:38:08 2023, max compression
+gzip compressed data, was "eos_downloader-0.9.0.tar", last modified: Tue Oct  3 11:50:26 2023, max compression
```

## Comparing `eos_downloader-0.8.2.tar` & `eos_downloader-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (999)    11403 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)    20616 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     6147 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/
--rw-r--r--   0 runner    (1001) docker     (999)     1470 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/cli/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1882 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1697 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/debug/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/cli/get/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6063 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/get/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/cli/info/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3662 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cli/info/commands.py
--rw-r--r--   0 runner    (1001) docker     (999)     8861 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/cvp.py
--rw-r--r--   0 runner    (1001) docker     (999)     2206 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/data.py
--rw-r--r--   0 runner    (1001) docker     (999)     2627 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/download.py
--rw-r--r--   0 runner    (1001) docker     (999)     6968 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader/models/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9000 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/models/version.py
--rw-r--r--   0 runner    (1001) docker     (999)    18478 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/object_downloader.py
--rw-r--r--   0 runner    (1001) docker     (999)      288 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/eos_downloader/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/eos_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    20616 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      783 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       86 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      488 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-29 08:38:08.000000 eos_downloader-0.8.2/eos_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     4908 2023-08-29 08:37:51.000000 eos_downloader-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 08:38:08.495553 eos_downloader-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.658751 eos_downloader-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2023-10-03 11:50:26.658751 eos_downloader-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/get/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/cli/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/info/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/cvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18968 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/object_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/eos_downloader/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 11:50:26.654751 eos_downloader-0.9.0/eos_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-03 11:50:26.000000 eos_downloader-0.9.0/eos_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2023-10-03 11:50:14.000000 eos_downloader-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-03 11:50:26.658751 eos_downloader-0.9.0/setup.cfg
```

### Comparing `eos_downloader-0.8.2/LICENSE` & `eos_downloader-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.8.2/PKG-INFO` & `eos_downloader-0.9.0/eos_downloader.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eos_downloader
-Version: 0.8.2
+Name: eos-downloader
+Version: 0.9.0
 Summary: Arista EOS/CVP downloader script
 Author-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 Maintainer-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 License: Copyright (c) 2019, Arista Networks
         All rights reserved.
         
                                          Apache License
@@ -227,18 +227,59 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
-
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+Requires-Dist: cryptography
+Requires-Dist: paramiko
+Requires-Dist: requests>=2.20.0
+Requires-Dist: requests-toolbelt
+Requires-Dist: scp
+Requires-Dist: tqdm
+Requires-Dist: loguru
+Requires-Dist: rich<13.7.0,>=13.5.2
+Requires-Dist: cvprac>=1.0.7
+Requires-Dist: click~=8.1.6
+Requires-Dist: click-help-colors~=0.9
+Requires-Dist: pydantic<3.0.0,>2.0.0
+Provides-Extra: dev
+Requires-Dist: isort==5.12.0; extra == "dev"
+Requires-Dist: mypy==1.5.1; extra == "dev"
+Requires-Dist: mypy-extensions>=0.4.3; extra == "dev"
+Requires-Dist: pre-commit>=2.20.0; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest>=7.1.2; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: pytest-dependency; extra == "dev"
+Requires-Dist: pytest-html>=3.1.1; extra == "dev"
+Requires-Dist: pytest-metadata>=1.11.0; extra == "dev"
+Requires-Dist: pylint-pydantic>=0.2.4; extra == "dev"
+Requires-Dist: tox~=4.11; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-paramiko; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: typing-extensions; extra == "dev"
+Requires-Dist: yamllint; extra == "dev"
+Requires-Dist: flake8>=4.0.1; extra == "dev"
+Requires-Dist: pyflakes>=2.4.0; extra == "dev"
+Requires-Dist: bumpver>=2023.1126; extra == "dev"
+
+[![tests](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)
+![GitHub release](https://img.shields.io/github/v/release/titom73/arista-downloader)
+![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+
+<!--
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+!-->
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
@@ -251,34 +292,46 @@
 ```bash
  ardl
 Usage: ardl [OPTIONS] COMMAND [ARGS]...
 
   Arista Network Download CLI
 
 Options:
+  --version     Show the version and exit.
   --token TEXT  Arista Token from your customer account  [env var:
                 ARISTA_TOKEN]
   --help        Show this message and exit.
 
 Commands:
   debug    Debug commands to work with ardl
   get      Download Arista from Arista website
-  version  Display version of ardl
 ```
 
 > **Warning**
 > To use this CLI you need to get a valid token from your [Arista Account page](https://www.arista.com/en/users/profile).
 > For technical reason, it is only available for customers with active maintenance contracts and not for personnal accounts
 
 ### Download EOS Package
 
-
+> **Note**
 > Supported packages are: EOS, cEOS, vEOS-lab, cEOS64
 
-You can download EOS packages with following commands:
+CLI gives an option to get latest version available. By default it takes latest `F` release
+
+```bash
+ardl get eos --image-type cEOS --latest
+```
+
+If you want to get latest M release, you can use `--release-type`:
+
+```bash
+ardl get eos --image-type cEOS --release-type M --latest
+```
+
+You can download a specific EOS packages with following commands:
 
 ```bash
 # Example for a cEOS package
 $ ardl get eos --version 4.28.3M --image-type cEOS
 ```
 
 Available options are :
@@ -396,15 +449,15 @@
 requests-toolbelt
 scp
 tqdm
 ```
 
 On EVE-NG, you may have to install/upgrade __pyOpenSSL__ in version `23.0.0`:
 
-```
+```bash
 # Error when running ardl: AttributeError: module 'lib' has no attribute 'X509_V_FLAG_CB_ISSUER_CHECK'
 
 $ pip install pyopenssl --upgrade
 ```
 
 ## Docker
```

### Comparing `eos_downloader-0.8.2/README.md` & `eos_downloader-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,17 @@
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+[![tests](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)
+![GitHub release](https://img.shields.io/github/v/release/titom73/arista-downloader)
+![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+
+<!--
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+!-->
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
@@ -15,34 +24,46 @@
 ```bash
  ardl
 Usage: ardl [OPTIONS] COMMAND [ARGS]...
 
   Arista Network Download CLI
 
 Options:
+  --version     Show the version and exit.
   --token TEXT  Arista Token from your customer account  [env var:
                 ARISTA_TOKEN]
   --help        Show this message and exit.
 
 Commands:
   debug    Debug commands to work with ardl
   get      Download Arista from Arista website
-  version  Display version of ardl
 ```
 
 > **Warning**
 > To use this CLI you need to get a valid token from your [Arista Account page](https://www.arista.com/en/users/profile).
 > For technical reason, it is only available for customers with active maintenance contracts and not for personnal accounts
 
 ### Download EOS Package
 
-
+> **Note**
 > Supported packages are: EOS, cEOS, vEOS-lab, cEOS64
 
-You can download EOS packages with following commands:
+CLI gives an option to get latest version available. By default it takes latest `F` release
+
+```bash
+ardl get eos --image-type cEOS --latest
+```
+
+If you want to get latest M release, you can use `--release-type`:
+
+```bash
+ardl get eos --image-type cEOS --release-type M --latest
+```
+
+You can download a specific EOS packages with following commands:
 
 ```bash
 # Example for a cEOS package
 $ ardl get eos --version 4.28.3M --image-type cEOS
 ```
 
 Available options are :
@@ -160,15 +181,15 @@
 requests-toolbelt
 scp
 tqdm
 ```
 
 On EVE-NG, you may have to install/upgrade __pyOpenSSL__ in version `23.0.0`:
 
-```
+```bash
 # Error when running ardl: AttributeError: module 'lib' has no attribute 'X509_V_FLAG_CB_ISSUER_CHECK'
 
 $ pip install pyopenssl --upgrade
 ```
 
 ## Docker
```

### Comparing `eos_downloader-0.8.2/eos_downloader/__init__.py` & `eos_downloader-0.9.0/eos_downloader/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 #!/usr/bin/python
 # coding: utf-8 -*-
 
 """
 EOS Downloader module.
 """
 
-from __future__ import (absolute_import, division,
-                        print_function, unicode_literals, annotations)
+from __future__ import (
+    absolute_import,
+    annotations,
+    division,
+    print_function,
+    unicode_literals,
+)
+
 import dataclasses
-from typing import Any
-import json
 import importlib.metadata
+import json
+from typing import Any
 
-__author__ = '@titom73'
-__email__ = 'tom@inetsix.net'
-__date__ = '2022-03-16'
+__author__ = "@titom73"
+__email__ = "tom@inetsix.net"
+__date__ = "2022-03-16"
 __version__ = importlib.metadata.version("eos-downloader")
 
 # __all__ = ["CvpAuthenticationItem", "CvFeatureManager", "EOSDownloader", "ObjectDownloader", "reverse"]
 
 ARISTA_GET_SESSION = "https://www.arista.com/custom_data/api/cvp/getSessionCode/"
 
-ARISTA_SOFTWARE_FOLDER_TREE = "https://www.arista.com/custom_data/api/cvp/getFolderTree/"
+ARISTA_SOFTWARE_FOLDER_TREE = (
+    "https://www.arista.com/custom_data/api/cvp/getFolderTree/"
+)
 
 ARISTA_DOWNLOAD_URL = "https://www.arista.com/custom_data/api/cvp/getDownloadLink/"
 
 MSG_TOKEN_EXPIRED = """The API token has expired. Please visit arista.com, click on your profile and
 select Regenerate Token then re-run the script with the new token.
 """
 
 MSG_TOKEN_INVALID = """The API token is incorrect. Please visit arista.com, click on your profile and
 check the Access Token. Then re-run the script with the correct token.
 """
 
 MSG_INVALID_DATA = """Invalid data returned by server
 """
 
-EVE_QEMU_FOLDER_PATH = '/opt/unetlab/addons/qemu/'
+EVE_QEMU_FOLDER_PATH = "/opt/unetlab/addons/qemu/"
 
 
 class EnhancedJSONEncoder(json.JSONEncoder):
     """Custom JSon encoder."""
+
     def default(self, o: Any) -> Any:
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
         return super().default(o)
```

### Comparing `eos_downloader-0.8.2/eos_downloader/cli/cli.py` & `eos_downloader-0.9.0/eos_downloader/cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,70 +7,68 @@
 
 
 """
 ARDL CLI Baseline.
 """
 
 import click
-from rich.console import Console
-import eos_downloader
-from eos_downloader.cli.get import commands as get_commands
+
+from eos_downloader import __version__
 from eos_downloader.cli.debug import commands as debug_commands
+from eos_downloader.cli.get import commands as get_commands
 from eos_downloader.cli.info import commands as info_commands
 
+from eos_downloader.cli.utils import AliasedGroup
+
 
-@click.group()
+@click.group(cls=AliasedGroup)
+@click.version_option(__version__)
 @click.pass_context
-@click.option('--token', show_envvar=True, default=None, help='Arista Token from your customer account')
+@click.option(
+    "--token",
+    show_envvar=True,
+    default=None,
+    help="Arista Token from your customer account",
+)
 def ardl(ctx: click.Context, token: str) -> None:
     """Arista Network Download CLI"""
     ctx.ensure_object(dict)
-    ctx.obj['token'] = token
+    ctx.obj["token"] = token
 
 
-@click.command()
-def version() -> None:
-    """Display version of ardl"""
-    console = Console()
-    console.print(f'ardl is running version {eos_downloader.__version__}')
-
-
-@ardl.group(no_args_is_help=True)
+@ardl.group(cls=AliasedGroup, no_args_is_help=True)
 @click.pass_context
-def get(ctx: click.Context) -> None:
+def get(ctx: click.Context, cls: click.Group = AliasedGroup) -> None:
     # pylint: disable=redefined-builtin
     """Download Arista from Arista website"""
 
 
-@ardl.group(no_args_is_help=True)
+@ardl.group(cls=AliasedGroup, no_args_is_help=True)
 @click.pass_context
-def info(ctx: click.Context) -> None:
+def info(ctx: click.Context, cls: click.Group = AliasedGroup) -> None:
     # pylint: disable=redefined-builtin
     """List information from Arista website"""
 
 
-@ardl.group(no_args_is_help=True)
+@ardl.group(cls=AliasedGroup, no_args_is_help=True)
 @click.pass_context
-def debug(ctx: click.Context) -> None:
+def debug(ctx: click.Context, cls: click.Group = AliasedGroup) -> None:
     # pylint: disable=redefined-builtin
     """Debug commands to work with ardl"""
 
+
 # ANTA CLI Execution
 
 
 def cli() -> None:
     """Load ANTA CLI"""
     # Load group commands
     get.add_command(get_commands.eos)
     get.add_command(get_commands.cvp)
     info.add_command(info_commands.eos_versions)
     debug.add_command(debug_commands.xml)
-    ardl.add_command(version)
     # Load CLI
-    ardl(
-        obj={},
-        auto_envvar_prefix='arista'
-    )
+    ardl(obj={}, auto_envvar_prefix="arista")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `eos_downloader-0.8.2/eos_downloader/cli/debug/commands.py` & `eos_downloader-0.9.0/eos_downloader/cli/debug/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,36 +18,55 @@
 from rich.console import Console
 
 import eos_downloader.eos
 
 
 @click.command()
 @click.pass_context
-@click.option('--output', default=str('arista.xml'), help='Path to save XML file', type=click.Path(), show_default=True)
-@click.option('--log-level', '--log', help='Logging level of the command', default=None, type=click.Choice(['debug', 'info', 'warning', 'error', 'critical'], case_sensitive=False))
+@click.option(
+    "--output",
+    default=str("arista.xml"),
+    help="Path to save XML file",
+    type=click.Path(),
+    show_default=True,
+)
+@click.option(
+    "--log-level",
+    "--log",
+    help="Logging level of the command",
+    default=None,
+    type=click.Choice(
+        ["debug", "info", "warning", "error", "critical"], case_sensitive=False
+    ),
+)
 def xml(ctx: click.Context, output: str, log_level: str) -> None:
     # sourcery skip: remove-unnecessary-cast
     """Extract XML directory structure"""
     console = Console()
     # Get from Context
-    token = ctx.obj['token']
+    token = ctx.obj["token"]
 
     logger.remove()
     if log_level is not None:
         logger.add("eos-downloader.log", rotation="10 MB", level=log_level.upper())
 
     my_download = eos_downloader.eos.EOSDownloader(
-        image='unset',
-        software='EOS',
-        version='unset',
+        image="unset",
+        software="EOS",
+        version="unset",
         token=token,
-        hash_method='sha512sum')
+        hash_method="sha512sum",
+    )
 
     my_download.authenticate()
-    xml_object: ET.ElementTree = my_download._get_folder_tree()  # pylint: disable=protected-access
+    xml_object: ET.ElementTree = (
+        my_download.get_folder_tree()
+    )  # pylint: disable=protected-access
     xml_content = xml_object.getroot()
 
-    xmlstr = minidom.parseString(ET.tostring(xml_content)).toprettyxml(indent="    ", newl='')
-    with open(output, "w", encoding='utf-8') as f:
+    xmlstr = minidom.parseString(ET.tostring(xml_content)).toprettyxml(
+        indent="    ", newl=""
+    )
+    with open(output, "w", encoding="utf-8") as f:
         f.write(str(xmlstr))
 
-    console.print(f'XML file saved in: { output }')
+    console.print(f"XML file saved in: { output }")
```

### Comparing `eos_downloader-0.8.2/eos_downloader/cli/info/commands.py` & `eos_downloader-0.9.0/eos_downloader/cli/info/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,68 +20,116 @@
 
 import eos_downloader.eos
 from eos_downloader.models.version import BASE_VERSION_STR, RTYPE_FEATURE, RTYPES
 
 
 @click.command(no_args_is_help=True)
 @click.pass_context
-@click.option('--latest', '-l', is_flag=True, type=click.BOOL, default=False, help='Get latest version in given branch. If --branch is not use, get the latest branch with specific release type')
-@click.option('--release-type', '-rtype', type=click.Choice(RTYPES, case_sensitive=False), default=RTYPE_FEATURE, help='EOS release type to search')
-@click.option('--branch', '-b', type=click.STRING, default=None, help='EOS Branch to list releases')
-@click.option('--verbose', '-v', is_flag=True, type=click.BOOL, default=False, help='Human readable output. Default is none to use output in script)')
-@click.option('--log-level', '--log', help='Logging level of the command', default='warning', type=click.Choice(['debug', 'info', 'warning', 'error', 'critical'], case_sensitive=False))
-def eos_versions(ctx: click.Context, log_level: str, branch: Union[str,None] = None, release_type: str = RTYPE_FEATURE, latest: bool = False, verbose: bool = False) -> None:
+@click.option(
+    "--latest",
+    "-l",
+    is_flag=True,
+    type=click.BOOL,
+    default=False,
+    help="Get latest version in given branch. If --branch is not use, get the latest branch with specific release type",
+)
+@click.option(
+    "--release-type",
+    "-rtype",
+    type=click.Choice(RTYPES, case_sensitive=False),
+    default=RTYPE_FEATURE,
+    help="EOS release type to search",
+)
+@click.option(
+    "--branch",
+    "-b",
+    type=click.STRING,
+    default=None,
+    help="EOS Branch to list releases",
+)
+@click.option(
+    "--verbose",
+    "-v",
+    is_flag=True,
+    type=click.BOOL,
+    default=False,
+    help="Human readable output. Default is none to use output in script)",
+)
+@click.option(
+    "--log-level",
+    "--log",
+    help="Logging level of the command",
+    default="warning",
+    type=click.Choice(
+        ["debug", "info", "warning", "error", "critical"], case_sensitive=False
+    ),
+)
+def eos_versions(
+    ctx: click.Context,
+    log_level: str,
+    branch: Union[str, None] = None,
+    release_type: str = RTYPE_FEATURE,
+    latest: bool = False,
+    verbose: bool = False,
+) -> None:
     # pylint: disable = too-many-branches
     """
     List Available EOS version on Arista.com website.
 
     Comes with some filters to get latest release (F or M) as well as branch filtering
 
       - To get latest M release available (without any branch): ardl info eos-versions --latest -rtype m
 
       - To get latest F release available: ardl info eos-versions --latest -rtype F
     """
     console = Console()
     # Get from Context
-    token = ctx.obj['token']
+    token = ctx.obj["token"]
 
     logger.remove()
     if log_level is not None:
         logger.add("eos-downloader.log", rotation="10 MB", level=log_level.upper())
 
     my_download = eos_downloader.eos.EOSDownloader(
-        image='unset',
-        software='EOS',
-        version='unset',
+        image="unset",
+        software="EOS",
+        version="unset",
         token=token,
-        hash_method='sha512sum')
+        hash_method="sha512sum",
+    )
 
     auth = my_download.authenticate()
     if verbose and auth:
-        console.print('✅ Authenticated on arista.com')
+        console.print("✅ Authenticated on arista.com")
 
     if release_type is not None:
         release_type = release_type.upper()
 
     if latest:
         if branch is None:
             branch = str(my_download.latest_branch(rtype=release_type).branch)
         latest_version = my_download.latest_eos(branch, rtype=release_type)
         if str(latest_version) == BASE_VERSION_STR:
-            console.print(f'[red]Error[/red], cannot find any version in {branch} for {release_type} release type')
+            console.print(
+                f"[red]Error[/red], cannot find any version in {branch} for {release_type} release type"
+            )
             sys.exit(1)
         if verbose:
-            console.print(f'Branch {branch} has been selected with release type {release_type}')
+            console.print(
+                f"Branch {branch} has been selected with release type {release_type}"
+            )
             if branch is not None:
-                console.print(f'Latest release for {branch}: {latest_version}')
+                console.print(f"Latest release for {branch}: {latest_version}")
             else:
-                console.print(f'Latest EOS release: {latest_version}')
+                console.print(f"Latest EOS release: {latest_version}")
         else:
-            console.print(f'{ latest_version }')
+            console.print(f"{ latest_version }")
     else:
         versions = my_download.get_eos_versions(branch=branch, rtype=release_type)
         if verbose:
-            console.print(f'List of available versions for {branch if branch is not None else "all branches"}')
+            console.print(
+                f'List of available versions for {branch if branch is not None else "all branches"}'
+            )
             for version in versions:
-                console.print(f'  → {str(version)}')
+                console.print(f"  → {str(version)}")
         else:
             pprint([str(version) for version in versions])
```

### Comparing `eos_downloader-0.8.2/eos_downloader/cvp.py` & `eos_downloader-0.9.0/eos_downloader/cvp.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,60 +2,64 @@
 # coding: utf-8 -*-
 
 """
 CVP Uploader content
 """
 
 import os
-from typing import List, Optional, Any
 from dataclasses import dataclass
-from loguru import logger
+from typing import Any, List, Optional
+
 from cvprac.cvp_client import CvpClient
 from cvprac.cvp_client_errors import CvpLoginError
+from loguru import logger
 
 # from eos_downloader.tools import exc_to_str
 
 # logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CvpAuthenticationItem:
     """
-     Data structure to represent Cloudvision Authentication
+    Data structure to represent Cloudvision Authentication
     """
+
     server: str
     port: int = 443
     token: Optional[str] = None
     timeout: int = 1200
     validate_cert: bool = False
 
 
-class Filer():
+class Filer:
     # pylint: disable=too-few-public-methods
     """
     Filer Helper for file management
     """
+
     def __init__(self, path: str) -> None:
         self.file_exist = False
-        self.filename = ''
-        self.absolute_path = ''
+        self.filename = ""
+        self.absolute_path = ""
         self.relative_path = path
         if os.path.exists(path):
             self.file_exist = True
             self.filename = os.path.basename(path)
             self.absolute_path = os.path.realpath(path)
 
     def __repr__(self) -> str:
-        return self.absolute_path if self.file_exist else ''
+        return self.absolute_path if self.file_exist else ""
 
 
-class CvFeatureManager():
+class CvFeatureManager:
     """
     CvFeatureManager Object to interect with Cloudvision
     """
+
     def __init__(self, authentication: CvpAuthenticationItem) -> None:
         """
         __init__ Class Creator
 
         Parameters
         ----------
         authentication : CvpAuthenticationItem
@@ -82,41 +86,43 @@
             cvprac session to cloudvision
         """
         client = CvpClient()
         if authentication.token is not None:
             try:
                 client.connect(
                     nodes=[authentication.server],
-                    username='',
-                    password='',
+                    username="",
+                    password="",
                     api_token=authentication.token,
                     is_cvaas=True,
                     port=authentication.port,
                     cert=authentication.validate_cert,
-                    request_timeout=authentication.timeout
+                    request_timeout=authentication.timeout,
                 )
             except CvpLoginError as error_data:
-                logger.error(f'Cannot connect to Cloudvision server {authentication.server}')
-                logger.debug(f'Error message: {error_data}')
-        logger.info('connected to Cloudvision server')
-        logger.debug(f'Connection info: {authentication}')
+                logger.error(
+                    f"Cannot connect to Cloudvision server {authentication.server}"
+                )
+                logger.debug(f"Error message: {error_data}")
+        logger.info("connected to Cloudvision server")
+        logger.debug(f"Connection info: {authentication}")
         return client
 
     def __get_images(self) -> List[Any]:
         """
         __get_images Collect information about images on Cloudvision
 
         Returns
         -------
         dict
             Fact returned by Cloudvision
         """
         images = []
-        logger.debug('  -> Collecting images')
-        images = self._cv_instance.api.get_images()['data']
+        logger.debug("  -> Collecting images")
+        images = self._cv_instance.api.get_images()["data"]
         return images if self.__check_api_result(images) else []
 
     # def __get_bundles(self):
     #     """
     #     __get_bundles [Not In use] Collect information about bundles on Cloudvision
 
     #     Returns
@@ -157,15 +163,19 @@
             Name of the image to search for
 
         Returns
         -------
         bool
             True if present
         """
-        return any(image_name == image['name'] for image in self._cv_images) if isinstance(self._cv_images, list) else False
+        return (
+            any(image_name == image["name"] for image in self._cv_images)
+            if isinstance(self._cv_images, list)
+            else False
+        )
 
     def _does_bundle_exist(self, bundle_name: str) -> bool:
         # pylint: disable=unused-argument
         """
         _does_bundle_exist Check if an image is referenced in Cloudvision facts
 
         Returns
@@ -188,27 +198,31 @@
         Returns
         -------
         bool
             True if succeeds
         """
         image_item = Filer(path=image_path)
         if image_item.file_exist is False:
-            logger.error(f'File not found: {image_item.relative_path}')
+            logger.error(f"File not found: {image_item.relative_path}")
             return False
-        logger.info(f'File path for image: {image_item}')
+        logger.info(f"File path for image: {image_item}")
         if self._does_image_exist(image_name=image_item.filename):
-            logger.error("Image found in Cloudvision , Please delete it before running this script")
+            logger.error(
+                "Image found in Cloudvision , Please delete it before running this script"
+            )
             return False
         try:
-            upload_result = self._cv_instance.api.add_image(filepath=image_item.absolute_path)
+            upload_result = self._cv_instance.api.add_image(
+                filepath=image_item.absolute_path
+            )
         except Exception as e:  # pylint: disable=broad-exception-caught
-            logger.error('An error occurred during upload, check CV connection')
-            logger.error(f'Exception message is: {e}')
+            logger.error("An error occurred during upload, check CV connection")
+            logger.error(f"Exception message is: {e}")
             return False
-        logger.debug(f'Upload Result is : {upload_result}')
+        logger.debug(f"Upload Result is : {upload_result}")
         return True
 
     def build_image_list(self, image_list: List[str]) -> List[Any]:
         """
         Builds a list of the image data structures, for a given list of image names.
         Parameters
         ----------
@@ -248,29 +262,34 @@
             List of images available on Cloudvision
 
         Returns
         -------
         bool
             True if succeeds
         """
-        logger.debug(f'Init creation of an image bundle {name} with following images {images_name}')
+        logger.debug(
+            f"Init creation of an image bundle {name} with following images {images_name}"
+        )
         all_images_present: List[bool] = []
         self._cv_images = self.__get_images()
         all_images_present.extend(
-            self._does_image_exist(image_name=image_name)
-            for image_name in images_name
+            self._does_image_exist(image_name=image_name) for image_name in images_name
         )
         # Bundle Create
         if self._does_bundle_exist(bundle_name=name) is False:
-            logger.debug(f'Creating image bundle {name} with following images {images_name}')
+            logger.debug(
+                f"Creating image bundle {name} with following images {images_name}"
+            )
             images_data = self.build_image_list(image_list=images_name)
             if images_data is not None:
-                logger.debug('Images information: {images_data}')
+                logger.debug("Images information: {images_data}")
                 try:
-                    data = self._cv_instance.api.save_image_bundle(name=name, images=images_data)
+                    data = self._cv_instance.api.save_image_bundle(
+                        name=name, images=images_data
+                    )
                 except Exception as e:  # pylint: disable=broad-exception-caught
-                    logger.critical(f'{e}')
+                    logger.critical(f"{e}")
                 else:
                     logger.debug(data)
                 return True
-            logger.critical('No data found for images')
+            logger.critical("No data found for images")
         return False
```

### Comparing `eos_downloader-0.8.2/eos_downloader/download.py` & `eos_downloader-0.9.0/eos_downloader/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,62 +4,73 @@
 
 """download module"""
 
 import os.path
 import signal
 from concurrent.futures import ThreadPoolExecutor
 from threading import Event
-from typing import Iterable, Any
+from typing import Any, Iterable
 
 import requests
 import rich
 from rich import console
-from rich.progress import (BarColumn, DownloadColumn, Progress, TaskID,
-                           TextColumn, TimeElapsedColumn, TransferSpeedColumn)
+from rich.progress import (
+    BarColumn,
+    DownloadColumn,
+    Progress,
+    TaskID,
+    TextColumn,
+    TimeElapsedColumn,
+    TransferSpeedColumn,
+)
 
 console = rich.get_console()
 done_event = Event()
 
 
 def handle_sigint(signum: Any, frame: Any) -> None:
     """Progress bar handler"""
     done_event.set()
 
 
 signal.signal(signal.SIGINT, handle_sigint)
 
 
-class DownloadProgressBar():
+class DownloadProgressBar:
     """
     Object to manage Download process with Progress Bar from Rich
     """
 
     def __init__(self) -> None:
         """
         Class Constructor
         """
         self.progress = Progress(
-            TextColumn("💾  Downloading [bold blue]{task.fields[filename]}", justify="right"),
+            TextColumn(
+                "💾  Downloading [bold blue]{task.fields[filename]}", justify="right"
+            ),
             BarColumn(bar_width=None),
             "[progress.percentage]{task.percentage:>3.1f}%",
             "•",
             TransferSpeedColumn(),
             "•",
             DownloadColumn(),
             "•",
             TimeElapsedColumn(),
             "•",
-            console=console
+            console=console,
         )
 
-    def _copy_url(self, task_id: TaskID, url: str, path: str, block_size: int = 1024) -> bool:
+    def _copy_url(
+        self, task_id: TaskID, url: str, path: str, block_size: int = 1024
+    ) -> bool:
         """Copy data from a url to a local file."""
         response = requests.get(url, stream=True, timeout=5)
         # This will break if the response doesn't contain content length
-        self.progress.update(task_id, total=int(response.headers['Content-Length']))
+        self.progress.update(task_id, total=int(response.headers["Content-Length"]))
         with open(path, "wb") as dest_file:
             self.progress.start_task(task_id)
             for data in response.iter_content(chunk_size=block_size):
                 dest_file.write(data)
                 self.progress.update(task_id, advance=len(data))
                 if done_event.is_set():
                     return True
@@ -67,11 +78,13 @@
         return False
 
     def download(self, urls: Iterable[str], dest_dir: str) -> None:
         """Download multuple files to the given directory."""
         with self.progress:
             with ThreadPoolExecutor(max_workers=4) as pool:
                 for url in urls:
-                    filename = url.split("/")[-1].split('?')[0]
+                    filename = url.split("/")[-1].split("?")[0]
                     dest_path = os.path.join(dest_dir, filename)
-                    task_id = self.progress.add_task("download", filename=filename, start=False)
+                    task_id = self.progress.add_task(
+                        "download", filename=filename, start=False
+                    )
                     pool.submit(self._copy_url, task_id, url, dest_path)
```

### Comparing `eos_downloader-0.8.2/eos_downloader/eos.py` & `eos_downloader-0.9.0/eos_downloader/eos.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,28 @@
 import xml.etree.ElementTree as ET
 from typing import List, Union
 
 import rich
 from loguru import logger
 from rich import console
 
-from eos_downloader.models.version import BASE_BRANCH_STR, BASE_VERSION_STR, REGEX_EOS_VERSION, RTYPE_FEATURE, EosVersion
+from eos_downloader.models.version import (
+    BASE_BRANCH_STR,
+    BASE_VERSION_STR,
+    REGEX_EOS_VERSION,
+    RTYPE_FEATURE,
+    EosVersion,
+)
 from eos_downloader.object_downloader import ObjectDownloader
 
 # logger = logging.getLogger(__name__)
 
 console = rich.get_console()
 
+
 class EOSDownloader(ObjectDownloader):
     """
     EOSDownloader Object to download EOS images from Arista.com website
 
     Supercharge ObjectDownloader to support EOS specific actions
 
     Parameters
@@ -43,74 +50,83 @@
         Create a file in the EOS image to disable ZTP process during initial boot
 
         Parameters
         ----------
         file_path : str
             Path where EOS image is located
         """
-        logger.info('Mounting volume to disable ZTP')
-        console.print('🚀 Mounting volume to disable ZTP')
+        logger.info("Mounting volume to disable ZTP")
+        console.print("🚀 Mounting volume to disable ZTP")
         raw_folder = os.path.join(file_path, "raw")
         os.system(f"rm -rf {raw_folder}")
         os.system(f"mkdir -p {raw_folder}")
         os.system(
-            f'guestmount -a {os.path.join(file_path, "hda.qcow2")} -m /dev/sda2 {os.path.join(file_path, "raw")}')
-        ztp_file = os.path.join(file_path, 'raw/zerotouch-config')
-        with open(ztp_file, 'w', encoding='ascii') as zfile:
-            zfile.write('DISABLE=True')
-        logger.info(f'Unmounting volume in {file_path}')
+            f'guestmount -a {os.path.join(file_path, "hda.qcow2")} -m /dev/sda2 {os.path.join(file_path, "raw")}'
+        )
+        ztp_file = os.path.join(file_path, "raw/zerotouch-config")
+        with open(ztp_file, "w", encoding="ascii") as zfile:
+            zfile.write("DISABLE=True")
+        logger.info(f"Unmounting volume in {file_path}")
         os.system(f"guestunmount {os.path.join(file_path, 'raw')}")
         os.system(f"rm -rf {os.path.join(file_path, 'raw')}")
         logger.info(f"Volume has been successfully unmounted at {file_path}")
 
-    def _parse_xml_for_version(self,root_xml: ET.ElementTree, xpath: str = './/dir[@label="Active Releases"]/dir/dir/[@label]') -> List[EosVersion]:
+    def _parse_xml_for_version(
+        self,
+        root_xml: ET.ElementTree,
+        xpath: str = './/dir[@label="Active Releases"]/dir/dir/[@label]',
+    ) -> List[EosVersion]:
         """
         Extract list of available EOS versions from Arista.com website
 
         Create a list of EosVersion object for all versions available on Arista.com
 
         Args:
             root_xml (ET.ElementTree): XML file with all versions available
             xpath (str, optional): XPATH to use to extract EOS version. Defaults to './/dir[@label="Active Releases"]/dir/dir/[@label]'.
 
         Returns:
             List[EosVersion]: List of EosVersion representing all available EOS versions
         """
         # XPATH: .//dir[@label="Active Releases"]/dir/dir/[@label]
         if self.eos_versions is None:
-            logger.debug(f'Using xpath {xpath}')
+            logger.debug(f"Using xpath {xpath}")
             eos_versions = []
             for node in root_xml.findall(xpath):
-                if 'label' in node.attrib and node.get('label') is not None:
-                    label = node.get('label')
+                if "label" in node.attrib and node.get("label") is not None:
+                    label = node.get("label")
                     if label is not None and REGEX_EOS_VERSION.match(label):
                         eos_version = EosVersion.from_str(label)
                         eos_versions.append(eos_version)
                         logger.debug(f"Found {label} - {eos_version}")
-            logger.debug(f'List of versions found on arista.com is: {eos_versions}')
+            logger.debug(f"List of versions found on arista.com is: {eos_versions}")
             self.eos_versions = eos_versions
         else:
-            logger.debug('receiving instruction to download versions, but already available')
+            logger.debug(
+                "receiving instruction to download versions, but already available"
+            )
         return self.eos_versions
 
     def _get_branches(self, with_rtype: str = RTYPE_FEATURE) -> List[str]:
         """
         Extract all EOS branches available from arista.com
 
         Call self._parse_xml_for_version and then build list of available branches
 
         Args:
             rtype (str, optional): Release type to find. Can be M or F, default to F
 
         Returns:
             List[str]: A lsit of string that represent all availables EOS branches
         """
-        root = self._get_folder_tree()
+        root = self.get_folder_tree()
         versions = self._parse_xml_for_version(root_xml=root)
-        return list({version.branch for version in versions if version.rtype == with_rtype})
+        return list(
+            {version.branch for version in versions if version.rtype == with_rtype}
+        )
 
     def latest_branch(self, rtype: str = RTYPE_FEATURE) -> EosVersion:
         """
         Get latest branch from semver standpoint
 
         Args:
             rtype (str, optional): Release type to find. Can be M or F, default to F
@@ -121,38 +137,46 @@
         selected_branch = EosVersion.from_str(BASE_BRANCH_STR)
         for branch in self._get_branches(with_rtype=rtype):
             branch = EosVersion.from_str(branch)
             if branch > selected_branch:
                 selected_branch = branch
         return selected_branch
 
-    def get_eos_versions(self, branch: Union[str,None] = None, rtype: Union[str,None] = None) -> List[EosVersion]:
+    def get_eos_versions(
+        self, branch: Union[str, None] = None, rtype: Union[str, None] = None
+    ) -> List[EosVersion]:
         """
         Get a list of available EOS version available on arista.com
 
         If a branch is provided, only version in this branch are listed.
         Otherwise, all versions are provided.
 
         Args:
             branch (str, optional): An EOS branch to filter. Defaults to None.
             rtype (str, optional): Release type to find. Can be M or F, default to F
 
         Returns:
             List[EosVersion]: A list of versions available
         """
-        root = self._get_folder_tree()
+        root = self.get_folder_tree()
         result = []
         for version in self._parse_xml_for_version(root_xml=root):
             if branch is None and (version.rtype == rtype or rtype is None):
                 result.append(version)
-            elif branch is not None and version.is_in_branch(branch) and version.rtype == rtype:
+            elif (
+                branch is not None
+                and version.is_in_branch(branch)
+                and version.rtype == rtype
+            ):
                 result.append(version)
         return result
 
-    def latest_eos(self, branch: Union[str,None] = None, rtype: str = RTYPE_FEATURE) -> EosVersion:
+    def latest_eos(
+        self, branch: Union[str, None] = None, rtype: str = RTYPE_FEATURE
+    ) -> EosVersion:
         """
         Get latest version of EOS
 
         If a branch is provided, only version in this branch are listed.
         Otherwise, all versions are provided.
         You can select what type of version to consider: M or F
 
@@ -164,14 +188,16 @@
             EosVersion: latest version selected
         """
         selected_version = EosVersion.from_str(BASE_VERSION_STR)
         if branch is None:
             latest_branch = self.latest_branch(rtype=rtype)
         else:
             latest_branch = EosVersion.from_str(branch)
-        for version in self.get_eos_versions(branch=str(latest_branch.branch), rtype=rtype):
+        for version in self.get_eos_versions(
+            branch=str(latest_branch.branch), rtype=rtype
+        ):
             if version > selected_version:
                 if rtype is not None and version.rtype == rtype:
                     selected_version = version
                 if rtype is None:
                     selected_version = version
         return selected_version
```

### Comparing `eos_downloader-0.8.2/eos_downloader/models/version.py` & `eos_downloader-0.9.0/eos_downloader/models/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,33 @@
 from loguru import logger
 from pydantic import BaseModel
 
 from eos_downloader.tools import exc_to_str
 
 # logger = logging.getLogger(__name__)
 
-BASE_VERSION_STR = '4.0.0F'
-BASE_BRANCH_STR = '4.0'
+BASE_VERSION_STR = "4.0.0F"
+BASE_BRANCH_STR = "4.0"
 
-RTYPE_FEATURE = 'F'
-RTYPE_MAINTENANCE = 'M'
+RTYPE_FEATURE = "F"
+RTYPE_MAINTENANCE = "M"
 RTYPES = [RTYPE_FEATURE, RTYPE_MAINTENANCE]
 
 # Regular Expression to capture multiple EOS version format
 # 4.24
 # 4.23.0
 # 4.21.1M
 # 4.28.10.F
 # 4.28.6.1M
-REGEX_EOS_VERSION = re.compile(r"^.*(?P<major>4)\.(?P<minor>\d{1,2})\.(?P<patch>\d{1,2})(?P<other>\.\d*)*(?P<rtype>[M,F])*$")
-REGEX_EOS_BRANCH = re.compile(r"^.*(?P<major>4)\.(?P<minor>\d{1,2})(\.?P<patch>\d)*(\.\d)*(?P<rtype>[M,F])*$")
+REGEX_EOS_VERSION = re.compile(
+    r"^.*(?P<major>4)\.(?P<minor>\d{1,2})\.(?P<patch>\d{1,2})(?P<other>\.\d*)*(?P<rtype>[M,F])*$"
+)
+REGEX_EOS_BRANCH = re.compile(
+    r"^.*(?P<major>4)\.(?P<minor>\d{1,2})(\.?P<patch>\d)*(\.\d)*(?P<rtype>[M,F])*$"
+)
 
 
 class EosVersion(BaseModel):
     """
     EosVersion object to play with version management in code
 
     Since EOS is not using strictly semver approach, this class mimic some functions from semver lib for Arista EOS versions
@@ -55,18 +59,19 @@
 
     >>> print(f'Is eos_version in branch 4.23: {eos_version.is_in_branch("4.23.0")}')
     Is eos_version in branch 4.23: True
 
     Args:
         BaseModel (Pydantic): Pydantic Base Model
     """
+
     major: int = 4
     minor: int = 0
     patch: int = 0
-    rtype: Optional[str] = 'F'
+    rtype: Optional[str] = "F"
     other: Any = None
 
     @classmethod
     def from_str(cls, eos_version: str) -> EosVersion:
         """
         Class constructor from a string representing EOS version
 
@@ -80,50 +85,50 @@
 
         Args:
             eos_version (str): EOS version in str format
 
         Returns:
             EosVersion object
         """
-        logger.debug(f'receiving version: {eos_version}')
+        logger.debug(f"receiving version: {eos_version}")
         if REGEX_EOS_VERSION.match(eos_version):
             matches = REGEX_EOS_VERSION.match(eos_version)
             # assert matches is not None
             assert matches is not None
             return cls(**matches.groupdict())
         if REGEX_EOS_BRANCH.match(eos_version):
             matches = REGEX_EOS_BRANCH.match(eos_version)
             # assert matches is not None
             assert matches is not None
             return cls(**matches.groupdict())
-        logger.error(f'Error occured with {eos_version}')
+        logger.error(f"Error occured with {eos_version}")
         return EosVersion()
 
     @property
     def branch(self) -> str:
         """
         Extract branch of version
 
         Returns:
             str: branch from version
         """
-        return f'{self.major}.{self.minor}'
+        return f"{self.major}.{self.minor}"
 
     def __str__(self) -> str:
         """
         Standard str representation
 
         Return string for EOS version like 4.23.3M
 
         Returns:
             str: A standard EOS version string representing <MAJOR>.<MINOR>.<PATCH><RTYPE>
         """
         if self.other is None:
-            return f'{self.major}.{self.minor}.{self.patch}{self.rtype}'
-        return f'{self.major}.{self.minor}.{self.patch}{self.other}{self.rtype}'
+            return f"{self.major}.{self.minor}.{self.patch}{self.rtype}"
+        return f"{self.major}.{self.minor}.{self.patch}{self.other}{self.rtype}"
 
     def _compare(self, other: EosVersion) -> float:
         """
         An internal comparison function to compare 2 EosVersion objects
 
         Do a deep comparison from Major to Release Type
         The return value is
@@ -137,66 +142,76 @@
         Raises:
             ValueError: Raise ValueError if input is incorrect type
 
         Returns:
             float: -1 if ver1 < ver2, 0 if ver1 == ver2, 1 if ver1 > ver2
         """
         if not isinstance(other, EosVersion):
-            raise ValueError(f'could not compare {other} as it is not an EosVersion object')
+            raise ValueError(
+                f"could not compare {other} as it is not an EosVersion object"
+            )
         comparison_flag: float = 0
-        logger.warning(f'current version {self.__str__()} - other {str(other)}')   # pylint: disable = unnecessary-dunder-call
+        logger.warning(
+            f"current version {self.__str__()} - other {str(other)}"  # pylint: disable = unnecessary-dunder-call
+        )
         for key, _ in self.dict().items():
-            if comparison_flag == 0 and self.dict()[key] is None or other.dict()[key] is None:
-                logger.debug(f'{key}: local None - remote None')
-                logger.debug(f'{key}: local {self.dict()} - remote {other.dict()}')
+            if (
+                comparison_flag == 0
+                and self.dict()[key] is None
+                or other.dict()[key] is None
+            ):
+                logger.debug(f"{key}: local None - remote None")
+                logger.debug(f"{key}: local {self.dict()} - remote {other.dict()}")
                 return comparison_flag
-            logger.debug(f'{key}: local {self.dict()[key]} - remote {other.dict()[key]}')
+            logger.debug(
+                f"{key}: local {self.dict()[key]} - remote {other.dict()[key]}"
+            )
             if comparison_flag == 0 and self.dict()[key] < other.dict()[key]:
                 comparison_flag = -1
             if comparison_flag == 0 and self.dict()[key] > other.dict()[key]:
                 comparison_flag = 1
             if comparison_flag != 0:
-                logger.info(f'comparison result is {comparison_flag}')
+                logger.info(f"comparison result is {comparison_flag}")
                 return comparison_flag
-        logger.info(f'comparison result is {comparison_flag}')
+        logger.info(f"comparison result is {comparison_flag}")
         return comparison_flag
 
     @typing.no_type_check
     def __eq__(self, other):
-        """ Implement __eq__ function (==) """
+        """Implement __eq__ function (==)"""
         return self._compare(other) == 0
 
     @typing.no_type_check
     def __ne__(self, other):
         # type: ignore
-        """ Implement __nw__ function (!=) """
+        """Implement __nw__ function (!=)"""
         return self._compare(other) != 0
 
     @typing.no_type_check
     def __lt__(self, other):
         # type: ignore
-        """ Implement __lt__ function (<) """
+        """Implement __lt__ function (<)"""
         return self._compare(other) < 0
 
     @typing.no_type_check
     def __le__(self, other):
         # type: ignore
-        """ Implement __le__ function (<=) """
+        """Implement __le__ function (<=)"""
         return self._compare(other) <= 0
 
     @typing.no_type_check
     def __gt__(self, other):
         # type: ignore
-        """ Implement __gt__ function (>) """
+        """Implement __gt__ function (>)"""
         return self._compare(other) > 0
 
     @typing.no_type_check
     def __ge__(self, other):
         # type: ignore
-        """ Implement __ge__ function (>=) """
+        """Implement __ge__ function (>=)"""
         return self._compare(other) >= 0
 
     def match(self, match_expr: str) -> bool:
         """
         Compare self to match a match expression.
 
         Example:
@@ -232,15 +247,15 @@
         else:
             raise ValueError(
                 "match_expr parameter should be in format <op><ver>, "
                 "where <op> is one of "
                 "['<', '>', '==', '<=', '>=', '!=']. "
                 f"You provided: {match_expr}"
             )
-        logger.debug(f'work on comparison {prefix} with base release {match_version}')
+        logger.debug(f"work on comparison {prefix} with base release {match_version}")
         possibilities_dict = {
             ">": (1,),
             "<": (-1,),
             "==": (0,),
             "!=": (-1, 1),
             ">=": (0, 1),
             "<=": (-1, 0),
@@ -259,14 +274,14 @@
         Args:
             branch_str (str): a string for EOS branch. It supports following formats 4.23 or 4.23.0
 
         Returns:
             bool: True if current version is in provided branch, otherwise False
         """
         try:
-            logger.debug(f'reading branch str:{branch_str}')
+            logger.debug(f"reading branch str:{branch_str}")
             branch = EosVersion.from_str(branch_str)
         except Exception as error:  # pylint: disable = broad-exception-caught
             logger.error(exc_to_str(error))
         else:
             return self.major == branch.major and self.minor == branch.minor
         return False
```

### Comparing `eos_downloader-0.8.2/eos_downloader/object_downloader.py` & `eos_downloader-0.9.0/eos_downloader/object_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-arguments
 
 """
 eos_downloader class definition
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals, annotations)
+from __future__ import (
+    absolute_import,
+    annotations,
+    division,
+    print_function,
+    unicode_literals,
+)
 
 import base64
 import glob
 import hashlib
 import json
 import os
 import sys
@@ -22,30 +27,43 @@
 
 import requests
 import rich
 from loguru import logger
 from rich import console
 from tqdm import tqdm
 
-from eos_downloader import (ARISTA_DOWNLOAD_URL, ARISTA_GET_SESSION,
-                            ARISTA_SOFTWARE_FOLDER_TREE, EVE_QEMU_FOLDER_PATH,
-                            MSG_INVALID_DATA, MSG_TOKEN_EXPIRED)
+from eos_downloader import (
+    ARISTA_DOWNLOAD_URL,
+    ARISTA_GET_SESSION,
+    ARISTA_SOFTWARE_FOLDER_TREE,
+    EVE_QEMU_FOLDER_PATH,
+    MSG_INVALID_DATA,
+    MSG_TOKEN_EXPIRED,
+)
 from eos_downloader.data import DATA_MAPPING
 from eos_downloader.download import DownloadProgressBar
 
 # logger = logging.getLogger(__name__)
 
 console = rich.get_console()
 
 
-class ObjectDownloader():
+class ObjectDownloader:
     """
     ObjectDownloader Generic Object to download from Arista.com
     """
-    def __init__(self, image: str, version: str, token: str, software: str = 'EOS', hash_method: str = 'md5sum'):
+
+    def __init__(
+        self,
+        image: str,
+        version: str,
+        token: str,
+        software: str = "EOS",
+        hash_method: str = "md5sum",
+    ):
         """
         __init__ Class constructor
 
         generic class constructor
 
         Parameters
         ----------
@@ -66,18 +84,18 @@
         self.token = token
         self.folder_level = 0
         self.session_id = None
         self.filename = self._build_filename()
         self.hash_method = hash_method
         self.timeout = 5
         # Logging
-        logger.debug(f'Filename built by _build_filename is {self.filename}')
+        logger.debug(f"Filename built by _build_filename is {self.filename}")
 
     def __str__(self) -> str:
-        return f'{self.software} - {self.image} - {self.version}'
+        return f"{self.software} - {self.image} - {self.version}"
 
     # def __repr__(self):
     #     return str(self.__dict__)
 
     @property
     def version(self) -> str:
         """Get version."""
@@ -98,24 +116,26 @@
         _build_filename Helper to build filename to search on arista.com
 
         Returns
         -------
         str:
             Filename to search for on Arista.com
         """
-        logger.info('start build')
+        logger.info("start build")
         if self.software in DATA_MAPPING:
-            logger.info(f'software in data mapping: {self.software}')
+            logger.info(f"software in data mapping: {self.software}")
             if self.image in DATA_MAPPING[self.software]:
-                logger.info(f'image in data mapping: {self.image}')
+                logger.info(f"image in data mapping: {self.image}")
                 return f"{DATA_MAPPING[self.software][self.image]['prepend']}-{self.version}{DATA_MAPPING[self.software][self.image]['extension']}"
             return f"{DATA_MAPPING[self.software]['default']['prepend']}-{self.version}{DATA_MAPPING[self.software]['default']['extension']}"
-        raise ValueError(f'Incorrect value for software {self.software}')
+        raise ValueError(f"Incorrect value for software {self.software}")
 
-    def _parse_xml_for_path(self, root_xml: ET.ElementTree, xpath: str, search_file: str) -> str:
+    def _parse_xml_for_path(
+        self, root_xml: ET.ElementTree, xpath: str, search_file: str
+    ) -> str:
         # sourcery skip: remove-unnecessary-cast
         """
         _parse_xml Read and extract data from XML using XPATH
 
         Get all interested nodes using XPATH and then get node that match search_file
 
         Parameters
@@ -128,26 +148,26 @@
             Filename to search for
 
         Returns
         -------
         str
             File Path on Arista server side
         """
-        logger.debug(f'Using xpath {xpath}')
-        logger.debug(f'Search for file {search_file}')
-        console.print(f'🔎  Searching file {search_file}')
+        logger.debug(f"Using xpath {xpath}")
+        logger.debug(f"Search for file {search_file}")
+        console.print(f"🔎  Searching file {search_file}")
         for node in root_xml.findall(xpath):
             # logger.debug('Found {}', node.text)
             if str(node.text).lower() == search_file.lower():
-                path = node.get('path')
-                console.print(f'    -> Found file at {path}')
+                path = node.get("path")
+                console.print(f"    -> Found file at {path}")
                 logger.info(f'Found {node.text} at {node.get("path")}')
-                return str(node.get('path')) if node.get('path') is not None else ''
-        logger.error(f'Requested file ({self.filename}) not found !')
-        return ''
+                return str(node.get("path")) if node.get("path") is not None else ""
+        logger.error(f"Requested file ({self.filename}) not found !")
+        return ""
 
     def _get_hash(self, file_path: str) -> str:
         """
         _get_hash Download HASH file from Arista server
 
         Parameters
         ----------
@@ -161,18 +181,18 @@
         """
         remote_hash_file = self._get_remote_hashpath(hash_method=self.hash_method)
         hash_url = self._get_url(remote_file_path=remote_hash_file)
         # hash_downloaded = self._download_file_raw(url=hash_url, file_path=file_path + "/" + os.path.basename(remote_hash_file))
         dl_rich_progress_bar = DownloadProgressBar()
         dl_rich_progress_bar.download(urls=[hash_url], dest_dir=file_path)
         hash_downloaded = f"{file_path}/{os.path.basename(remote_hash_file)}"
-        hash_content = 'unset'
-        with open(hash_downloaded, 'r', encoding='utf-8') as f:
+        hash_content = "unset"
+        with open(hash_downloaded, "r", encoding="utf-8") as f:
             hash_content = f.read()
-        return hash_content.split(' ')[0]
+        return hash_content.split(" ")[0]
 
     @staticmethod
     def _compute_hash_md5sum(file: str, hash_expected: str) -> bool:
         """
         _compute_hash_md5sum Compare MD5 sum
 
         Do comparison between local md5 of the file and value provided by arista.com
@@ -191,15 +211,17 @@
         """
         hash_md5 = hashlib.md5()
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
         if hash_md5.hexdigest() == hash_expected:
             return True
-        logger.warning(f'Downloaded file is corrupt: local md5 ({hash_md5.hexdigest()}) is different to md5 from arista ({hash_expected})')
+        logger.warning(
+            f"Downloaded file is corrupt: local md5 ({hash_md5.hexdigest()}) is different to md5 from arista ({hash_expected})"
+        )
         return False
 
     @staticmethod
     def _compute_hash_sh512sum(file: str, hash_expected: str) -> bool:
         """
         _compute_hash_sh512sum Compare SHA512 sum
 
@@ -219,76 +241,82 @@
         """
         hash_sha512 = hashlib.sha512()
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_sha512.update(chunk)
         if hash_sha512.hexdigest() == hash_expected:
             return True
-        logger.warning(f'Downloaded file is corrupt: local sha512 ({hash_sha512.hexdigest()}) is different to sha512 from arista ({hash_expected})')
+        logger.warning(
+            f"Downloaded file is corrupt: local sha512 ({hash_sha512.hexdigest()}) is different to sha512 from arista ({hash_expected})"
+        )
         return False
 
-    def _get_folder_tree(self) -> ET.ElementTree:
+    def get_folder_tree(self) -> ET.ElementTree:
         """
         _get_folder_tree Download XML tree from Arista server
 
         Returns
         -------
         ET.ElementTree
             XML document
         """
         if self.session_id is None:
             self.authenticate()
-        jsonpost = {'sessionCode': self.session_id}
-        result = requests.post(ARISTA_SOFTWARE_FOLDER_TREE, data=json.dumps(jsonpost), timeout=self.timeout)
+        jsonpost = {"sessionCode": self.session_id}
+        result = requests.post(
+            ARISTA_SOFTWARE_FOLDER_TREE, data=json.dumps(jsonpost), timeout=self.timeout
+        )
         try:
             folder_tree = result.json()["data"]["xml"]
             return ET.ElementTree(ET.fromstring(folder_tree))
         except KeyError as error:
             logger.error(MSG_INVALID_DATA)
-            logger.error(f'Server returned: {error}')
-            console.print(f'❌  {MSG_INVALID_DATA}', style="bold red")
+            logger.error(f"Server returned: {error}")
+            console.print(f"❌  {MSG_INVALID_DATA}", style="bold red")
             sys.exit(1)
 
     def _get_remote_filepath(self) -> str:
         """
         _get_remote_filepath Helper to get path of the file to download
 
         Set XPATH and return result of _parse_xml for the file to download
 
         Returns
         -------
         str
             Remote path of the file to download
         """
-        root = self._get_folder_tree()
+        root = self.get_folder_tree()
         logger.debug("GET XML content from ARISTA.com")
         xpath = f'.//dir[@label="{self.software}"]//file'
-        return self._parse_xml_for_path(root_xml=root, xpath=xpath, search_file=self.filename)
+        return self._parse_xml_for_path(
+            root_xml=root, xpath=xpath, search_file=self.filename
+        )
 
-    def _get_remote_hashpath(self, hash_method: str = 'md5sum') -> str:
+    def _get_remote_hashpath(self, hash_method: str = "md5sum") -> str:
         """
         _get_remote_hashpath Helper to get path of the hash's file to download
 
         Set XPATH and return result of _parse_xml for the file to download
 
         Returns
         -------
         str
             Remote path of the hash's file to download
         """
-        root = self._get_folder_tree()
+        root = self.get_folder_tree()
         logger.debug("GET XML content from ARISTA.com")
         xpath = f'.//dir[@label="{self.software}"]//file'
         return self._parse_xml_for_path(
             root_xml=root,
             xpath=xpath,
-            search_file=f'{self.filename}.{hash_method}',
+            search_file=f"{self.filename}.{hash_method}",
         )
 
-    def _get_url(self, remote_file_path: str) ->  str:
+    def _get_url(self, remote_file_path: str) -> str:
         """
         _get_url Get URL to use for downloading file from Arista server
 
         Send remote_file_path to get correct URL to use for download
 
         Parameters
         ----------
@@ -298,21 +326,23 @@
         Returns
         -------
         str
             URL link to use for download
         """
         if self.session_id is None:
             self.authenticate()
-        jsonpost = {'sessionCode': self.session_id, 'filePath': remote_file_path}
-        result = requests.post(ARISTA_DOWNLOAD_URL, data=json.dumps(jsonpost), timeout=self.timeout)
-        if 'data' in result.json() and 'url' in result.json()['data']:
+        jsonpost = {"sessionCode": self.session_id, "filePath": remote_file_path}
+        result = requests.post(
+            ARISTA_DOWNLOAD_URL, data=json.dumps(jsonpost), timeout=self.timeout
+        )
+        if "data" in result.json() and "url" in result.json()["data"]:
             # logger.debug('URL to download file is: {}', result.json())
             return result.json()["data"]["url"]
-        logger.critical(f'Server returns following message: {result.json()}')
-        return ''
+        logger.critical(f"Server returns following message: {result.json()}")
+        return ""
 
     @staticmethod
     def _download_file_raw(url: str, file_path: str) -> str:
         """
         _download_file Helper to download file from Arista.com
 
         [extended_summary]
@@ -327,39 +357,48 @@
         Returns
         -------
         str
             File path
         """
         chunkSize = 1024
         r = requests.get(url, stream=True, timeout=5)
-        with open(file_path, 'wb') as f:
-            pbar = tqdm(unit="B", total=int(r.headers['Content-Length']), unit_scale=True, unit_divisor=1024)
+        with open(file_path, "wb") as f:
+            pbar = tqdm(
+                unit="B",
+                total=int(r.headers["Content-Length"]),
+                unit_scale=True,
+                unit_divisor=1024,
+            )
             for chunk in r.iter_content(chunk_size=chunkSize):
                 if chunk:
                     pbar.update(len(chunk))
                 f.write(chunk)
         return file_path
 
-    def _download_file(self, file_path: str, filename: str, rich_interface: bool = True) -> Union[None, str]:
+    def _download_file(
+        self, file_path: str, filename: str, rich_interface: bool = True
+    ) -> Union[None, str]:
         remote_file_path = self._get_remote_filepath()
-        logger.info(f'File found on arista server: {remote_file_path}')
+        logger.info(f"File found on arista server: {remote_file_path}")
         file_url = self._get_url(remote_file_path=remote_file_path)
         if file_url is not False:
             if not rich_interface:
-                return self._download_file_raw(url=file_url, file_path=os.path.join(file_path, filename))
+                return self._download_file_raw(
+                    url=file_url, file_path=os.path.join(file_path, filename)
+                )
             rich_downloader = DownloadProgressBar()
             rich_downloader.download(urls=[file_url], dest_dir=file_path)
             return os.path.join(file_path, filename)
-        logger.error(f'Cannot download file {file_path}')
+        logger.error(f"Cannot download file {file_path}")
         return None
 
     @staticmethod
     def _create_destination_folder(path: str) -> None:
         # os.makedirs(path, mode, exist_ok=True)
-        os.system(f'mkdir -p {path}')
+        os.system(f"mkdir -p {path}")
 
     @staticmethod
     def _disable_ztp(file_path: str) -> None:
         pass
 
     # ------------------------------------------------------------------------ #
     # Public METHODS
@@ -375,32 +414,37 @@
         Returns
         -------
         bool
             True if authentication succeeds=, False in all other situations.
         """
         credentials = (base64.b64encode(self.token.encode())).decode("utf-8")
         session_code_url = ARISTA_GET_SESSION
-        jsonpost = {'accessToken': credentials}
+        jsonpost = {"accessToken": credentials}
 
-        result = requests.post(session_code_url, data=json.dumps(jsonpost), timeout=self.timeout)
+        result = requests.post(
+            session_code_url, data=json.dumps(jsonpost), timeout=self.timeout
+        )
 
-        if result.json()["status"]["message"] in[ 'Access token expired',  'Invalid access token']:
-            console.print(f'❌  {MSG_TOKEN_EXPIRED}', style="bold red")
+        if result.json()["status"]["message"] in [
+            "Access token expired",
+            "Invalid access token",
+        ]:
+            console.print(f"❌  {MSG_TOKEN_EXPIRED}", style="bold red")
             logger.error(MSG_TOKEN_EXPIRED)
             return False
 
         try:
-            if 'data' in result.json():
+            if "data" in result.json():
                 self.session_id = result.json()["data"]["session_code"]
-                logger.info('Authenticated on arista.com')
+                logger.info("Authenticated on arista.com")
                 return True
-            logger.debug(f'{result.json()}')
+            logger.debug(f"{result.json()}")
             return False
         except KeyError as error_arista:
-            logger.error(f'Error: {error_arista}')
+            logger.error(f"Error: {error_arista}")
             sys.exit(1)
 
     def download_local(self, file_path: str, checksum: bool = False) -> bool:
         # sourcery skip: move-assign
         """
         download_local Entrypoint for local download feature
 
@@ -418,33 +462,41 @@
             Execute checksum or not, by default False
 
         Returns
         -------
         bool
             True if everything went well, False if any problem appears
         """
-        file_downloaded = str(self._download_file(file_path=file_path, filename=self.filename))
+        file_downloaded = str(
+            self._download_file(file_path=file_path, filename=self.filename)
+        )
 
         # Check file HASH
         hash_result = False
         if checksum:
-            logger.info('🚀  Running checksum validation')
-            console.print('🚀  Running checksum validation')
-            if self.hash_method == 'md5sum':
+            logger.info("🚀  Running checksum validation")
+            console.print("🚀  Running checksum validation")
+            if self.hash_method == "md5sum":
                 hash_expected = self._get_hash(file_path=file_path)
-                hash_result = self._compute_hash_md5sum(file=file_downloaded, hash_expected=hash_expected)
-            elif self.hash_method == 'sha512sum':
+                hash_result = self._compute_hash_md5sum(
+                    file=file_downloaded, hash_expected=hash_expected
+                )
+            elif self.hash_method == "sha512sum":
                 hash_expected = self._get_hash(file_path=file_path)
-                hash_result = self._compute_hash_sh512sum(file=file_downloaded, hash_expected=hash_expected)
+                hash_result = self._compute_hash_sh512sum(
+                    file=file_downloaded, hash_expected=hash_expected
+                )
         if not hash_result:
-            logger.error('Downloaded file is corrupted, please check your connection')
-            console.print('❌  Downloaded file is corrupted, please check your connection')
+            logger.error("Downloaded file is corrupted, please check your connection")
+            console.print(
+                "❌  Downloaded file is corrupted, please check your connection"
+            )
             return False
-        logger.info('Downloaded file is correct.')
-        console.print('✅  Downloaded file is correct.')
+        logger.info("Downloaded file is correct.")
+        console.print("✅  Downloaded file is correct.")
         return True
 
     def provision_eve(self, noztp: bool = False, checksum: bool = True) -> None:
         # pylint: disable=unused-argument
         """
         provision_eve Entrypoint for EVE-NG download and provisioning
 
@@ -462,52 +514,55 @@
             Flag to deactivate ZTP in EOS image, by default False
         checksum : bool, optional
             Flag to ask for hash validation, by default True
         """
         # Build image name to use in folder path
         eos_image_name = self.filename.rstrip(".vmdk").lower()
         if noztp:
-            eos_image_name = f'{eos_image_name}-noztp'
+            eos_image_name = f"{eos_image_name}-noztp"
         # Create full path for EVE-NG
         file_path = os.path.join(EVE_QEMU_FOLDER_PATH, eos_image_name.rstrip())
         # Create folders in filesystem
         self._create_destination_folder(path=file_path)
 
         # Download file to local destination
         file_downloaded = self._download_file(
-            file_path=file_path, filename=self.filename)
+            file_path=file_path, filename=self.filename
+        )
 
         # Convert to QCOW2 format
         file_qcow2 = os.path.join(file_path, "hda.qcow2")
-        logger.info('Converting VMDK to QCOW2 format')
-        console.print('🚀  Converting VMDK to QCOW2 format...')
+        logger.info("Converting VMDK to QCOW2 format")
+        console.print("🚀  Converting VMDK to QCOW2 format...")
 
-        os.system(f'$(which qemu-img) convert -f vmdk -O qcow2 {file_downloaded} {file_qcow2}')
+        os.system(
+            f"$(which qemu-img) convert -f vmdk -O qcow2 {file_downloaded} {file_qcow2}"
+        )
 
-        logger.info('Applying unl_wrapper to fix permissions')
-        console.print('Applying unl_wrapper to fix permissions')
+        logger.info("Applying unl_wrapper to fix permissions")
+        console.print("Applying unl_wrapper to fix permissions")
 
-        os.system('/opt/unetlab/wrappers/unl_wrapper -a fixpermissions')
-        os.system(f'rm -f {file_downloaded}')
+        os.system("/opt/unetlab/wrappers/unl_wrapper -a fixpermissions")
+        os.system(f"rm -f {file_downloaded}")
 
         if noztp:
             self._disable_ztp(file_path=file_path)
 
     def docker_import(self, image_name: str = "arista/ceos") -> None:
         """
         Import docker container to your docker server.
 
         Import downloaded container to your local docker engine.
 
         Args:
             version (str):
             image_name (str, optional): Image name to use. Defaults to "arista/ceos".
         """
-        docker_image = f'{image_name}:{self.version}'
-        logger.info(f'Importing image {self.filename} to {docker_image}')
-        console.print(f'🚀 Importing image {self.filename} to {docker_image}')
-        os.system(f'$(which docker) import {self.filename} {docker_image}')
-        for filename in glob.glob(f'{self.filename}*'):
+        docker_image = f"{image_name}:{self.version}"
+        logger.info(f"Importing image {self.filename} to {docker_image}")
+        console.print(f"🚀 Importing image {self.filename} to {docker_image}")
+        os.system(f"$(which docker) import {self.filename} {docker_image}")
+        for filename in glob.glob(f"{self.filename}*"):
             try:
                 os.remove(filename)
             except FileNotFoundError:
-                console.print(f'File not found: {filename}')
+                console.print(f"File not found: {filename}")
```

### Comparing `eos_downloader-0.8.2/eos_downloader.egg-info/PKG-INFO` & `eos_downloader-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eos-downloader
-Version: 0.8.2
+Name: eos_downloader
+Version: 0.9.0
 Summary: Arista EOS/CVP downloader script
 Author-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 Maintainer-email: Thomas Grimonet <thomas.grimonet@gmail.com>
 License: Copyright (c) 2019, Arista Networks
         All rights reserved.
         
                                          Apache License
@@ -227,18 +227,59 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
-
- [![code-testing](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/titom73/arista-downloader) ![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+Requires-Dist: cryptography
+Requires-Dist: paramiko
+Requires-Dist: requests>=2.20.0
+Requires-Dist: requests-toolbelt
+Requires-Dist: scp
+Requires-Dist: tqdm
+Requires-Dist: loguru
+Requires-Dist: rich<13.7.0,>=13.5.2
+Requires-Dist: cvprac>=1.0.7
+Requires-Dist: click~=8.1.6
+Requires-Dist: click-help-colors~=0.9
+Requires-Dist: pydantic<3.0.0,>2.0.0
+Provides-Extra: dev
+Requires-Dist: isort==5.12.0; extra == "dev"
+Requires-Dist: mypy==1.5.1; extra == "dev"
+Requires-Dist: mypy-extensions>=0.4.3; extra == "dev"
+Requires-Dist: pre-commit>=2.20.0; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest>=7.1.2; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: pytest-dependency; extra == "dev"
+Requires-Dist: pytest-html>=3.1.1; extra == "dev"
+Requires-Dist: pytest-metadata>=1.11.0; extra == "dev"
+Requires-Dist: pylint-pydantic>=0.2.4; extra == "dev"
+Requires-Dist: tox~=4.11; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-paramiko; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: typing-extensions; extra == "dev"
+Requires-Dist: yamllint; extra == "dev"
+Requires-Dist: flake8>=4.0.1; extra == "dev"
+Requires-Dist: pyflakes>=2.4.0; extra == "dev"
+Requires-Dist: bumpver>=2023.1126; extra == "dev"
+
+[![tests](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml/badge.svg?event=push)](https://github.com/titom73/eos-downloader/actions/workflows/pr-management.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eos-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)
+![GitHub release](https://img.shields.io/github/v/release/titom73/arista-downloader)
+![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+
+<!--
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+!-->
 
 # Arista Software Downloader
 
 Script to download Arista softwares to local folder, Cloudvision or EVE-NG.
 
 ```bash
 pip install eos-downloader
@@ -251,34 +292,46 @@
 ```bash
  ardl
 Usage: ardl [OPTIONS] COMMAND [ARGS]...
 
   Arista Network Download CLI
 
 Options:
+  --version     Show the version and exit.
   --token TEXT  Arista Token from your customer account  [env var:
                 ARISTA_TOKEN]
   --help        Show this message and exit.
 
 Commands:
   debug    Debug commands to work with ardl
   get      Download Arista from Arista website
-  version  Display version of ardl
 ```
 
 > **Warning**
 > To use this CLI you need to get a valid token from your [Arista Account page](https://www.arista.com/en/users/profile).
 > For technical reason, it is only available for customers with active maintenance contracts and not for personnal accounts
 
 ### Download EOS Package
 
-
+> **Note**
 > Supported packages are: EOS, cEOS, vEOS-lab, cEOS64
 
-You can download EOS packages with following commands:
+CLI gives an option to get latest version available. By default it takes latest `F` release
+
+```bash
+ardl get eos --image-type cEOS --latest
+```
+
+If you want to get latest M release, you can use `--release-type`:
+
+```bash
+ardl get eos --image-type cEOS --release-type M --latest
+```
+
+You can download a specific EOS packages with following commands:
 
 ```bash
 # Example for a cEOS package
 $ ardl get eos --version 4.28.3M --image-type cEOS
 ```
 
 Available options are :
@@ -396,15 +449,15 @@
 requests-toolbelt
 scp
 tqdm
 ```
 
 On EVE-NG, you may have to install/upgrade __pyOpenSSL__ in version `23.0.0`:
 
-```
+```bash
 # Error when running ardl: AttributeError: module 'lib' has no attribute 'X509_V_FLAG_CB_ISSUER_CHECK'
 
 $ pip install pyopenssl --upgrade
 ```
 
 ## Docker
```

### Comparing `eos_downloader-0.8.2/eos_downloader.egg-info/SOURCES.txt` & `eos_downloader-0.9.0/eos_downloader.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 eos_downloader.egg-info/SOURCES.txt
 eos_downloader.egg-info/dependency_links.txt
 eos_downloader.egg-info/entry_points.txt
 eos_downloader.egg-info/requires.txt
 eos_downloader.egg-info/top_level.txt
 eos_downloader/cli/__init__.py
 eos_downloader/cli/cli.py
+eos_downloader/cli/utils.py
 eos_downloader/cli/debug/__init__.py
 eos_downloader/cli/debug/commands.py
 eos_downloader/cli/get/__init__.py
 eos_downloader/cli/get/commands.py
 eos_downloader/cli/info/__init__.py
 eos_downloader/cli/info/commands.py
 eos_downloader/models/__init__.py
```

### Comparing `eos_downloader-0.8.2/pyproject.toml` & `eos_downloader-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eos_downloader"
-version = "v0.8.2"
+version = "v0.9.0"
 readme = "README.md"
 authors = [{ name = "Thomas Grimonet", email = "thomas.grimonet@gmail.com" }]
 maintainers = [
   { name = "Thomas Grimonet", email = "thomas.grimonet@gmail.com" },
 ]
 description = "Arista EOS/CVP downloader script"
 license = { file = "LICENSE" }
@@ -18,15 +18,15 @@
   "cryptography",
   "paramiko",
   "requests>=2.20.0",
   "requests-toolbelt",
   "scp",
   "tqdm",
   "loguru",
-  "rich~=13.5.2",
+  "rich>=13.5.2,<13.7.0",
   "cvprac>=1.0.7",
   "click~=8.1.6",
   "click-help-colors~=0.9",
   "pydantic>2.0.0,<3.0.0",
 ]
 keywords = ["eos_downloader", "Arista", "eos", "cvp", "network", "automation", "networking", "devops", "netdevops"]
 classifiers = [
@@ -58,15 +58,15 @@
   "pylint",
   "pytest>=7.1.2",
   "pytest-cov>=2.11.1",
   "pytest-dependency",
   "pytest-html>=3.1.1",
   "pytest-metadata>=1.11.0",
   "pylint-pydantic>=0.2.4",
-  "tox==4.10.0",
+  "tox~=4.11",
   "types-PyYAML",
   "types-paramiko",
   "types-requests",
   "typing-extensions",
   "yamllint",
   "flake8>=4.0.1",
   "pyflakes>=2.4.0",
@@ -90,15 +90,15 @@
 include = ["eos_downloader*"]
 namespaces = false
 
 ################################
 # Version
 ################################
 [tool.bumpver]
-current_version = "0.8.2"
+current_version = "0.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump: Version {old_version} -> {new_version}"
 commit = true
 # No tag
 tag = false
 push = false
```

