# Comparing `tmp/pynumstim-0.2.2b0.tar.gz` & `tmp/pynumstim-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.2b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.3.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.2b0.tar` & `pynumstim-0.3.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.2b0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.2b0/LICENSE
--rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.2.2b0/README.md
--rw-r--r--   0        0        0      363 2024-04-15 14:03:24.122330 pynumstim-0.2.2b0/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.2b0/pynumstim/_data_sets.py
--rw-r--r--   0        0        0     6440 2024-04-15 11:49:38.946539 pynumstim-0.2.2b0/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.2b0/pynumstim/_number.py
--rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.2b0/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.2b0/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.2b0/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.2b0/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.2b0/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.2b0/trial_list.txt
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 pynumstim-0.2.2b0/PKG-INFO
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

### Comparing `pynumstim-0.2.2b0/.gitignore` & `pynumstim-0.3.dev0/.gitignore`

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

### Comparing `pynumstim-0.2.2b0/LICENSE` & `pynumstim-0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/README.md` & `pynumstim-0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_data_sets.py` & `pynumstim-0.3.dev0/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_mplist.py` & `pynumstim-0.3.dev0/pynumstim/_mplist.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_number.py` & `pynumstim-0.3.dev0/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_problem.py` & `pynumstim-0.3.dev0/pynumstim/_problem.py`

 * *Files 1% similar despite different names*

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
@@ -203,14 +203,16 @@
     def hash(self) -> str:
         md5_object = md5(self.label().encode())
         return md5_object.hexdigest()
 
     def is_correct(self):
         if self._result is None:
             return False
+        print(self.calc())
+        print(type(self._op1))
         return self.calc() == self._result.py_number
 
     def n_carry(self) -> Optional[int]:
         """number of carry operations for addition and subtraction
         else None"""
 
         if self.operant1.is_fraction() or self.operant2.is_fraction():
```

### Comparing `pynumstim-0.2.2b0/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.3.dev0/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/image.py` & `pynumstim-0.3.dev0/pynumstim/image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,71 @@
 import os
 from pathlib import Path
 from typing import Optional, Union
 from sympy import preview
 
-from ._problem import MathProblem, LATEX_SYMBOL_NAMES
+from ._problem import MathProblem, SYMBOL_NAMES
 from ._mplist import MathProblemList
 
-
-def create_images(
-        source: Union[str, MathProblem, MathProblemList],
-        path: Optional[Union[Path, str]] = None,
-        segmented=False,
-        resolution: int = 400,
-        fg: str = "White",
-        bg: str = "Transparent"):
-
-    if path is None:
-        if isinstance(source, MathProblem):
-            path = source.label() + ".png"  # use label
-        else:
-            raise ValueError(
-                f"Path is required, if you create images from {type(source)}"
-            )
-
-    if isinstance(source, MathProblem):
-        return _from_problem(source, folder=path, segmented=segmented,
-                             resolution=resolution, fg=fg, bg=bg)
-    elif isinstance(source, MathProblemList):
-        return _from_problem_list(source, folder=path, segmented=segmented,
-                                  resolution=resolution, fg=fg, bg=bg)
-    elif isinstance(source, str):
-        return _from_tex(source, filename=path, resolution=resolution, fg=fg, bg=bg)
-
-
-def _from_tex(
-        tex_str: str,
-        filename: Union[Path, str],
-        resolution: int = 400,
-        fg: str = "White",
-        bg: str = "Transparent"):
-    """latex to PNG"""
+def from_tex(tex_str: str,
+             filename: Union[Path, str],
+             resolution: int = 400,
+             fg: str = "White", bg: str = "Transparent"):
+    """latex to PNG """
     return preview(tex_str,
-                   dvioptions=["-D", str(resolution), "-fg", fg, "-bg", bg],
-                   viewer="file", filename=filename,
-                   euler=False)
-
+                   dvioptions=['-D', str(resolution), "-fg", fg, "-bg", bg],
+                   viewer='file', filename=filename, euler=False)
 
-def _from_problem(
-        problem: MathProblem,
-        folder: Union[Path, str],
-        segmented: bool = False,
-        resolution: int = 400,
-        fg: str = "White",
-        bg: str = "Transparent") -> str:
-    """returns the filename, if not segmented"""
 
