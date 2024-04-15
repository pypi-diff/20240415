# Comparing `tmp/node_graph-0.0.3.tar.gz` & `tmp/node_graph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node_graph-0.0.3.tar", last modified: Mon Dec 11 08:09:30 2023, max compression
+gzip compressed data, was "node_graph-0.0.4.tar", last modified: Mon Apr 15 12:08:01 2024, max compression
```

## Comparing `node_graph-0.0.3.tar` & `node_graph-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.959613 node_graph-0.0.3/
--rw-r--r--   0 jovyan    (1000) users      (100)     1064 2023-12-02 14:41:14.000000 node_graph-0.0.3/LICENSE
--rw-r--r--   0 jovyan    (1000) users      (100)     1128 2023-12-11 08:09:30.959613 node_graph-0.0.3/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      827 2023-12-02 14:41:14.000000 node_graph-0.0.3/README.md
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.955613 node_graph-0.0.3/node_graph/
--rw-r--r--   0 jovyan    (1000) users      (100)       34 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)    13105 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/analysis.py
--rw-r--r--   0 jovyan    (1000) users      (100)    11038 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/collection.py
--rw-r--r--   0 jovyan    (1000) users      (100)    10297 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/decorator.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3473 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/link.py
--rw-r--r--   0 jovyan    (1000) users      (100)    18230 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/node.py
--rw-r--r--   0 jovyan    (1000) users      (100)    11430 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/node_graph.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.959613 node_graph-0.0.3/node_graph/nodes/
--rw-r--r--   0 jovyan    (1000) users      (100)       85 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/nodes/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4600 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/nodes/test_nodes.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.959613 node_graph-0.0.3/node_graph/properties/
--rw-r--r--   0 jovyan    (1000) users      (100)       93 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/properties/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)    11956 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/properties/builtin.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3032 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/property.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1541 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/serializer.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4039 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/socket.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.959613 node_graph-0.0.3/node_graph/sockets/
--rw-r--r--   0 jovyan    (1000) users      (100)       89 2023-12-04 08:23:59.000000 node_graph-0.0.3/node_graph/sockets/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3332 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/sockets/builtin.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2550 2023-12-02 22:27:16.000000 node_graph-0.0.3/node_graph/utils.py
--rw-r--r--   0 jovyan    (1000) users      (100)      103 2023-12-02 14:41:14.000000 node_graph-0.0.3/node_graph/version.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-12-11 08:09:30.959613 node_graph-0.0.3/node_graph.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1128 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      689 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      212 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       50 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       11 2023-12-11 08:09:30.000000 node_graph-0.0.3/node_graph.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-12-11 08:09:30.959613 node_graph-0.0.3/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)     1361 2023-12-11 08:07:57.000000 node_graph-0.0.3/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.4/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-15 12:08:01.495976 node_graph-0.0.4/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      827 2023-12-03 08:36:19.000000 node_graph-0.0.4/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.491976 node_graph-0.0.4/node_graph/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11972 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10311 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18230 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/node_graph.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/nodes/test_nodes.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/properties/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3032 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/serializer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/sockets/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-15 12:08:01.495976 node_graph-0.0.4/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-04-15 12:07:57.000000 node_graph-0.0.4/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_entry_point.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.4/tests/test_hooks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_yaml.py
```

### Comparing `node_graph-0.0.3/LICENSE` & `node_graph-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/PKG-INFO` & `node_graph-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: click
+Requires-Dist: pyyaml
+Requires-Dist: colorama
+Requires-Dist: termcolor
+Requires-Dist: cloudpickle
 
 # NodeGraph
 
 [![Unit test](https://github.com/scinode/node_graph/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/scinode/node_graph/actions/workflows/unit_test.yaml)
 
 A platform for designing node-based workflows.
```

### Comparing `node_graph-0.0.3/README.md` & `node_graph-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/analysis.py` & `node_graph-0.0.4/node_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/collection.py` & `node_graph-0.0.4/node_graph/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,32 @@
     Attributes:
         path (str): path to import the module.
     """
 
     path: str = ""
     parent_name: str = "parent"
 
-    def __init__(self, parent=None, pool=None, entry_point=None) -> None:
+    def __init__(self, parent=None, pool=None, entry_point=None,
+                 post_creation_hooks=None,
+                 post_deletion_hooks=None) -> None:
         """Init a collection instance
 
         Args:
             parent (unknow): object this collection belongs to.
         """
         self._items = []
         self.parent = parent
         # one can specify the pool or entry_point to get the pool
         # if pool is not None, entry_point will be ignored, e.g., Link has no pool
         if pool is not None:
             self.pool = pool
         elif entry_point is not None:
             self.pool = get_entries(entry_point_name=entry_point)
+        self.post_creation_hooks = post_creation_hooks or []
+        self.post_deletion_hooks = post_deletion_hooks or []
 
     def __iter__(self):
         for item in self._items:
             yield item
 
     def __getitem__(self, index):
         if isinstance(index, int):
@@ -129,14 +133,15 @@
 
         Args:
             name (str): _description_
         """
         for index, item in enumerate(self._items):
             if item.name == name:
                 del self._items[index]
+                self.execute_post_deletion_hooks(item)
                 return
 
     def __len__(self):
         return len(self._items)
 
     def __repr__(self) -> str:
         s = ""
@@ -144,14 +149,24 @@
         return s
 
     def copy(self, parent=None):
         coll = self.__class__(parent=parent)
         coll._items = [item.copy() for item in self._items]
         return coll
 
+    def execute_post_creation_hooks(self, item):
+        """Execute all functions in post_creation_hooks with the given item."""
+        for func in self.post_creation_hooks:
+            func(self, item)
+    
+    def execute_post_deletion_hooks(self, item):
+        """Execute all functions in post_deletion_hooks with the given item."""
+        for func in self.post_deletion_hooks:
+            func(self, item)
+
 
 def decorator_check_identifier_name(func):
     """Check identifier and name exist or not.
 
     Args:
         func (_type_): _description_
     """
@@ -184,16 +199,16 @@
 
 
 class NodeCollection(Collection):
     """Node colleciton"""
 
     parent_name = "node_graph"
 
-    def __init__(self, parent=None, pool=None, entry_point="node_graph.node") -> None:
-        super().__init__(parent, pool=pool, entry_point=entry_point)
+    def __init__(self, parent=None, pool=None, entry_point="node_graph.node", post_creation_hooks=None) -> None:
+        super().__init__(parent, pool=pool, entry_point=entry_point, post_creation_hooks=post_creation_hooks)
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None, uuid=None, **kwargs):
         from node_graph.node import Node
 
         inner_id = self.get_inner_id()
         if isinstance(identifier, str):
@@ -205,14 +220,16 @@
         ):
             ItemClass = identifier.node
         else:
             raise Exception(f"Identifier {identifier} is not a node or node name.")
         item = ItemClass(inner_id=inner_id, name=name, uuid=uuid, parent=self.parent)
         self.append(item)
         item.set(kwargs)
