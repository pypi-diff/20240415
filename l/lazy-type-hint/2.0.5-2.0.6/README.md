# Comparing `tmp/lazy_type_hint-2.0.5.tar.gz` & `tmp/lazy_type_hint-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.5.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.6.tar", max compression
```

## Comparing `lazy_type_hint-2.0.5.tar` & `lazy_type_hint-2.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.5/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     4415 2024-04-14 14:25:09.969451 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6525 2024-04-15 06:58:33.554062 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.5/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.5/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.5/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9518 2024-04-15 06:56:46.749622 lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.5/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.5/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.5/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.5/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.5/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.5/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.5/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.5/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.5/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2397 2024-04-15 07:01:02.231383 lazy_type_hint-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     6857 2024-04-15 06:41:49.885418 lazy_type_hint-2.0.5/README.md
--rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.6/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     5631 2024-04-15 11:24:42.289742 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6525 2024-04-15 06:58:33.554062 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-15 11:24:42.296743 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     8646 2024-04-15 11:24:42.302827 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.6/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1809 2024-04-15 11:24:42.310740 lazy_type_hint-2.0.6/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.6/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.6/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.6/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.6/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.6/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.6/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.6/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2397 2024-04-15 11:24:42.318741 lazy_type_hint-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6857 2024-04-15 06:41:49.885418 lazy_type_hint-2.0.6/README.md
+-rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.6/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,32 +17,62 @@
 OVERLOAD_TEMPLATE: Final = """    @overload  # type: ignore
     def __getitem__(self, key: Literal["{literal}"]) -> {rtype}:
         ...
 """
 TEMPLATE: Final = """class {class_name}(pd.DataFrame):
 
 {overloads}
+    @overload
     def __getitem__(
         self,
         key: Union[
             "pd.Series[bool]",
-            str,
+            {allowed_types},
             pd.DataFrame,
             pd.Index,
             npt.NDArray[np.bool_],
             npt.NDArray[np.str_],
             List[Union[Scalar, Tuple[Hashable, ...]]],
         ],
     ) -> Union[pd.Series, pd.DataFrame]:
+        ...
+
+    def __getitem__(
+        self,
+        key: Union[
+            "pd.Series[bool]",
+            {allowed_types},
+            pd.DataFrame,
+            pd.Index,
+            npt.NDArray[np.bool_],
+            npt.NDArray[np.str_],
+            List[Union[Scalar, Tuple[Hashable, ...]]],
+        ],
+    ) -> Union[pd.Series, pd.DataFrame]:
+        return super().__getitem__(key)"""
+
+TEMPLATE_NO_PD: Final = """class {class_name}(pd.DataFrame):
+
+{overloads}
+    def __getitem__(
+        self,
+        key: Union[
+            {allowed_types},
+            npt.NDArray[np.bool_],
+            npt.NDArray[np.str_],
+            List[Union[Scalar, Tuple[Hashable, ...]]],
+        ],
+    ) -> Union[pd.Series, pd.DataFrame]:
         return super().__getitem__(key)"""
 
 
 class PandasDataFrameDataTypeTree(MappingDataTypeTree):
     wraps = pd.DataFrame
     data: pd.DataFrame
+    children: Mapping[str, DataTypeTree]  # type: ignore[assignment]
 
     @override
     @property
     def permission_to_be_created_as_type_alias(self) -> bool:
         return bool(len(self) >= 1 and self.are_columns_either_all_str_or_all_tuple)
 
     @property
@@ -87,22 +117,22 @@
                     if column[0] not in columns_processed:
                         columns_processed.add(column[0])
                         children[column[0]] = self._create_child(column[0])
         return children
 
     @override
     def _get_hash(self) -> str:
-        if not self.strategies.pandas_type_hint_columns:
+        if self.strategies.pandas_strategies == "Do not type hint columns":
             return "pd.DataFrame"
         return str(self.data.columns)
 
     @override
     def _get_str_top_node(self) -> str:
         self.imports.add("pandas")
