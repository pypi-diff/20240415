# Comparing `tmp/guitool_ibeis-2.1.2.tar.gz` & `tmp/guitool_ibeis-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitool_ibeis-2.1.2.tar", last modified: Sun Jan 29 01:20:29 2023, max compression
+gzip compressed data, was "guitool_ibeis-2.2.0.tar", last modified: Mon Apr 15 15:21:48 2024, max compression
```

## Comparing `guitool_ibeis-2.1.2.tar` & `guitool_ibeis-2.2.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1915 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/guitool_ibeis/
--rw-r--r--   0 runner    (1001) docker     (123)    40884 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/PrefWidget2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18696 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/PreferenceWidget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/QtCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/QtGui.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/QtTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/QtWidgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/_internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3744 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7686 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_button_delegate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44250 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_item_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16478 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_item_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20647 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_item_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6323 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_table_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27115 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_thumb_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_timestamp_delegate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14384 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_tree_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6225 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/api_tree_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4238 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/filter_proxy_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104479 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_components.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3638 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_delegates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25911 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_dialogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7267 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7968 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15472 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/guitool_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/mpl_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/mpl_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/qt_enums.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5899 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/qtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5464 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/stripe_proxy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/guitool_ibeis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/guitool_ibeis/tests/test_treenode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-01-29 01:20:29.000000 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-29 01:20:29.000000 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 01:20:29.000000 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-01-29 01:20:29.000000 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-29 01:20:29.000000 guitool_ibeis-2.1.2/guitool_ibeis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 01:20:29.053601 guitool_ibeis-2.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9234 2023-01-29 01:20:23.000000 guitool_ibeis-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.308434 guitool_ibeis-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31022 2024-04-15 15:21:48.308434 guitool_ibeis-2.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1915 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.260434 guitool_ibeis-2.2.0/guitool_ibeis/
+-rw-r--r--   0 runner    (1001) docker     (127)    40910 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/PrefWidget2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18696 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/PreferenceWidget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.260434 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/QtCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/QtGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/QtTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/QtWidgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1233 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/_internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7686 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_button_delegate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44250 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_item_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16464 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_item_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20565 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_item_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6323 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_table_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27115 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_thumb_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_timestamp_delegate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14343 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_tree_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6225 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/api_tree_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4238 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/filter_proxy_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104438 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_components.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3638 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_delegates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25885 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_dialogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7267 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7940 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15439 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/guitool_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/mpl_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/mpl_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/qt_enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5899 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/qtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5464 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/stripe_proxy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.260434 guitool_ibeis-2.2.0/guitool_ibeis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2693 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/guitool_ibeis/tests/test_treenode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.260434 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31022 2024-04-15 15:21:48.000000 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-15 15:21:48.000000 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:21:48.000000 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-15 15:21:48.000000 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 15:21:48.000000 guitool_ibeis-2.2.0/guitool_ibeis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:21:48.308434 guitool_ibeis-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9806 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:21:48.260434 guitool_ibeis-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 15:20:44.000000 guitool_ibeis-2.2.0/tests/test_import.py
```

### Comparing `guitool_ibeis-2.1.2/LICENSE` & `guitool_ibeis-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/README.rst` & `guitool_ibeis-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/PrefWidget2.py` & `guitool_ibeis-2.2.0/guitool_ibeis/PrefWidget2.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,15 +752,16 @@
             for child in self.children:
                 if child.name in cfg:
                     child_cfg = cfg[child.name]
                     child._set_to_external(child_cfg)
 
     def iter_children(self):
         if self.children is None:
-            raise StopIteration()
+            return None
+            # raise StopIteration()
         for child in self.children:
             yield child
 
     @property
     def type_(self):
         return None if self.param_info is None else self.param_info.type_
 
@@ -976,15 +977,15 @@
         self.vbox.addWidget(self.tree_view)
         if self._with_buttons:
             self.vbox.addLayout(self.hbox)
         self.setWindowTitle(_translate('self', 'Edit Config Widget', None))
 
     def init_mvc(self):
         import operator