+        # Execute post creation hooks
+        self.execute_post_creation_hooks(item)
         return item
 
     def copy(self, parent=None):
         coll = self.__class__(parent=parent)
         coll._items = [item.copy(parent=parent) for item in self._items]
         return coll
 
@@ -329,14 +346,17 @@
         super().__init__(parent)
 
     def new(self, input, output, type=1):
         from node_graph.link import NodeLink
 
         item = NodeLink(input, output)
         self.append(item)
+        # Execute post creation hooks
+        self.execute_post_creation_hooks(item)
+        return item
 
     def __delitem__(self, index):
         """Delete link from this collection.
 
         First remove the link in the nodes by calling the unmount method.
 
         Args:
```

### Comparing `node_graph-0.0.3/node_graph/decorator.py` & `node_graph-0.0.4/node_graph/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     Returns:
         _type_: _description_
     """
     from node_graph.node import Node
 
     Node = ndata.get("node_class", Node)
 
-    class MyNode(Node):
+    class DecoratedNode(Node):
         identifier: str = ndata["identifier"]
         node_type: str = ndata.get("node_type", "NORMAL")
         catalog = ndata.get("catalog", "Others")
 
         def create_properties(self):
             for prop in ndata.get("properties", []):
                 kwargs = prop[2] if len(prop) > 2 else {}
