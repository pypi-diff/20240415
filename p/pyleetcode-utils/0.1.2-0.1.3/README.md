# Comparing `tmp/pyleetcode_utils-0.1.2.tar.gz` & `tmp/pyleetcode_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleetcode_utils-0.1.2.tar", max compression
+gzip compressed data, was "pyleetcode_utils-0.1.3.tar", max compression
```

## Comparing `pyleetcode_utils-0.1.2.tar` & `pyleetcode_utils-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1098 2024-03-17 13:37:38.266351 pyleetcode_utils-0.1.2/LICENSE
--rw-r--r--   0        0        0     1371 2024-03-17 13:37:38.266351 pyleetcode_utils-0.1.2/README.md
--rw-r--r--   0        0        0       12 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/datatypes/__init__.py
--rw-r--r--   0        0        0     1615 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/datatypes/tree.py
--rw-r--r--   0        0        0        0 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/examples/__init__.py
--rw-r--r--   0        0        0      918 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/examples/tree.py
--rw-r--r--   0        0        0       90 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyleetcode_utils/py.typed
--rw-r--r--   0        0        0     1126 2024-03-17 13:37:38.270351 pyleetcode_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 pyleetcode_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1371 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       12 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/datatypes/__init__.py
+-rw-r--r--   0        0        0     1611 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/datatypes/tree.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/examples/__init__.py
+-rw-r--r--   0        0        0      918 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/examples/tree.py
+-rw-r--r--   0        0        0       90 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyleetcode_utils/py.typed
+-rw-r--r--   0        0        0     1132 2024-04-15 21:53:27.516021 pyleetcode_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 pyleetcode_utils-0.1.3/PKG-INFO
```

### Comparing `pyleetcode_utils-0.1.2/LICENSE` & `pyleetcode_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleetcode_utils-0.1.2/README.md` & `pyleetcode_utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyleetcode_utils-0.1.2/pyleetcode_utils/datatypes/tree.py` & `pyleetcode_utils-0.1.3/pyleetcode_utils/datatypes/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,12 +41,12 @@
         tree_arg = (_make_tree(args[1]),)
         return start_args + tree_arg + end_args
 
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         try:
             new_args = prepare_new_args(args, **kwargs)
-            return func(*new_args, **kwargs)
         except Exception:
             raise exceptions.NotBinaryTreeError('Not valid binary tree has been provided!')
+        return func(*new_args, **kwargs)
 
     return wrapper  # type: ignore[return-value]
```

### Comparing `pyleetcode_utils-0.1.2/pyleetcode_utils/examples/tree.py` & `pyleetcode_utils-0.1.3/pyleetcode_utils/examples/tree.py`

 * *Files identical despite different names*

### Comparing `pyleetcode_utils-0.1.2/pyproject.toml` & `pyleetcode_utils-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pyleetcode-utils"
 description = "Python Leetcode utilities"
-version = "0.1.2"
+version = "0.1.3"
 license = "MIT"
 
 authors = ["Vadim Gazizov <i.am.vadim.gazizov@gmail.com>"]
 
 readme = "README.md"
 
 repository = "https://github.com/smokevadim/pyleetcode-utils"
@@ -26,15 +26,15 @@
 mypy = "^1.8"
 
 wemake-python-styleguide = "^0.18"
 flake8-pytest-style = "^1.6"
 nitpick = "^0.35"
 
 pytest = "^8.0"
-pytest-cov = "^4.1"
+pytest-cov = ">=4.1,<6.0"
 pytest-randomly = "^3.15"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.1"
```

### Comparing `pyleetcode_utils-0.1.2/PKG-INFO` & `pyleetcode_utils-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleetcode-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Leetcode utilities
 Home-page: https://github.com/smokevadim/pyleetcode-utils
 License: MIT
 Author: Vadim Gazizov
 Author-email: i.am.vadim.gazizov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

