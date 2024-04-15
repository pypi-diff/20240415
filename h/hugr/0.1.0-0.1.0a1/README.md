# Comparing `tmp/hugr-0.1.0.tar.gz` & `tmp/hugr-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugr-0.1.0.tar", max compression
+gzip compressed data, was "hugr-0.1.0a1.tar", max compression
```

## Comparing `hugr-0.1.0.tar` & `hugr-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1446 2024-04-15 16:30:20.119342 hugr-0.1.0/README.md
--rw-r--r--   0        0        0     1130 2024-04-15 16:30:20.119342 hugr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      209 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/py.typed
--rw-r--r--   0        0        0       62 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/serialization/__init__.py
--rw-r--r--   0        0        0    16294 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/serialization/ops.py
--rw-r--r--   0        0        0      894 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/serialization/serial_hugr.py
--rw-r--r--   0        0        0     8033 2024-04-15 16:30:20.119342 hugr-0.1.0/src/hugr/serialization/tys.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 hugr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1446 2024-04-03 17:19:08.176174 hugr-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1132 2024-04-03 17:19:08.176174 hugr-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/__init__.py
+-rw-r--r--   0        0        0    17296 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/ops.py
+-rw-r--r--   0        0        0      894 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/serial_hugr.py
+-rw-r--r--   0        0        0     8041 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/tys.py
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 hugr-0.1.0a1/PKG-INFO
```

### Comparing `hugr-0.1.0/README.md` & `hugr-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `hugr-0.1.0/pyproject.toml` & `hugr-0.1.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 name = "hugr"
-version = "0.1.0"
+version = "0.1.0a1"
 description = "Quantinuum's common representation for quantum programs"
 #keywords = []
 authors = ["TKET development team <tket-support@cambridgequantum.com>"]
 maintainers = ["TKET development team <tket-support@cambridgequantum.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/CQCL/hugr"
```

### Comparing `hugr-0.1.0/src/hugr/serialization/ops.py` & `hugr-0.1.0a1/src/hugr/serialization/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -296,14 +296,21 @@
 class LoadConstant(DataflowOp):
     """An operation that loads a static constant in to the local dataflow graph."""
 
     op: Literal["LoadConstant"] = "LoadConstant"
     datatype: Type
 
 
+class LeafOpBase(DataflowOp):
+    """Simple operation that has only value inputs+outputs and (potentially) StateOrder
+    edges."""
+
+    op: Literal["LeafOp"] = "LeafOp"
+
+
 class DFG(DataflowOp):
     """A simply nested dataflow graph."""
 
     op: Literal["DFG"] = "DFG"
     signature: FunctionType = Field(default_factory=FunctionType.empty)
 
     def insert_child_dfg_signature(self, inputs: TypeRow, outputs: TypeRow) -> None:
@@ -382,19 +389,24 @@
             input=list(inputs), output=list(outputs), extension_reqs=ExtensionSet([])
         )
 
 
 ControlFlowOp = Conditional | TailLoop | CFG
 
 
-class CustomOp(DataflowOp):
+# -----------------------------------------
+# --------------- LeafOp ------------------
+# -----------------------------------------
+
+
+class CustomOp(LeafOpBase):
     """A user-defined operation that can be downcasted by the extensions that define
     it."""
 
-    op: Literal["CustomOp"] = "CustomOp"
+    lop: Literal["CustomOp"] = "CustomOp"
     extension: ExtensionId
     op_name: str
     signature: tys.FunctionType = Field(default_factory=tys.FunctionType.empty)
     description: str = ""
     args: list[tys.TypeArg] = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
@@ -409,64 +421,90 @@
             "description": (
                 "A user-defined operation that can be downcasted by the extensions that "
                 "define it."
             )
         }
 
 
-class Noop(DataflowOp):
+class Noop(LeafOpBase):
     """A no-op operation."""
 
-    op: Literal["Noop"] = "Noop"
+    lop: Literal["Noop"] = "Noop"
     ty: Type
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         assert len(in_types) == 1
         assert len(out_types) == 1
         assert in_types[0] == out_types[0]
         self.ty = in_types[0]
 
 
-class MakeTuple(DataflowOp):
+class MakeTuple(LeafOpBase):
     """An operation that packs all its inputs into a tuple."""
 
-    op: Literal["MakeTuple"] = "MakeTuple"
+    lop: Literal["MakeTuple"] = "MakeTuple"
     tys: TypeRow = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         # If we have a single order edge as input, this is a unit
         if in_types == [None]:
             in_types = []
         self.tys = list(in_types)
 
 
-class UnpackTuple(DataflowOp):
+class UnpackTuple(LeafOpBase):
     """An operation that packs all its inputs into a tuple."""
 
-    op: Literal["UnpackTuple"] = "UnpackTuple"
+    lop: Literal["UnpackTuple"] = "UnpackTuple"
     tys: TypeRow = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         self.tys = list(out_types)
 
 
-class Tag(DataflowOp):
+class Tag(LeafOpBase):
     """An operation that creates a tagged sum value from one of its variants."""
 
-    op: Literal["Tag"] = "Tag"
+    lop: Literal["Tag"] = "Tag"
     tag: int  # The variant to create.
     variants: TypeRow  # The variants of the sum type.
 
 
-class Lift(DataflowOp):
+class TypeApply(LeafOpBase):
     """Fixes some TypeParams of a polymorphic type by providing TypeArgs."""
 
