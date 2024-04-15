# Comparing `tmp/fancy_collections-0.2.1.tar.gz` & `tmp/fancy_collections-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancy_collections-0.2.1.tar", last modified: Tue Jun 20 09:01:30 2023, max compression
+gzip compressed data, was "fancy_collections-0.3.0.tar", last modified: Mon Apr 15 13:31:44 2024, max compression
```

## Comparing `fancy_collections-0.2.1.tar` & `fancy_collections-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 fancy_collections-0.2.1/LICENSE
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      467 2022-12-17 23:31:27.000000 fancy_collections-0.2.1/README.md
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/fancy_collections/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      208 2023-02-20 20:19:59.000000 fancy_collections-0.2.1/fancy_collections/__init__.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)    10009 2023-06-19 15:49:47.000000 fancy_collections-0.2.1/fancy_collections/core.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6233 2023-02-21 15:45:06.000000 fancy_collections-0.2.1/fancy_collections/formatting.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     5895 2023-02-20 20:38:24.000000 fancy_collections-0.2.1/fancy_collections/lib.py
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/fancy_collections.egg-info/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-06-20 09:01:30.000000 fancy_collections-0.2.1/fancy_collections.egg-info/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      427 2023-06-20 09:01:30.000000 fancy_collections-0.2.1/fancy_collections.egg-info/SOURCES.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-06-20 09:01:30.000000 fancy_collections-0.2.1/fancy_collections.egg-info/dependency_links.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       69 2023-06-20 09:01:30.000000 fancy_collections-0.2.1/fancy_collections.egg-info/requires.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2023-06-20 09:01:30.000000 fancy_collections-0.2.1/fancy_collections.egg-info/top_level.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      791 2023-06-20 08:59:49.000000 fancy_collections-0.2.1/pyproject.toml
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/setup.cfg
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 09:01:30.799807 fancy_collections-0.2.1/tests/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     4120 2023-06-19 15:54:20.000000 fancy_collections-0.2.1/tests/test_axis.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1172 2023-02-16 12:26:32.000000 fancy_collections-0.2.1/tests/test_frame.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       22 2023-02-16 11:15:19.000000 fancy_collections-0.2.1/tests/test_lib.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      740 2023-06-19 11:15:15.000000 fancy_collections-0.2.1/tests/test_pickle.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 fancy_collections-0.3.0/LICENSE
+-rw-r--r--   0 palmb     (1000) palmb     (1000)     1214 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      467 2022-12-17 23:31:27.000000 fancy_collections-0.3.0/README.md
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/fancy_collections/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      208 2023-02-20 20:19:59.000000 fancy_collections-0.3.0/fancy_collections/__init__.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    11298 2024-04-15 13:16:38.000000 fancy_collections-0.3.0/fancy_collections/core.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     7387 2024-04-15 12:57:44.000000 fancy_collections-0.3.0/fancy_collections/formatting.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     5895 2023-02-20 20:38:24.000000 fancy_collections-0.3.0/fancy_collections/lib.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/fancy_collections.egg-info/
+-rw-r--r--   0 palmb     (1000) palmb     (1000)     1214 2024-04-15 13:31:44.000000 fancy_collections-0.3.0/fancy_collections.egg-info/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      427 2024-04-15 13:31:44.000000 fancy_collections-0.3.0/fancy_collections.egg-info/SOURCES.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2024-04-15 13:31:44.000000 fancy_collections-0.3.0/fancy_collections.egg-info/dependency_links.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       69 2024-04-15 13:31:44.000000 fancy_collections-0.3.0/fancy_collections.egg-info/requires.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2024-04-15 13:31:44.000000 fancy_collections-0.3.0/fancy_collections.egg-info/top_level.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      791 2024-04-15 13:31:24.000000 fancy_collections-0.3.0/pyproject.toml
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/setup.cfg
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2024-04-15 13:31:44.027012 fancy_collections-0.3.0/tests/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     4120 2023-06-19 15:54:20.000000 fancy_collections-0.3.0/tests/test_axis.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1172 2023-02-16 12:26:32.000000 fancy_collections-0.3.0/tests/test_frame.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       22 2023-02-16 11:15:19.000000 fancy_collections-0.3.0/tests/test_lib.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      740 2023-06-19 11:15:15.000000 fancy_collections-0.3.0/tests/test_pickle.py
```

### Comparing `fancy_collections-0.2.1/LICENSE` & `fancy_collections-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.2.1/PKG-INFO` & `fancy_collections-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: fancy_collections
-Version: 0.2.1
+Version: 0.3.0
 Summary: Some useful collection classes.
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/fancy-collections
 Project-URL: Bug Tracker, https://github.com/palmb/fancy-collections/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: sliceable-dict>=0.4.1