-    os.makedirs(folder, exist_ok=True)
-    flname = os.path.join(folder, "p" + f"{problem.label()}.png")
-    if not segmented:
-        _from_tex(f"$${problem.tex()}$$", filename=flname,
-                  resolution=resolution, fg=fg, bg=bg)
-    else:
-        # segmented
-        os.makedirs(folder, exist_ok=True)
-        _create_latex_symbols(folder, resolution=resolution, fg=fg, bg=bg)
-        stim = set()
-        stim.add((problem.operant1.tex(), problem.operant1.label()))
-        stim.add((problem.operant2.tex(), problem.operant2.label()))
-        if problem.result is not None:
-            stim.add((problem.result.tex(), problem.result.label()))
-        for tex, label in stim:
-            print("png: " + label)
-            _from_tex(f"$${tex}$$",
-                      filename=os.path.join(folder, "n" + f"{label}.png"),
-                      resolution=resolution, fg=fg, bg=bg)
-
-    return flname
-
-
-def _from_problem_list(
-        problems: MathProblemList,
-        folder: Union[Path, str],
-        segmented=False,
-        resolution: int = 400,
-        fg: str = "White",
-        bg: str = "Transparent"):
+def from_problem(problem: MathProblem,
+                 filename: Optional[Union[Path, str]] = None,
+                 resolution: int = 400,
+                 fg: str = "White",
+                 bg: str = "Transparent"):
+    if filename is None:
+        filename = problem.label() + ".png"
+    return from_tex(f'$${problem.tex()}$$',
+                    filename=filename,
+                    resolution=resolution,
+                    fg=fg, bg=bg)
+
+
+def from_problem_list(problems: MathProblemList,
+                      folder: Union[Path, str],
+                      segmented=False,
+                      resolution: int = 400,
+                      fg: str = "White",
+                      bg: str = "Transparent"):
     """segmented: single files for each number and operation"""
     # make pictures
     os.makedirs(folder, exist_ok=True)
     if not segmented:
         done = set()
         for x in problems.list:
             print("png: ", x.label())
-            if x.label() not in done:
-                _from_problem(x, folder=folder, segmented=False,
-                              resolution=resolution, fg=fg, bg=bg)
-                done.add(x.label())
+            flname = os.path.join(folder, "p" + x.label() + ".png")
+            if flname not in done:
+                from_problem(x, filename=flname, resolution=resolution,
+                             fg=fg, bg=bg)
+                done.add(flname)
     else:
-        _create_latex_symbols(folder=folder,
-                              resolution=resolution, fg=fg, bg=bg)
+        # create symbols
+        for symbol, name in SYMBOL_NAMES.items():
+            from_tex(f'$${symbol}$$',
+                     filename=os.path.join(folder, f"{name}.png"),
+                     resolution=resolution,
+                     fg=fg, bg=bg)
         # problem_stimuli
         stim = set()
         for x in problems.list:
             stim.add((x.operant1.tex(), x.operant1.label()))
             stim.add((x.operant2.tex(), x.operant2.label()))
+
             if x.result is not None:
                 stim.add((x.result.tex(), x.result.label()))
 
         for tex, label in stim:
             print("png: " + label)
-            _from_tex(f"$${tex}$$",
-                      filename=os.path.join(folder, "n" + f"{label}.png"),
-                      resolution=resolution,
-                      fg=fg, bg=bg)
-
-
-def _create_latex_symbols(folder: Union[Path, str],
-                          resolution: int = 400,
-                          fg: str = "White",
-                          bg: str = "Transparent"):
-    # create symbols, segmented
-    for symbol, name in LATEX_SYMBOL_NAMES.items():
-        _from_tex(f"$${symbol}$$",
-                  filename=os.path.join(folder, f"{name}.png"),
-                  resolution=resolution, fg=fg, bg=bg)
+            from_tex(f'$${tex}$$',
+                    filename=os.path.join(folder, "n" + f"{label}.png"),
+                    resolution=resolution,
+                    fg=fg, bg=bg)
```

### Comparing `pynumstim-0.2.2b0/pyproject.toml` & `pynumstim-0.3.dev0/pyproject.toml`

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

### Comparing `pynumstim-0.2.2b0/trial_list.txt` & `pynumstim-0.3.dev0/trial_list.txt`

 * *Files identical despite different names*

