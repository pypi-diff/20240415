# Comparing `tmp/PythonProjectBootstrapperTest2-0.1.8-py3-none-any.whl.zip` & `tmp/PythonProjectBootstrapperTest2-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7624 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3611 b- defN 24-Mar-09 16:26 BuildBinary.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Mar-09 16:26 PythonProjectBootstrapperTest2/EntryPoint.py
--rw-r--r--  2.0 unx      876 b- defN 24-Mar-09 16:26 PythonProjectBootstrapperTest2/Math.py
--rw-r--r--  2.0 unx      639 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2/__init__.py
--rw-r--r--  2.0 unx     1132 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5813 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       97 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      987 b- defN 24-Mar-09 16:27 PythonProjectBootstrapperTest2-0.1.8.dist-info/RECORD
-10 files, 15881 bytes uncompressed, 5884 bytes compressed:  62.9%
+Zip file size: 7868 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3611 b- defN 24-Mar-11 16:38 BuildBinary.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Mar-11 16:38 PythonProjectBootstrapperTest2/EntryPoint.py
+-rw-r--r--  2.0 unx      876 b- defN 24-Mar-11 16:38 PythonProjectBootstrapperTest2/Math.py
+-rw-r--r--  2.0 unx      639 b- defN 24-Mar-11 16:39 PythonProjectBootstrapperTest2/__init__.py
+-rw-r--r--  2.0 unx     1132 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6490 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       97 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       43 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 24-Mar-11 16:40 PythonProjectBootstrapperTest2-0.1.9.dist-info/RECORD
+10 files, 16558 bytes uncompressed, 6128 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: PythonProjectBootstrapperTest2/Math.py
 Comment: 
 
 Filename: PythonProjectBootstrapperTest2/__init__.py
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/LICENSE.txt
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/METADATA
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/WHEEL
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/entry_points.txt
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/top_level.txt
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTest2-0.1.8.dist-info/RECORD
+Filename: PythonProjectBootstrapperTest2-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PythonProjectBootstrapperTest2/__init__.py

```diff
@@ -5,10 +5,10 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 from .Math import Add, Sub, Mult, Div
```

## Comparing `PythonProjectBootstrapperTest2-0.1.8.dist-info/LICENSE.txt` & `PythonProjectBootstrapperTest2-0.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PythonProjectBootstrapperTest2-0.1.8.dist-info/METADATA` & `PythonProjectBootstrapperTest2-0.1.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonProjectBootstrapperTest2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Testing output produced by PythonProjectBootstrapper
 Author-email: Scientific Software Engineering Center at Georgia Tech <sse-center@gatech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/gt-sse-center/PythonProjectBootstrapperTest2
 Project-URL: Documentation, https://github.com/gt-sse-center/PythonProjectBootstrapperTest2
 Project-URL: Repository, https://github.com/gt-sse-center/PythonProjectBootstrapperTest2
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Requires-Dist: build ==1.* ; extra == 'package'
 Requires-Dist: cx-Freeze ==6.* ; extra == 'package'
 Requires-Dist: twine ==4.* ; extra == 'package'
 
 # PythonProjectBootstrapperTest2
 
 [![CI](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions/workflows/standard.yaml/badge.svg?event=push)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions/workflows/standard.yaml)
