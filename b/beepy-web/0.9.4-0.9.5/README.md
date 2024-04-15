# Comparing `tmp/beepy_web-0.9.4.tar.gz` & `tmp/beepy_web-0.9.5.tar.gz`

## Comparing `beepy_web-0.9.4.tar` & `beepy_web-0.9.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.env.template
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.python-version
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.4/requirements.txt
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/__init__.py
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/attrs.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/children.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/components.py
--rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/context.py
--rw-r--r--   0        0        0    21111 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/framework.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/listeners.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/router.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/style.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/tags.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/trackable.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/types.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/__init__.py
--rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/__main__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/actions.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/plot.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/table.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/internal.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/js_py.py
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 beepy_web-0.9.4/scripts/publish.sh
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/package-lock.json
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.4/LICENSE
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.4/README.md
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 beepy_web-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.5/.env.template
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.5/.python-version
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.5/requirements.txt
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/__init__.py
+-rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/attrs.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/children.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/components.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/context.py
+-rw-r--r--   0        0        0    21151 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/listeners.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/router.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/style.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/trackable.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/dev/__init__.py
+-rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/table.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.5/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.5/scripts/publish.sh
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/package-lock.json
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/webpack.prod.js
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.5/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.5/README.md
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 beepy_web-0.9.5/PKG-INFO
```

### Comparing `beepy_web-0.9.4/.pre-commit-config.yaml` & `beepy_web-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/__init__.py` & `beepy_web-0.9.5/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/attrs.py` & `beepy_web-0.9.5/beepy/attrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
                 if _prevent_model and _prevent_model in (True, self) and handler.__name__.startswith('@attr'):
                     continue
                 call_handler_with_optional_arguments(handler, instance, {'value': value})
 
         if self.notify:
             instance.__notify__(self.name, self, value)
 
-    def _set_first_value(self, instance, value, parent):
+    def _set_first_value(self, instance, value, parent):  # noqa: ARG002 - unused `parent
         if self.model and (
             isinstance(value, attr) and value.name is not None and (instance, self, None) not in value._from_model_cache
         ):
             value._from_model_cache.append((instance, self, value.name))
             instance._kwargs.pop(self.name)
 
     def _fset(self, instance, value):
```

### Comparing `beepy_web-0.9.4/beepy/children.py` & `beepy_web-0.9.5/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/components.py` & `beepy_web-0.9.5/beepy/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 return self._ref
             else:
                 raise TypeError(f'Component {self._context_name_} already is child')
         ref = beepy.children.ComponentRef(self)
         self._set_ref(parent, ref)
         return ref
 
-    def _set_ref(self, parent: Tag | None, ref: ComponentRef):
+    def _set_ref(self, parent: Tag | None, ref: ComponentRef):  # noqa: ARG002 - unused `parent
         self._ref = ref
 
     def _clone(self, parent=None) -> Self:
         clone = super()._clone(parent=parent)
         clone._listeners = defaultdict(list, **nested_copy(self._listeners))
         clone._handlers = defaultdict(list, **nested_copy(self._handlers))
         return clone
```

### Comparing `beepy_web-0.9.4/beepy/context.py` & `beepy_web-0.9.5/beepy/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 import enum
 from abc import ABCMeta
 from typing import TYPE_CHECKING, TypeVar
 
-from boltons.typeutils import make_sentinel
-
 import beepy
 from beepy.attrs import attr
 from beepy.utils import js
 from beepy.utils.common import get_random_name, log10_ceil, to_kebab_case
 from beepy.utils.js_py import Interval, create_once_callable
 
 if TYPE_CHECKING:
```

### Comparing `beepy_web-0.9.4/beepy/framework.py` & `beepy_web-0.9.5/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __CONFIG__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
-__version__ = '0.9.4'  # For internal development set to 0.0a0
+__version__ = '0.9.5'  # For internal development set to 0.0a0
 __CONFIG__['version'] = __version__
 
 
 _TAG_INITIALIZED = False
 
 
 class _MetaTag(_MetaComponent):
@@ -111,15 +111,15 @@
                         ref_children.append(_ref)
 
                     if isinstance(child, ChildRef) and child.child._force_ref:
                         children_arg.insert(0, child)
                         ref_children.append(child)
 
             for _index, child in enumerate(children_arg):
-                if isinstance(child, str):
+                if isinstance(child, str) and not isinstance(child, SpecialChild):
                     children_arg[_index] = StringWrapper(child)
 
                 if isinstance(child, Component) and child not in ref_children:
                     # TODO: replace 5 in get_random_name(5) with some log
                     children_arg[_index] = namespace[f'_{get_random_name(5)}_'] = child._as_child(None)
 
         cls: type[Tag] | type = super().__new__(mcs, _name, bases, namespace, **kwargs)
```

### Comparing `beepy_web-0.9.4/beepy/listeners.py` & `beepy_web-0.9.5/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/router.py` & `beepy_web-0.9.5/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/style.py` & `beepy_web-0.9.5/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/tags.py` & `beepy_web-0.9.5/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/trackable.py` & `beepy_web-0.9.5/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/types.py` & `beepy_web-0.9.5/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/dev/__main__.py` & `beepy_web-0.9.5/beepy/dev/__main__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/modules/context_menu.py` & `beepy_web-0.9.5/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/modules/local_storage.py` & `beepy_web-0.9.5/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/modules/modal.py` & `beepy_web-0.9.5/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/modules/table.py` & `beepy_web-0.9.5/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/modules/tabs.py` & `beepy_web-0.9.5/beepy/modules/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/api.py` & `beepy_web-0.9.5/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/asyncio.py` & `beepy_web-0.9.5/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/common.py` & `beepy_web-0.9.5/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/dev.py` & `beepy_web-0.9.5/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/import_hooks.py` & `beepy_web-0.9.5/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/internal.py` & `beepy_web-0.9.5/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/js.py` & `beepy_web-0.9.5/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/beepy/utils/js_py.py` & `beepy_web-0.9.5/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/scripts/publish.sh` & `beepy_web-0.9.5/scripts/publish.sh`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 cd ..
 
 
 ### Python part ###
 # Create dist/* files
 hatch build
 # Actual publishing
-twine upload "dist/*$new_version[-.]*"
+twine upload "dist/*$2[-.]*"
```

### Comparing `beepy_web-0.9.4/web/package-lock.json` & `beepy_web-0.9.5/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.5'}}", "'version'": "'0.9.5'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.4"
+            "version": "0.9.5"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.9.4"
+    "version": "0.9.5"
 }
```

### Comparing `beepy_web-0.9.4/web/package.json` & `beepy_web-0.9.5/web/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.5'"}*

```diff
@@ -31,9 +31,9 @@
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.4"
+    "version": "0.9.5"
 }
```

### Comparing `beepy_web-0.9.4/web/webpack.prod.js` & `beepy_web-0.9.5/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/web/src/beepy.js` & `beepy_web-0.9.5/web/src/beepy.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.4'
+    __version__ = '0.9.5'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.9.4/web/src/dev-server.js` & `beepy_web-0.9.5/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/web/src/files.js` & `beepy_web-0.9.5/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/web/src/main.css` & `beepy_web-0.9.5/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/web/src/python.js` & `beepy_web-0.9.5/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/web/src/utils.js` & `beepy_web-0.9.5/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/.gitignore` & `beepy_web-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/LICENSE` & `beepy_web-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/README.md` & `beepy_web-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/pyproject.toml` & `beepy_web-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.4/PKG-INFO` & `beepy_web-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.4
+Version: 0.9.5
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://kor0p.github.io/BeePy/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

