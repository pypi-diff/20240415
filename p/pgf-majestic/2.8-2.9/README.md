# Comparing `tmp/pgf_majestic-2.8-cp39-cp39-win_amd64.whl.zip` & `tmp/pgf_majestic-2.9-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 112467 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   249344 b- defN 24-Jan-18 11:36 pgf.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    18686 b- defN 24-Jan-18 11:32 pgf_majestic-2.8.data/data/pgf.pyi
--rw-rw-rw-  2.0 fat      493 b- defN 24-Jan-18 11:36 pgf_majestic-2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Jan-18 11:36 pgf_majestic-2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Jan-18 11:36 pgf_majestic-2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      482 b- defN 24-Jan-18 11:36 pgf_majestic-2.8.dist-info/RECORD
-6 files, 269109 bytes uncompressed, 111597 bytes compressed:  58.5%
+Zip file size: 119694 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   265216 b- defN 24-Apr-15 09:29 pgf.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    19696 b- defN 24-Apr-15 09:24 pgf_majestic-2.9.data/data/pgf.pyi
+-rw-rw-rw-  2.0 fat      493 b- defN 24-Apr-15 09:29 pgf_majestic-2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 24-Apr-15 09:29 pgf_majestic-2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-15 09:29 pgf_majestic-2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      483 b- defN 24-Apr-15 09:29 pgf_majestic-2.9.dist-info/RECORD
+6 files, 285994 bytes uncompressed, 118822 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: pgf.cp39-win_amd64.pyd
+Filename: pgf.cp311-win_amd64.pyd
 Comment: 
 
-Filename: pgf_majestic-2.8.data/data/pgf.pyi
+Filename: pgf_majestic-2.9.data/data/pgf.pyi
 Comment: 
 
-Filename: pgf_majestic-2.8.dist-info/METADATA
+Filename: pgf_majestic-2.9.dist-info/METADATA
 Comment: 
 
-Filename: pgf_majestic-2.8.dist-info/WHEEL
+Filename: pgf_majestic-2.9.dist-info/WHEEL
 Comment: 
 
-Filename: pgf_majestic-2.8.dist-info/top_level.txt
+Filename: pgf_majestic-2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pgf_majestic-2.8.dist-info/RECORD
+Filename: pgf_majestic-2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pgf_majestic-2.8.data/data/pgf.pyi` & `pgf_majestic-2.9.data/data/pgf.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -110,23 +110,33 @@
         """
         Computes the conditional log-probability - log P(e | C)
         by summing the probabilities of all functions appearing
         in the tree.
         """
         ...
 
-    def generateRandom(cat : Type, depth : int = 5) -> tuple[Expr,float]:
+    def generateRandom(self, cat : Type, depth : int = 5) -> tuple[Expr,float]:
         """
         Generates a random abstract syntax trees of the given type.
         The depth parameter specifies the maximal distance between
         the root and a leaf in the tree. The float value in
         the result is the probability of the tree.
         """
         ...
 
+    def graphvizAbstractTree(self, e: Expr,
+                             noFun:bool=False, noCat:bool=False,
+                             nodeFont:str="",
+                             nodeColor:str="",
+                             nodeEdgeStyle:str="") -> str:
+        """
+        Renders an abstract syntax tree in a Graphviz format
+        """
+        ...
+
     def newTransaction(self) -> Transaction:
         """
         Starts a new transaction which makes it possible to update
         the grammar dynamically. The method is supposed to be used
         in the with statements:
 
         with gr.newTransaction() as t:
@@ -204,27 +214,43 @@
 
 class Concr:
     @property
     def name(self) -> str:
         """The name of the concrete syntax"""
         ...
 
-    def linearize(e: Expr) -> str:
+    def linearize(self, e: Expr) -> str:
         """Linearizes the abstract expression and returns as string"""
         ...
 
-    def bracketedLinearize(e: Expr) -> list[Any]:
+    def bracketedLinearize(self, e: Expr) -> list[Any]:
         """
         Produces a bracketed linearization where syntactic phrases
         are represented as objects of type Bracket and terminal tokens
         are represented as string. When two tokens have to be glued
         together, an object of type BIND is inserted.
         """
         ...
 
+    def hasLinearization(self, fun: Str) -> bool:
+        """
+        Returns true if the given function has linearization in the concrete syntax
+        """
+        ...
+
+    def graphvizParseTree(self, e: Expr,
+                          noLeaves:bool=False, noFun:bool=False, noCat:bool=False,
+                          nodeFont:str="", leafFont:str="",
+                          nodeColor:str="", leafColor:str="",
+                          nodeEdgeStyle:str="", leafEdgeStyle:str="") -> str:
+        """
+        Renders an abstract syntax tree as a parse tree in Graphviz format
+        """
+        ...
+
 class PGFError:
     """
     This is the exception that several functions throw
     when something unexpected happens.
     """
     ...
```

