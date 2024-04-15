# Comparing `tmp/envzy-0.2.3.tar.gz` & `tmp/envzy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envzy-0.2.3.tar", max compression
+gzip compressed data, was "envzy-0.2.4.tar", max compression
```

## Comparing `envzy-0.2.3.tar` & `envzy-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.2.3/AUTHORS
--rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.2.3/CONTRIBUTING
--rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.2.3/LICENSE
--rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.2.3/README.md
--rw-r--r--   0        0        0      375 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/__init__.py
--rw-r--r--   0        0        0     5487 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/auto.py
--rw-r--r--   0        0        0      541 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/base.py
--rw-r--r--   0        0        0    17568 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/classify.py
--rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/exceptions.py
--rw-r--r--   0        0        0      636 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/packages.py
--rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/py.typed
--rw-r--r--   0        0        0     4896 2024-01-26 11:07:00.879796 envzy-0.2.3/envzy/pypi.py
--rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.2.3/envzy/search.py
--rw-r--r--   0        0        0     8796 2024-01-26 11:07:00.883796 envzy-0.2.3/envzy/utils.py
--rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.2.3/envzy/version.py
--rw-r--r--   0        0        0     1369 2024-01-26 11:07:00.883796 envzy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.2.4/AUTHORS
+-rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.2.4/CONTRIBUTING
+-rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.2.4/README.md
+-rw-r--r--   0        0        0      375 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/__init__.py
+-rw-r--r--   0        0        0     5487 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/auto.py
+-rw-r--r--   0        0        0      541 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/base.py
+-rw-r--r--   0        0        0    17568 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/classify.py
+-rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/exceptions.py
+-rw-r--r--   0        0        0      636 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/packages.py
+-rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/py.typed
+-rw-r--r--   0        0        0     4896 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/pypi.py
+-rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.2.4/envzy/search.py
+-rw-r--r--   0        0        0     8969 2024-04-15 08:19:12.388985 envzy-0.2.4/envzy/utils.py
+-rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.2.4/envzy/version.py
+-rw-r--r--   0        0        0     1369 2024-04-15 08:20:00.149436 envzy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.2.4/PKG-INFO
```

### Comparing `envzy-0.2.3/CONTRIBUTING` & `envzy-0.2.4/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/LICENSE` & `envzy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/README.md` & `envzy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/auto.py` & `envzy-0.2.4/envzy/auto.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/base.py` & `envzy-0.2.4/envzy/base.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/classify.py` & `envzy-0.2.4/envzy/classify.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/packages.py` & `envzy-0.2.4/envzy/packages.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/pypi.py` & `envzy-0.2.4/envzy/pypi.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/search.py` & `envzy-0.2.4/envzy/search.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.3/envzy/utils.py` & `envzy-0.2.4/envzy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,17 +216,20 @@
     if top_level_module_name == 'torch':
         if module_filename in ['torch.ops', '_ops.py', '_classes.py']:
             return True
     return False
 
 
 def is_lazy_module(module: types.ModuleType) -> bool:
+    module_package = getattr(module.__class__, '__module__', None)
+    module_name = type(module).__name__
     return (
-        getattr(module.__class__, '__module__', None) == 'tensorboard.lazy' and
-        type(module).__name__ == 'LazyModule'
+        (module_package == 'tensorboard.lazy' and module_name == 'LazyModule')
+        or
+        (module_package == 'tensorflow.python.util.lazy_loader' and module_name == 'KerasLazyLoader')
     )
 
 
 def get_distribution_files(distribution: Distribution) -> Tuple[Path, ...]:
     try:
         # NB: TODO: distribution.files could be empty in case of
         # dist-packages & .egg-info.
```

### Comparing `envzy-0.2.3/pyproject.toml` & `envzy-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envzy"
-version = "0.2.3"
+version = "0.2.4"
 description = "A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies."
 license = "Apache-2.0"
 authors = ["Vladimir Lipkin <lipkin@yandex-team.ru>"]
 readme = "README.md"
 homepage = "https://github.com/lambdazy/envzy"
 repository = "https://github.com/lambdazy/envzy"
 include = ["AUTHORS", "CONTRIBUTING"]
```

### Comparing `envzy-0.2.3/PKG-INFO` & `envzy-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envzy
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies.
 Home-page: https://github.com/lambdazy/envzy
 License: Apache-2.0
 Author: Vladimir Lipkin
 Author-email: lipkin@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