@@ -128,15 +128,15 @@
             self.var_args = ndata.get("var_args", None)
             self.var_kwargs = ndata.get("var_kwargs", None)
 
         def get_executor(self):
             executor = ndata.get("executor", {})
             return executor
 
-    return MyNode
+    return DecoratedNode
 
 
 def create_node_group(ngdata):
     """Create a node group class from node group data.
 
     Args:
         ngdata (dict): node data
```

### Comparing `node_graph-0.0.3/node_graph/link.py` & `node_graph-0.0.4/node_graph/link.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/node.py` & `node_graph-0.0.4/node_graph/node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/node_graph.py` & `node_graph-0.0.4/node_graph/node_graph.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/nodes/test_nodes.py` & `node_graph-0.0.4/node_graph/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/properties/builtin.py` & `node_graph-0.0.4/node_graph/properties/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/property.py` & `node_graph-0.0.4/node_graph/property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/serializer.py` & `node_graph-0.0.4/node_graph/serializer.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/socket.py` & `node_graph-0.0.4/node_graph/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     """
 
     # this is the class of the property object
     node_property = NodeProperty
 
     identifier: str = "NodeSocket"
     default_value: float = 0.0
-    link_limit: int = 1
 
-    def __init__(self, name, parent=None, type="INPUT", inner_id=0, uuid=None) -> None:
+    def __init__(self, name, parent=None, type="INPUT", inner_id=0, uuid=None, link_limit=1) -> None:
         """Init a instance of NodeSocket.
 
         Args:
             name (str): name of the socket
             node (_type_, optional): _description_. Defaults to None.
             inner_id (int, optional): _description_. Defaults to 0.
         """
         self.name = name
         self.parent = parent
         self.type = type
         self.inner_id = inner_id
         self.uuid = uuid or str(uuid1())
         self.links = []
         self.property = None
+        self.link_limit = link_limit
 
     @property
     def node(self):
         return self.parent
 
     def to_dict(self):
         """Export to a dictionary.
```

### Comparing `node_graph-0.0.3/node_graph/sockets/builtin.py` & `node_graph-0.0.4/node_graph/sockets/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph/utils.py` & `node_graph-0.0.4/node_graph/utils.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.3/node_graph.egg-info/PKG-INFO` & `node_graph-0.0.4/node_graph.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
-Name: node-graph
-Version: 0.0.3
+Name: node_graph
+Version: 0.0.4
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: click
+Requires-Dist: pyyaml
+Requires-Dist: colorama
+Requires-Dist: termcolor
+Requires-Dist: cloudpickle
 
 # NodeGraph
 
 [![Unit test](https://github.com/scinode/node_graph/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/scinode/node_graph/actions/workflows/unit_test.yaml)
 
 A platform for designing node-based workflows.
```

### Comparing `node_graph-0.0.3/node_graph.egg-info/SOURCES.txt` & `node_graph-0.0.4/node_graph.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,17 @@
 node_graph.egg-info/requires.txt
 node_graph.egg-info/top_level.txt
 node_graph/nodes/__init__.py
 node_graph/nodes/test_nodes.py
 node_graph/properties/__init__.py
 node_graph/properties/builtin.py
 node_graph/sockets/__init__.py
-node_graph/sockets/builtin.py
+node_graph/sockets/builtin.py
+tests/test_collection.py
+tests/test_decorator.py
+tests/test_entry_point.py
+tests/test_hooks.py
+tests/test_node.py
+tests/test_nodetree.py
+tests/test_property.py
+tests/test_socket.py
+tests/test_yaml.py
```

### Comparing `node_graph-0.0.3/setup.py` & `node_graph-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="node_graph",
-    version="0.0.3",
+    version="0.0.4",
     description="Create node-based workflow",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/node-graph",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

