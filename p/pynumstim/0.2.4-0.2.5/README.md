# Comparing `tmp/pynumstim-0.2.4.tar.gz` & `tmp/pynumstim-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.4.tar` & `pynumstim-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.4/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.4/LICENSE
--rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.2.4/README.md
--rw-r--r--   0        0        0      362 2024-04-15 14:19:33.358866 pynumstim-0.2.4/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.4/pynumstim/_data_sets.py
--rw-r--r--   0        0        0     6623 2024-04-15 14:13:36.920875 pynumstim-0.2.4/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.4/pynumstim/_number.py
--rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.4/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.4/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.4/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.4/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.4/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.4/trial_list.txt
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 pynumstim-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.5/LICENSE
+-rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.5/README.md
+-rw-r--r--   0        0        0      362 2024-04-15 15:15:15.406181 pynumstim-0.2.5/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.5/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0     7690 2024-04-15 15:16:26.059357 pynumstim-0.2.5/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.5/pynumstim/_number.py
+-rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.5/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.5/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.5/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.5/pynumstim/image.py
+-rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.5/trial_list.txt
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.5/PKG-INFO
```

### Comparing `pynumstim-0.2.4/.gitignore` & `pynumstim-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/LICENSE` & `pynumstim-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/README.md` & `pynumstim-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/pynumstim?style=flat)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pynumstim?style=flat)](https://pypi.org/project/pynumstim/)
 
 (c) Oliver Lindemann (lindemann@cognitive-psychology.eu)
 
 Project homepage: https://github.com/lindemann09/PyNumStim
 
+## Install via pip
+
+```
+pip install pynumstim
+```
+
 
 ## Requirements
 
 * Python >= 3.10
 * dvipng
```

### Comparing `pynumstim-0.2.4/pynumstim/_data_sets.py` & `pynumstim-0.2.5/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/pynumstim/_mplist.py` & `pynumstim-0.2.5/pynumstim/_mplist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from pathlib import Path
 from random import randint, shuffle
 from typing import List, Optional, Tuple, Union
+import re
 
 import pandas as pd
 import toml
 
 from ._number import TNum
 from ._problem import MathProblem, TProperties
 
@@ -125,19 +126,15 @@
         return df
 
     #def to_toml(self, filename: Union[Path, str]) -> pd.DataFrame:
     #    """pandas data frame, includes problem ids, if first_id is defined"""
     #    # FIXME categories are lots
 
     def import_toml(self, filename: Union[Path, str]):
-        return self.import_dict(toml.load(filename))
-
-    def import_dict(self, problem_dict: dict,
-                    sections: Union[None, str, Tuple[str], List[str]] = None):
-        """imports dicts
+        """imports toml
 
         the following methods exist (illustrated by toml representation):
         method a:
 
             [category]
             op1 = [12, 13, 14]
             op2 = [6, 7, 8, 9]
@@ -156,20 +153,57 @@
             problems = [ "1 + 5 = 8",
                         "1/2 + 1/4 = 9"]
 
         Args:
             problem_dict: _description_
             sections: _description_. Defaults to None.
         """
-        if sections is None:
-            sections = list(problem_dict.keys())
-        elif isinstance(sections, (tuple, list)):
-            sections = list(sections)
+        return self.import_dict(toml.load(filename))
+
+    def import_markdown(self, filename: Union[Path, str]):
+        """importing from markdown file
+
+        Example
+        -------
+        Markdown file:
+            ```
+            # CATEGORY NAME
+
+            * 1 + 2 = 2
+            * 23_26 - 1_2 = 8
+
+            comment
+            * 4 / 7 = 19
+            ```
+        """
+        with open(filename, "r", encoding="utf-8") as fl:
+            curr_cat = None
+            for l in fl:
+                x = re.match(r"^\s*#+\s+", l)
+                if isinstance(x, re.Match):
+                    curr_cat = l[x.span()[1]:].strip()
+                else:
+                    x = re.match(r"^\s*\*+\s+", l)
+                    if isinstance(x, re.Match):
+                        problem_str = l[x.span()[1]:].strip()
+                        p = MathProblem.parse(problem_str)
+                        if curr_cat is not None:
+                            p.update_properties({"category": curr_cat})
+                        self.append(p)
+
+    def import_dict(self, problem_dict: dict,
+                    categories: Union[None, str, Tuple[str], List[str]] = None):
+        """see doc import toml for structure of dict"""
+
+        if categories is None:
+            categories = list(problem_dict.keys())
+        elif isinstance(categories, (tuple, list)):
+            categories = list(categories)
 
-        for s in sections:
+        for s in categories:
             prop = {"category": s}
             d = problem_dict[s]
             if "problems" in d:
                 for x in d["problems"]:
                     if isinstance(x, list):
                         p = MathProblem(x[0], x[1], x[2])
                     else:
```

### Comparing `pynumstim-0.2.4/pynumstim/_number.py` & `pynumstim-0.2.5/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/pynumstim/_problem.py` & `pynumstim-0.2.5/pynumstim/_problem.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.2.5/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/pynumstim/image.py` & `pynumstim-0.2.5/pynumstim/image.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/pyproject.toml` & `pynumstim-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/trial_list.txt` & `pynumstim-0.2.5/trial_list.txt`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.4/PKG-INFO` & `pynumstim-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumstim
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library to create symbolic number and arithmetic stimuli for psychological experiments
 Keywords: experiment control,open science,experimental psychology
 Author-email: Oliver Lindemann <lindemann@essb.eur.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,20 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/pynumstim?style=flat)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pynumstim?style=flat)](https://pypi.org/project/pynumstim/)
 
 (c) Oliver Lindemann (lindemann@cognitive-psychology.eu)
 
 Project homepage: https://github.com/lindemann09/PyNumStim
 
+## Install via pip
+
+```
+pip install pynumstim
+```
+
 
 ## Requirements
 
 * Python >= 3.10
 * dvipng
```