-        if len(self) == 0 or not self.strategies.pandas_type_hint_columns:
+        if len(self) == 0 or not self.strategies.pandas_strategies:
             self.imports.add("TypeAlias")
             return f"{self.name}: TypeAlias = pd.DataFrame"
         self.imports.add("overload")
         self.imports.add("Union")
         self.imports.add("Literal")
         self.imports.add("npt")
         self.imports.add("tuple")
@@ -114,8 +144,15 @@
         overloads: List[str] = []
         for literal, child in self.children.items():
             if child.permission_to_be_created_as_type_alias:
                 overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=child.name))
             else:
                 rtype = "Union[pd.DataFrame, pd.Series]"
                 overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=rtype))
-        return TEMPLATE.format(class_name=self.name, overloads="\n".join(overloads))
+        if self.strategies.pandas_strategies == "Full type hint":
+            all_literals = ", ".join(f'"{key}"' for key in self.children)
+            allowed_types = f"Literal[{all_literals}]"
+            template = TEMPLATE_NO_PD
+        else:
+            allowed_types = "str"
+            template = TEMPLATE
+        return template.format(class_name=self.name, overloads="\n".join(overloads), allowed_types=allowed_types)
```

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 class LazyTypeHintABC(ABC):
     strategies: ParsingStrategies
     """Strategies to follow when parsing the objects."""
 
     def __init__(
         self,
-        *,
         strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
         **kwargs: Any,
     ) -> None:
         self.strategies = strategies
 
     def from_yaml_file(
         self,
```

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import os
 import re
 import shutil
 from pathlib import Path
-from types import ModuleType
 from typing import (
     Any,
     Callable,
     Dict,
     Final,
     Literal,  # noqa: F401
     Mapping,
     Optional,
     Sequence,
-    Tuple,
     TypeVar,
     Union,
     final,
     overload,  # noqa: F401
 )
 
 from typing_extensions import TypeAlias, override
 
-import lazy_type_hint
 from lazy_type_hint.file_modifiers.py_file_modifier import PyFileModifier
 from lazy_type_hint.file_modifiers.yaml_file_modifier import YAML_COMMENTS_POSITION
 from lazy_type_hint.generators.lazy_type_hint_abc import LazyTypeHintABC
 from lazy_type_hint.strategies import ParsingStrategies
 from lazy_type_hint.utils import (
     TAB,
     is_string_python_keyword_compatible,
@@ -44,41 +41,30 @@
 
 class LazyTypeHintLive(LazyTypeHintABC):
     # Utils
     this_file_pyi: PyFileModifier
     """.pyi representation of this same module."""
     this_file_pyi_path: Path
     """Path to the .pyi file associated to this same module."""
-    custom_classes_dir: Tuple[Union[ModuleType, str], ...]
-    """Hold the information where the class interfaces will be created.
-    
-    First one is `ModuleType`. Following ones are strings. At least one must be provided.
-    """
     strategies: ParsingStrategies
     """Strategies to follow when parsing the objects."""
 
     # Constants that should not be modified
     header: Final = "# Class automatically generated. DO NOT MODIFY."
     """Header that will be prepended to all new classes created."""
     classes_created: "TypeAlias" = Any
     """Classes created by the class. Do not modify."""
     methods_to_be_overloaded: Final = ("from_data", "from_yaml_file")
     """Methods that will be modified in the PYI interface when new classes are added."""
 
     @final
     def __init__(
         self,
-        *,
         strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
-        generated_classes_custom_dir: Tuple[Union[ModuleType, str], ...] = (
-            lazy_type_hint,
-            "build",
-        ),
     ) -> None:
-        self.custom_classes_dir = generated_classes_custom_dir
         self.strategies = strategies
 
         self.this_file_pyi_path = Path(__file__).with_suffix(".pyi")
         if not self.this_file_pyi_path.exists():
             self.this_file_pyi = self._generate_this_file_pyi()
         else:
             self.this_file_pyi = PyFileModifier(self.this_file_pyi_path.read_text(encoding="utf-8"))
@@ -123,19 +109,19 @@
         class_name: str,
         **kwargs: Any,
     ) -> ObjectT:
         if not is_string_python_keyword_compatible(class_name):
             raise LazyTypeHintLiveError(
                 f"Given class_name is not compatible with Python class naming conventions: {class_name}"
             )
