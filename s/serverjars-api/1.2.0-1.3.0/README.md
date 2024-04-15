# Comparing `tmp/serverjars-api-1.2.0.tar.gz` & `tmp/serverjars-api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverjars-api-1.2.0.tar", last modified: Sun Aug 27 23:54:15 2023, max compression
+gzip compressed data, was "serverjars-api-1.3.0.tar", last modified: Mon Apr 15 03:49:40 2024, max compression
```

## Comparing `serverjars-api-1.2.0.tar` & `serverjars-api-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-27 23:54:15.976698 serverjars-api-1.2.0/
--rw-rw-rw-   0        0        0     2109 2023-08-27 23:54:15.977699 serverjars-api-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-07-04 21:38:28.000000 serverjars-api-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-27 23:54:15.958733 serverjars-api-1.2.0/serverjars/
--rw-rw-rw-   0        0        0    10137 2023-08-27 23:41:34.000000 serverjars-api-1.2.0/serverjars/__init__.py
--rw-rw-rw-   0        0        0      580 2023-04-20 19:20:46.000000 serverjars-api-1.2.0/serverjars/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-27 23:54:15.976698 serverjars-api-1.2.0/serverjars_api.egg-info/
--rw-rw-rw-   0        0        0     2109 2023-08-27 23:54:15.000000 serverjars-api-1.2.0/serverjars_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-08-27 23:54:15.000000 serverjars-api-1.2.0/serverjars_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-27 23:54:15.000000 serverjars-api-1.2.0/serverjars_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-27 23:54:15.000000 serverjars-api-1.2.0/serverjars_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-27 23:54:15.000000 serverjars-api-1.2.0/serverjars_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-08-27 23:54:15.977699 serverjars-api-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-08-27 21:44:35.000000 serverjars-api-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:49:40.682987 serverjars-api-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 03:49:33.000000 serverjars-api-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 03:49:40.682987 serverjars-api-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-15 03:49:33.000000 serverjars-api-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:49:40.682987 serverjars-api-1.3.0/serverjars/
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-15 03:49:33.000000 serverjars-api-1.3.0/serverjars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-15 03:49:33.000000 serverjars-api-1.3.0/serverjars/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:49:40.682987 serverjars-api-1.3.0/serverjars_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 03:49:40.000000 serverjars-api-1.3.0/serverjars_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 03:49:40.682987 serverjars-api-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:49:33.000000 serverjars-api-1.3.0/setup.py
```

### Comparing `serverjars-api-1.2.0/PKG-INFO` & `serverjars-api-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,54 @@
-Metadata-Version: 2.1
-Name: serverjars-api
-Version: 1.2.0
-Summary: The unofficial Python wrapper for serverjars.com
-Home-page: https://github.com/legopitstop/serverjars-python-api-wrapper
-Author: Legopitstop
-Author-email: officiallegopitstop@gmail.com
-License: MIT
-Keywords: ServerJars,Minecraft,Servers,Bedrock,API
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# serverjars-api
-
-[![PyPI](https://img.shields.io/pypi/v/serverjars-api)](https://pypi.org/project/serverjars-api/)
-[![Python](https://img.shields.io/pypi/pyversions/serverjars-api)](https://www.python.org/downloads//)
-![Downloads](https://img.shields.io/pypi/dm/serverjars-api)
-![Status](https://img.shields.io/pypi/status/serverjars-api)
-[![Issues](https://img.shields.io/github/issues/legopitstop/serverjars-python-api-wrapper)](https://github.com/legopitstop/serverjars-python-api-wrapper/issues)
-
-The unofficial Python wrapper for [serverjars.com](https://serverjars.com/)
-
-## Installation
-Install the module with pip:
-```bat
-pip3 install serverjars-api
-```
-Update existing installation: `pip3 install serverjars-api --upgrade`
-
-## Code Examples:
-Fetching the latest jar:
-```python
-import serverjars
-latest = serverjars.fetchLatest('vanilla')
-print(latest)
-```
-
-Fetching all the Jars:
-```python
-import serverjars
-allJars = serverjars.fetchAll('paper')
-print(allJars)
-```
-
-Fetching types:
-```python
-import serverjars
-types = serverjars.fetchTypes()
-print(types)
-```
-
-Fetching subtypes:
-```python
-import serverjars
-subtypes = serverjars.fetchTypes('bedrock')
-print(subtypes)
-```
-
-Downloading Jars:
-```python
-import serverjars
-
-def on_finish(jar):
-    print('Downloaded', jar)
-
-serverjars.downloadJar('snapshot', finishcommand=on_finish)
-```
+# serverjars-api
+
+[![PyPI](https://img.shields.io/pypi/v/serverjars-api)](https://pypi.org/project/serverjars-api/)
+[![Python](https://img.shields.io/pypi/pyversions/serverjars-api)](https://www.python.org/downloads//)
+![Downloads](https://img.shields.io/pypi/dm/serverjars-api)
+![Status](https://img.shields.io/pypi/status/serverjars-api)
+[![Issues](https://img.shields.io/github/issues/legopitstop/serverjars-python-api-wrapper)](https://github.com/legopitstop/serverjars-python-api-wrapper/issues)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+The unofficial Python wrapper for [serverjars.com](https://serverjars.com/)
+
+## Installation
+Install the module with pip:
+```bat
+pip3 install serverjars-api
+```
+Update existing installation: `pip3 install serverjars-api --upgrade`
+
+## Code Examples:
+Fetching the latest jar:
+```python
+import serverjars
+latest = serverjars.fetch_latest('vanilla', 'vanilla')
+print(latest)
+```
+
+Fetching all the Jars:
+```python
+import serverjars
+allJars = serverjars.fetch_all('vanilla', 'snapshot')
+print(allJars)
+```
+
+Fetching types:
+```python
+import serverjars
+subtypes = serverjars.fetch_types('modded')
+print(subtypes)
+```
+
+Downloading Jars:
+```python
+import serverjars
+
+serverjars.download_jar('vanilla', "vanilla")
+```
+
+Create and run a Minecraft server
+```python
+import serverjars
+
+app = serverjars.App.create('vanilla', "vanilla", fp="svr/server.jar")
+app.run()
+```
```