-        from six.moves import reduce
+        from functools import reduce
         edit_triggers = reduce(operator.__or__, [
             QtWidgets.QAbstractItemView.CurrentChanged,
             QtWidgets.QAbstractItemView.DoubleClicked,
             QtWidgets.QAbstractItemView.SelectedClicked,
             # QtWidgets.QAbstractItemView.EditKeyPressed,
             # QtWidgets.QAbstractItemView.AnyKeyPressed,
         ])
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/PreferenceWidget.py` & `guitool_ibeis-2.2.0/guitool_ibeis/PreferenceWidget.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/__init__.py` & `guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/__init__.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/__PYQT__/_internal.py` & `guitool_ibeis-2.2.0/guitool_ibeis/__PYQT__/_internal.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/__init__.py` & `guitool_ibeis-2.2.0/guitool_ibeis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.1.2'
+__version__ = '2.2.0'
 
 import utool as ut
 ut.noinject(__name__, '[guitool_ibeis.__init__]')
 
 from guitool_ibeis import __PYQT__  # NOQA
 
 from guitool_ibeis import api_item_model  # NOQA
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_button_delegate.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_button_delegate.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_item_model.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_item_model.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_item_view.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_item_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from guitool_ibeis.__PYQT__.QtCore import Qt
 import functools
 from guitool_ibeis import qtype
 from guitool_ibeis import api_button_delegate
 from guitool_ibeis import api_thumb_delegate
 from guitool_ibeis import guitool_main
 from guitool_ibeis import guitool_misc
-from six.moves import range, reduce  # NOQA
 import utool
 import utool as ut
 import operator
+from functools import reduce
 # Valid API Models
 from guitool_ibeis.stripe_proxy_model import StripeProxyModel
 from guitool_ibeis.filter_proxy_model import FilterProxyModel
 from guitool_ibeis.api_item_model import APIItemModel
 
 (print, rrr, profile) = utool.inject2(__name__, '[APIItemView]')
 
@@ -392,15 +392,15 @@
     """ QtOverride: Returns item delegate for this index """
     # Does this even work? TODO: testme
     return API_VIEW_BASE.itemDelegate(view, qindex)
 
 
 def setModel(view, model):
     """ QtOverride: Returns item delegate for this index """
