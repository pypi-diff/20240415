# Comparing `tmp/dsp_ifsc-0.0.3.tar.gz` & `tmp/dsp_ifsc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.3.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.4.tar", max compression
```

## Comparing `dsp_ifsc-0.0.3.tar` & `dsp_ifsc-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.3/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.3/README.md
--rw-r--r--   0        0        0      990 2024-04-14 20:35:35.153798 dsp_ifsc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.4/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0     6700 2024-04-14 21:15:14.608747 dsp_ifsc-0.0.4/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0      990 2024-04-14 21:16:34.866582 dsp_ifsc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.4/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.3/LICENSE` & `dsp_ifsc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.3/pyproject.toml` & `dsp_ifsc-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.3"
+version = "0.0.4"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.3/PKG-INFO` & `dsp_ifsc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