-    op: Literal["Lift"] = "Lift"
-    type_row: TypeRow
-    new_extension: ExtensionId
+    lop: Literal["TypeApply"] = "TypeApply"
+    ta: "TypeApplication"
+
+
+class TypeApplication(BaseModel):
+    """Records details of an application of a PolyFuncType to some TypeArgs and the
+    result (a less-, but still potentially-, polymorphic type).
+    """
+
+    input: PolyFuncType
+    args: list[tys.TypeTypeArg]
+    output: PolyFuncType
+
+    class Config:
+        # Needed to avoid random '\n's in the pydantic description
+        json_schema_extra = {
+            "description": (
+                "Records details of an application of a PolyFuncType to some TypeArgs "
+                "and the result (a less-, but still potentially-, polymorphic type)."
+            )
+        }
+
+
+class LeafOp(RootModel):
+    """A constant operation."""
+
+    root: CustomOp | Noop | MakeTuple | UnpackTuple | Tag | TypeApply = Field(
+        discriminator="lop"
+    )
 
 
 class OpType(RootModel):
     """A constant operation."""
 
     root: (
         Module
@@ -480,20 +518,15 @@
         | TailLoop
         | CFG
         | Input
         | Output
         | Call
         | CallIndirect
         | LoadConstant
-        | CustomOp
-        | Noop
-        | MakeTuple
-        | UnpackTuple
-        | Tag
-        | Lift
+        | LeafOp
         | DFG
     ) = Field(discriminator="op")
 
 
 # --------------------------------------
 # --------------- OpDef ----------------
 # --------------------------------------
```

### Comparing `hugr-0.1.0/src/hugr/serialization/serial_hugr.py` & `hugr-0.1.0a1/src/hugr/serialization/serial_hugr.py`

 * *Files identical despite different names*

### Comparing `hugr-0.1.0/src/hugr/serialization/tys.py` & `hugr-0.1.0a1/src/hugr/serialization/tys.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
 # ----------------------------------------------
 # --------------- ClassicType ------------------
 # ----------------------------------------------
 
 
 class Variable(BaseModel):
-    """A type variable identified by an index into the array of TypeParams."""
+    """A type variable identified by a de Bruijn index."""
 
     t: Literal["V"] = "V"
     i: int
     b: "TypeBound"
 
 
 class USize(BaseModel):
@@ -185,16 +185,14 @@
     t: Literal["I"] = "I"
 
 
 class FunctionType(BaseModel):
     """A graph encoded as a value. It contains a concrete signature and a set of
     required resources."""
 
-    t: Literal["G"] = "G"
-
     input: "TypeRow"  # Value inputs of the function.
     output: "TypeRow"  # Value outputs of the function.
     # The extension requirements which are added by the operation
     extension_reqs: "ExtensionSet" = Field(default_factory=list)
 
     @classmethod
     def empty(cls) -> "FunctionType":
@@ -207,35 +205,38 @@
                 "A graph encoded as a value. It contains a concrete signature and "
                 "a set of required resources."
             )
         }
 
 
 class PolyFuncType(BaseModel):
-    """A polymorphic type scheme, i.e. of a FuncDecl, FuncDefn or OpDef.
-    (Nodes/operations in the Hugr are not polymorphic.)"""
+    """A graph encoded as a value. It contains a concrete signature and a set of
+    required resources."""
+
+    t: Literal["G"] = "G"
 
     # The declared type parameters, i.e., these must be instantiated with the same
-    # number of TypeArgs before the function can be called. This defines the indices
-    # used for variables within the body.
+    # number of TypeArgs before the function can be called. Note that within the body,
+    # variable (DeBruijn) index 0 is element 0 of this array, i.e. the variables are
+    # bound from right to left.
     params: list[TypeParam]
 
     # Template for the function. May contain variables up to length of `params`
     body: FunctionType
 
     @classmethod
     def empty(cls) -> "PolyFuncType":
         return PolyFuncType(params=[], body=FunctionType.empty())
 
     class Config:
         # Needed to avoid random '\n's in the pydantic description
         json_schema_extra = {
             "description": (
-                "A polymorphic type scheme, i.e. of a FuncDecl, FuncDefn or OpDef.  "
-                "(Nodes/operations in the Hugr are not polymorphic.)"
+                "A graph encoded as a value. It contains a concrete signature and "
+                "a set of required resources."
             )
         }
 
 
 class TypeBound(Enum):
     Eq = "E"
     Copyable = "C"
@@ -274,15 +275,15 @@
     t: Literal["Q"] = "Q"
 
 
 class Type(RootModel):
     """A HUGR type."""
 
     root: Annotated[
-        Qubit | Variable | USize | FunctionType | Array | SumType | Opaque,
+        Qubit | Variable | USize | PolyFuncType | Array | SumType | Opaque,
         WrapValidator(_json_custom_error_validator),
     ] = Field(discriminator="t")
 
 
 # -------------------------------------------
 # --------------- TypeRow -------------------
 # -------------------------------------------
```

### Comparing `hugr-0.1.0/PKG-INFO` & `hugr-0.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugr
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: Quantinuum's common representation for quantum programs
 Home-page: https://github.com/CQCL/hugr
 License: Apache-2.0
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 Maintainer: TKET development team
 Maintainer-email: tket-support@cambridgequantum.com
```