-    assert isinstance(model, VALID_API_MODELS),\
+    assert isinstance(model, VALID_API_MODELS), \
             ('APIItemViews only accepts APIItemModels (or one of its proxys),'
              'received a %r' % type(model))
     # Learn some things about the model before you fully connect it.
     if VERBOSE:
         print('[view] setting model')
     model._rows_updated.connect(view.on_rows_updated)
     #view.infer_delegates_from_model(model=model)
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_item_widget.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_item_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 """
 from __future__ import absolute_import, division, print_function
 from guitool_ibeis.__PYQT__ import QtCore
 from guitool_ibeis.__PYQT__ import QtWidgets
 from guitool_ibeis.api_item_model import APIItemModel
 from guitool_ibeis.api_table_view import APITableView
 from guitool_ibeis.api_tree_view import APITreeView
-#from guitool_ibeis import guitool_components as comp
 from functools import partial
-from six.moves import range
 import utool as ut
 import six
 (print, rrr, profile) = ut.inject2(__name__, '[APIItemWidget]')
 
 
 WIDGET_BASE = QtWidgets.QWidget
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_table_view.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_table_view.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_thumb_delegate.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_thumb_delegate.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_timestamp_delegate.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_timestamp_delegate.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_tree_node.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_tree_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # TODO: Rename api_item_model
 from __future__ import absolute_import, division, print_function
-from guitool_ibeis.__PYQT__ import QtCore  # NOQA
+from guitool_ibeis.__PYQT__ import QtCore
 from types import GeneratorType
-from six.moves import zip, range
 import utool
 import utool as ut
 (print, print_, rrr) = utool.inject2(__name__)
 
 
 TREE_NODE_BASE = QtCore.QObject
 #TREE_NODE_BASE = object
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/api_tree_view.py` & `guitool_ibeis-2.2.0/guitool_ibeis/api_tree_view.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/filter_proxy_model.py` & `guitool_ibeis-2.2.0/guitool_ibeis/filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_components.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, division, print_function
 import six
-from six.moves import map, range  # NOQA
 from guitool_ibeis.__PYQT__ import QtCore, QtGui
 from guitool_ibeis.__PYQT__ import QtWidgets
 from guitool_ibeis.__PYQT__.QtCore import Qt
 from guitool_ibeis.__PYQT__._internal import GUITOOL_PYQT_VERSION  # NOQA
 import utool as ut
 import ubelt as ub
 from guitool_ibeis import guitool_dialogs
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_decorators.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_decorators.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_delegates.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_delegates.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_dialogs.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import absolute_import, division, print_function
-from six.moves import map
 from guitool_ibeis.__PYQT__ import QtCore, QtGui  # NOQA
 from guitool_ibeis.__PYQT__ import QtWidgets  # NOQA
 from guitool_ibeis.__PYQT__.QtCore import Qt
 import os
 from os.path import dirname
 import platform
 from utool import util_cache, util_path
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_main.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_main.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_misc.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import, division, print_function
 from guitool_ibeis.__PYQT__ import QtCore, QtGui
 from guitool_ibeis.__PYQT__ import QtWidgets  # NOQA
 import six
 import utool
 import sys
 import logging
-from six.moves import range
 from guitool_ibeis.guitool_decorators import slot_
 from guitool_ibeis import guitool_main
 import utool as ut
 ut.noinject(__name__)
 
 
 # For some reason QtCore.Qt.ALT doesn't work right
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/guitool_tables.py` & `guitool_ibeis-2.2.0/guitool_ibeis/guitool_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # DEPRICATE?
 from __future__ import absolute_import, division, print_function
 from guitool_ibeis.__PYQT__ import QtCore, QtGui
 from guitool_ibeis.__PYQT__ import QtWidgets
 from guitool_ibeis.__PYQT__.QtCore import Qt
 from guitool_ibeis.guitool_delegates import ComboDelegate, ButtonDelegate
 from guitool_ibeis import qtype
-from six.moves import range, map
 import utool
 (print, rrr, profile) = utool.inject2(__name__)
 
 
 class ColumnListTableView(QtWidgets.QTableView):
     """ Table View for an AbstractItemModel """
     def __init__(view, *args, **kwargs):
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/mpl_embed.py` & `guitool_ibeis-2.2.0/guitool_ibeis/mpl_embed.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/mpl_widget.py` & `guitool_ibeis-2.2.0/guitool_ibeis/mpl_widget.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/qt_enums.py` & `guitool_ibeis-2.2.0/guitool_ibeis/qt_enums.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/qtype.py` & `guitool_ibeis-2.2.0/guitool_ibeis/qtype.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/stripe_proxy_model.py` & `guitool_ibeis-2.2.0/guitool_ibeis/stripe_proxy_model.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis/tests/test_treenode.py` & `guitool_ibeis-2.2.0/guitool_ibeis/tests/test_treenode.py`

 * *Files identical despite different names*

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis.egg-info/SOURCES.txt` & `guitool_ibeis-2.2.0/guitool_ibeis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 guitool_ibeis/__PYQT__/QtCore.py
 guitool_ibeis/__PYQT__/QtGui.py
 guitool_ibeis/__PYQT__/QtTest.py
 guitool_ibeis/__PYQT__/QtWidgets.py
 guitool_ibeis/__PYQT__/__init__.py
 guitool_ibeis/__PYQT__/_internal.py
 guitool_ibeis/tests/__init__.py
-guitool_ibeis/tests/test_treenode.py
+guitool_ibeis/tests/test_treenode.py
+tests/test_import.py
```

### Comparing `guitool_ibeis-2.1.2/guitool_ibeis.egg-info/requires.txt` & `guitool_ibeis-2.2.0/guitool_ibeis.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,196 +1,271 @@
-six
-ubelt
-utool
-vtool_ibeis
+ubelt>=1.3.4
+utool>=2.2.0
+vtool_ibeis>=2.2.0
 
 [:python_version < "3.10" and python_version >= "3.9"]
-cachetools
-matplotlib
+matplotlib>=3.3.3
+cachetools>=4.2.0
 
 [:python_version < "3.11" and python_version >= "3.10"]
-cachetools
-matplotlib
+matplotlib>=3.5.0
+cachetools>=5.0.0
+
+[:python_version < "3.12"]
+six>=1.10.0
+
+[:python_version < "3.12" and python_version >= "2.7"]
+pyqt5>=5.15.5
+
+[:python_version < "3.12" and python_version >= "3.11"]
+matplotlib>=3.5.0
 
 [:python_version < "3.7" and python_version >= "3.6"]
-cachetools
-matplotlib
+matplotlib>=1.5.3
+cachetools>=4.0.0
 
 [:python_version < "3.8" and python_version >= "3.7"]
-cachetools
-matplotlib
+matplotlib>=2.2.2
+cachetools>=5.0.0
 
 [:python_version < "3.9" and python_version >= "3.8"]
-cachetools
-matplotlib
+matplotlib>=3.6.0
+cachetools>=4.0.0
 
 [:python_version < "4.0" and python_version >= "3.11"]
-cachetools
-matplotlib
+cachetools>=5.0.0
 
-[:python_version > "2.7"]
-pyqt5
+[:python_version < "4.0" and python_version >= "3.12"]
+six>=1.16.0
+matplotlib>=3.8.4
+pyqt5>=5.15.10
 
 [all]
-codecov
-pytest-timeout
-six
-ubelt
-utool
-vtool_ibeis
-xdoctest
+ubelt>=1.3.4
+utool>=2.2.0
+vtool_ibeis>=2.2.0
+xdoctest>=1.1.3
+setuptools>=34.1.0
+wheel
+scikit-build
+cmake
+ninja
 
 [all-strict]
-codecov==2.0.15
-pytest-timeout==1.4.2
-six==1.10.0
-ubelt==1.2.2
-utool==2.1.6
+ubelt==1.3.4
+utool==2.2.0
 vtool_ibeis==2.2.0
-xdoctest==0.14.0
+xdoctest==1.1.3
+setuptools==34.1.0
+wheel
+scikit-build
+cmake
+ninja
 
 [all-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [all-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.10" and python_version >= "3.9"]
+matplotlib==3.3.3
 cachetools==4.2.0
+pytest==8.1.1
 coverage==5.3.1
-matplotlib==3.3.3
-
-[all-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
 
 [all-strict:python_version < "3.11" and python_version >= "3.10"]
+matplotlib==3.5.0
 cachetools==5.0.0
+pytest==8.1.1
+coverage==6.1.1
+
+[all-strict:python_version < "3.12"]
+six==1.10.0
+pytest_timeout==1.4.2
+
+[all-strict:python_version < "3.12" and python_version >= "2.7"]
+pyqt5==5.15.5
+
+[all-strict:python_version < "3.12" and python_version >= "3.11"]
 matplotlib==3.5.0
+pytest==8.1.1
+coverage==7.0.0
+
+[all-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [all-strict:python_version < "3.4" and python_version >= "2.7"]
 coverage==5.3.1
 
 [all-strict:python_version < "3.5" and python_version >= "3.4"]
 coverage==4.3.4
 
 [all-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.6" and python_version >= "3.5"]
 coverage==5.3.1
 
 [all-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [all-strict:python_version < "3.7" and python_version >= "3.6"]
+matplotlib==1.5.3
 cachetools==4.0.0
 coverage==6.1.1
-matplotlib==1.5.3
-
-[all-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
 
 [all-strict:python_version < "3.8" and python_version >= "3.7"]
+matplotlib==2.2.2
 cachetools==5.0.0
+pytest==4.6.0
 coverage==6.1.1
-matplotlib==2.2.2
 
 [all-strict:python_version < "3.9" and python_version >= "3.8"]
+matplotlib==3.6.0
 cachetools==4.0.0
+pytest==8.1.1
 coverage==6.1.1
-matplotlib==3.6.0
 
 [all-strict:python_version < "4.0" and python_version >= "3.11"]
 cachetools==5.0.0
-matplotlib==3.5.0
 
-[all-strict:python_version > "2.7"]
-pyqt5==5.15.5
+[all-strict:python_version < "4.0" and python_version >= "3.12"]
+six==1.16.0
+matplotlib==3.8.4
+pyqt5==5.15.10
+pytest_timeout==2.3.1
+coverage==7.3.0
 
-[all-strict:python_version >= "3.10"]
-coverage==6.1.1
-
-[all-strict:python_version >= "3.10.0"]
-pytest==6.2.5
+[all-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [all:python_version < "2.7" and python_version >= "2.6"]
-coverage
+coverage>=4.5
 
 [all:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.10" and python_version >= "3.9"]
-cachetools
-coverage
-matplotlib
-
-[all:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+matplotlib>=3.3.3
+cachetools>=4.2.0
+pytest>=8.1.1
+coverage>=5.3.1
 
 [all:python_version < "3.11" and python_version >= "3.10"]
-cachetools
-matplotlib
+matplotlib>=3.5.0
+cachetools>=5.0.0
+pytest>=8.1.1
+coverage>=6.1.1
+
+[all:python_version < "3.12"]
+six>=1.10.0
+pytest_timeout>=1.4.2
+
+[all:python_version < "3.12" and python_version >= "2.7"]
+pyqt5>=5.15.5
+
+[all:python_version < "3.12" and python_version >= "3.11"]
+matplotlib>=3.5.0
+pytest>=8.1.1
+coverage>=7.0.0
+
+[all:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [all:python_version < "3.4" and python_version >= "2.7"]
-coverage
+coverage>=5.3.1
 
 [all:python_version < "3.5" and python_version >= "3.4"]
-coverage
+coverage>=4.3.4
 
 [all:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.6" and python_version >= "3.5"]
-coverage
+coverage>=5.3.1
 
 [all:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [all:python_version < "3.7" and python_version >= "3.6"]
-cachetools
-coverage
-matplotlib
-
-[all:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+matplotlib>=1.5.3
+cachetools>=4.0.0
+coverage>=6.1.1
 
 [all:python_version < "3.8" and python_version >= "3.7"]
-cachetools
-coverage
-matplotlib
+matplotlib>=2.2.2
+cachetools>=5.0.0
+pytest>=4.6.0
+coverage>=6.1.1
 
 [all:python_version < "3.9" and python_version >= "3.8"]
-cachetools
-coverage
-matplotlib
+matplotlib>=3.6.0
+cachetools>=4.0.0
+pytest>=8.1.1
+coverage>=6.1.1
 
 [all:python_version < "4.0" and python_version >= "3.11"]
-cachetools
-matplotlib
+cachetools>=5.0.0
 
-[all:python_version > "2.7"]
-pyqt5
+[all:python_version < "4.0" and python_version >= "3.12"]
+six>=1.16.0
+matplotlib>=3.8.4
+pyqt5>=5.15.10
+pytest_timeout>=2.3.1
+coverage>=7.3.0
 
-[all:python_version >= "3.10"]
-coverage
-
-[all:python_version >= "3.10.0"]
-pytest
+[all:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
 [all:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
+
+[build]
+setuptools>=34.1.0
+wheel
+scikit-build
+cmake
+ninja
+
+[build-strict]
+setuptools==34.1.0
+wheel
+scikit-build
+cmake
+ninja
+
+[docs]
+sphinx>=5.0.1
+sphinx-autobuild>=2021.3.14
+sphinx_rtd_theme>=1.0.0
+sphinxcontrib-napoleon>=0.7
+sphinx-autoapi>=1.8.4
+Pygments>=2.9.0
+myst_parser>=0.18.0
+sphinx-reredirects>=0.0.1
+
+[docs-strict]
+sphinx==5.0.1
+sphinx-autobuild==2021.3.14
+sphinx_rtd_theme==1.0.0
+sphinxcontrib-napoleon==0.7
+sphinx-autoapi==1.8.4
+Pygments==2.9.0
+myst_parser==0.18.0
+sphinx-reredirects==0.0.1
 
 [graphics]
 
 [graphics-strict]
 
 [graphics-strict:python_version < "3.10" and python_version >= "3.9"]
 opencv-python==3.4.15.55
@@ -216,39 +291,39 @@
 [graphics-strict:python_version < "3.9" and python_version >= "3.8"]
 opencv-python==3.4.15.55
 
 [graphics-strict:python_version < "4.0" and python_version >= "3.11"]
 opencv-python==4.5.5.64
 
 [graphics:python_version < "3.10" and python_version >= "3.9"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "3.11" and python_version >= "3.10"]
-opencv-python
+opencv-python>=4.5.4.58
 
 [graphics:python_version < "3.4" and python_version >= "2.7"]
-opencv-python
+opencv-python>=3.1.0.0
 
 [graphics:python_version < "3.5" and python_version >= "3.4"]
-opencv-python
+opencv-python>=3.1.0.5
 
 [graphics:python_version < "3.6" and python_version >= "3.5"]
-opencv-python
+opencv-python>=3.1.0.2
 
 [graphics:python_version < "3.7" and python_version >= "3.6"]
-opencv-python
+opencv-python>=3.4.13.47
 
 [graphics:python_version < "3.8" and python_version >= "3.7"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "3.9" and python_version >= "3.8"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "4.0" and python_version >= "3.11"]
-opencv-python
+opencv-python>=4.5.5.64
 
 [headless]
 
 [headless-strict]
 
 [headless-strict:python_version < "3.10" and python_version >= "3.9"]
 opencv-python-headless==3.4.15.55
@@ -274,181 +349,252 @@
 [headless-strict:python_version < "3.9" and python_version >= "3.8"]
 opencv-python-headless==3.4.15.55
 
 [headless-strict:python_version < "4.0" and python_version >= "3.11"]
 opencv-python-headless==4.5.5.64
 
 [headless:python_version < "3.10" and python_version >= "3.9"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "3.11" and python_version >= "3.10"]
-opencv-python-headless
+opencv-python-headless>=4.5.4.58
 
 [headless:python_version < "3.4" and python_version >= "2.7"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.5" and python_version >= "3.4"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.6" and python_version >= "3.5"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.7" and python_version >= "3.6"]
-opencv-python-headless
+opencv-python-headless>=3.4.13.47
 
 [headless:python_version < "3.8" and python_version >= "3.7"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "3.9" and python_version >= "3.8"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "4.0" and python_version >= "3.11"]
-opencv-python-headless
+opencv-python-headless>=4.5.5.64
 
 [optional]
 
 [optional-strict]
 
+[runtime]
+ubelt>=1.3.4
+utool>=2.2.0
+vtool_ibeis>=2.2.0
+
 [runtime-strict]
-six==1.10.0
-ubelt==1.2.2
-utool==2.1.6
+ubelt==1.3.4
+utool==2.2.0
 vtool_ibeis==2.2.0
 
 [runtime-strict:python_version < "3.10" and python_version >= "3.9"]
-cachetools==4.2.0
 matplotlib==3.3.3
+cachetools==4.2.0
 
 [runtime-strict:python_version < "3.11" and python_version >= "3.10"]
+matplotlib==3.5.0
 cachetools==5.0.0
+
+[runtime-strict:python_version < "3.12"]
+six==1.10.0
+
+[runtime-strict:python_version < "3.12" and python_version >= "2.7"]
+pyqt5==5.15.5
+
+[runtime-strict:python_version < "3.12" and python_version >= "3.11"]
 matplotlib==3.5.0
 
 [runtime-strict:python_version < "3.7" and python_version >= "3.6"]
-cachetools==4.0.0
 matplotlib==1.5.3
+cachetools==4.0.0
 
 [runtime-strict:python_version < "3.8" and python_version >= "3.7"]
-cachetools==5.0.0
 matplotlib==2.2.2
+cachetools==5.0.0
 
 [runtime-strict:python_version < "3.9" and python_version >= "3.8"]
-cachetools==4.0.0
 matplotlib==3.6.0
+cachetools==4.0.0
 
 [runtime-strict:python_version < "4.0" and python_version >= "3.11"]
 cachetools==5.0.0
-matplotlib==3.5.0
 
-[runtime-strict:python_version > "2.7"]
-pyqt5==5.15.5
+[runtime-strict:python_version < "4.0" and python_version >= "3.12"]
+six==1.16.0
+matplotlib==3.8.4
+pyqt5==5.15.10
+
+[runtime:python_version < "3.10" and python_version >= "3.9"]
+matplotlib>=3.3.3
+cachetools>=4.2.0
+
+[runtime:python_version < "3.11" and python_version >= "3.10"]
+matplotlib>=3.5.0
+cachetools>=5.0.0
+
+[runtime:python_version < "3.12"]
+six>=1.10.0
+
+[runtime:python_version < "3.12" and python_version >= "2.7"]
+pyqt5>=5.15.5
+
+[runtime:python_version < "3.12" and python_version >= "3.11"]
+matplotlib>=3.5.0
+
+[runtime:python_version < "3.7" and python_version >= "3.6"]
+matplotlib>=1.5.3
+cachetools>=4.0.0
+
+[runtime:python_version < "3.8" and python_version >= "3.7"]
+matplotlib>=2.2.2
+cachetools>=5.0.0
+
+[runtime:python_version < "3.9" and python_version >= "3.8"]
+matplotlib>=3.6.0
+cachetools>=4.0.0
+
+[runtime:python_version < "4.0" and python_version >= "3.11"]
+cachetools>=5.0.0
+
+[runtime:python_version < "4.0" and python_version >= "3.12"]
+six>=1.16.0
+matplotlib>=3.8.4
+pyqt5>=5.15.10
 
 [tests]
-codecov
-pytest-timeout
-xdoctest
+xdoctest>=1.1.3
 
 [tests-strict]
-codecov==2.0.15
-pytest-timeout==1.4.2
-xdoctest==0.14.0
+xdoctest==1.1.3
 
 [tests-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [tests-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.10" and python_version >= "3.9"]
+pytest==8.1.1
 coverage==5.3.1
 
-[tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
+[tests-strict:python_version < "3.11" and python_version >= "3.10"]
+pytest==8.1.1
+coverage==6.1.1
+
+[tests-strict:python_version < "3.12"]
+pytest_timeout==1.4.2
+
+[tests-strict:python_version < "3.12" and python_version >= "3.11"]
+pytest==8.1.1
+coverage==7.0.0
+
+[tests-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [tests-strict:python_version < "3.4" and python_version >= "2.7"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.5" and python_version >= "3.4"]
 coverage==4.3.4
 
 [tests-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.6" and python_version >= "3.5"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [tests-strict:python_version < "3.7" and python_version >= "3.6"]
 coverage==6.1.1
 
-[tests-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
-
 [tests-strict:python_version < "3.8" and python_version >= "3.7"]
+pytest==4.6.0
 coverage==6.1.1
 
 [tests-strict:python_version < "3.9" and python_version >= "3.8"]
+pytest==8.1.1
 coverage==6.1.1
 
-[tests-strict:python_version >= "3.10"]
-coverage==6.1.1
+[tests-strict:python_version < "4.0" and python_version >= "3.12"]
+pytest_timeout==2.3.1
+coverage==7.3.0
 
-[tests-strict:python_version >= "3.10.0"]
-pytest==6.2.5
+[tests-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
 
 [tests-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [tests:python_version < "2.7" and python_version >= "2.6"]
-coverage
+coverage>=4.5
 
 [tests:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.10" and python_version >= "3.9"]
-coverage
+pytest>=8.1.1
+coverage>=5.3.1
 
-[tests:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+[tests:python_version < "3.11" and python_version >= "3.10"]
+pytest>=8.1.1
+coverage>=6.1.1
+
+[tests:python_version < "3.12"]
+pytest_timeout>=1.4.2
+
+[tests:python_version < "3.12" and python_version >= "3.11"]
+pytest>=8.1.1
+coverage>=7.0.0
+
+[tests:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [tests:python_version < "3.4" and python_version >= "2.7"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.5" and python_version >= "3.4"]
-coverage
+coverage>=4.3.4
 
 [tests:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.6" and python_version >= "3.5"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [tests:python_version < "3.7" and python_version >= "3.6"]
-coverage
-
-[tests:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+coverage>=6.1.1
 
 [tests:python_version < "3.8" and python_version >= "3.7"]
-coverage
+pytest>=4.6.0
+coverage>=6.1.1
 
 [tests:python_version < "3.9" and python_version >= "3.8"]
-coverage
+pytest>=8.1.1
+coverage>=6.1.1
 
-[tests:python_version >= "3.10"]
-coverage
+[tests:python_version < "4.0" and python_version >= "3.12"]
+pytest_timeout>=2.3.1
+coverage>=7.3.0
 
-[tests:python_version >= "3.10.0"]
-pytest
+[tests:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
 [tests:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
```

### Comparing `guitool_ibeis-2.1.2/pyproject.toml` & `guitool_ibeis-2.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 description = "Guitool - tools for PyQt5 guis"
 url="https://github.com/Erotemic/guitool_ibeis"
 author="Jon Crall"
 version = "{mod_dpath}/__init__.py::__version__"
 author_email="erotemic@gmail.com"
 license = "Apache 2"
 dev_status = "beta"
-min_python = 3.7
+min_python = 3.8
 # ci_cpython_versions = ["3.7", "3.8", "3.9", "3.10"]
-supported_python_versions = ["3.7", "3.8", "3.9", "3.10"]
+#supported_python_versions = ["3.7", "3.8", "3.9", "3.10"]
 ci_pypy_versions = []
 autostage = true
 os = [ "linux" ]
 
 [tool.pytest.ini_options]
-addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
-filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
+addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=docs"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
+filterwarnings = [
+    "default",
+    "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning",
+    "ignore:.*Define the __nice__ method for.*:Warning",
+    "ignore:.*private pytest class or function.*:Warning",
+]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
 omit = [ "guitool_ibeis/__main__.py", "*/setup.py",]
```

### Comparing `guitool_ibeis-2.1.2/setup.py` & `guitool_ibeis-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Generated by ~/code/xcookie/xcookie/builders/setup.py
 # based on part ~/code/xcookie/xcookie/rc/setup.py.in
 import sys
-from os.path import exists
+import re
+from os.path import exists, dirname, join
 from setuptools import find_packages
 from setuptools import setup
 
 
 def parse_version(fpath):
     """
     Statically parse the version number from a python file