-[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/gt-sse-center/2f9d770d13e3a148424f374f74d41f4b/raw/PythonProjectBootstrapperTest2_coverage.json)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions)
+[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/davidbrownell/2f9d770d13e3a148424f374f74d41f4b/raw/PythonProjectBootstrapperTest2_coverage.json)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions)
 [![License](https://img.shields.io/github/license/gt-sse-center/PythonProjectBootstrapperTest2?color=dark-green)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/blob/master/LICENSE.txt)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/gt-sse-center/PythonProjectBootstrapperTest2?color=dark-green)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/commits/main/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PythonProjectBootstrapperTest2?color=dark-green)](https://pypi.org/project/pythonprojectbootstrappertest2/)
 [![PyPI - Version](https://img.shields.io/pypi/v/PythonProjectBootstrapperTest2?color=dark-green)](https://pypi.org/project/pythonprojectbootstrappertest2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/PythonProjectBootstrapperTest2)](https://pypistats.org/packages/pythonprojectbootstrappertest2)
 
 # PythonProjectBootstrapperTest2
@@ -42,20 +42,31 @@
 
 TODO: Complete this section
 
 ### How to use PythonProjectBootstrapperTest2
 
 TODO: Complete this section
 
+## Installation via Executable
+
+Download an executable for Linux, MacOS, or Windows to use the functionality provided by this repository without a dependency on [Python](https://www.python.org).
+
+1. Download the archive for the latest release [here](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/releases/latest); the files will begin with `exe.` and contain the name of your operating system.
+2. Decompress the archive
+
 ## Installation via pip
 
+Install the PythonProjectBootstrapperTest2 package via [pip](https://pip.pypa.io/en/stable/) (Package Installer for Python) to use it with your python code.
+
 `pip install PythonProjectBootstrapperTest2`
 
 ## Local Development
 
+Follow these steps to prepare the repository for local development activities.
+
 1) Clone this repository
 2) Bootstrap the local repository by running...
     | Operating System | Command |
     | --- | --- |
     | Linux / MacOS | <p>Standard:<br/>`Bootstrap.sh`</p><p>Standard + packaging:<br/>`Bootstrap.sh --package`</p> |
     | Windows | <p>Standard:<br/>`Bootstrap.cmd`</p><p>Standard + packaging:<br/>`Bootstrap.cmd --package`</p> |
 3) Activate the development environment by running...
```

## Comparing `PythonProjectBootstrapperTest2-0.1.8.dist-info/RECORD` & `PythonProjectBootstrapperTest2-0.1.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BuildBinary.py,sha256=LQ5ysNxjBS-G9MqHEIIq8KjUWLxnNHOEwxVoW7AzAPQ,3611
 PythonProjectBootstrapperTest2/EntryPoint.py,sha256=KZaBzltbSTB1rV9y3tg-EUI5q3fhJcD9evH5-1NewJQ,2591
 PythonProjectBootstrapperTest2/Math.py,sha256=wznhaBVUBEB9EZb7gi33SPY4_HvlVEoK3VqmgU4nwXc,876
-PythonProjectBootstrapperTest2/__init__.py,sha256=2ZyIXPvJhfII-qau6OzoGbOVXn_21ukmja9A363DlKY,639
-PythonProjectBootstrapperTest2-0.1.8.dist-info/LICENSE.txt,sha256=zc7f3T2QcYWfeQLzALc_PNFXPegKkIYxfFvfCGOtVFg,1132
-PythonProjectBootstrapperTest2-0.1.8.dist-info/METADATA,sha256=W-xxXzbHnqP2vqKpo_-QpHQ6eGKROkRcJZihGDI3cK4,5813
-PythonProjectBootstrapperTest2-0.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-PythonProjectBootstrapperTest2-0.1.8.dist-info/entry_points.txt,sha256=eRZTiO8Isf61ctnbDDGIovRrglvLCrJo6Hu6g5Ppv0Y,97
-PythonProjectBootstrapperTest2-0.1.8.dist-info/top_level.txt,sha256=1yWj2bp-XgrFlCkjQSo3J-sXBW2uHM0vzBUPd46xl1M,43
-PythonProjectBootstrapperTest2-0.1.8.dist-info/RECORD,,
+PythonProjectBootstrapperTest2/__init__.py,sha256=uFMeSnyU9ofL6v_L2M-v0uZlR1TkbheVSZUpX2izx1Q,639
+PythonProjectBootstrapperTest2-0.1.9.dist-info/LICENSE.txt,sha256=zc7f3T2QcYWfeQLzALc_PNFXPegKkIYxfFvfCGOtVFg,1132
+PythonProjectBootstrapperTest2-0.1.9.dist-info/METADATA,sha256=FSVlbjCI9oLEj9ZXssRo3tCdogxK-CtH-9s4qaOzFks,6490
+PythonProjectBootstrapperTest2-0.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+PythonProjectBootstrapperTest2-0.1.9.dist-info/entry_points.txt,sha256=eRZTiO8Isf61ctnbDDGIovRrglvLCrJo6Hu6g5Ppv0Y,97
+PythonProjectBootstrapperTest2-0.1.9.dist-info/top_level.txt,sha256=1yWj2bp-XgrFlCkjQSo3J-sXBW2uHM0vzBUPd46xl1M,43
+PythonProjectBootstrapperTest2-0.1.9.dist-info/RECORD,,
```

