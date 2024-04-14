# Comparing `tmp/dsp_ifsc-0.0.4.tar.gz` & `tmp/dsp_ifsc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.4.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.5.tar", max compression
```

## Comparing `dsp_ifsc-0.0.4.tar` & `dsp_ifsc-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.4/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/sequence.py
--rw-r--r--   0        0        0     6700 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/signal.py
--rw-r--r--   0        0        0      990 2024-04-14 21:16:34.866582 dsp_ifsc-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.5/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.5/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-14 22:03:29.782544 dsp_ifsc-0.0.5/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0    11838 2024-04-14 22:41:37.958897 dsp_ifsc-0.0.5/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0     1007 2024-04-14 22:43:55.336954 dsp_ifsc-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.5/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.4/LICENSE` & `dsp_ifsc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.4/dsp_ifsc/sequence.py` & `dsp_ifsc-0.0.5/dsp_ifsc/sequence.py`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.4/pyproject.toml` & `dsp_ifsc-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.4"
+version = "0.0.5"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -19,14 +19,15 @@
 repository = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 license = "MIT"
 packages = [{include = "dsp_ifsc"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 numpy = "*"
+matplotlib = "*"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dsp_ifsc-0.0.4/PKG-INFO` & `dsp_ifsc-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib
 Requires-Dist: numpy
 Project-URL: Issues, https://github.com/JoaoMario109/ifsc-dsp-2024/issues
 Project-URL: Repository, https://github.com/JoaoMario109/ifsc-dsp-2024
 Description-Content-Type: text/markdown
 
 # DSP - IFSC (Campus Florianópolis)
```

