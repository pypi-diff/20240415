# Comparing `tmp/toolfuse-0.1.15.tar.gz` & `tmp/toolfuse-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.15.tar", max compression
+gzip compressed data, was "toolfuse-0.1.16.tar", max compression
```

## Comparing `toolfuse-0.1.15.tar` & `toolfuse-0.1.16.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.15/LICENSE
--rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.15/README.md
--rw-r--r--   0        0        0      803 2024-04-10 15:05:04.066332 toolfuse-0.1.15/pyproject.toml
--rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.15/toolfuse/__init__.py
--rw-r--r--   0        0        0    19587 2024-04-10 15:04:52.103260 toolfuse-0.1.15/toolfuse/base.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.16/LICENSE
+-rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.16/README.md
+-rw-r--r--   0        0        0      803 2024-04-15 00:39:00.528715 toolfuse-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.16/toolfuse/__init__.py
+-rw-r--r--   0        0        0    19575 2024-04-15 00:38:34.973759 toolfuse-0.1.16/toolfuse/base.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.16/PKG-INFO
```

### Comparing `toolfuse-0.1.15/LICENSE` & `toolfuse-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.15/README.md` & `toolfuse-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.15/pyproject.toml` & `toolfuse-0.1.16/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.15"
+version = "0.1.16"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.15/toolfuse/base.py` & `toolfuse-0.1.16/toolfuse/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,23 +430,23 @@
             # Add the Action to the tool's actions list
             self._actions_list.append(action)
 
     FunctionTool.__name__ = f"{function.__name__}_tool"
     return FunctionTool
 
 
-def tool_from_object(obj: Any) -> Type[Tool]:
+def tool_from_object(obj: Any) -> Tool:
     """
     Dynamically creates a subclass of `Tool` that encapsulates the methods of a given object instance as actions.
 
     Args:
         obj (Any): The object instance whose methods are to be encapsulated as actions in the Tool.
 
     Returns:
-        Type[Tool]: A new subclass of Tool that includes the object's methods as actions.
+        Tool: A new subclass of Tool that includes the object's methods as actions.
     """
 
     class ObjectTool(Tool):
         def __init__(self, obj_instance: Any):
             super().__init__()
             self.obj_instance = obj_instance
             self._register_methods_from_object()
```

### Comparing `toolfuse-0.1.15/PKG-INFO` & `toolfuse-0.1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.15
+Version: 0.1.16
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