+Requires-Dist: pandas>1.0.0
+Requires-Dist: numpy>1.0.0
+Provides-Extra: tests
+Requires-Dist: black; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # fancy-collections
 
 This package provide some useful classes to store data in a structured way.
 Up to now mostly advanced dictionaries are provided.
```

### Comparing `fancy_collections-0.2.1/fancy_collections/core.py` & `fancy_collections-0.3.0/fancy_collections/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
+import numpy as np
+
 import functools
 import warnings
 from typing import List, Any
 
 import pandas as pd
 from sliceable_dict import TypedSliceDict, SliceDict
 
@@ -130,52 +132,67 @@
             return name
         i = 1
         self.union_index()
         while f"{name}({i})" in self.keys():
             i += 1
         return f"{name}({i})"
 
-    def flatten(self, promote_index: bool = False) -> DictOfPandas:
+    def flatten(
+        self, promote_index: bool = False, multiindex: bool = False
+    ) -> DictOfPandas:
         """
         Promote dataframe columns to first level columns.
 
         Prepend column names of an inner dataframe with the
         key/column name of the outer frame.
 
         Parameters
         ----------
         promote_index : bool, default False
             Makes `pandas.Series` from items of type `pandas.Index` if True.
             Every item of the resulting DictOfPandas be a series then.
+        multiindex: bool, default False
+            If True, the result column names will be pd.MultiIndex like, if False, unique
+            column names will be generated from the different levels of column indices.
 
         Returns
         -------
         DictOfPandas
 
         Examples
         --------
+        >>> from fancy_collections import DictOfPandas
         >>> frame = DictOfPandas(key0=pd.DataFrame({'c0': [1, 1], "c1": [2, 2]}))
         >>> frame   # doctest: +NORMALIZE_WHITESPACE
              key0 |
         ========= |
            c0  c1 |
         0   1   2 |
         1   1   2 |
 
         >>> frame.flatten()   # doctest: +NORMALIZE_WHITESPACE
         key0_c0 | key0_c1 |
         ======= | ======= |
         0     1 | 0     2 |
         1     1 | 1     2 |
+
+        >>> frame.flatten(multiindex=True)   # doctest: +NORMALIZE_WHITESPACE
+        ('key0', 'c0') | ('key0', 'c1') |
+        ============== | ============== |
+             0  1      |      0  2      |
+             1  1      |      1  2      |
         """
         data = dict()
         for key, value in self.items():
             if isinstance(value, pd.DataFrame):
                 for col, ser in dict(value).items():
-                    data[self._uniquify_name(f"{key}_{col}")] = ser
+                    if multiindex:
+                        data[(key, col)] = ser
+                    else:
+                        data[self._uniquify_name(f"{key}_{col}")] = ser
             elif promote_index and isinstance(value, pd.Index):
                 data[key] = value.to_series()
             else:
                 data[key] = value
         return self.__class__(data)
 
     def to_dataframe(self, how="outer") -> pd.DataFrame:
@@ -187,15 +204,17 @@
         """
         warnings.warn(
             f"`to_dataframe()` is deprecated use `to_pandas()` instead.",
             category=DeprecationWarning,
         )
         return self.to_pandas(how)
 
-    def to_pandas(self, how="outer") -> pd.DataFrame:
+    def to_pandas(
+        self, how="outer", fill_value=np.nan, multiindex=False
+    ) -> pd.DataFrame:
         """
         Transform DictOfPandas to a pandas.DataFrame.
 
         Because a pandas.DataFrame can not handle data of different
         length, but DictOfPandas can, the missing data is filled with
         NaNs or is dropped, depending on the keyword `how`.
 