@@ -49,16 +50,14 @@
     """
     Parse the description in the README file
 
     CommandLine:
         pandoc --from=markdown --to=rst --output=README.rst README.md
         python -c "import setup; print(setup.parse_description())"
     """
-    from os.path import dirname, join, exists
-
     readme_fpath = join(dirname(__file__), "README.rst")
     # This breaks on pip install, so check that it exists.
     if exists(readme_fpath):
         with open(readme_fpath, "r") as f:
             text = f.read()
         return text
     return ""
@@ -73,18 +72,18 @@
         fname (str): path to requirements file
         versions (bool | str, default=False):
             If true include version specs.
             If strict, then pin to the minimum version.
 
     Returns:
         List[str]: list of requirements items
-    """
-    from os.path import exists, dirname, join
-    import re
 
+    CommandLine:
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
+    """
     require_fpath = fname
 
     def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
 
         line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
@@ -194,59 +193,65 @@
 #             raise KeyError(versions)
 #     requirements = [r.replace(' ', '') for r in requirements]
 #     return requirements
 
 
 NAME = "guitool_ibeis"
 INIT_PATH = "guitool_ibeis/__init__.py"
-VERSION = parse_version("guitool_ibeis/__init__.py")
+VERSION = parse_version(INIT_PATH)
 
 if __name__ == "__main__":
     setupkw = {}
 
