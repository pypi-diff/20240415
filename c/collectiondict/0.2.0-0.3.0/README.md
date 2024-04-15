# Comparing `tmp/collectiondict-0.2.0.tar.gz` & `tmp/collectiondict-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collectiondict-0.2.0.tar", max compression
+gzip compressed data, was "collectiondict-0.3.0.tar", max compression
```

## Comparing `collectiondict-0.2.0.tar` & `collectiondict-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1498 2024-03-26 13:14:44.667211 collectiondict-0.2.0/LICENSE
--rw-r--r--   0        0        0     1122 2024-03-26 13:14:44.667211 collectiondict-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6189 2024-03-26 13:14:44.667211 collectiondict-0.2.0/src/collectiondict/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 13:14:44.667211 collectiondict-0.2.0/src/collectiondict/py.typed
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 collectiondict-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-04-15 07:29:08.111850 collectiondict-0.3.0/LICENSE
+-rw-r--r--   0        0        0      314 2024-04-15 07:29:08.115850 collectiondict-0.3.0/README.md
+-rw-r--r--   0        0        0     1530 2024-04-15 07:29:08.115850 collectiondict-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/__init__.py
+-rw-r--r--   0        0        0     7143 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/_collectiondict.py
+-rw-r--r--   0        0        0     3341 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/_reverse_mapping.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/py.typed
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 collectiondict-0.3.0/PKG-INFO
```

### Comparing `collectiondict-0.2.0/LICENSE` & `collectiondict-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collectiondict-0.2.0/pyproject.toml` & `collectiondict-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 [tool.poetry]
 name = "collectiondict"
-version = "0.2.0"
+version = "0.3.0"
 description = "Helpers to create dictionaries that collect values into collections"
 authors = ["Max Görner <5477952+MaxG87@users.noreply.github.com>"]
 license = "BSD-3-Clause"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
+    "Topic :: Software Development :: Libraries",
+]
+homepage = "https://github.com/MaxG87/collectiondict/"
+repository = "https://github.com/MaxG87/collectiondict/"
+
+[tool.poetry.urls]
+Changelog = "https://github.com/MaxG87/collectiondict/releases/"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.99.9"
 pytest = "^8.1.1"
@@ -24,15 +36,14 @@
 allow_any_unimported = false
 warn_unreachable = true
 enable_error_code = [
     "possibly-undefined"
 ]
 strict = true
 
-
 [tool.pytest.ini_options]
 addopts = [
     "--cov", "src",
     "--doctest-modules",
     "--cov-branch",
     "--cov-fail-under", "95"
 ]
```

### Comparing `collectiondict-0.2.0/src/collectiondict/__init__.py` & `collectiondict-0.3.0/src/collectiondict/_collectiondict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import typing as t
 from collections import Counter
 
-_T = t.TypeVar("_T")
-_CollectionT = t.Generic[_T]
 _KeyT = t.TypeVar("_KeyT", bound=t.Hashable)
 _ValueT = t.TypeVar("_ValueT")
 _HashableValueT = t.TypeVar("_HashableValueT", bound=t.Hashable)
 
+# TODO Currently, the type annotations are not perfect. Due to the limited
+# nature of Python's type annotations, it is not possible to specify the correct
+# return type for the custom classes. Thus, custom classes are supported but the
+# return type is not inferred to be the parent class.
+
 
 @t.overload
 def collectiondict(  # pragma: nocover
     clct: t.Type[Counter[_HashableValueT]],
     iterable: t.Iterable[tuple[_KeyT, _HashableValueT]],
 ) -> dict[_KeyT, Counter[_HashableValueT]]: ...
 
@@ -74,21 +77,35 @@
     examples covers this scenario.
 
     The supported collections are fixed. Only the built-in collections
     `Counter`, `frozenset`, `list`, `set`, and `tuple` as well as their
     subclasses are supported. If a unsupported collection is passed, an
     exception is raised. However, `mypy` will warn about it.
 
+    Due to the limits of Pythons type annotations, it is not possible to
+    specify the correct return type for the custom classes. Thus, custom
+    classes are supported but the return type is not inferred to be the parent
+    class.
+
+    In order to have the best type inference, it is recommended to **cast**
+    `clct` to specify the value type. Passing a specialised collection class is
+    **not** supported currently. The examples show how to use a cast.
 
     Examples:
     ---------
     Simple usage using `set`:
     >>> collectiondict(set, [("a", 1), ("b", 2), ("a", 3)])
     {'a': {1, 3}, 'b': {2}}
 
+    Usage using `frozenset` and a cast to have the best type inference:
+    >>> import typing as t
+    >>> clct = t.cast(t.Type[frozenset[int]], frozenset)
+    >>> collectiondict(clct, [("a", 1), ("b", 2), ("a", 3)])
+    {'a': frozenset({1, 3}), 'b': frozenset({2})}
+
     Scenario that might exceed memory:
     >>> N=1000  # could be humongous, e.g. 10**20
     >>> collectiondict(set, ((str(n%2), n%3) for n in range(N)))
     {'0': {0, 1, 2}, '1': {0, 1, 2}}
     """
 
     if issubclass(clct, Counter):
@@ -97,15 +114,15 @@
         return _collectiondict_for_lists(clct, iterable)
     elif issubclass(clct, set):
         return _collectiondict_for_sets(clct, iterable)
     elif issubclass(clct, frozenset):
         return _collectiondict_for_frozensets(clct, iterable)
     elif issubclass(clct, tuple):
         return _collectiondict_for_tuple(clct, iterable)
-    else:  # pragma: nocover
+    else:
         # Due to compatiblity with Python 3.9 and 3.10, we cannot use
         # t.assert_never here. That would be preferable, though.
         raise AssertionError("Invalid collection type passed!")  # type: ignore[unreachable, unused-ignore]
 
 
 def _collectiondict_for_counter(
     clct: t.Type[Counter[_HashableValueT]],
```

### Comparing `collectiondict-0.2.0/PKG-INFO` & `collectiondict-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 Metadata-Version: 2.1
 Name: collectiondict
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helpers to create dictionaries that collect values into collections
+Home-page: https://github.com/MaxG87/collectiondict/
 License: BSD-3-Clause
 Author: Max Görner
 Author-email: 5477952+MaxG87@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Project-URL: Changelog, https://github.com/MaxG87/collectiondict/releases/
+Project-URL: Repository, https://github.com/MaxG87/collectiondict/
+Description-Content-Type: text/markdown
+
+# collectiondict - Create multidicts more easily
+
+This package simplifies the creation of dictionaries which collect a stream of
+key-value-pairs into a dictionaries of containers. It is conceptunally similar
+to [multidict](https://pypi.org/project/multidict/) but much broader with
+respect to the supported types.
+
```