@@ -213,14 +232,19 @@
             - ``outer`` : The resulting DataFrame index is the combination
                 of all indices merged together. If a column misses values at
                 new index locations, `NaN`'s are filled.
             - ``inner`` : Only indices that are present in all columns are used
                 for the resulting index. Filling logic is not needed, but values
                 are dropped, if a column has indices that are not known to all
                 other columns.
+        fill_value:
+            Value to use for missing values. Defaults to NaN, but can be any “compatible” value.
+        multiindex: bool, default True
+            If True, the result column names will be pd.MultiIndex like, if False, unique
+            column names will be generated from the different levels of column indices
 
         Returns
         -------
         frame: pandas.DataFrame
 
         See Also
         --------
@@ -249,24 +273,29 @@
         2   NaN  22.0   NaN
         4   NaN   NaN  33.0
         7   NaN   NaN  33.0
 
         or is dropped if `how='inner'`
 
         >>> di.to_pandas(how='inner')   # doctest: +NORMALIZE_WHITESPACE
-              a     b     c
-        1  11.0  22.0  33.0
+                a   b   c
+            1  11  22  33
 
         todo: examples with dataframe
         """
         if how not in ["inner", "outer"]:
             raise ValueError("`how` must be one of 'inner' or 'outer'")
-        df = pd.DataFrame(dict(self.flatten(promote_index=True)))
-        if how == "inner":
-            df = df.reindex(self.shared_index())
+        flat = dict(self.flatten(promote_index=True, multiindex=multiindex))
+        if how == "outer":
+            target_index = self.union_index()
+        else:  # how == "inner"
+            target_index = self.shared_index()
+        df = pd.DataFrame(
+            {k: v.reindex(target_index, fill_value=fill_value) for k, v in flat.items()}
+        )
         return df
 
     def __repr__(self) -> str:
         max_rows = pd.get_option("display.max_rows")
         min_rows = pd.get_option("display.min_rows")
         return self.to_string(max_rows=max_rows, min_rows=min_rows)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fancy_collections-0.2.1/fancy_collections/formatting.py` & `fancy_collections-0.3.0/fancy_collections/formatting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
+import shutil
 from typing import Tuple, List, Iterable, Any
 
 import pandas as pd
 
 
 class Formatter:
     column_seperator = " | "
@@ -12,17 +13,19 @@
 
     def __init__(
         self,
         obj,
         max_rows: int | None = None,
         min_rows: int | None = None,
         show_df_column_names: bool = True,
+        max_colwidth: int = 50,
     ):
         self.show_df_column_names = show_df_column_names
         self._trunc_options = dict(max_rows=max_rows, min_rows=min_rows)
+        self._max_colwidth = max_colwidth
         self._obj = obj
         self.__to_render = []
 
     def key_to_string(self, key: Any, obj: Any) -> str:  # noqa
         """
         stringify key.
 
