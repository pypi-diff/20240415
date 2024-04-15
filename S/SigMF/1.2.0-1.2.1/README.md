# Comparing `tmp/SigMF-1.2.0.tar.gz` & `tmp/sigmf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SigMF-1.2.0.tar", last modified: Wed Feb 14 18:44:09 2024, max compression
+gzip compressed data, was "sigmf-1.2.1.tar", last modified: Mon Apr 15 17:09:47 2024, max compression
```

## Comparing `SigMF-1.2.0.tar` & `sigmf-1.2.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.690226 SigMF-1.2.0/
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.686226 SigMF-1.2.0/.github/
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.686226 SigMF-1.2.0/.github/workflows/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      609 2024-02-14 18:37:28.000000 SigMF-1.2.0/.github/workflows/main.yml
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      160 2024-02-14 18:37:28.000000 SigMF-1.2.0/.gitignore
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7652 2023-03-13 23:50:08.000000 SigMF-1.2.0/COPYING-LGPL
--rw-r--r--   0 kal29868  (1000) kal29868  (1000)     9394 2024-02-14 18:44:09.690226 SigMF-1.2.0/PKG-INFO
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     8209 2024-02-14 18:37:28.000000 SigMF-1.2.0/README.md
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.690226 SigMF-1.2.0/SigMF.egg-info/
--rw-r--r--   0 kal29868  (1000) kal29868  (1000)     9394 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/PKG-INFO
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      684 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/SOURCES.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        1 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/dependency_links.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      149 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/entry_points.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       93 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/requires.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        6 2024-02-14 18:44:09.000000 SigMF-1.2.0/SigMF.egg-info/top_level.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     2902 2024-02-14 18:37:28.000000 SigMF-1.2.0/pyproject.toml
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       38 2024-02-14 18:44:09.690226 SigMF-1.2.0/setup.cfg
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.690226 SigMF-1.2.0/sigmf/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      460 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/__init__.py
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.690226 SigMF-1.2.0/sigmf/apps/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/apps/__init__.py
--rwxrwxr-x   0 kal29868  (1000) kal29868  (1000)     2474 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/apps/convert_wav.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    27983 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/apps/gui.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     5118 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/archive.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3424 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/archivereader.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      694 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/error.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     9076 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/schema-collection.json
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    16539 2024-01-24 15:36:05.000000 SigMF-1.2.0/sigmf/schema-meta.json
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      708 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/schema.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      876 2023-03-13 23:50:08.000000 SigMF-1.2.0/sigmf/sigmf_hash.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    40202 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/sigmffile.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3289 2023-12-20 00:15:00.000000 SigMF-1.2.0/sigmf/utils.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3829 2024-02-14 18:37:28.000000 SigMF-1.2.0/sigmf/validate.py
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:44:09.690226 SigMF-1.2.0/tests/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        0 2023-03-13 23:50:08.000000 SigMF-1.2.0/tests/__init__.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     1829 2023-09-01 15:40:17.000000 SigMF-1.2.0/tests/conftest.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     5258 2023-03-13 23:50:08.000000 SigMF-1.2.0/tests/test_archive.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     2832 2023-10-25 16:39:14.000000 SigMF-1.2.0/tests/test_archivereader.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    14615 2024-01-24 15:36:05.000000 SigMF-1.2.0/tests/test_sigmffile.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3797 2024-01-24 15:36:05.000000 SigMF-1.2.0/tests/test_validation.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     4130 2023-10-25 16:39:14.000000 SigMF-1.2.0/tests/testdata.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.185892 sigmf-1.2.1/
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.177891 sigmf-1.2.1/.github/
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.181892 sigmf-1.2.1/.github/workflows/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      609 2024-02-14 18:37:28.000000 sigmf-1.2.1/.github/workflows/main.yml
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      160 2024-02-14 18:37:28.000000 sigmf-1.2.1/.gitignore
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7652 2023-03-13 23:50:08.000000 sigmf-1.2.1/COPYING-LGPL
+-rw-r--r--   0 kal29868  (1000) kal29868  (1000)     9483 2024-04-15 17:09:47.185892 sigmf-1.2.1/PKG-INFO
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     8199 2024-04-15 17:01:56.000000 sigmf-1.2.1/README.md
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.181892 sigmf-1.2.1/SigMF.egg-info/
+-rw-r--r--   0 kal29868  (1000) kal29868  (1000)     9483 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/PKG-INFO
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      704 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/SOURCES.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        1 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/dependency_links.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      149 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/entry_points.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       93 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/requires.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        6 2024-04-15 17:09:47.000000 sigmf-1.2.1/SigMF.egg-info/top_level.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     2994 2024-04-15 17:01:56.000000 sigmf-1.2.1/pyproject.toml
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       38 2024-04-15 17:09:47.185892 sigmf-1.2.1/setup.cfg
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.181892 sigmf-1.2.1/sigmf/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      573 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/__init__.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.181892 sigmf-1.2.1/sigmf/apps/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        0 2024-02-14 18:37:28.000000 sigmf-1.2.1/sigmf/apps/__init__.py
+-rwxrwxr-x   0 kal29868  (1000) kal29868  (1000)     2963 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/apps/convert_wav.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    28019 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/apps/gui.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     5124 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/archive.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3395 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/archivereader.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      701 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/error.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     9073 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/schema-collection.json
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    16536 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/schema-meta.json
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      715 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/schema.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      883 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/sigmf_hash.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    40170 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/sigmffile.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3590 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/utils.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3780 2024-04-15 17:01:56.000000 sigmf-1.2.1/sigmf/validate.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2024-04-15 17:09:47.181892 sigmf-1.2.1/tests/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        0 2023-03-13 23:50:08.000000 sigmf-1.2.1/tests/__init__.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     1034 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/conftest.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     5443 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/test_archive.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3062 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/test_archivereader.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    13727 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/test_sigmffile.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     1202 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/test_utils.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3042 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/test_validation.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3217 2024-04-15 17:01:56.000000 sigmf-1.2.1/tests/testdata.py
```

### Comparing `SigMF-1.2.0/.github/workflows/main.yml` & `sigmf-1.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `SigMF-1.2.0/COPYING-LGPL` & `sigmf-1.2.1/COPYING-LGPL`

 * *Files identical despite different names*

