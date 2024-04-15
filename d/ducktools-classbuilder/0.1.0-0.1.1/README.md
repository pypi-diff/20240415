# Comparing `tmp/ducktools-classbuilder-0.1.0.tar.gz` & `tmp/ducktools_classbuilder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools-classbuilder-0.1.0.tar", last modified: Thu Apr 11 18:32:41 2024, max compression
+gzip compressed data, was "ducktools_classbuilder-0.1.1.tar", last modified: Mon Apr 15 13:32:09 2024, max compression
```

## Comparing `ducktools-classbuilder-0.1.0.tar` & `ducktools_classbuilder-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:32:41.924637 ducktools-classbuilder-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-11 18:32:41.924637 ducktools-classbuilder-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:32:41.924637 ducktools-classbuilder-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:32:41.920637 ducktools-classbuilder-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:32:41.920637 ducktools-classbuilder-0.1.0/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:32:41.920637 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/prefab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 18:32:35.000000 ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:32:41.924637 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-11 18:32:41.000000 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-11 18:32:41.000000 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:32:41.000000 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 18:32:41.000000 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 18:32:41.000000 ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/approach_vs_tool.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19176 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/extension_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/perf/performance_tests.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/docs/prefab/
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/docs/prefab/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:32:09.594660 ducktools_classbuilder-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.582660 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29675 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:32:09.000000 ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.578660 ducktools_classbuilder-0.1.1/tests/prefab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.586660 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_compare_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_pre_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_slots_novalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/dynamic/test_slotted_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.586660 ducktools_classbuilder-0.1.1/tests/prefab/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:32:09.590660 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 13:32:05.000000 ducktools_classbuilder-0.1.1/tests/prefab/shared/test_repr.py
```

### Comparing `ducktools-classbuilder-0.1.0/LICENSE.md` & `ducktools_classbuilder-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ducktools-classbuilder-0.1.0/PKG-INFO` & `ducktools_classbuilder-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,40 +36,96 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: mypy; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 # Ducktools: Class Builder #
 
 `ducktools-classbuilder` is *the* Python package that will bring you the **joy**
 of writing... functions... that will bring back the **joy** of writing classes.
 
 Maybe.
 
 While `attrs` and `dataclasses` are class boilerplate generators, 
-`ducktools.classbuilder` is intended to be a dataclasses-like generator.
+`ducktools.classbuilder` is intended to be a `@dataclass`-like generator.
 The goal is to handle some of the basic functions and to allow for flexible
 customization of both the field collection and the method generation.
 
 `ducktools.classbuilder.prefab` includes a prebuilt implementation using these tools.
 
+Install from PyPI with:
+`python -m pip install ducktools-classbuilder`
+
+## Usage: building a class decorator ##
+
+In order to create a class decorator using `ducktools.classbuilder` there are
+a few things you need to prepare.
+
+1. A field gathering function to analyse the class and collect valid `Field`s.
+   * An example `slot_gatherer` is included.
+2. Code generators that can make use of the gathered `Field`s to create magic method
+   source code.
+   * Example `init_maker`, `repr_maker` and `eq_maker` generators are included.
+3. A function that calls the `builder` function to apply both of these steps.
+
+A field gathering function needs to take the original class as an argument and 
+return a dictionary of `{key: Field(...)}` pairs.
+
+> [!NOTE]
+> The `builder` will handle inheritance so do not collect fields from parent classes.
+
+The code generators take the class as the only argument and return a tuple 
+of method source code and globals to be provided to `exec(code, globs)` in order 
+to generate the actual method. 
+
+The provided `slot_gatherer` looks for `__slots__` being assigned a `SlotFields` 
+class[^1] where keyword arguments define the names and values for the fields. 
+
+Code generator functions need to be converted to descriptors before being used. 
+This is done using the provided `MethodMaker` descriptor class. 
+ex: `init_desc = MethodMaker("__init__", init_maker)`
+
+These parts can then be used to make a basic class boilerplate generator by 
+providing them to the `builder` function.
+
+```python
+from ducktools.classbuilder import (
+    builder, 
+    slot_gatherer, 
+    init_maker, eq_maker, repr_maker,
+    MethodMaker,
+)
+
+init_desc = MethodMaker("__init__", init_maker)
+repr_desc = MethodMaker("__repr__", repr_maker)
+eq_desc = MethodMaker("__eq__", eq_maker)
+
+def slotclass(cls):
+    return builder(cls, gatherer=slot_gatherer, methods={init_desc, repr_desc, eq_desc})
+```
+
 ## Slot Class Usage ##
 