@@ -41,59 +44,95 @@
         key: str
         """
         return str(key)
 
     def to_string(self) -> str:
         if len(self._obj) == 0:
             return self._stringify_empty_class(self._obj)
+
+        display_width = (
+            int(shutil.get_terminal_size().columns) - 3 - len(self.column_seperator)
+        )
+
+        objects = {}
+        widths = {}
         for key, val in self._obj.items():
             key = self.key_to_string(key, val)
-            try:
-                string = self.stringify(val)
-            except Exception:  # noqa
-                string = NotImplemented
-            if string is NotImplemented:
-                string = str(val)
-            self._add(key, string.splitlines())
+            lines = self.stringify(val).splitlines()
+            objects[key] = lines
+            widths[key] = self._get_maxlen(lines + [key])
+
+        keys = tuple(widths.keys())
+        front_keys, back_keys = set(), set()
+        line_length = 0
+        for fkey, bkey in zip(keys, keys[::-1]):
+            line_length += widths[fkey] + len(self.column_seperator)
+            if line_length < display_width:
+                front_keys.add(fkey)
+            line_length += widths[bkey] + len(self.column_seperator)
+            if line_length < display_width:
+                back_keys.add(bkey)
+
+        if not front_keys:
+            # ensure that we have at least on column
+            front_keys.add(keys[0])
+
+        for k, v in objects.items():
+            if k in front_keys:
+                self._add(k, v)
+
+        if len(front_keys) + len(back_keys) < len(keys):
+            self._add("...", ["..."])
+
+        for k, v in objects.items():
+            if k in back_keys and k not in front_keys:
+                self._add(k, objects[k])
+
         return self._render()
 
-    def stringify(self, obj: Any) -> str | NotImplemented:
+    def stringify(self, obj: Any) -> str:
         if isinstance(obj, pd.Index):
             return self._stringify_Index(obj)
         if isinstance(obj, pd.Series):
             return self._stringify_Series(obj)
         if isinstance(obj, pd.DataFrame):
             return self._stringify_DataFrame(obj)
-        return NotImplemented
+        return str(obj)
 
     def _stringify_DataFrame(self, df: pd.DataFrame) -> str:
         # if df.empty and not df.index.empty:
         #     return f"Empty DataFrame\n" + self._stringify_Index(df.index)
 
         if df.empty:
             r, c = df.shape
             return self._justify(
                 f"{self._stringify_empty_class(df)}\n"  # prevent black formatting
                 f" rows:    {r}\n"
                 f" columns: {c}\n"
             )
         return df.to_string(
-            **self._trunc_options, header=self.show_df_column_names, index_names=False
+            **self._trunc_options,
+            header=self.show_df_column_names,
+            index_names=False,
+            max_colwidth=self._max_colwidth,
         )
 
     def _stringify_Series(self, s: pd.Series) -> str:
         if s.empty:
             return self._justify(
                 f"{self._stringify_empty_class(s)}\n"  # prevent black formatting
                 f" rows: {len(s)}\n"
             )
         # We use to_frame because it uses less space between index and values
         # return s.to_string(**self._trunc_options, header=False)
         return s.to_frame(name=" ").to_string(
-            **self._trunc_options, header=False, index_names=False
+            **self._trunc_options,
+            header=False,
+            index_names=False,
+            max_colwidth=self._max_colwidth,
         )
 
     def _stringify_Index(self, idx: pd.Index) -> str:
         if idx.empty:
             return f"{self._stringify_empty_class(idx)}"
         idx = pd.Series("", index=idx, dtype=str)
         return idx.to_string(**self._trunc_options, header=False)
```

### Comparing `fancy_collections-0.2.1/fancy_collections/lib.py` & `fancy_collections-0.3.0/fancy_collections/lib.py`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.2.1/fancy_collections.egg-info/PKG-INFO` & `fancy_collections-0.3.0/fancy_collections.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
-Name: fancy-collections
-Version: 0.2.1
+Name: fancy_collections
+Version: 0.3.0
 Summary: Some useful collection classes.
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/fancy-collections
 Project-URL: Bug Tracker, https://github.com/palmb/fancy-collections/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: sliceable-dict>=0.4.1
+Requires-Dist: pandas>1.0.0
+Requires-Dist: numpy>1.0.0
+Provides-Extra: tests
+Requires-Dist: black; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # fancy-collections
 
 This package provide some useful classes to store data in a structured way.
 Up to now mostly advanced dictionaries are provided.
```

### Comparing `fancy_collections-0.2.1/pyproject.toml` & `fancy_collections-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fancy_collections"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Bert Palm", email="bert.palm.home@gmail.com" },
 ]
 description = "Some useful collection classes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fancy_collections-0.2.1/tests/test_axis.py` & `fancy_collections-0.3.0/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.2.1/tests/test_frame.py` & `fancy_collections-0.3.0/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.2.1/tests/test_pickle.py` & `fancy_collections-0.3.0/tests/test_pickle.py`

 * *Files identical despite different names*

