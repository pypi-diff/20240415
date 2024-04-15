# Comparing `tmp/dsp_ifsc-0.0.7.tar.gz` & `tmp/dsp_ifsc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.7.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.8.tar", max compression
```

## Comparing `dsp_ifsc-0.0.7.tar` & `dsp_ifsc-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.7/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.7/dsp_ifsc/__init__.py
--rw-r--r--   0        0        0     2281 2024-04-14 23:21:14.820331 dsp_ifsc-0.0.7/dsp_ifsc/sequence.py
--rw-r--r--   0        0        0    12337 2024-04-14 23:22:16.931388 dsp_ifsc-0.0.7/dsp_ifsc/signal.py
--rw-r--r--   0        0        0     1007 2024-04-14 23:22:39.458439 dsp_ifsc-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.8/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.8/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     2281 2024-04-14 23:28:11.770848 dsp_ifsc-0.0.8/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0    12337 2024-04-14 23:28:33.847900 dsp_ifsc-0.0.8/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0     1007 2024-04-14 23:31:34.274392 dsp_ifsc-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.8/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.7/LICENSE` & `dsp_ifsc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.7/dsp_ifsc/sequence.py` & `dsp_ifsc-0.0.8/dsp_ifsc/sequence.py`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.7/dsp_ifsc/signal.py` & `dsp_ifsc-0.0.8/dsp_ifsc/signal.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -484,16 +484,16 @@
 
 
     @staticmethod
     def from_impulse(n: numpy.ndarray, position: int = 0) -> 'Signal':
         """
         Generates an impulse signal.
         Args:
-            position: The position of the impulse.
             n: The sequence of n values.
+            position: The position of the impulse.
 
         Returns:
             signal: The impulse Signal class.
         """
 
         x, _n = sequence.impulse(position, n.min(), n.max())
```

### Comparing `dsp_ifsc-0.0.7/pyproject.toml` & `dsp_ifsc-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.7"
+version = "0.0.8"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.7/PKG-INFO` & `dsp_ifsc-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