-The building toolkit also includes a basic implementation that uses
-`__slots__` to define the fields by assigning a `SlotFields` instance.
+This created `slotclass` function can then be used as a decorator to generate classes in 
+a similar manner to the `@dataclass` decorator from `dataclasses`. 
+
+> [!NOTE] 
+> `ducktools.classbuilder` includes a premade version of `slotclass` that can
+> be used directly. (The included version has some extra features).
 
 ```python
-from ducktools.classbuilder import slotclass, Field, SlotFields
+from ducktools.classbuilder import Field, SlotFields
 
 @slotclass
 class SlottedDC:
     __slots__ = SlotFields(
         the_answer=42,
         the_question=Field(
             default="What do you get if you multiply six by nine?",
@@ -77,36 +133,44 @@
         ),
     )
     
 ex = SlottedDC()
 print(ex)
 ```
 
-## Why does the basic implementation use slots? ##
-
-Dataclasses has a problem when you use `@dataclass(slots=True)`, 
-although this is not unique to dataclasses but inherent to the way both
-`__slots__` and decorators work.
-
-In order for this to *appear* to work, dataclasses has to make a new class 
-and attempt to copy over everything from the original. This is because 
-decorators operate on classes *after they have been created* while slots 
-need to be declared beforehand. While you can change the value of `__slots__` 
-after a class has been created, this will have no effect on the internal
-structure of the class.
+> [!TIP]
+> For more information and examples of creating class generators with additional 
+> features using the builder see 
+> [the docs](https://ducktools-classbuilder.readthedocs.io/en/latest/extension_examples.html)
+
+## Why does your example use `__slots__` instead of annotations? ##
+
+If you want to use `__slots__` in order to save memory you have to declare
+them when the class is originally created as you can't add them later.
+
+When you use `@dataclass(slots=True)`[^2] with `dataclasses` in order for 
+this to work, `dataclasses` has to make a new class and attempt to
+copy over everything from the original. 
+This is because decorators operate on classes *after they have been created* 
+while slots need to be declared beforehand. 
+While you can change the value of `__slots__` after a class has been created, 
+this will have no effect on the internal structure of the class.
 
 By declaring the class using `__slots__` on the other hand, we can take
 advantage of the fact that it accepts a mapping, where the keys will be
 used as the attributes to create as slots. The values can then be used as
-the default values equivalently to how type hints are used in dataclasses.
+the default values equivalently to how type hints are used in `dataclasses`.
 
-For example these two classes would be roughly equivalent, except 
+For example these two classes would be roughly equivalent, except that
 `@dataclass` has had to recreate the class from scratch while `@slotclass`
-has simply added the methods on to the original class. This is easy to 
-demonstrate using another decorator.
+has added the methods on to the original class. 
+This means that any references stored to the original class *before*
+`@dataclass` has rebuilt the class will not be pointing towards the 
+correct class. 
+This can be demonstrated using a simple class register decorator.
 
 > This example requires Python 3.10 as earlier versions of 
 > `dataclasses` did not support the `slots` argument.
 
 ```python
 from dataclasses import dataclass
 from ducktools.classbuilder import slotclass, SlotFields
@@ -136,15 +200,14 @@
 
 
 print(DataCoords())
 print(SlotCoords())
 
 print(f"{DataCoords is class_register[DataCoords.__name__] = }")
 print(f"{SlotCoords is class_register[SlotCoords.__name__] = }")
-
 ```
 
 ## What features does this have? ##
 
 Included as an example implementation, the `slotclass` generator supports 
 `default_factory` for creating mutable defaults like lists, dicts etc.
 It also supports default values that are not builtins (try this on 
@@ -154,17 +217,14 @@
 `__annotations__` dictionary of the class. 
 Values provided to `doc` will be placed in the final `__slots__` 
 field so they are present on the class if `help(...)` is called.
 
 If you want something with more features you can look at the `prefab.py`
 implementation which provides a 'prebuilt' implementation.
 
-For more information on creating class generators using the builder
-see [the docs](https://ducktools-classbuilder.readthedocs.io/en/latest/extension_examples.html)
-
 ## Will you add \<feature\> to `classbuilder.prefab`? ##
 
 No. Not unless it's something I need or find interesting.
 
 The original version of `prefab_classes` was intended to have every feature
 anybody could possibly require, but this is no longer the case with this
 rebuilt version.
@@ -173,7 +233,13 @@
 
 However the whole goal of this module is if you want to have a class generator
 with a specific feature, you can create or add it yourself.
 
 ## Credit ##
 
 Heavily inspired by [David Beazley's Cluegen](https://github.com/dabeaz/cluegen)
+
+[^1]: `SlotFields` is actually just a subclassed `dict` with no changes. `__slots__`
+      works with dictionaries using the values of the keys, while fields are normally
+      used for documentation.
+
+[^2]: or `@attrs.define`.
```

### Comparing `ducktools-classbuilder-0.1.0/pyproject.toml` & `ducktools_classbuilder-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ducktools.classbuilder.__version__"}
 
 [project.optional-dependencies]
-testing = ["pytest", "pytest-cov"]
+testing = ["pytest", "pytest-cov", "mypy"]
 docs = ["sphinx", "myst-parser", "sphinx_rtd_theme"]
 
 [project.urls]
 "Homepage" = "https://github.com/davidcellis/ducktools-classbuilder"
 
 [tool.pytest.ini_options]
 addopts= "--cov=src/ --cov-report=term-missing"
```

### Comparing `ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/__init__.py` & `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "v0.1.0"
+__version__ = "v0.1.1"
 
 # Change this name if you make heavy modifications
 INTERNALS_DICT = "__classbuilder_internals__"
 
 
 def get_internals(cls):
     """
@@ -411,8 +411,8 @@
 
     cls = builder(
         cls,
         gatherer=slot_gatherer,
         methods=field_methods
     )
 
-    return cls
+    return cls
```

### Comparing `ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/__init__.pyi` & `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import typing
 from collections.abc import Callable
 
+_py_type = type  # Alias for type where it is used as a name
+
 __version__: str
 INTERNALS_DICT: str
 
 def get_internals(cls) -> dict[str, typing.Any] | None: ...
 
 def get_fields(cls: type) -> dict[str, Field]: ...
 
@@ -34,78 +36,76 @@
 def eq_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 
 init_desc: MethodMaker
 repr_desc: MethodMaker
 eq_desc: MethodMaker
 default_methods: frozenset[MethodMaker]
 
+_T = typing.TypeVar("_T")
+
 @typing.overload
 def builder(
-    cls: type,
+    cls: type[_T],
     /,
     *,
     gatherer: Callable[[type], dict[str, Field]],
     methods: frozenset[MethodMaker] | set[MethodMaker]
-) -> typing.Any: ...
+) -> type[_T]: ...
 
 @typing.overload
 def builder(
     cls: None = None,
     /,
     *,
     gatherer: Callable[[type], dict[str, Field]],
     methods: frozenset[MethodMaker] | set[MethodMaker]
-) -> Callable[[type], type]: ...
-
+) -> Callable[[type[_T]], type[_T]]: ...
 
-_Self = typing.TypeVar("_Self", bound="Field")
 
 class Field:
     default: _NothingType | typing.Any
     default_factory: _NothingType | typing.Any
-    type: _NothingType | type
+    type: _NothingType | _py_type
     doc: None | str
 
+    __classbuilder_internals__: dict
+
     def __init__(
         self,
         *,
         default: _NothingType | typing.Any = NOTHING,
         default_factory: _NothingType | typing.Any = NOTHING,
-        type: _NothingType | type = NOTHING,
+        type: _NothingType | _py_type = NOTHING,
         doc: None | str = None,
     ) -> None: ...
-    @property
-    def _inherited_slots(self) -> list[str]: ...
     def __repr__(self) -> str: ...
-    @typing.overload
-    def __eq__(self, other: _Self) -> bool: ...
-    @typing.overload
-    def __eq__(self, other: object) -> NotImplemented: ...
+    def __eq__(self, other: Field | object) -> bool: ...
     def validate_field(self) -> None: ...
     @classmethod
-    def from_field(cls, fld: Field, **kwargs: typing.Any) -> _Self: ...
+    def from_field(cls, fld: Field, /, **kwargs: typing.Any) -> Field: ...
 
 
 class SlotFields(dict):
     ...
 
 def slot_gatherer(cls: type) -> dict[str, Field]:
     ...
 
 @typing.overload
 def slotclass(
-    cls: type,
+    cls: type[_T],
     /,
     *,
     methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
     syntax_check: bool = True
-) -> typing.Any: ...
+) -> type[_T]: ...
 
+@typing.overload
 def slotclass(
     cls: None = None,
     /,
     *,
     methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
     syntax_check: bool = True
-) -> Callable[[type], type]: ...
+) -> Callable[[type[_T]], type[_T]]: ...
 
-def fieldclass(cls: type) -> typing.Any: ...
+def fieldclass(cls: type[_T]) -> type[_T]: ...
```

### Comparing `ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/prefab.py` & `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,20 +315,27 @@
         return code, globs
 
     return MethodMaker("__eq__", __eq__)
 
 
 def get_iter_maker():
     def __iter__(cls: "type") -> "tuple[str, dict]":
-        field_names = get_attributes(cls).keys()
+        fields = get_attributes(cls)
 
-        if field_names:
-            values = "\n".join(f"    yield self.{name} " for name in field_names)
-        else:
+        valid_fields = (
+            name for name, attrib in fields.items()
+            if attrib.iter and not attrib.exclude_field
+        )
+
+        values = "\n".join(f"    yield self.{name}" for name in valid_fields)
+
+        # if values is an empty string
+        if not values:
             values = "    yield from ()"
+
         code = f"def __iter__(self):\n{values}"
         globs = {}
         return code, globs
 
     return MethodMaker("__iter__", __iter__)
 
 
@@ -362,14 +369,15 @@
         return code, globs
 
     # Pass the exception to exec
     return MethodMaker("__setattr__", __setattr__)
 
 
 def get_frozen_delattr_maker():
+    # noinspection PyUnusedLocal
     def __delattr__(cls: "type") -> "tuple[str, dict]":
         body = (
             '    raise TypeError(\n'
             '        f"{type(self).__name__!r} object "\n'
             '        f"does not support attribute deletion"\n'
             '    )\n'
         )
@@ -411,14 +419,15 @@
 # Updated field with additional attributes
 @fieldclass
 class Attribute(Field):
     __slots__ = SlotFields(
         init=True,
         repr=True,
         compare=True,
+        iter=True,
         kw_only=False,
         in_dict=True,
         exclude_field=False,
     )
 
     def validate_field(self):
         super().validate_field()
@@ -432,30 +441,31 @@
 def attribute(
     *,
     default=NOTHING,
     default_factory=NOTHING,
     init=True,
     repr=True,
     compare=True,
+    iter=True,
     kw_only=False,
     in_dict=True,
     exclude_field=False,
     doc=None,
     type=NOTHING,
 ):
     """
-    Additional definition for how to generate standard methods
-    for an instance attribute.
+    Get an object to define a prefab Attribute
 
     :param default: Default value for this attribute
     :param default_factory: 0 argument callable to give a default value
                             (for otherwise mutable defaults, eg: list)
     :param init: Include this attribute in the __init__ parameters
     :param repr: Include this attribute in the class __repr__
     :param compare: Include this attribute in the class __eq__
+    :param iter: Include this attribute in the class __iter__ if generated
     :param kw_only: Make this argument keyword only in init
     :param in_dict: Include this attribute in methods that serialise to dict
     :param exclude_field: Exclude this field from all magic method generation
                           apart from __init__ signature
                           and do not include it in PREFAB_FIELDS
                           Must be assigned in __prefab_post_init__
     :param doc: Parameter documentation for slotted classes
@@ -465,14 +475,15 @@
     """
     return Attribute(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         compare=compare,
+        iter=iter,
         kw_only=kw_only,
         in_dict=in_dict,
         exclude_field=exclude_field,
         doc=doc,
         type=type,
     )
 
@@ -702,15 +713,15 @@
             if name in local_fields:
                 local_fields[name] = attrib
 
         # Excluded fields *MUST* be forwarded to post_init
         if attrib.exclude_field:
             if name not in post_init_args:
                 raise PrefabError(
-                    f"{name} is an excluded attribute but is not passed to post_init"
+                    f"{name!r} is an excluded attribute but is not passed to post_init"
                 )
         else:
             valid_args.append(name)
 
         if not kw_only:
             # Syntax check arguments for __init__ don't have non-default after default
             if attrib.init and not attrib.kw_only:
```

### Comparing `ducktools-classbuilder-0.1.0/src/ducktools/classbuilder/prefab.pyi` & `ducktools_classbuilder-0.1.1/src/ducktools/classbuilder/prefab.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import typing
+from typing_extensions import dataclass_transform
+
 from collections.abc import Callable
 
 from . import (
     INTERNALS_DICT, NOTHING,
     Field, MethodMaker, SlotFields as SlotFields,
     builder, fieldclass, get_internals, slot_gatherer
 )
 
+# noinspection PyUnresolvedReferences
+from . import _NothingType
+
 PREFAB_FIELDS: str
 PREFAB_INIT_FUNC: str
 PRE_INIT_FUNC: str
 POST_INIT_FUNC: str
 
 
 # noinspection PyPep8Naming
@@ -52,49 +57,49 @@
 
 class Attribute(Field):
     __slots__: dict
 
     init: bool
     repr: bool
     compare: bool
+    iter: bool
     kw_only: bool
     in_dict: bool
     exclude_field: bool
 
     def __init__(
         self,
         *,
-        default: typing.Any | NOTHING =NOTHING,
-        default_factory: typing.Any | NOTHING = NOTHING,
-        type: type | NOTHING = NOTHING,
+        default: typing.Any | _NothingType = NOTHING,
+        default_factory: typing.Any | _NothingType = NOTHING,
+        type: type | _NothingType = NOTHING,
         doc: str | None = None,
         init: bool = True,
         repr: bool = True,
         compare: bool = True,
+        iter: bool = True,
         kw_only: bool = False,
         in_dict: bool = True,
         exclude_field: bool = False,
     ) -> None: ...
 
     def __repr__(self) -> str: ...
-    @typing.overload
-    def __eq__(self, other: Attribute) -> bool: ...
-    def __eq__(self, other: object) -> NotImplemented: ...
-
+    def __eq__(self, other: Attribute | object) -> bool: ...
     def validate_field(self) -> None: ...
 
 def attribute(
     *,
-    default: typing.Any | NOTHING = NOTHING,
-    default_factory: typing.Any | NOTHING = NOTHING,
-    type: type | NOTHING = NOTHING,
+    default: typing.Any | _NothingType = NOTHING,
+    default_factory: typing.Any | _NothingType = NOTHING,
+    type: type | _NothingType = NOTHING,
     doc: str | None = None,
     init: bool = True,
     repr: bool = True,
     compare: bool = True,
+    iter: bool = True,
     kw_only: bool = False,
     in_dict: bool = True,
     exclude_field: bool = False,
 ) -> Attribute: ...
 
 def attribute_gatherer(cls: type) -> dict[str, Attribute]: ...
 
@@ -108,28 +113,33 @@
     match_args: bool = True,
     kw_only: bool = False,
     frozen: bool = False,
     dict_method: bool = False,
     recursive_repr: bool = False,
 ) -> type: ...
 
-@typing.dataclass_transform
+_T = typing.TypeVar("_T")
+
+
+# For some reason PyCharm can't see 'attribute'?!?
+# noinspection PyUnresolvedReferences
+@dataclass_transform(field_specifiers=(Attribute, attribute))
 def prefab(
-    cls: type | None = None,
+    cls: type[_T] | None = None,
     *,
     init: bool = True,
     repr: bool = True,
     eq: bool = True,
     iter: bool = False,
     match_args: bool = True,
     kw_only: bool = False,
     frozen: bool = False,
     dict_method: bool = False,
     recursive_repr: bool = False,
-) -> type | Callable[[type], type]: ...
+) -> type[_T] | Callable[[type[_T]], type[_T]]: ...
 
 def build_prefab(
     class_name: str,
     attributes: list[tuple[str, Attribute]],
     *,
     bases: tuple[type, ...] = (),
     class_dict: dict[str, typing.Any] | None = None,
```

### Comparing `ducktools-classbuilder-0.1.0/src/ducktools_classbuilder.egg-info/PKG-INFO` & `ducktools_classbuilder-0.1.1/src/ducktools_classbuilder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,40 +36,96 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: mypy; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 # Ducktools: Class Builder #
 
 `ducktools-classbuilder` is *the* Python package that will bring you the **joy**
 of writing... functions... that will bring back the **joy** of writing classes.
 
 Maybe.
 
 While `attrs` and `dataclasses` are class boilerplate generators, 
-`ducktools.classbuilder` is intended to be a dataclasses-like generator.
+`ducktools.classbuilder` is intended to be a `@dataclass`-like generator.
 The goal is to handle some of the basic functions and to allow for flexible
 customization of both the field collection and the method generation.
 
 `ducktools.classbuilder.prefab` includes a prebuilt implementation using these tools.
 
+Install from PyPI with:
+`python -m pip install ducktools-classbuilder`
+
+## Usage: building a class decorator ##
+
+In order to create a class decorator using `ducktools.classbuilder` there are
+a few things you need to prepare.
+
+1. A field gathering function to analyse the class and collect valid `Field`s.
+   * An example `slot_gatherer` is included.
+2. Code generators that can make use of the gathered `Field`s to create magic method
+   source code.
+   * Example `init_maker`, `repr_maker` and `eq_maker` generators are included.
+3. A function that calls the `builder` function to apply both of these steps.
+
+A field gathering function needs to take the original class as an argument and 
+return a dictionary of `{key: Field(...)}` pairs.
+
+> [!NOTE]
+> The `builder` will handle inheritance so do not collect fields from parent classes.
+
+The code generators take the class as the only argument and return a tuple 
+of method source code and globals to be provided to `exec(code, globs)` in order 
+to generate the actual method. 
+
+The provided `slot_gatherer` looks for `__slots__` being assigned a `SlotFields` 
+class[^1] where keyword arguments define the names and values for the fields. 
+
+Code generator functions need to be converted to descriptors before being used. 
+This is done using the provided `MethodMaker` descriptor class. 
+ex: `init_desc = MethodMaker("__init__", init_maker)`
+
+These parts can then be used to make a basic class boilerplate generator by 
+providing them to the `builder` function.
+
+```python
+from ducktools.classbuilder import (
+    builder, 
+    slot_gatherer, 
+    init_maker, eq_maker, repr_maker,
+    MethodMaker,
+)
+
+init_desc = MethodMaker("__init__", init_maker)
+repr_desc = MethodMaker("__repr__", repr_maker)
+eq_desc = MethodMaker("__eq__", eq_maker)
+
+def slotclass(cls):
+    return builder(cls, gatherer=slot_gatherer, methods={init_desc, repr_desc, eq_desc})
+```
+
 ## Slot Class Usage ##
 
-The building toolkit also includes a basic implementation that uses
-`__slots__` to define the fields by assigning a `SlotFields` instance.
+This created `slotclass` function can then be used as a decorator to generate classes in 
+a similar manner to the `@dataclass` decorator from `dataclasses`. 
+
+> [!NOTE] 
+> `ducktools.classbuilder` includes a premade version of `slotclass` that can
+> be used directly. (The included version has some extra features).
 
 ```python
-from ducktools.classbuilder import slotclass, Field, SlotFields
+from ducktools.classbuilder import Field, SlotFields
 
 @slotclass
 class SlottedDC:
     __slots__ = SlotFields(
         the_answer=42,
         the_question=Field(
             default="What do you get if you multiply six by nine?",
@@ -77,36 +133,44 @@
         ),
     )
     
 ex = SlottedDC()
 print(ex)
 ```
 
-## Why does the basic implementation use slots? ##
-
-Dataclasses has a problem when you use `@dataclass(slots=True)`, 
-although this is not unique to dataclasses but inherent to the way both
-`__slots__` and decorators work.
-
-In order for this to *appear* to work, dataclasses has to make a new class 
-and attempt to copy over everything from the original. This is because 
-decorators operate on classes *after they have been created* while slots 
-need to be declared beforehand. While you can change the value of `__slots__` 
-after a class has been created, this will have no effect on the internal
-structure of the class.
+> [!TIP]
+> For more information and examples of creating class generators with additional 
+> features using the builder see 
+> [the docs](https://ducktools-classbuilder.readthedocs.io/en/latest/extension_examples.html)
+
+## Why does your example use `__slots__` instead of annotations? ##
+
+If you want to use `__slots__` in order to save memory you have to declare
+them when the class is originally created as you can't add them later.
+
+When you use `@dataclass(slots=True)`[^2] with `dataclasses` in order for 
+this to work, `dataclasses` has to make a new class and attempt to
+copy over everything from the original. 
+This is because decorators operate on classes *after they have been created* 
+while slots need to be declared beforehand. 
+While you can change the value of `__slots__` after a class has been created, 
+this will have no effect on the internal structure of the class.
 
 By declaring the class using `__slots__` on the other hand, we can take
 advantage of the fact that it accepts a mapping, where the keys will be
 used as the attributes to create as slots. The values can then be used as
-the default values equivalently to how type hints are used in dataclasses.
+the default values equivalently to how type hints are used in `dataclasses`.
 
-For example these two classes would be roughly equivalent, except 
+For example these two classes would be roughly equivalent, except that
 `@dataclass` has had to recreate the class from scratch while `@slotclass`
-has simply added the methods on to the original class. This is easy to 
-demonstrate using another decorator.
+has added the methods on to the original class. 
+This means that any references stored to the original class *before*
+`@dataclass` has rebuilt the class will not be pointing towards the 
+correct class. 
+This can be demonstrated using a simple class register decorator.
 
 > This example requires Python 3.10 as earlier versions of 
 > `dataclasses` did not support the `slots` argument.
 
 ```python
 from dataclasses import dataclass
 from ducktools.classbuilder import slotclass, SlotFields
@@ -136,15 +200,14 @@
 
 
 print(DataCoords())
 print(SlotCoords())
 
 print(f"{DataCoords is class_register[DataCoords.__name__] = }")
 print(f"{SlotCoords is class_register[SlotCoords.__name__] = }")
-
 ```
 
 ## What features does this have? ##
 
 Included as an example implementation, the `slotclass` generator supports 
 `default_factory` for creating mutable defaults like lists, dicts etc.
 It also supports default values that are not builtins (try this on 
@@ -154,17 +217,14 @@
 `__annotations__` dictionary of the class. 
 Values provided to `doc` will be placed in the final `__slots__` 
 field so they are present on the class if `help(...)` is called.
 
 If you want something with more features you can look at the `prefab.py`
 implementation which provides a 'prebuilt' implementation.
 
-For more information on creating class generators using the builder
-see [the docs](https://ducktools-classbuilder.readthedocs.io/en/latest/extension_examples.html)
-
 ## Will you add \<feature\> to `classbuilder.prefab`? ##
 
 No. Not unless it's something I need or find interesting.
 
 The original version of `prefab_classes` was intended to have every feature
 anybody could possibly require, but this is no longer the case with this
 rebuilt version.
@@ -173,7 +233,13 @@
 
 However the whole goal of this module is if you want to have a class generator
 with a specific feature, you can create or add it yourself.
 
 ## Credit ##
 
 Heavily inspired by [David Beazley's Cluegen](https://github.com/dabeaz/cluegen)
+
+[^1]: `SlotFields` is actually just a subclassed `dict` with no changes. `__slots__`
+      works with dictionaries using the values of the keys, while fields are normally
+      used for documentation.
+
+[^2]: or `@attrs.define`.
```