### Comparing `SigMF-1.2.0/PKG-INFO` & `sigmf-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: SigMF
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easily interact with Signal Metadata Format (SigMF) recordings.
 Project-URL: repository, https://github.com/sigmf/sigmf-python
-Keywords: gnuradio
+Keywords: gnuradio,radio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING-LGPL
 Requires-Dist: numpy
 Requires-Dist: jsonschema
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Provides-Extra: apps
 Requires-Dist: scipy; extra == "apps"
 Requires-Dist: PySimpleGUI<5.0.0; extra == "apps"
 
-<p align="center"><img src="https://github.com/gnuradio/SigMF/blob/sigmf-v1.x/logo/sigmf_logo.svg" alt="Rendered SigMF Logo"/></p>
+<p align="center"><img src="https://github.com/sigmf/SigMF/blob/v1.2.0/logo/sigmf_logo.png" alt="Rendered SigMF Logo"/></p>
 
 This python module makes it easy to interact with Signal Metadata Format
 (SigMF) recordings. This module works with Python 3.7+ and is distributed
 freely under the terms GNU Lesser GPL v3 License.
 
 The [SigMF specification document](https://github.com/sigmf/SigMF/blob/HEAD/sigmf-spec.md)
-is located in the [SigMF](https://github.com/gnuradio/SigMF) repository.
+is located in the [SigMF](https://github.com/sigmf/SigMF) repository.
 
 # Installation
 
 To install the latest PyPi release, install from pip:
 
 ```bash
 pip install sigmf
```

### Comparing `SigMF-1.2.0/README.md` & `sigmf-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-<p align="center"><img src="https://github.com/gnuradio/SigMF/blob/sigmf-v1.x/logo/sigmf_logo.svg" alt="Rendered SigMF Logo"/></p>
+<p align="center"><img src="https://github.com/sigmf/SigMF/blob/v1.2.0/logo/sigmf_logo.png" alt="Rendered SigMF Logo"/></p>
 
 This python module makes it easy to interact with Signal Metadata Format
 (SigMF) recordings. This module works with Python 3.7+ and is distributed
 freely under the terms GNU Lesser GPL v3 License.
 
 The [SigMF specification document](https://github.com/sigmf/SigMF/blob/HEAD/sigmf-spec.md)
-is located in the [SigMF](https://github.com/gnuradio/SigMF) repository.
+is located in the [SigMF](https://github.com/sigmf/SigMF) repository.
 
 # Installation
 
 To install the latest PyPi release, install from pip:
 
 ```bash
 pip install sigmf
```

### Comparing `SigMF-1.2.0/SigMF.egg-info/PKG-INFO` & `sigmf-1.2.1/SigMF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: SigMF
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easily interact with Signal Metadata Format (SigMF) recordings.
 Project-URL: repository, https://github.com/sigmf/sigmf-python
-Keywords: gnuradio
+Keywords: gnuradio,radio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING-LGPL
 Requires-Dist: numpy
 Requires-Dist: jsonschema
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Provides-Extra: apps
 Requires-Dist: scipy; extra == "apps"
 Requires-Dist: PySimpleGUI<5.0.0; extra == "apps"
 
-<p align="center"><img src="https://github.com/gnuradio/SigMF/blob/sigmf-v1.x/logo/sigmf_logo.svg" alt="Rendered SigMF Logo"/></p>
+<p align="center"><img src="https://github.com/sigmf/SigMF/blob/v1.2.0/logo/sigmf_logo.png" alt="Rendered SigMF Logo"/></p>
 
 This python module makes it easy to interact with Signal Metadata Format
 (SigMF) recordings. This module works with Python 3.7+ and is distributed
 freely under the terms GNU Lesser GPL v3 License.
 
 The [SigMF specification document](https://github.com/sigmf/SigMF/blob/HEAD/sigmf-spec.md)
-is located in the [SigMF](https://github.com/gnuradio/SigMF) repository.
+is located in the [SigMF](https://github.com/sigmf/SigMF) repository.
 
 # Installation
 
 To install the latest PyPi release, install from pip:
 
 ```bash
 pip install sigmf
```

### Comparing `SigMF-1.2.0/SigMF.egg-info/SOURCES.txt` & `sigmf-1.2.1/SigMF.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 sigmf/apps/convert_wav.py
 sigmf/apps/gui.py
 tests/__init__.py
 tests/conftest.py
 tests/test_archive.py
 tests/test_archivereader.py
 tests/test_sigmffile.py
+tests/test_utils.py
 tests/test_validation.py
 tests/testdata.py
```

### Comparing `SigMF-1.2.0/pyproject.toml` & `sigmf-1.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "SigMF"
 description = "Easily interact with Signal Metadata Format (SigMF) recordings."
-keywords = ["gnuradio"]
+keywords = ["gnuradio", "radio"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Communications :: Ham Radio",
 ]
 dynamic = ["version", "readme"]
 requires-python = ">=3.7"
 dependencies = [
     "numpy",        # for vector math
     "jsonschema",   # for spec validation
 ]
```

### Comparing `SigMF-1.2.0/sigmf/apps/convert_wav.py` & `sigmf-1.2.1/sigmf/apps/convert_wav.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,93 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 """converter for wav containers"""
 
-import os
-import tempfile
-import datetime
-import pathlib
 import argparse
+import datetime
 import getpass
+import logging
+import os
+import pathlib
+import tempfile
 
 from scipy.io import wavfile
 
+from .. import SigMFFile, __specification__
+from .. import __version__ as toolversion
 from .. import archive
-from ..sigmffile import SigMFFile
 from ..utils import get_data_type_str
 
+log = logging.getLogger()
+
 
 def convert_wav(input_wav_filename, archive_filename=None, start_datetime=None, author=None):
     """
     read a .wav and write a .sigmf archive
     """
+    input_path = pathlib.Path(input_wav_filename)
+    input_stem = input_path.stem
     samp_rate, wav_data = wavfile.read(input_wav_filename)
 
     global_info = {
         SigMFFile.AUTHOR_KEY: getpass.getuser() if author is None else author,
         SigMFFile.DATATYPE_KEY: get_data_type_str(wav_data),
         SigMFFile.DESCRIPTION_KEY: f"Converted from {input_wav_filename}",
         SigMFFile.NUM_CHANNELS_KEY: 1 if len(wav_data.shape) < 2 else wav_data.shape[1],
         SigMFFile.RECORDER_KEY: os.path.basename(__file__),
         SigMFFile.SAMPLE_RATE_KEY: samp_rate,
+        SigMFFile.VERSION_KEY: __specification__,
     }
 
     if start_datetime is None:
-        fname = pathlib.Path(input_wav_filename)
-        mtime = datetime.datetime.fromtimestamp(fname.stat().st_mtime)
+        mtime = datetime.datetime.fromtimestamp(input_path.stat().st_mtime)
         start_datetime = mtime.isoformat() + "Z"
 
     capture_info = {SigMFFile.START_INDEX_KEY: 0}
     if start_datetime is not None:
         capture_info[SigMFFile.DATETIME_KEY] = start_datetime
 
     tmpdir = tempfile.mkdtemp()
-    sigmf_data_filename = input_wav_filename + archive.SIGMF_DATASET_EXT
+    sigmf_data_filename = input_stem + archive.SIGMF_DATASET_EXT
     sigmf_data_path = os.path.join(tmpdir, sigmf_data_filename)
     wav_data.tofile(sigmf_data_path)
 
     meta = SigMFFile(data_file=sigmf_data_path, global_info=global_info)
     meta.add_capture(0, metadata=capture_info)
 
     if archive_filename is None:
-        archive_filename = os.path.basename(input_wav_filename) + archive.SIGMF_ARCHIVE_EXT
+        archive_filename = input_stem + archive.SIGMF_ARCHIVE_EXT
     meta.tofile(archive_filename, toarchive=True)
     return os.path.abspath(archive_filename)
 
 
 def main():
     """
     entry-point for sigmf_convert_wav
     """
     parser = argparse.ArgumentParser(description="Convert .wav to .sigmf container.")
     parser.add_argument("input", type=str, help="Wavfile path")
     parser.add_argument("--author", type=str, default=None, help=f"set {SigMFFile.AUTHOR_KEY} metadata")
+    parser.add_argument('-v', '--verbose', action='count', default=0)
+    parser.add_argument('--version', action='version', version=f'%(prog)s v{toolversion}')
     args = parser.parse_args()
 
+    level_lut = {
+        0: logging.WARNING,
+        1: logging.INFO,
+        2: logging.DEBUG,
+    }
+    logging.basicConfig(level=level_lut[min(args.verbose, 2)])
+
     out_fname = convert_wav(
         input_wav_filename=args.input,
         author=args.author,
     )
-    print("Wrote", out_fname)
+    log.info(f"Write {out_fname}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `SigMF-1.2.0/sigmf/apps/gui.py` & `sigmf-1.2.1/sigmf/apps/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 '''GUI for creating & editing SigMF Files'''
 
-import os
+import argparse
 import logging
+import os
+
 from PySimpleGUI import *
 
-from ..sigmffile import SigMFFile, fromarchive, dtype_info
+from .. import __version__ as toolversion
 from ..archive import SIGMF_ARCHIVE_EXT
+from ..sigmffile import SigMFFile, dtype_info, fromarchive
 
 log = logging.getLogger()
 
 validate_button = Button('Update', bind_return_key=False, enable_events=True)
 submit_button = Button('Save Archive', disabled=True, button_color=('white', '#D3D3D3'))
 load_button = Button('Load', key='Load Archive')
 combo_button = InputCombo((), size=(20, 1), enable_events=True, key='Capture Combo')
@@ -377,21 +380,18 @@
     capture_selector_dict.update({new_val: capture_dict})
     if new_val not in list(new_values):
         new_values = list(new_values) + [new_val]
         combo_button.Update(values=tuple(new_values), value=new_val)
 
 
 def main():
-    import argparse
-    from sigmf import __version__ as toolversion
-
     parser = argparse.ArgumentParser(description='Edit SigMF Archive.')
     parser.add_argument('-i', '--input', help='Input SigMF Archive Path.', default=None)
     parser.add_argument('-v', '--verbose', action='count', default=0)
-    parser.add_argument('--version', action='version', version=f'%(prog)s {toolversion}')
+    parser.add_argument('--version', action='version', version=f'%(prog)s v{toolversion}')
     args = parser.parse_args()
 
     level_lut = {
         0: logging.WARNING,
         1: logging.INFO,
         2: logging.DEBUG,
     }
@@ -634,7 +634,10 @@
             f.archive(archive_file)
             PopupOK('Saved archive as \n', archive_file, title='')
         elif event in ['Cancel', None, 'Exit']:
             window.Close()
             break
 
     window.Close()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `SigMF-1.2.0/sigmf/archive.py` & `sigmf-1.2.1/sigmf/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 """Create and extract SigMF archives."""
 
 import os
 import shutil
 import tarfile
 import tempfile
 
 from .error import SigMFFileError
 
-
 SIGMF_ARCHIVE_EXT = ".sigmf"
 SIGMF_METADATA_EXT = ".sigmf-meta"
 SIGMF_DATASET_EXT = ".sigmf-data"
 SIGMF_COLLECTION_EXT = ".sigmf-collection"
 
 
 class SigMFArchive():
```

### Comparing `SigMF-1.2.0/sigmf/archivereader.py` & `sigmf-1.2.1/sigmf/archivereader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/gnuradio/SigMF
+# This file is part of sigmf-python. https://github.com/sigmf/SigMF
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 """Access SigMF archives without extracting them."""
 
 import os
 import shutil
 import tarfile
 import tempfile
 
-from . import __version__  #, schema, sigmf_hash, validate
+from . import __version__
+from .archive import SIGMF_ARCHIVE_EXT, SIGMF_DATASET_EXT, SIGMF_METADATA_EXT, SigMFArchive
+from .error import SigMFFileError
 from .sigmffile import SigMFFile
-from .archive import SigMFArchive, SIGMF_DATASET_EXT, SIGMF_METADATA_EXT, SIGMF_ARCHIVE_EXT
 from .utils import dict_merge
-from .error import SigMFFileError
 
 
 class SigMFArchiveReader():
     """Access data within SigMF archive `tar` in-place without extracting.
 
     Parameters:
```

### Comparing `SigMF-1.2.0/sigmf/error.py` & `sigmf-1.2.1/sigmf/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 """Defines SigMF exception classes."""
 
 
 class SigMFError(Exception):
```

### Comparing `SigMF-1.2.0/sigmf/schema-collection.json` & `sigmf-1.2.1/sigmf/schema-collection.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285486516034985%*

 * *Differences: {"'$id'": "'https://github.com/sigmf/SigMF'",*

 * * "'properties'": "{'collection': {'properties': {'core:version': {'examples': ['1.2.0']}}}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://github.com/gnuradio/SigMF",
+    "$id": "https://github.com/sigmf/SigMF",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": true,
     "default": {},
     "properties": {
         "collection": {
             "$id": "#/properties/collection",
             "additionalProperties": true,
@@ -149,15 +149,15 @@
                     },
                     "type": "array"
                 },
                 "core:version": {
                     "$id": "#/properties/collection/properties/core%3Aversion",
                     "description": "The version of the SigMF specification used to create the Collection file.",
                     "examples": [
-                        "1.0.0"
+                        "1.2.0"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "core:version"
             ],
```

### Comparing `SigMF-1.2.0/sigmf/schema-meta.json` & `sigmf-1.2.1/sigmf/schema-meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$id'": "'https://github.com/sigmf/SigMF'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://github.com/gnuradio/SigMF",
+    "$id": "https://github.com/sigmf/SigMF",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "default": [
         "global",
         "captures",
         "annotations"
     ],
```

### Comparing `SigMF-1.2.0/sigmf/schema.py` & `sigmf-1.2.1/sigmf/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 '''Schema IO'''
 
-import os
 import json
+import os
 
 from . import utils
 
 SCHEMA_META = 'schema-meta.json'
 SCHEMA_COLLECTION = 'schema-collection.json'
```

### Comparing `SigMF-1.2.0/sigmf/sigmf_hash.py` & `sigmf-1.2.1/sigmf/sigmf_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 '''Hashing Functions'''
 
 import hashlib
 import os
```

### Comparing `SigMF-1.2.0/sigmf/sigmffile.py` & `sigmf-1.2.1/sigmf/sigmffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 '''SigMFFile Object'''
 
-from collections import OrderedDict
 import codecs
 import json
 import tarfile
 import tempfile
-from os import path
 import warnings
+from collections import OrderedDict
+from os import path
+
 import numpy as np
 
-from . import __version__, schema, sigmf_hash, validate
-from .archive import SigMFArchive, SIGMF_DATASET_EXT, SIGMF_METADATA_EXT, SIGMF_ARCHIVE_EXT, SIGMF_COLLECTION_EXT
+from . import __specification__, __version__, schema, sigmf_hash, validate
+from .archive import SIGMF_ARCHIVE_EXT, SIGMF_COLLECTION_EXT, SIGMF_DATASET_EXT, SIGMF_METADATA_EXT, SigMFArchive
+from .error import SigMFAccessError, SigMFFileError
 from .utils import dict_merge
-from .error import SigMFFileError, SigMFAccessError
+
 
 class SigMFMetafile():
     VALID_KEYS = {}
     def __init__(self):
         self.version = None
         self.schema = None
         self._metadata = None
@@ -170,25 +172,24 @@
         self.sample_count = 0
         self._memmap = None
         self.is_complex_data = False  # numpy.iscomplexobj(self._memmap) is not adequate for fixed-point complex case
 
         if metadata is None:
             self._metadata = {self.GLOBAL_KEY:{}, self.CAPTURE_KEY:[], self.ANNOTATION_KEY:[]}
             self._metadata[self.GLOBAL_KEY][self.NUM_CHANNELS_KEY] = 1
+            self._metadata[self.GLOBAL_KEY][self.VERSION_KEY] = __specification__
         elif isinstance(metadata, dict):
             self._metadata = metadata
         else:
             self._metadata = json.loads(metadata)
         if global_info is not None:
             self.set_global_info(global_info)
         if data_file is not None:
             self.set_data_file(data_file, skip_checksum=skip_checksum, map_readonly=map_readonly)
 
-        self._metadata[self.GLOBAL_KEY][self.VERSION_KEY] = '1.0.0'
-
     def __len__(self):
         return self._memmap.shape[0]
 
     def __next__(self):
         '''get next batch of samples'''
         if self.iter_position < len(self):
             # normal batch
@@ -720,16 +721,14 @@
             self.metafiles = []
         else:
             self.set_streams(metafiles)
 
         if not self.skip_checksums:
             self.verify_stream_hashes()
 
-        self._metadata[self.COLLECTION_KEY][self.VERSION_KEY] = '1.0.0'
-
     def __len__(self):
         '''
         the length of a collection is the number of streams
         '''
         return len(self.get_stream_names())
 
     def verify_stream_hashes(self):
```

### Comparing `SigMF-1.2.0/sigmf/utils.py` & `sigmf-1.2.1/sigmf/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 """Utilities"""
 
+import re
+import sys
 from copy import deepcopy
 from datetime import datetime
-import sys
+
 import numpy as np
 
 from . import error
 
 SIGMF_DATETIME_ISO8601_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
@@ -26,14 +28,21 @@
     Parse an iso8601 string as a datetime
 
     Example
     -------
     >>> parse_iso8601_datetime("1955-11-05T06:15:00Z")
     datetime.datetime(1955, 11, 5, 6, 15)
     """
+    # provided string exceeds max precision -> truncate to µs
+    match = re.match(r"^(?P<dt>.*)(?P<frac>\.[0-9]{7,})Z$", datestr)
+    if match:
+        md = match.groupdict()
+        length = min(7, len(md["frac"]))
+        datestr = ''.join([md["dt"], md["frac"][:length], "Z"])
+
     try:
         timestamp = datetime.strptime(datestr, '%Y-%m-%dT%H:%M:%S.%fZ')
     except ValueError:
         timestamp = datetime.strptime(datestr, '%Y-%m-%dT%H:%M:%SZ')
     return timestamp
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SigMF-1.2.0/sigmf/validate.py` & `sigmf-1.2.1/sigmf/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # Copyright: Multiple Authors
 #
-# This file is part of SigMF. https://github.com/sigmf/sigmf-python
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 '''SigMF Validator'''
 
+import argparse
+import json
+import logging
+
 import jsonschema
 
-from . import schema
+from . import __version__ as toolversion
+from . import error, schema, sigmffile
 
 
 def extend_with_default(validator_class):
     '''
     Boilerplate code from [1] to retrieve jsonschema default dict.
 
     References
@@ -76,23 +81,14 @@
             if new_count < count:
                 raise jsonschema.exceptions.ValidationError(f'{key} has bad order')
             else:
                 count = new_count
 
 
 def main():
-    import argparse
-    import logging
-    import json
-
-    from . import sigmffile
-    from . import error
-
-    from sigmf import __version__ as toolversion
-
     parser = argparse.ArgumentParser(description='Validate SigMF Archive or file pair against JSON schema.',
                                      prog='sigmf_validate')
     parser.add_argument('filename', help='SigMF path (extension optional).')
     parser.add_argument('--skip-checksum', action='store_true', help='Skip reading dataset to validate checksum.')
     parser.add_argument('-v', '--verbose', action='count', default=0)
     parser.add_argument('--version', action='version', version=f'%(prog)s {toolversion}')
```

### Comparing `SigMF-1.2.0/tests/test_archive.py` & `sigmf-1.2.1/tests/test_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+# Copyright: Multiple Authors
+#
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
+#
+# SPDX-License-Identifier: LGPL-3.0-or-later
+
+"""Tests for SigMFArchive"""
+
 import codecs
 import json
 import tarfile
 import tempfile
 from os import path
 
+import jsonschema
 import numpy as np
 import pytest
-import jsonschema
 
 from sigmf import error
 from sigmf.archive import SIGMF_DATASET_EXT, SIGMF_METADATA_EXT
 
 from .testdata import TEST_FLOAT32_DATA, TEST_METADATA
 
 
@@ -71,15 +79,15 @@
         with pytest.raises(error.SigMFFileError):
             test_sigmffile.archive(fileobj=temp)
 
 
 def test_unwritable_name_throws_fileerror(test_sigmffile):
     # Cannot assume /root/ is unwritable (e.g. Docker environment)
     # so use invalid filename
-    unwritable_file = '/bad_name/'
+    unwritable_file = "/bad_name/"
     with pytest.raises(error.SigMFFileError):
         test_sigmffile.archive(name=unwritable_file)
 
 
 def test_tarfile_layout(test_sigmffile):
     with tempfile.NamedTemporaryFile() as temp:
         sigmf_tarfile = create_test_archive(test_sigmffile, temp)
```

### Comparing `SigMF-1.2.0/tests/test_archivereader.py` & `sigmf-1.2.1/tests/test_archivereader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-# Copyright 2023 GNU Radio Foundation
+# Copyright: Multiple Authors
+#
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
+#
+# SPDX-License-Identifier: LGPL-3.0-or-later
+
+"""Tests for SigMFArchiveReader"""
+
 import tempfile
-import numpy as np
 import unittest
 
-import sigmf
-from sigmf import SigMFFile, SigMFArchiveReader
+import numpy as np
+
+from sigmf import SigMFArchiveReader, SigMFFile, __specification__
 
 
 class TestArchiveReader(unittest.TestCase):
     def setUp(self):
         # in order to check shapes we need some positive number of samples to work with
         # number of samples should be lowest common factor of num_channels
         self.raw_count = 16
@@ -38,14 +45,15 @@
                     # for real or complex
                     target_count = self.raw_count
                     temp_meta = SigMFFile(
                         data_file=temp_path,
                         global_info={
                             SigMFFile.DATATYPE_KEY: f"{complex_prefix}{key}_le",
                             SigMFFile.NUM_CHANNELS_KEY: num_channels,
+                            SigMFFile.VERSION_KEY: __specification__,
                         },
                     )
                     temp_meta.tofile(temp_archive, toarchive=True)
 
                     readback = SigMFArchiveReader(temp_archive)
                     readback_samples = readback[:]
```

### Comparing `SigMF-1.2.0/tests/test_sigmffile.py` & `sigmf-1.2.1/tests/test_sigmffile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-# Copyright 2017 GNU Radio Foundation
+# Copyright: Multiple Authors
 #
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
+# This file is part of sigmf-python. https://github.com/sigmf/sigmf-python
 #
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
+# SPDX-License-Identifier: LGPL-3.0-or-later
+
+"""Tests for SigMFFile Object"""
 
+import copy
+import json
 import os
 import shutil
 import tempfile
-import json
+import unittest
 from pathlib import Path
+
 import numpy as np
-import unittest
-import copy
 
 from sigmf import sigmffile, utils
 from sigmf.sigmffile import SigMFFile
 
 from .testdata import *
 
 
@@ -58,51 +47,51 @@
     def test_iterator_basic(self):
         """make sure default batch_size works"""
         count = 0
         for _ in self.sigmf_object:
             count += 1
         self.assertEqual(count, len(self.sigmf_object))
 
-class TestAnnotationHandling(unittest.TestCase):
 
+class TestAnnotationHandling(unittest.TestCase):
     def test_get_annotations_with_index(self):
         """Test that only annotations containing index are returned from get_annotations()"""
         smf = SigMFFile(copy.deepcopy(TEST_METADATA))
         smf.add_annotation(start_index=1)
         smf.add_annotation(start_index=4, length=4)
         annotations_idx10 = smf.get_annotations(index=10)
         self.assertListEqual(
             annotations_idx10,
             [
                 {SigMFFile.START_INDEX_KEY: 0, SigMFFile.LENGTH_INDEX_KEY: 16},
                 {SigMFFile.START_INDEX_KEY: 1},
             ]
         )
-    
+
     def test__count_samples_from_annotation(self):
         """Make sure sample count from annotations use correct end index"""
         smf = SigMFFile(copy.deepcopy(TEST_METADATA))
         smf.add_annotation(start_index=0, length=32)
         smf.add_annotation(start_index=4, length=4)
         sample_count = smf._count_samples()
         self.assertEqual(sample_count, 32)
-    
+
     def test_set_data_file_without_annotations(self):
         """
         Make sure setting data_file with no annotations registered does not
         raise any errors
         """
         smf = SigMFFile(copy.deepcopy(TEST_METADATA))
         smf._metadata[SigMFFile.ANNOTATION_KEY].clear()
         with tempfile.TemporaryDirectory() as tmpdir:
             temp_path_data = os.path.join(tmpdir, "datafile")
             TEST_FLOAT32_DATA.tofile(temp_path_data)
             smf.set_data_file(temp_path_data)
             samples = smf.read_samples()
-            self.assertTrue(len(samples)==16)
+            self.assertTrue(len(samples) == 16)
 
     def test_set_data_file_with_annotations(self):
         """
         Make sure setting data_file with annotations registered use sample
         count from data_file and issue a warning if annotations have end
         indices bigger than file end index
         """
@@ -111,40 +100,39 @@
         with tempfile.TemporaryDirectory() as tmpdir:
             temp_path_data = os.path.join(tmpdir, "datafile")
             TEST_FLOAT32_DATA.tofile(temp_path_data)
             with self.assertWarns(Warning):
                 # Issues warning since file ends before the final annotatio
                 smf.set_data_file(temp_path_data)
                 samples = smf.read_samples()
-                self.assertTrue(len(samples)==16)
+                self.assertTrue(len(samples) == 16)
+
 
 def simulate_capture(sigmf_md, n, capture_len):
     start_index = capture_len * n
 
     capture_md = {"core:datetime": utils.get_sigmf_iso8601_datetime_now()}
 
     sigmf_md.add_capture(start_index=start_index, metadata=capture_md)
 
     annotation_md = {
         "core:latitude": 40.0 + 0.0001 * n,
         "core:longitude": -105.0 + 0.0001 * n,
     }
 
-    sigmf_md.add_annotation(start_index=start_index,
-                            length=capture_len,
-                            metadata=annotation_md)
+    sigmf_md.add_annotation(start_index=start_index, length=capture_len, metadata=annotation_md)
 
 
 def test_default_constructor():
     SigMFFile()
 
 
 def test_set_non_required_global_field():
     sigf = SigMFFile()
-    sigf.set_global_field('this_is:not_in_the_schema', None)
+    sigf.set_global_field("this_is:not_in_the_schema", None)
 
 
 def test_add_capture():
     sigf = SigMFFile()
     sigf.add_capture(start_index=0, metadata={})
 
 
@@ -233,97 +221,103 @@
         # read after the first sample
         temp_samples = temp_signal.read_samples(start_index=1, autoscale=False)
         # assure samples are in the order we expect
         self.assertTrue(np.all(temp_samples[:, 0] == np.array([6 + 7j, 12 + 13j])))
 
 
 def test_key_validity():
-    '''assure the keys in test metadata are valid'''
+    """assure the keys in test metadata are valid"""
     for top_key, top_val in TEST_METADATA.items():
         if type(top_val) is dict:
             for core_key in top_val.keys():
-                assert core_key in vars(SigMFFile)[f'VALID_{top_key.upper()}_KEYS']
+                assert core_key in vars(SigMFFile)[f"VALID_{top_key.upper()}_KEYS"]
         elif type(top_val) is list:
             # annotations are in a list
             for annot in top_val:
                 for core_key in annot.keys():
                     assert core_key in SigMFFile.VALID_ANNOTATION_KEYS
         else:
-            raise ValueError('expected list or dict')
+            raise ValueError("expected list or dict")
 
 
 def test_ordered_metadata():
-    '''check to make sure the metadata is sorted as expected'''
+    """check to make sure the metadata is sorted as expected"""
     sigf = SigMFFile()
-    top_sort_order = ['global', 'captures', 'annotations']
+    top_sort_order = ["global", "captures", "annotations"]
     for kdx, key in enumerate(sigf.ordered_metadata()):
         assert kdx == top_sort_order.index(key)
 
 
 def test_captures_checking():
-    '''
+    """
     these tests make sure the various captures access tools work properly
-    '''
-    np.array(TEST_U8_DATA0, dtype=np.uint8).tofile('/tmp/d0.sigmf-data')
-    with open('/tmp/d0.sigmf-meta','w') as f0: json.dump(TEST_U8_META0, f0)
-    np.array(TEST_U8_DATA1, dtype=np.uint8).tofile('/tmp/d1.sigmf-data')
-    with open('/tmp/d1.sigmf-meta','w') as f1: json.dump(TEST_U8_META1, f1)
-    np.array(TEST_U8_DATA2, dtype=np.uint8).tofile('/tmp/d2.sigmf-data')
-    with open('/tmp/d2.sigmf-meta','w') as f2: json.dump(TEST_U8_META2, f2)
-    np.array(TEST_U8_DATA3, dtype=np.uint8).tofile('/tmp/d3.sigmf-data')
-    with open('/tmp/d3.sigmf-meta','w') as f3: json.dump(TEST_U8_META3, f3)
-    np.array(TEST_U8_DATA4, dtype=np.uint8).tofile('/tmp/d4.sigmf-data')
-    with open('/tmp/d4.sigmf-meta','w') as f4: json.dump(TEST_U8_META4, f4)
-
-    sigmf0 = sigmffile.fromfile('/tmp/d0.sigmf-meta', skip_checksum=True)
-    sigmf1 = sigmffile.fromfile('/tmp/d1.sigmf-meta', skip_checksum=True)
-    sigmf2 = sigmffile.fromfile('/tmp/d2.sigmf-meta', skip_checksum=True)
-    sigmf3 = sigmffile.fromfile('/tmp/d3.sigmf-meta', skip_checksum=True)
-    sigmf4 = sigmffile.fromfile('/tmp/d4.sigmf-meta', skip_checksum=True)
+    """
+    np.array(TEST_U8_DATA0, dtype=np.uint8).tofile("/tmp/d0.sigmf-data")
+    with open("/tmp/d0.sigmf-meta", "w") as f0:
+        json.dump(TEST_U8_META0, f0)
+    np.array(TEST_U8_DATA1, dtype=np.uint8).tofile("/tmp/d1.sigmf-data")
+    with open("/tmp/d1.sigmf-meta", "w") as f1:
+        json.dump(TEST_U8_META1, f1)
+    np.array(TEST_U8_DATA2, dtype=np.uint8).tofile("/tmp/d2.sigmf-data")
+    with open("/tmp/d2.sigmf-meta", "w") as f2:
+        json.dump(TEST_U8_META2, f2)
+    np.array(TEST_U8_DATA3, dtype=np.uint8).tofile("/tmp/d3.sigmf-data")
+    with open("/tmp/d3.sigmf-meta", "w") as f3:
+        json.dump(TEST_U8_META3, f3)
+    np.array(TEST_U8_DATA4, dtype=np.uint8).tofile("/tmp/d4.sigmf-data")
+    with open("/tmp/d4.sigmf-meta", "w") as f4:
+        json.dump(TEST_U8_META4, f4)
+
+    sigmf0 = sigmffile.fromfile("/tmp/d0.sigmf-meta", skip_checksum=True)
+    sigmf1 = sigmffile.fromfile("/tmp/d1.sigmf-meta", skip_checksum=True)
+    sigmf2 = sigmffile.fromfile("/tmp/d2.sigmf-meta", skip_checksum=True)
+    sigmf3 = sigmffile.fromfile("/tmp/d3.sigmf-meta", skip_checksum=True)
+    sigmf4 = sigmffile.fromfile("/tmp/d4.sigmf-meta", skip_checksum=True)
 
     assert sigmf0._count_samples() == 256
     assert sigmf0._is_conforming_dataset()
-    assert (0,0) == sigmf0.get_capture_byte_boundarys(0)
-    assert (0,256) == sigmf0.get_capture_byte_boundarys(1)
+    assert (0, 0) == sigmf0.get_capture_byte_boundarys(0)
+    assert (0, 256) == sigmf0.get_capture_byte_boundarys(1)
     assert np.array_equal(TEST_U8_DATA0, sigmf0.read_samples(autoscale=False))
     assert np.array_equal(np.array([]), sigmf0.read_samples_in_capture(0))
-    assert np.array_equal(TEST_U8_DATA0, sigmf0.read_samples_in_capture(1,autoscale=False))
+    assert np.array_equal(TEST_U8_DATA0, sigmf0.read_samples_in_capture(1, autoscale=False))
 
     assert sigmf1._count_samples() == 192
     assert not sigmf1._is_conforming_dataset()
-    assert (32,160) == sigmf1.get_capture_byte_boundarys(0)
-    assert (160,224) == sigmf1.get_capture_byte_boundarys(1)
-    assert np.array_equal(np.array(range(128)), sigmf1.read_samples_in_capture(0,autoscale=False))
-    assert np.array_equal(np.array(range(128,192)), sigmf1.read_samples_in_capture(1,autoscale=False))
+    assert (32, 160) == sigmf1.get_capture_byte_boundarys(0)
+    assert (160, 224) == sigmf1.get_capture_byte_boundarys(1)
+    assert np.array_equal(np.array(range(128)), sigmf1.read_samples_in_capture(0, autoscale=False))
+    assert np.array_equal(np.array(range(128, 192)), sigmf1.read_samples_in_capture(1, autoscale=False))
 
     assert sigmf2._count_samples() == 192
     assert not sigmf2._is_conforming_dataset()
-    assert (32,160) == sigmf2.get_capture_byte_boundarys(0)
-    assert (176,240) == sigmf2.get_capture_byte_boundarys(1)
-    assert np.array_equal(np.array(range(128)), sigmf2.read_samples_in_capture(0,autoscale=False))
-    assert np.array_equal(np.array(range(128,192)), sigmf2.read_samples_in_capture(1,autoscale=False))
+    assert (32, 160) == sigmf2.get_capture_byte_boundarys(0)
+    assert (176, 240) == sigmf2.get_capture_byte_boundarys(1)
+    assert np.array_equal(np.array(range(128)), sigmf2.read_samples_in_capture(0, autoscale=False))
+    assert np.array_equal(np.array(range(128, 192)), sigmf2.read_samples_in_capture(1, autoscale=False))
 
     assert sigmf3._count_samples() == 192
     assert not sigmf3._is_conforming_dataset()
-    assert (32,64) == sigmf3.get_capture_byte_boundarys(0)
-    assert (64,160) == sigmf3.get_capture_byte_boundarys(1)
-    assert (192,256) == sigmf3.get_capture_byte_boundarys(2)
-    assert np.array_equal(np.array(range(32)), sigmf3.read_samples_in_capture(0,autoscale=False))
-    assert np.array_equal(np.array(range(32,128)), sigmf3.read_samples_in_capture(1,autoscale=False))
-    assert np.array_equal(np.array(range(128,192)), sigmf3.read_samples_in_capture(2,autoscale=False))
+    assert (32, 64) == sigmf3.get_capture_byte_boundarys(0)
+    assert (64, 160) == sigmf3.get_capture_byte_boundarys(1)
+    assert (192, 256) == sigmf3.get_capture_byte_boundarys(2)
+    assert np.array_equal(np.array(range(32)), sigmf3.read_samples_in_capture(0, autoscale=False))
+    assert np.array_equal(np.array(range(32, 128)), sigmf3.read_samples_in_capture(1, autoscale=False))
+    assert np.array_equal(np.array(range(128, 192)), sigmf3.read_samples_in_capture(2, autoscale=False))
 
     assert sigmf4._count_samples() == 96
     assert not sigmf4._is_conforming_dataset()
-    assert (32,160) == sigmf4.get_capture_byte_boundarys(0)
-    assert (160,224) == sigmf4.get_capture_byte_boundarys(1)
-    assert np.array_equal(np.array(range(64)), sigmf4.read_samples_in_capture(0,autoscale=False)[:,0])
-    assert np.array_equal(np.array(range(64,96)), sigmf4.read_samples_in_capture(1,autoscale=False)[:,1])
+    assert (32, 160) == sigmf4.get_capture_byte_boundarys(0)
+    assert (160, 224) == sigmf4.get_capture_byte_boundarys(1)
+    assert np.array_equal(np.array(range(64)), sigmf4.read_samples_in_capture(0, autoscale=False)[:, 0])
+    assert np.array_equal(np.array(range(64, 96)), sigmf4.read_samples_in_capture(1, autoscale=False)[:, 1])
+
 
 def test_slicing():
-    '''Test __getitem___ builtin for sigmffile, make sure slicing and indexing works as expected.'''
+    """Test __getitem___ builtin for sigmffile, make sure slicing and indexing works as expected."""
     _, temp_data0 = tempfile.mkstemp()
     np.array(TEST_U8_DATA0, dtype=np.uint8).tofile(temp_data0)
     sigmf0 = SigMFFile(metadata=TEST_U8_META0, data_file=temp_data0)
     assert np.array_equal(TEST_U8_DATA0, sigmf0[:])
     assert TEST_U8_DATA0[6] == sigmf0[6]
 
     # test float32
@@ -333,12 +327,12 @@
     assert np.array_equal(TEST_FLOAT32_DATA, sigmf1[:])
     assert sigmf1[10] == TEST_FLOAT32_DATA[10]
 
     # test multiple channels
     _, temp_data2 = tempfile.mkstemp()
     np.array(TEST_U8_DATA4, dtype=np.uint8).tofile(temp_data2)
     sigmf2 = SigMFFile(TEST_U8_META4, data_file=temp_data2)
-    channelized = np.array(TEST_U8_DATA4).reshape((128,2))
+    channelized = np.array(TEST_U8_DATA4).reshape((128, 2))
     assert np.array_equal(channelized, sigmf2[:][:])
     assert np.array_equal(sigmf2[10:20, 91:112], sigmf2.read_samples(autoscale=False)[10:20, 91:112])
     assert np.array_equal(sigmf2[0], channelized[0])
-    assert np.array_equal(sigmf2[1,:], channelized[1,:])
+    assert np.array_equal(sigmf2[1, :], channelized[1, :])
```

