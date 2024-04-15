# Comparing `tmp/pypotage-0.1.1a0.tar.gz` & `tmp/pypotage-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotage-0.1.1a0.tar", last modified: Mon Apr  8 20:12:32 2024, max compression
+gzip compressed data, was "pypotage-0.1.2a0.tar", last modified: Mon Apr 15 14:49:47 2024, max compression
```

## Comparing `pypotage-0.1.1a0.tar` & `pypotage-0.1.2a0.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.274870 pypotage-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 20:12:32.274870 pypotage-0.1.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/pypotage/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_chef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/_pot.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/src/pypotage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/src/pypotage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 20:12:32.000000 pypotage-0.1.1a0/src/pypotage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:12:32.270870 pypotage-0.1.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_abstract_ingredients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_listchef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-08 20:12:23.000000 pypotage-0.1.1a0/tests/test_pot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.586138 pypotage-0.1.2a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.586138 pypotage-0.1.2a0/src/pypotage/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_chef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/_pot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/src/pypotage/chefs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/genericChef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/chefs/listChef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/src/pypotage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/src/pypotage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 14:49:47.000000 pypotage-0.1.2a0/src/pypotage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:49:47.590139 pypotage-0.1.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_abstract_ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_genericchef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_listchef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_nocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_pot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-15 14:49:41.000000 pypotage-0.1.2a0/tests/test_preparechefline.py
```

### Comparing `pypotage-0.1.1a0/PKG-INFO` & `pypotage-0.1.2a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pypotage-0.1.1a0/setup.cfg` & `pypotage-0.1.2a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pypotage
-version = v0.1.1-alpha
+version = v0.1.2-alpha
 author = Pavalso
 author_email = author@example.com
 description = Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pavalso/potage
 project_urls = 
@@ -14,15 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pypotage-0.1.1a0/src/pypotage/_pot.py` & `pypotage-0.1.2a0/src/pypotage/_pot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,92 @@
 from typing import Callable, Type, TypeVar
 from functools import cache
 from math import inf
 
 from .chefs.listChef import ListChef
-
-from ._ingredient import _Ingredient, _IngredientProxy, _IngredientData
+from .chefs.genericChef import GenericChef
+from ._ingredient import (
+    Ingredient,
+    _OrderedIngredientProxy,
+    IngredientProxy,
+    IngredientData,
+    NoCallIngredient
+)
 from .utils import traverse_subclasses
 from ._chef import Chef
 
 
 _B = TypeVar("_B")
 
 
 class _Pot:
 
-    ingredients: dict[Type, list[_Ingredient]]
+    ingredients: dict[Type, list[Ingredient]]
     chefs: list[Chef]
 
     def __init__(self) -> None:
-        self.ingredients: dict[Type, list[_Ingredient]] = {}
+        self.ingredients: dict[Type, list[Ingredient]] = {}
         self.chefs: list[Chef] = [
             ListChef(),
+            GenericChef()
         ]
 
-    def create(self, func: Callable, /, **kwargs) -> _Ingredient:
-        return _Ingredient(_c=cache(func), **kwargs)
+    def create(self, func: Callable, /,
+               _ingredient: Type[Ingredient],
+               **kwargs) -> Ingredient:
+        ingredient = _ingredient(
+            _c=cache(func),
+            formula=IngredientData(**kwargs))
+        ingredient.formula._type = ingredient.type
+        return ingredient
 
-    def add(self, ingredient: _Ingredient, _id: str) -> _Ingredient:
-        (_l := self.ingredients.setdefault((ingredient.type, _id), [])) \
-            .insert(0, ingredient)
-        list.sort(_l, key=lambda _b: _b.priority)
+    def add(self, ingredient: Ingredient) -> Ingredient:
+        _l = self.ingredients.setdefault(
+            (ingredient.formula._type, ingredient.formula._id), [])
+        _l.insert(0, ingredient)
         return ingredient
 
-    def get(self, _type: Type, _id: str) -> _Ingredient:
-        classes = [_type]
-        classes.extend(traverse_subclasses(_type))
+    def get(self, formula: IngredientData) -> Ingredient:
+        classes = [formula._type]
+        classes.extend(traverse_subclasses(formula._type))
 
         ingredients = []
 
         for _type in classes:
-            if (ingredient := self.ingredients.get((_type, _id))) is not None:
+            ingredient = self.ingredients.get((_type, formula._id))
+            if ingredient is not None:
                 ingredients.extend(ingredient)
 
-        list.sort(ingredients, key=lambda ingredient: ingredient.priority)
-
         return ingredients
 
     def prepare(self, _f: _B = None, /,
                 lazy: bool = False, order: int = inf,
-                primary: bool = False, _id: str = None) -> _B:
-        def _wrapper(_f) -> _Ingredient:
+                primary: bool = False, _id: str = None,
+                no_call: bool = False) -> _B:
+        def _wrapper(_f) -> Ingredient:
             ingredient = self.create(
-                _f, lazy=lazy, order=order, primary=primary)
-            self.add(ingredient, _id=_id)
+                _f, lazy=lazy,
+                _ingredient=NoCallIngredient if no_call else Ingredient,
+                order=order, primary=primary,
+                _id=_id)
+
+            for chef in self.chefs:
+                ingredient = chef.prepare(ingredient)
+
+            self.add(ingredient)
             return _f
         return _wrapper(_f) if _f is not None else _wrapper
 
-    def cook(self, _type: _B, _id: str = None) -> _IngredientProxy[_B]:
+    def cook(self, _type: _B, _id: str = None) -> IngredientProxy[_B]:
         if not (_t := getattr(_type, "type", None)):
             _t = _type
 
-        chef_line = _IngredientProxy(
+        chef_line = _OrderedIngredientProxy(
             _f=self.get,
-            formula=_IngredientData(_type=_t, _id=_id))
+            formula=IngredientData(_type=_t, _id=_id))
 
         for chef in self.chefs:
             chef_line = chef.cook(chef_line)
 
         return chef_line
```

### Comparing `pypotage-0.1.1a0/src/pypotage.egg-info/PKG-INFO` & `pypotage-0.1.2a0/src/pypotage.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypotage
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: Beans is a simple and lightweight Python library based on Spring Framework. It provides a simple way to manage beans and their dependencies.
 Home-page: https://github.com/pavalso/potage
 Author: Pavalso
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pavalso/potage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pypotage-0.1.1a0/tests/test_abstract_ingredients.py` & `pypotage-0.1.2a0/tests/test_abstract_ingredients.py`

 * *Files identical despite different names*

### Comparing `pypotage-0.1.1a0/tests/test_listchef.py` & `pypotage-0.1.2a0/tests/test_listchef.py`

 * *Files identical despite different names*

### Comparing `pypotage-0.1.1a0/tests/test_pot.py` & `pypotage-0.1.2a0/tests/test_pot.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 
 
 def test_cook_lazy():
     class Bean:
         def __init__(self):
             raise Exception("Should be called on take_out() (On lazy beans)")
 
+    def bean():
+        return Bean()
+
+    pytest.raises(Exception, pypotage.prepare, bean)
+
     @pypotage.prepare(lazy=True)
-    def bean() -> str:
+    def bean() -> Bean:
         return Bean()
 
-    assert pypotage.cook(str).is_present()
-    pytest.raises(Exception, pypotage.cook(str).take_out)
-    pytest.raises(Exception, pypotage.prepare, Bean)
+    assert pypotage.cook(Bean).is_present()
+    pytest.raises(Exception, pypotage.cook(Bean).take_out)
```

