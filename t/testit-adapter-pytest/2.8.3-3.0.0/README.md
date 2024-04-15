# Comparing `tmp/testit-adapter-pytest-2.8.3.tar.gz` & `tmp/testit_adapter_pytest-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-pytest-2.8.3.tar", last modified: Fri Mar 15 06:55:29 2024, max compression
+gzip compressed data, was "testit_adapter_pytest-3.0.0.tar", last modified: Mon Apr 15 10:42:42 2024, max compression
```

## Comparing `testit-adapter-pytest-2.8.3.tar` & `testit_adapter_pytest-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:29.216719 testit-adapter-pytest-2.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/models/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-03-15 06:55:25.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:29.220719 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 06:55:29.000000 testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:42.335951 testit_adapter_pytest-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/models/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-15 10:42:38.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:42.339951 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 10:42:42.000000 testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit-adapter-pytest-2.8.3/PKG-INFO` & `testit_adapter_pytest-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.8.3
+Version: 3.0.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==2.8.3
+Requires-Dist: testit-python-commons==3.0.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit-adapter-pytest-2.8.3/README.md` & `testit_adapter_pytest-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/setup.py` & `testit_adapter_pytest-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='2.8.3',
+    version='3.0.0',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -19,10 +19,10 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==2.8.3'],
+    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==3.0.0'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_context.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_context.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_manager.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_manager.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/fixture_storage.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/fixture_storage.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/listener.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,64 +124,49 @@
     @classmethod
     @adapter_logger
     def __get_separation_of_tests(cls, items, resolved_autotests) -> SeparationOfTests:
         separation_of_tests = SeparationOfTests()
         index = 0
 
         for item in items:
-            if hasattr(item.function, 'test_external_id'):
-                item.test_external_id = item.function.test_external_id
-            else:
-                item.test_external_id = utils.get_hash(item.nodeid + item.function.__name__)
+            if not hasattr(item.function, 'test_external_id'):
+                item.function.test_external_id = utils.get_hash(item.parent.nodeid + item.function.__name__)
 
             if item.own_markers:
                 for mark in item.own_markers:
                     if mark.name == 'parametrize':
                         if not hasattr(item, 'array_parametrize_mark_id'):
                             item.array_parametrize_mark_id = []
                         item.array_parametrize_mark_id.append(
                             item.own_markers.index(mark))
 
             params = utils.get_all_parameters(item)
-            item.test_external_id = utils.collect_parameters_in_string_attribute(
-                item.test_external_id,
+            item.function.test_external_id = utils.collect_parameters_in_string_attribute(
+                item.function.test_external_id,
                 params)
 
             item.index = index
             item_id = items.index(item)
             index = index + 1 if len(items) > item_id + 1 and items[item_id + 1].originalname == item.originalname \
                 else 0
 
-            if cls.__check_external_id_in_resolved_autotests(item.test_external_id, resolved_autotests):
+            if cls.__check_external_id_in_resolved_autotests(item.function.test_external_id, resolved_autotests):
                 separation_of_tests.add_item_to_selected_items(item)
             else:
                 separation_of_tests.add_item_to_deselected_items(item)
 
         return separation_of_tests
 
     @staticmethod
     @adapter_logger
     def __check_external_id_in_resolved_autotests(external_id: str, resolved_autotests: dict) -> bool:
         return resolved_autotests is not None and external_id in resolved_autotests
 
     @pytest.hookimpl(tryfirst=True)
     def pytest_runtest_protocol(self, item):
-        if not hasattr(item.function, 'test_external_id'):
-            item.test_external_id = utils.get_hash(item.nodeid + item.function.__name__)
-
-        if not hasattr(item.function, 'test_displayname'):
-            item.test_displayname = item.function.__doc__ if \
-                item.function.__doc__ else item.function.__name__
-        else:
-            params = utils.get_all_parameters(item)
-
-            item.test_displayname = utils.collect_parameters_in_string_attribute(
-                item.function.test_displayname,
-                params)
-
         self.__executable_test = utils.form_test(item)
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_setup(self, item):
         if not self.__executable_test:
             return
 
@@ -331,16 +316,16 @@
             group_uuid = self._cache.get(fixturedef)
             if group_uuid:
                 group = self.fixture_manager.get_item(group_uuid)
             else:
                 group_uuid = self._cache.push(fixturedef)
                 group = FixturesContainer(uuid=group_uuid)
                 self.fixture_manager.start_group(group_uuid, group)
-            if item.test_external_id not in group.external_ids:
-                self.fixture_manager.update_group(group_uuid, external_ids=item.test_external_id)
+            if item.function.test_external_id not in group.external_ids:
+                self.fixture_manager.update_group(group_uuid, external_ids=item.function.test_external_id)
 
 
 def _test_fixtures(item):
     fixturemanager = item.session._fixturemanager
     fixturedefs = []
 
     if hasattr(item, "_request") and hasattr(item._request, "fixturenames"):
```

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/models/fixture.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/models/fixture.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/plugin.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest/utils.py` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     return collect_parameters_in_string_attribute(display_name, get_all_parameters(item))
 
 
 def __get_external_id_from(item):
     external_id = __search_attribute(item, 'test_external_id')
 
     if not external_id:
-        return get_hash(item.nodeid + item.function.__name__)
+        return get_hash(item.parent.nodeid + item.function.__name__)
 
     return collect_parameters_in_string_attribute(external_id, get_all_parameters(item))
 
 
 def __get_title_from(item):
     title = __search_attribute(item, 'test_title')
```

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.8.3
+Version: 3.0.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==2.8.3
+Requires-Dist: testit-python-commons==3.0.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit-adapter-pytest-2.8.3/src/testit_adapter_pytest.egg-info/SOURCES.txt` & `testit_adapter_pytest-3.0.0/src/testit_adapter_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