-        if class_name in self._get_classes_added():
-            return data
         string_representation = str(super().from_data(data=data, class_name=class_name))
         string_representation = self.header + "\n" + string_representation
         self._create_custom_class_py(string_representation, class_name)
+        if class_name in self._get_classes_added():
+            return data
         self._add_new_class_to_loader_pyi(new_class=class_name)
         return data
 
     def reset(self) -> None:
         self._reset_custom_class_pyi()
         self.this_file_pyi = self._generate_this_file_pyi()
         self._update_this_file_pyi()
@@ -148,20 +134,15 @@
         file_handler.remove_all_method_bodies()
         file_handler.remove_all_private_methods()
         file_handler.remove_all_instance_variables(class_name=(type(self)).__name__)
         return file_handler
 
     @property
     def _custom_class_dir_path(self) -> Path:
-        package_path: Path = Path(self.custom_classes_dir[0].__path__[0])  # type: ignore
-        sub_paths: Sequence[Path] = self.custom_classes_dir[1:]  # type: ignore
-
-        for string in sub_paths:
-            package_path = package_path / string
-        return package_path
+        return self.this_file_pyi_path.parent / "build"
 
     def _create_custom_class_py(self, string: str, class_name: str) -> None:
         if not self._custom_class_dir_path.exists():
             os.makedirs(self._custom_class_dir_path)
 
         path = self._custom_class_dir_path / f"{class_name}.py"
         path.write_text(string)
@@ -176,18 +157,15 @@
     @final
     def _reset_custom_class_pyi(self) -> None:
         if self._custom_class_dir_path.exists():
             shutil.rmtree(self._custom_class_dir_path)
 
     @final
     def _add_import_to_this_file_pyi(self, new_class: str) -> None:
-        import_statement = (
-            f"from {self.custom_classes_dir[0].__name__}."  # type: ignore
-            f"{'.'.join(self.custom_classes_dir[1:])}.{new_class} import {new_class}"  # type: ignore
-        )
+        import_statement = f"from lazy_type_hint.generators.build.{new_class} import {new_class}"
         self.this_file_pyi.add_imports(
             import_statement,
             in_type_checking_block=False,
         )
         self._update_this_file_pyi()
 
     @final
```

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.6/lazy_type_hint/strategies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dataclasses import dataclass, fields
 from typing import Literal, get_args, get_type_hints
 
 LIST_STRATEGIES = Literal["Sequence", "list"]
 TUPLE_SIZE_STRATEGIES = Literal["fixed", "any size"]
 MAPPING_STRATEGIES = Literal["TypedDict", "Mapping", "dict"]
+PANDAS_STRATEGIES = Literal["Full type hint", "Type hint only for autocomplete", "Do not type hint columns"]
 
 
 @dataclass(frozen=True)
 class ParsingStrategies:
     list_strategy: LIST_STRATEGIES = "list"
     tuple_size_strategy: TUPLE_SIZE_STRATEGIES = "fixed"
     dict_strategy: MAPPING_STRATEGIES = "TypedDict"
-    pandas_type_hint_columns: bool = True
+    pandas_strategies: PANDAS_STRATEGIES = "Full type hint"
     min_height_to_define_type_alias: int = 1
     key_used_as_doc: str = ""
     merge_different_typed_dicts_if_similarity_above: int = 50
     typed_dict_read_only_values: bool = False
 
     def __post_init__(self) -> None:
         type_hints = get_type_hints(self)
```

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.6/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/pyproject.toml` & `lazy_type_hint-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.5"
+version = "2.0.6"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
```

### Comparing `lazy_type_hint-2.0.5/README.md` & `lazy_type_hint-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.5/PKG-INFO` & `lazy_type_hint-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.5
+Version: 2.0.6
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

