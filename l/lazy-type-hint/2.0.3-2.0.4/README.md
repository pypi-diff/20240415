# Comparing `tmp/lazy_type_hint-2.0.3.tar.gz` & `tmp/lazy_type_hint-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.3.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.4.tar", max compression
```

## Comparing `lazy_type_hint-2.0.3.tar` & `lazy_type_hint-2.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.3/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     4415 2024-04-14 14:25:09.969451 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6523 2024-04-14 14:47:20.360570 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.3/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.3/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.3/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.3/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.3/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.3/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.3/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.3/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.3/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.3/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.3/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2397 2024-04-14 14:51:46.202054 lazy_type_hint-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.3/README.md
--rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.4/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     4415 2024-04-14 14:25:09.969451 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6523 2024-04-14 14:47:20.360570 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.4/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.4/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.4/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.4/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.4/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.4/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.4/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.4/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.4/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.4/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.4/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.4/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2397 2024-04-15 06:42:14.113353 lazy_type_hint-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6857 2024-04-15 06:41:49.885418 lazy_type_hint-2.0.4/README.md
+-rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.4/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.4/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.4/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.4/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.4/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.4/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.4/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.3/pyproject.toml` & `lazy_type_hint-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.3"
+version = "2.0.4"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
```

### Comparing `lazy_type_hint-2.0.3/README.md` & `lazy_type_hint-2.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,23 +77,23 @@
    ```
 2. [EXPERIMENTAL] Get type hints live with `LazyTypeHintLive`. The API changes its local
    interface as soon as you use it, allowing to automatically infer and reuse your type
    hints after executing your program once.
 
    |   Before executing the code    |   After executing the code    |
     |:-------------:|:-------------:|
-    | ![Before executing the code](img/before.PNG) | ![After executing the code](img/after.PNG) |
+    | ![Before executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/before.PNG?raw=true) | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/after.PNG?raw=true) |
 
     This will allow you to:
 
-   |   Imagen 1    |   Imagen 2    |
+   |       |       |
     |:-------------:|:-------------:|
-    | Perform static analysis to detect issues | ![After executing the code](img/errors.PNG) |
-    | Reuse your available type hints | ![After executing the code](img/reuse_classes.PNG) |
-    | Have full autocompletion support from your IDE | ![After executing the code](img/autocomplete.PNG) |
+    | Perform static analysis to detect issues | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/errors.PNG?raw=true) |
+    | Reuse your available type hints | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/reuse_classes.PNG?raw=true) |
+    | Have full autocompletion support from your IDE | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/autocomplete.PNG?raw=true) |
 
 
 
 
 3. Easily type hint your files (YAML, JSON) and parse extra comments found within this
    file as part of the type hint docstrings. Given a yaml file like:
```

### Comparing `lazy_type_hint-2.0.3/PKG-INFO` & `lazy_type_hint-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.3
+Version: 2.0.4
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -93,23 +93,23 @@
    ```
 2. [EXPERIMENTAL] Get type hints live with `LazyTypeHintLive`. The API changes its local
    interface as soon as you use it, allowing to automatically infer and reuse your type
    hints after executing your program once.
 
    |   Before executing the code    |   After executing the code    |
     |:-------------:|:-------------:|
-    | ![Before executing the code](img/before.PNG) | ![After executing the code](img/after.PNG) |
+    | ![Before executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/before.PNG?raw=true) | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/after.PNG?raw=true) |
 
     This will allow you to:
 
-   |   Imagen 1    |   Imagen 2    |
+   |       |       |
     |:-------------:|:-------------:|
-    | Perform static analysis to detect issues | ![After executing the code](img/errors.PNG) |
-    | Reuse your available type hints | ![After executing the code](img/reuse_classes.PNG) |
-    | Have full autocompletion support from your IDE | ![After executing the code](img/autocomplete.PNG) |
+    | Perform static analysis to detect issues | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/errors.PNG?raw=true) |
+    | Reuse your available type hints | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/reuse_classes.PNG?raw=true) |
+    | Have full autocompletion support from your IDE | ![After executing the code](https://github.com/mflova/lazy-type-hint/blob/main/img/autocomplete.PNG?raw=true) |
 
 
 
 
 3. Easily type hint your files (YAML, JSON) and parse extra comments found within this
    file as part of the type hint docstrings. Given a yaml file like:
```