-    setupkw["install_requires"] = parse_requirements("requirements/runtime.txt")
+    setupkw["install_requires"] = parse_requirements(
+        "requirements/runtime.txt", versions="loose"
+    )
     setupkw["extras_require"] = {
-        "all": parse_requirements("requirements.txt"),
-        "tests": parse_requirements("requirements/tests.txt"),
-        "optional": parse_requirements("requirements/optional.txt"),
-        "headless": parse_requirements("requirements/headless.txt"),
-        "graphics": parse_requirements("requirements/graphics.txt"),
-        # Strict versions
+        "all": parse_requirements("requirements.txt", versions="loose"),
+        "headless": parse_requirements("requirements/headless.txt", versions="loose"),
+        "graphics": parse_requirements("requirements/graphics.txt", versions="loose"),
+        "build": parse_requirements("requirements/build.txt", versions="loose"),
+        "docs": parse_requirements("requirements/docs.txt", versions="loose"),
+        "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+        "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+        "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+        "all-strict": parse_requirements("requirements.txt", versions="strict"),
         "headless-strict": parse_requirements(
             "requirements/headless.txt", versions="strict"
         ),
         "graphics-strict": parse_requirements(
             "requirements/graphics.txt", versions="strict"
         ),
-        "all-strict": parse_requirements("requirements.txt", versions="strict"),
+        "build-strict": parse_requirements("requirements/build.txt", versions="strict"),
+        "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
+        "optional-strict": parse_requirements(
+            "requirements/optional.txt", versions="strict"
+        ),
         "runtime-strict": parse_requirements(
             "requirements/runtime.txt", versions="strict"
         ),
         "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
-        "optional-strict": parse_requirements(
-            "requirements/optional.txt", versions="strict"
-        ),
     }
-
     setupkw["name"] = NAME
     setupkw["version"] = VERSION
     setupkw["author"] = "Jon Crall"
     setupkw["author_email"] = "erotemic@gmail.com"
     setupkw["url"] = "https://github.com/Erotemic/guitool_ibeis"
     setupkw["description"] = "Guitool - tools for PyQt5 guis"
     setupkw["long_description"] = parse_description()
     setupkw["long_description_content_type"] = "text/x-rst"
     setupkw["license"] = "Apache 2"
     setupkw["packages"] = find_packages(".")
-    setupkw["python_requires"] = ">=3.7"
+    setupkw["python_requires"] = ">=3.8"
     setupkw["classifiers"] = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ]
     setup(**setupkw)
```

