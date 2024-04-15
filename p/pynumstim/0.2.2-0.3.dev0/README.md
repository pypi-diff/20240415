# Comparing `tmp/pynumstim-0.2.2.tar.gz` & `tmp/pynumstim-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.3.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.2.tar` & `pynumstim-0.3.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.2/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.2/LICENSE
--rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.2.2/README.md
--rw-r--r--   0        0        0      362 2024-04-15 13:55:42.110443 pynumstim-0.2.2/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.2/pynumstim/_data_sets.py
--rw-r--r--   0        0        0     6440 2024-04-15 11:49:38.946539 pynumstim-0.2.2/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.2/pynumstim/_number.py
--rw-r--r--   0        0        0     9462 2024-04-15 13:28:42.292326 pynumstim-0.2.2/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.2/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.2/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4567 2024-04-15 13:55:36.462351 pynumstim-0.2.2/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.2/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.2/trial_list.txt
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 pynumstim-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2746 2024-04-13 13:07:33.180060 pynumstim-0.3.dev0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.3.dev0/LICENSE
+-rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.3.dev0/README.md
+-rw-r--r--   0        0        0      365 2024-04-15 12:29:12.989780 pynumstim-0.3.dev0/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.3.dev0/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0     6440 2024-04-15 11:49:38.946539 pynumstim-0.3.dev0/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.3.dev0/pynumstim/_number.py
+-rw-r--r--   0        0        0     9448 2024-04-15 11:47:58.116879 pynumstim-0.3.dev0/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.3.dev0/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.3.dev0/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0     2572 2024-04-13 13:00:16.192637 pynumstim-0.3.dev0/pynumstim/image.py
+-rw-r--r--   0        0        0      528 2024-04-15 11:55:28.456306 pynumstim-0.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.3.dev0/trial_list.txt
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 pynumstim-0.3.dev0/PKG-INFO
```

### Comparing `pynumstim-0.2.2/.gitignore` & `pynumstim-0.3.dev0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,9 +154,9 @@
 
 
 .vscode/
 
 ## test runs
 ttest*
 stim/
-*.png
+
 aristim
```

### Comparing `pynumstim-0.2.2/LICENSE` & `pynumstim-0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/README.md` & `pynumstim-0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/pynumstim/_data_sets.py` & `pynumstim-0.3.dev0/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/pynumstim/_mplist.py` & `pynumstim-0.3.dev0/pynumstim/_mplist.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/pynumstim/_number.py` & `pynumstim-0.3.dev0/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/pynumstim/_problem.py` & `pynumstim-0.3.dev0/pynumstim/_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from copy import copy
 from fractions import Fraction
 from hashlib import md5
 from typing import Any, Dict, Optional
 
 from ._number import Num, TNum, TPyNum
 
-LATEX_TIMES = "\\times"  # "\\cdot"
-LATEX_SYMBOL_NAMES = {"=": "equal",
+SYMBOL_NAMES = {"=": "equal",
                 "+": "plus",
-                LATEX_TIMES: "multiply",
+                "*": "multiply",
                 "/": "divide",
                 "-": "minus"}
+LATEX_TIMES = "\\times"  # "\\cdot"
 
 TProperties = Dict[str, Any]
 
 
 class MathProblem(object):
 
     LABEL_MULTI = "t"  # multiplication, times
```

### Comparing `pynumstim-0.2.2/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.3.dev0/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2/pyproject.toml` & `pynumstim-0.3.dev0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,23 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pynumstim"
 authors = [{name = "Oliver Lindemann", email = "lindemann@essb.eur.nl"}]
 license = {file = "LICENSE"}
+classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-readme = "README.md"
-keywords = ["experiment control", "open science",
-            "experimental psychology"]
-classifiers = [
-  "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3",
-  "Operating System :: OS Independent"
-]
-
 requires-python = ">=3.10"
 dependencies =  ["pandas>=2.1", "toml>=0.10.2", "sympy>=1.12"]
 
 [project.urls]
 Documentation = "https://github.com/lindemann09/PyNumStim"
 Source = "https://github.com/lindemann09/PyNumStim"
```

### Comparing `pynumstim-0.2.2/trial_list.txt` & `pynumstim-0.3.dev0/trial_list.txt`

 * *Files identical despite different names*

