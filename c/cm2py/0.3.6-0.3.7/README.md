# Comparing `tmp/cm2py-0.3.6.tar.gz` & `tmp/cm2py-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.3.6.tar", last modified: Wed Mar  6 02:34:40 2024, max compression
+gzip compressed data, was "cm2py-0.3.7.tar", last modified: Mon Apr 15 07:01:24 2024, max compression
```

## Comparing `cm2py-0.3.6.tar` & `cm2py-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-06 02:34:40.994446 cm2py-0.3.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1096 2024-03-06 00:37:08.000000 cm2py-0.3.6/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3013 2024-03-06 02:34:40.994446 cm2py-0.3.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1186 2024-03-06 02:33:15.000000 cm2py-0.3.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      651 2024-03-06 02:33:15.000000 cm2py-0.3.6/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-06 02:34:40.994446 cm2py-0.3.6/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-06 02:34:40.990446 cm2py-0.3.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-06 02:34:40.990446 cm2py-0.3.6/src/cm2py/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      264 2024-03-06 02:33:15.000000 cm2py-0.3.6/src/cm2py/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7579 2024-03-06 02:33:15.000000 cm2py-0.3.6/src/cm2py/cm2py.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-06 02:34:40.994446 cm2py-0.3.6/src/cm2py.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3013 2024-03-06 02:34:40.000000 cm2py-0.3.6/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      255 2024-03-06 02:34:40.000000 cm2py-0.3.6/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-06 02:34:40.000000 cm2py-0.3.6/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2024-03-06 02:34:40.000000 cm2py-0.3.6/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2024-03-06 02:34:40.000000 cm2py-0.3.6/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-06 02:34:40.990446 cm2py-0.3.6/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3195 2024-03-06 02:33:15.000000 cm2py-0.3.6/tests/test_app.py
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/
+-rw-rw-r--   0 skm       (1000) skm       (1000)     1096 2024-04-15 05:31:45.000000 cm2py-0.3.7/LICENSE
+-rw-r--r--   0 skm       (1000) skm       (1000)     3013 2024-04-15 07:01:24.837779 cm2py-0.3.7/PKG-INFO
+-rw-rw-r--   0 skm       (1000) skm       (1000)     1186 2024-04-15 05:31:45.000000 cm2py-0.3.7/README.md
+-rw-rw-r--   0 skm       (1000) skm       (1000)      651 2024-04-15 06:57:25.000000 cm2py-0.3.7/pyproject.toml
+-rw-rw-r--   0 skm       (1000) skm       (1000)       38 2024-04-15 07:01:24.837779 cm2py-0.3.7/setup.cfg
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.833779 cm2py-0.3.7/src/
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.833779 cm2py-0.3.7/src/cm2py/
+-rw-rw-r--   0 skm       (1000) skm       (1000)      264 2024-04-15 05:31:45.000000 cm2py-0.3.7/src/cm2py/__init__.py
+-rw-rw-r--   0 skm       (1000) skm       (1000)     7880 2024-04-15 06:40:40.000000 cm2py-0.3.7/src/cm2py/cm2py.py
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/src/cm2py/utilities/
+-rw-rw-r--   0 skm       (1000) skm       (1000)       48 2024-04-15 06:53:57.000000 cm2py-0.3.7/src/cm2py/utilities/__init__.py
+-rw-rw-r--   0 skm       (1000) skm       (1000)     7419 2024-04-15 07:01:05.000000 cm2py-0.3.7/src/cm2py/utilities/utilities.py
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/src/cm2py.egg-info/
+-rw-r--r--   0 skm       (1000) skm       (1000)     3013 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/PKG-INFO
+-rw-rw-r--   0 skm       (1000) skm       (1000)      320 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-r--   0 skm       (1000) skm       (1000)        1 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-r--   0 skm       (1000) skm       (1000)       11 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/requires.txt
+-rw-rw-r--   0 skm       (1000) skm       (1000)        6 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/top_level.txt
+drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/tests/
+-rw-rw-r--   0 skm       (1000) skm       (1000)     3195 2024-04-15 05:31:45.000000 cm2py-0.3.7/tests/test_app.py
```

### Comparing `cm2py-0.3.6/LICENSE` & `cm2py-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.3.6/PKG-INFO` & `cm2py-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.3.6
+Version: 0.3.7
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.3.6/README.md` & `cm2py-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.3.6/pyproject.toml` & `cm2py-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.3.6"
+version = "0.3.7"
 authors = [{ name = "SKM GEEK", email = "qestudios17@gmail.com" }]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `cm2py-0.3.6/src/cm2py/cm2py.py` & `cm2py-0.3.7/src/cm2py/cm2py.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,62 +4,121 @@
 This module contains utilities to generate and manipulate save strings
 for the Roblox game Circuit Maker 2 by ismellbeef1.
 """
 
 __author__ = "SKM GEEK"
 __contact__ = "qestudios17@gmail.com"
 __copyright__ = "Copyright 2024, SKM GEEK"
-__date__ = "2023/05/21"
+__date__ = "2024/04/14"
 __deprecated__ = False
 __email__ = "qestudios17@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 from uuid import uuid4
 import math
 import regex as re
+from typing import Literal, Callable
+import string
+import struct
+
+
+class Block:
+    __initialised = False
+
+    def __init__(self, blockId, pos, state=False, properties=None):
+        assert (
+            isinstance(blockId, int) and 0 <= blockId <= 17
+        ), "blockId must be an integer between 0 and 17"
+        assert (
+            isinstance(pos, tuple)
+            and len(pos) == 3
+            and (isinstance(pos[0], (float, int)))
+            and (isinstance(pos[1], (float, int)))
+            and (isinstance(pos[2], (float, int)))
+        ), "pos must be a 3d tuple of integers or floats"
+        assert isinstance(state, bool), "state must be a boolean"
+        assert (
+            isinstance(properties, list) or properties is None
+        ), "properties must be a list of numbers, or None."
+        self.blockId = blockId
+        self.pos = pos
+        self.x = self.pos[0]
+        self.y = self.pos[1]
+        self.z = self.pos[2]
+        self.state = state
+        self.properties = properties
+        self.uuid = str(uuid4())
+
+        self.__initialised = True
+
+    def __setattr__(self, name, value):
+        self.__dict__[name] = value
+        if not self.__initialised:
+            return
+        if name == "pos":
+            self.__dict__["x"] = self.pos[0]
+            self.__dict__["y"] = self.pos[1]
+            self.__dict__["z"] = self.pos[2]
+        elif name in ["x", "y", "z"]:
+            self.__dict__["pos"] = (self.x, self.y, self.z)
+
+
+class Connection:
+    def __init__(self, source, target):
+        assert isinstance(source, Block), "source must be a Block object"
+        assert isinstance(target, Block), "target must be a Block object"
+        self.source = source
+        self.target = target
 
 
 class Save:
     """A class to represent a save, which can be modified."""
 
     def __init__(self):
         self.blocks = {}
         self.connections = {}
         self.blockCount = 0
         self.connectionCount = 0
 
-    def addBlock(self, blockId, pos, state=False, properties=None, snapToGrid=True):
+    def addBlock(
+        self,
+        blockId: int,
+        pos: tuple[float, float, float],
+        state: bool = False,
+        properties: bool = None,
+        snapToGrid: bool = True,
+    ) -> Block:
         """Add a block to the save."""
         if snapToGrid:
             newBlock = Block(
                 blockId,
                 tuple([int(math.floor(i)) for i in pos]),
                 state=state,
                 properties=properties,
             )
         else:
             newBlock = Block(blockId, pos, state=state, properties=properties)
         self.blocks[newBlock.uuid] = newBlock
         self.blockCount += 1
         return newBlock
 
-    def addConnection(self, source, target):
+    def addConnection(self, source: Block, target: Block) -> Connection:
         """Add a connection to the save."""
         newConnection = Connection(source, target)
         if newConnection.target.uuid in self.connections:
             self.connections[newConnection.target.uuid].append(newConnection)
         else:
             self.connections[newConnection.target.uuid] = [newConnection]
         self.connectionCount += 1
         return newConnection
 
-    def exportSave(self):
+    def exportSave(self) -> str:
         """Export the save to a Circuit Maker 2 save string."""
         string = ""
         blockIndexes = {}
         index = 0
 
         assert self.blockCount > 0, "Saves with less than 1 block cannot be exported."
 
@@ -76,94 +135,45 @@
                     f"{blockIndexes[n.source.uuid]+1},{blockIndexes[n.target.uuid]+1};"
                 )
         if self.connectionCount > 0:
             string = string[:-1]
         string = string + "??"  # TODO: Custom build support & sign data support
         return string
 
-    def deleteBlock(self, blockRef):
+    def deleteBlock(self, blockRef: Block) -> None:
         """Delete a block from the save."""
         assert isinstance(blockRef, Block), "blockRef must be a Block object"
         assert blockRef.uuid in self.blocks, "block does not exist in save"
         for c in self.connections.values():
             for n in c:
                 if n.source.uuid == blockRef.uuid or n.target.uuid == blockRef.uuid:
                     del self.connections[n.target.uuid][
                         self.connections[n.target.uuid].index(n)
                     ]
                     break
         del self.blocks[blockRef.uuid]
         self.blockCount -= 1
         return
 
-    def deleteConnection(self, connectionRef):
+    def deleteConnection(self, connectionRef: Connection) -> None:
         """Delete a connection from the save."""
         assert isinstance(
             connectionRef, Connection
         ), "connectionRef must be a Connection object"
         assert connectionRef in (n for c in self.connections.values() for n in c)
         for c in self.connections.values():
             for n in c:
                 if connectionRef == n:
                     del self.connections[n.target.uuid][
                         self.connections[n.target.uuid].index(n)
                     ]
         self.connectionCount -= 1
 
 
-class Block:
-    __initialised = False
-
-    def __init__(self, blockId, pos, state=False, properties=None):
-        assert (
-            isinstance(blockId, int) and 0 <= blockId <= 17
-        ), "blockId must be an integer between 0 and 17"
-        assert (
-            isinstance(pos, tuple)
-            and len(pos) == 3
-            and (isinstance(pos[0], (float, int)))
-            and (isinstance(pos[1], (float, int)))
-            and (isinstance(pos[2], (float, int)))
-        ), "pos must be a 3d tuple of integers or floats"
-        assert isinstance(state, bool), "state must be a boolean"
-        assert (
-            isinstance(properties, list) or properties is None
-        ), "properties must be a list of numbers, or None."
-        self.blockId = blockId
-        self.pos = pos
-        self.x = self.pos[0]
-        self.y = self.pos[1]
-        self.z = self.pos[2]
-        self.state = state
-        self.properties = properties
-        self.uuid = str(uuid4())
-
-        self.__initialised = True
-
-    def __setattr__(self, name, value):
-        self.__dict__[name] = value
-        if not self.__initialised:
-            return
-        if name == "pos":
-            self.__dict__["x"] = self.pos[0]
-            self.__dict__["y"] = self.pos[1]
-            self.__dict__["z"] = self.pos[2]
-        elif name in ["x", "y", "z"]:
-            self.__dict__["pos"] = (self.x, self.y, self.z)
-
-
-class Connection:
-    def __init__(self, source, target):
-        assert isinstance(source, Block), "source must be a Block object"
-        assert isinstance(target, Block), "target must be a Block object"
-        self.source = source
-        self.target = target
-
-
-def validateSave(string):
+def validateSave(string: str) -> re.Match | None:
     """Check whether a string is a valid savestring or not."""
     # fmt: off
     regex = (
         r"(?<![\d\w,;?+])" # Blocks
         r"(?>"
           r"(?<b>"
             r"\d+,"
@@ -197,15 +207,15 @@
         r")*"
         r"(?![\d\w,;?+])$"
     )
     # fmt: on
     return re.match(regex, string)
 
 
-def importSave(string, snapToGrid=True):
+def importSave(string: str, snapToGrid: bool = True) -> Save:
     """Import a Circuit Maker 2 save string as a save."""
     assert validateSave(string), "invalid save string"
 
     newSave = Save()
 
     sections = string.split("?")
     blockString = sections[0].split(";")
```

### Comparing `cm2py-0.3.6/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.3.7/src/cm2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.3.6
+Version: 0.3.7
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.3.6/tests/test_app.py` & `cm2py-0.3.7/tests/test_app.py`

 * *Files identical despite different names*

