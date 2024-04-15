# Comparing `tmp/optype-0.3.1.tar.gz` & `tmp/optype-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optype-0.3.1.tar", max compression
+gzip compressed data, was "optype-0.4.0.tar", max compression
```

## Comparing `optype-0.3.1.tar` & `optype-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1505 2024-01-28 23:47:55.624920 optype-0.3.1/LICENSE
--rw-r--r--   0        0        0    42333 2024-04-01 18:53:22.419171 optype-0.3.1/README.md
--rw-r--r--   0        0        0     9442 2024-03-21 20:06:54.536298 optype-0.3.1/optype/__init__.py
--rw-r--r--   0        0        0    18908 2024-04-01 18:53:22.419171 optype-0.3.1/optype/_can.py
--rw-r--r--   0        0        0     6166 2024-04-01 18:53:22.419171 optype-0.3.1/optype/_do.py
--rw-r--r--   0        0        0    13819 2024-03-21 20:06:54.540298 optype-0.3.1/optype/_does.py
--rw-r--r--   0        0        0     2145 2024-03-21 20:06:54.540298 optype-0.3.1/optype/_has.py
--rw-r--r--   0        0        0        0 2024-01-28 23:47:08.164059 optype-0.3.1/optype/py.typed
--rw-r--r--   0        0        0     4733 2024-04-01 18:53:22.583175 optype-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    42751 1970-01-01 00:00:00.000000 optype-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-01-28 23:47:55.624920 optype-0.4.0/LICENSE
+-rw-r--r--   0        0        0    42903 2024-04-15 04:46:42.981133 optype-0.4.0/README.md
+-rw-r--r--   0        0        0     9442 2024-03-21 20:06:54.536298 optype-0.4.0/optype/__init__.py
+-rw-r--r--   0        0        0    22789 2024-04-15 04:46:42.981133 optype-0.4.0/optype/_can.py
+-rw-r--r--   0        0        0     6500 2024-04-15 04:46:42.981133 optype-0.4.0/optype/_do.py
+-rw-r--r--   0        0        0    14220 2024-04-15 04:46:42.981133 optype-0.4.0/optype/_does.py
+-rw-r--r--   0        0        0     2769 2024-04-15 04:46:42.981133 optype-0.4.0/optype/_has.py
+-rw-r--r--   0        0        0        0 2024-01-28 23:47:08.164059 optype-0.4.0/optype/py.typed
+-rw-r--r--   0        0        0     5415 2024-04-15 04:46:43.125137 optype-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    43987 1970-01-01 00:00:00.000000 optype-0.4.0/PKG-INFO
```

### Comparing `optype-0.3.1/LICENSE` & `optype-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optype-0.3.1/README.md` & `optype-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,46 +7,46 @@
 <p align="center">
     Building blocks for precise & flexible type hints.
 </p>
 
 <p align="center">
     <a href="https://github.com/jorenham/optype/actions?query=workflow%3ACI">
         <img
-            alt="Continuous Integration"
+            alt="optype - CI"
             src="https://github.com/jorenham/optype/workflows/CI/badge.svg"
         />
     </a>
     <a href="https://pypi.org/project/optype/">
         <img
-            alt="PyPI"
+            alt="optype - PyPI"
             src="https://img.shields.io/pypi/v/optype?style=flat"
         />
     </a>
     <a href="https://github.com/jorenham/optype">
         <img
-            alt="Python Versions"
+            alt="optype - Python Versions"
             src="https://img.shields.io/pypi/pyversions/optype?style=flat"
         />
     </a>
     <a href="https://github.com/jorenham/optype">
         <img
-            alt="License"
+            alt="optype - license"
             src="https://img.shields.io/github/license/jorenham/optype?style=flat"
         />
     </a>
-    <a href="https://github.com/astral-sh/ruff">
+    <a href="https://detachhead.github.io/basedpyright">
         <img
-            alt="Ruff"
-            src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json"
+            alt="optype - basedpyright"
+            src="https://img.shields.io/badge/basedpyright-checked-42b983"
         />
     </a>
-    <a href="https://github.com/microsoft/pyright">
+    <a href="https://github.com/astral-sh/ruff">
         <img
-            alt="Checked with pyright"
-            src="https://microsoft.github.io/pyright/img/pyright_badge.svg"
+            alt="optype - ruff"
+            src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json"
         />
     </a>
 </p>
 
 ---
 
 ## Installation
@@ -74,34 +74,85 @@
 
 This is where `optype` comes in handy, which has single-method protocols for
 *all* the builtin special methods.
 For `twice`, we can use `optype.CanRMul[X, Y]`, which, as the name suggests,
 is a protocol with (only) the `def __rmul__(self, x: X) -> Y: ...` method.
 With this, the `twice` function can written as:
 
+<table>
+<tr>
+<th>Python 3.11</th>
+<th>Python 3.12</th>
+</tr>
+<tr>
+<td>
+
+```python
+from typing import Literal, TypeAlias, TypeVar
+from optype import CanRMul
+
+Y = TypeVar('Y')
+Two: TypeAlias = Literal[2]
+
+def twice(x: CanRMul[Two, Y]) -> Y:
+    return 2 * x
+```
+
+</td>
+<td>
+
 ```python
-import typing
-import optype
+from typing import Literal
+from optype import CanRMul
 
-type Two = typing.Literal[2]
 
-def twice[Y](x: optype.CanRMul[Two, Y], /) -> Y:
+type Two = Literal[2]
+
+def twice[Y](x: CanRMul[Two, Y]) -> Y:
     return 2 * x
 ```
 
+</td>
+</tr>
+</table>
+
 But what about types that implement `__add__` but not `__radd__`?
-In this case, we could return `x * 2` as fallback.
+In this case, we could return `x * 2` as fallback (assuming commutativity).
 Because the `optype.Can*` protocols are runtime-checkable, the revised
 `twice2` function can be compactly written as:
 
+<table>
+<tr>
+<th>Python 3.11</th>
+<th>Python 3.12</th>
+</tr>
+<tr>
+<td>
+
 ```python
-def twice2[Y](x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y:
-    return 2 * x if isinstance(x, optype.CanRMul) else x * 2
+from optype import CanMul
+
+def twice2(x: CanRMul[Two, Y] | CanMul[Two, Y]) -> Y:
+    return 2 * x if isinstance(x, CanRMul) else x * 2
 ```
 
+</td>
+<td>
+
+```python
+from optype import CanMul
+
+def twice2[Y](x: CanRMul[Two, Y] | CanMul[Two, Y]) -> Y:
+    return 2 * x if isinstance(x, CanRMul) else x * 2
+```
+
+</td>
+</tr>
+</table>
+
 See [`examples/twice.py`](examples/twice.py) for the full example.
 
 ## Overview
 
 The API of `optype` is flat; a single `import optype` is all you need.
 There are four flavors of things that live within `optype`,
 
@@ -1392,15 +1443,14 @@
 It can conveniently be used to check whether a type or instance is a
 dataclass, i.e. `isinstance(obj, optype.HasDataclassFields)`.
 
 [DC]: https://docs.python.org/3/library/dataclasses.html
 
 ## Future plans
 
-- Support for Python versions before 3.12 (#19).
 - [numpy][NP] interfaces for arrays-like types (no deps) (#24)
 - [array-api][API-ND] interfaces (no deps) (#25)
 - [dataframe-api][API-DF] interfaces (no deps) (#26)
 
 [NP]: https://github.com/numpy/numpy
 [API-ND]: https://data-apis.org/array-api/latest/
 [API-DF]: https://data-apis.org/dataframe-api/draft/index.html
```

#### html2text {}

```diff
@@ -1,51 +1,59 @@
                              ************ ooppttyyppee ************
                            One protocol, one method.
               Building blocks for precise & flexible type hints.
-  _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_C_h_e_c_k_e_d_ _w_i_t_h
-                                   _p_y_r_i_g_h_t_]
+_[_o_p_t_y_p_e_ _-_ _C_I_]_[_o_p_t_y_p_e_ _-_ _P_y_P_I_]_[_o_p_t_y_p_e_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_o_p_t_y_p_e_ _-_ _l_i_c_e_n_s_e_]_[_o_p_t_y_p_e
+                        _-_ _b_a_s_e_d_p_y_r_i_g_h_t_]_[_o_p_t_y_p_e_ _-_ _r_u_f_f_]
 --- ## Installation Optype is available as [`optype`][OPTYPE] on PyPI: ```shell
 pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Example
 Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
 Implementing it is trivial, but what about the type annotations? Because `twice
 (2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it might seem like a
 good idea to type it as `twice[T](x: T) -> T: ...`. However, that wouldn't
 include cases such as `twice(True) == 2` or `twice((42, True)) == (42, True,
 42, True)`, where the input- and output types differ. Moreover, `twice` should
 accept *any* type with a custom `__rmul__` method that accepts `2` as argument.
 This is where `optype` comes in handy, which has single-method protocols for
 *all* the builtin special methods. For `twice`, we can use `optype.CanRMul[X,
 Y]`, which, as the name suggests, is a protocol with (only) the `def __rmul__
 (self, x: X) -> Y: ...` method. With this, the `twice` function can written as:
-```python import typing import optype type Two = typing.Literal[2] def twice[Y]
-(x: optype.CanRMul[Two, Y], /) -> Y: return 2 * x ``` But what about types that
-implement `__add__` but not `__radd__`? In this case, we could return `x * 2`
-as fallback. Because the `optype.Can*` protocols are runtime-checkable, the
-revised `twice2` function can be compactly written as: ```python def twice2[Y]
-(x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y: return 2 * x if
-isinstance(x, optype.CanRMul) else x * 2 ``` See [`examples/twice.py`]
-(examples/twice.py) for the full example. ## Overview The API of `optype` is
-flat; a single `import optype` is all you need. There are four flavors of
-things that live within `optype`, - `optype.Can{}` types describe *what can be
-done* with it. For instance, any `CanAbs[T]` type can be used as argument to
-the `abs()` builtin function with return type `T`. Most `Can{}` implement a
-single special method, whose name directly matched that of the type. `CanAbs`
-implements `__abs__`, `CanAdd` implements `__add__`, etc. - `optype.Has{}` is
-the analogue of `Can{}`, but for special *attributes*. `HasName` has the
-`__name__: str` attribute, `HasDict` has a `__dict__`, etc. - `optype.Does{}`
-describe the *type of operators*. So `DoesAbs` is the type of the `abs({})`
-builtin function, and `DoesPos` the type of the `+{}` prefix operator. -
-`optype.do_{}` are the correctly-typed implementations of `Does{}`. For each
-`do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is the typed
-alias of `abs({})`, and `do_pos: DoesPos` is a typed version of `operator.pos`.
-The `optype.do_` operators are more complete than `operators`, has runtime-
-accessible type annotations, and uses a fully predictable naming scheme. ##
-Reference All [typing protocols][PC] here live in the root `optype` namespace.
-They are [runtime-checkable][RC] so that you can do e.g. `isinstance('snail',
-optype.CanAdd)`, in case you want to check whether `snail` implements
+PPyytthhoonn 33..1111                             PPyytthhoonn 33..1122
+```python from typing import Literal,   ```python from typing import Literal
+TypeAlias, TypeVar from optype import   from optype import CanRMul type Two =
+CanRMul Y = TypeVar('Y') Two: TypeAlias Literal[2] def twice[Y](x: CanRMul[Two,
+= Literal[2] def twice(x: CanRMul[Two,  Y]) -> Y: return 2 * x ```
+Y]) -> Y: return 2 * x ```
+But what about types that implement `__add__` but not `__radd__`? In this case,
+we could return `x * 2` as fallback (assuming commutativity). Because the
+`optype.Can*` protocols are runtime-checkable, the revised `twice2` function
+can be compactly written as:
+PPyytthhoonn 33..1111                             PPyytthhoonn 33..1122
+```python from optype import CanMul def ```python from optype import CanMul def
+twice2(x: CanRMul[Two, Y] | CanMul[Two, twice2[Y](x: CanRMul[Two, Y] | CanMul
+Y]) -> Y: return 2 * x if isinstance(x, [Two, Y]) -> Y: return 2 * x if
+CanRMul) else x * 2 ```                 isinstance(x, CanRMul) else x * 2 ```
+See [`examples/twice.py`](examples/twice.py) for the full example. ## Overview
+The API of `optype` is flat; a single `import optype` is all you need. There
+are four flavors of things that live within `optype`, - `optype.Can{}` types
+describe *what can be done* with it. For instance, any `CanAbs[T]` type can be
+used as argument to the `abs()` builtin function with return type `T`. Most
+`Can{}` implement a single special method, whose name directly matched that of
+the type. `CanAbs` implements `__abs__`, `CanAdd` implements `__add__`, etc. -
+`optype.Has{}` is the analogue of `Can{}`, but for special *attributes*.
+`HasName` has the `__name__: str` attribute, `HasDict` has a `__dict__`, etc. -
+`optype.Does{}` describe the *type of operators*. So `DoesAbs` is the type of
+the `abs({})` builtin function, and `DoesPos` the type of the `+{}` prefix
+operator. - `optype.do_{}` are the correctly-typed implementations of `Does{}`.
+For each `do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is
+the typed alias of `abs({})`, and `do_pos: DoesPos` is a typed version of
+`operator.pos`. The `optype.do_` operators are more complete than `operators`,
+has runtime-accessible type annotations, and uses a fully predictable naming
+scheme. ## Reference All [typing protocols][PC] here live in the root `optype`
+namespace. They are [runtime-checkable][RC] so that you can do e.g. `isinstance
+('snail', optype.CanAdd)`, in case you want to check whether `snail` implements
 `__add__`. > [!NOTE] > It is bad practice to use a [`typing.Protocol`][PC] as
 base class for your > implementation. Because of [`@typing.runtime_checkable`]
 [RC], you can use > `isinstance` either way. Unlike`collections.abc`,
 `optype`'s protocols aren't abstract base classes, i.e. they don't extend
 `abc.ABC`, only `typing.Protocol`. This allows the `optype` protocols to be
 used as building blocks for `.pyi` type stubs. [PC]: https://
 typing.readthedocs.io/en/latest/spec/protocol.html [RC]: https://
@@ -322,13 +330,12 @@
 __getnewargs_ex__ () -> tuple[tuple[*Args], dict
 __new__           [str, Kw]]                       CanGetnewargsEx[*Args, Kw]
                   (*Args, **dict[str, Kw]) -> Self
 ### `dataclasses` For the [`dataclasses`][DC] standard library, `optype`
 provides the `optype.HasDataclassFields` interface It can conveniently be used
 to check whether a type or instance is a dataclass, i.e. `isinstance(obj,
 optype.HasDataclassFields)`. [DC]: https://docs.python.org/3/library/
-dataclasses.html ## Future plans - Support for Python versions before 3.12
-(#19). - [numpy][NP] interfaces for arrays-like types (no deps) (#24) - [array-
-api][API-ND] interfaces (no deps) (#25) - [dataframe-api][API-DF] interfaces
-(no deps) (#26) [NP]: https://github.com/numpy/numpy [API-ND]: https://data-
-apis.org/array-api/latest/ [API-DF]: https://data-apis.org/dataframe-api/draft/
-index.html
+dataclasses.html ## Future plans - [numpy][NP] interfaces for arrays-like types
+(no deps) (#24) - [array-api][API-ND] interfaces (no deps) (#25) - [dataframe-
+api][API-DF] interfaces (no deps) (#26) [NP]: https://github.com/numpy/numpy
+[API-ND]: https://data-apis.org/array-api/latest/ [API-DF]: https://data-
+apis.org/dataframe-api/draft/index.html
```

### Comparing `optype-0.3.1/optype/__init__.py` & `optype-0.4.0/optype/__init__.py`

 * *Files identical despite different names*

### Comparing `optype-0.3.1/optype/_do.py` & `optype-0.4.0/optype/_do.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import math as _math
 import operator as _o
-from typing import TYPE_CHECKING
+import sys as _sys
+from typing import TYPE_CHECKING, ParamSpec, TypeVar
 
 import optype._can as _c
 import optype._does as _d
 
 
+_K = TypeVar('_K')
+_V = TypeVar('_V')
+_D = TypeVar('_D')
+_X = TypeVar('_X')
+_Y = TypeVar('_Y')
+_Xss = ParamSpec('_Xss')
+
+
 # type conversion
 do_bool: _d.DoesBool = bool
 do_int: _d.DoesInt = int
 do_float: _d.DoesFloat = float
 do_complex: _d.DoesComplex = complex
 do_bytes: _d.DoesBytes = bytes
 do_str: _d.DoesStr = str
@@ -45,52 +54,61 @@
 do_setattr: _d.DoesSetattr = setattr
 do_delattr: _d.DoesDelattr = delattr
 do_dir: _d.DoesDir = dir
 
 
 # callables
 
-do_call: _d.DoesCall = _o.call
+if _sys.version_info < (3, 11):
+    def do_call(
+        f: _c.CanCall[_Xss, _Y],
+        /,
+        *args: _Xss.args,
+        **kwargs: _Xss.kwargs,
+    ) -> _Y:
+        return f(*args, **kwargs)
+else:
+    do_call: _d.DoesCall = _o.call
 
 
 # containers and sequences
 
 do_len: _d.DoesLen = len
 do_length_hint: _d.DoesLengthHint = _o.length_hint
 
 
 # `operator.getitem` isn't used, because it has an (unreasonably loose, and
 # redundant) overload for `(Sequence[T], slice) -> Sequence[T]`
 # https://github.com/python/typeshed/blob/main/stdlib/_operator.pyi#L84-L86
-def do_getitem[K, V, M](
-    obj:  _c.CanGetitem[K, V] | _c.CanGetMissing[K, V, M],
-    key: K,
+def do_getitem(
+    obj:  _c.CanGetitem[_K, _V] | _c.CanGetMissing[_K, _V, _D],
+    key: _K,
     /,
-) -> V | M:
+) -> _V | _D:
     """Same as `value = obj[key]`."""
     return obj[key]
 
 
-def do_setitem[K, V](obj: _c.CanSetitem[K, V], key: K, value: V, /) -> None:
+def do_setitem(obj: _c.CanSetitem[_K, _V], key: _K, value: _V, /) -> None:
     """Same as `obj[key] = value`."""
     obj[key] = value
 
 
-def do_delitem[K](obj: _c.CanDelitem[K], key: K, /) -> None:
+def do_delitem(obj: _c.CanDelitem[_K], key: _K, /) -> None:
     """Same as `del obj[key]`."""
     del obj[key]
 
 
-def do_missing[K, V](obj: _c.CanMissing[K, V], key: K, /) -> V:
+def do_missing(obj: _c.CanMissing[_K, _V], key: _K, /) -> _V:
     return obj.__missing__(key)
 
 
 # `operator.contains` cannot be used, as it incorrectly requires `key`
 # to be an **invariant** `object` instance...
-def do_contains[K](obj: _c.CanContains[K], key: K, /) -> bool:
+def do_contains(obj: _c.CanContains[_K], key: _K, /) -> bool:
     """Same as `key in obj`."""
     return key in obj
 
 
 # `builtins.reversed` is annotated incorrectly within typeshed:
 # https://github.com/python/typeshed/issues/11645
 do_reversed: _d.DoesReversed = reversed  # pyright: ignore[reportAssignmentType]
@@ -113,80 +131,81 @@
 do_or: _d.DoesOr = _o.or_
 
 
 # reflected ops
 # (a DRY `do_r*` decorator won't work; the overloads get lost during casting to
 # `CanCall` or `Callable`, within the decorator function signature).
 
-def do_radd[X, Y](a: _c.CanRAdd[X, Y], b: X) -> Y:
+
+def do_radd(a: _c.CanRAdd[_X, _Y], b: _X) -> _Y:
     """Same as `b + a`."""
     return b + a
 
 
-def do_rsub[X, Y](a: _c.CanRSub[X, Y], b: X) -> Y:
+def do_rsub(a: _c.CanRSub[_X, _Y], b: _X) -> _Y:
     """Same as `b - a`."""
     return b - a
 
 
-def do_rmul[X, Y](a: _c.CanRMul[X, Y], b: X) -> Y:
+def do_rmul(a: _c.CanRMul[_X, _Y], b: _X) -> _Y:
     """Same as `b * a`."""
     return b * a
 
 
-def do_rmatmul[X, Y](a: _c.CanRMatmul[X, Y], b: X) -> Y:
+def do_rmatmul(a: _c.CanRMatmul[_X, _Y], b: _X) -> _Y:
     """Same as `b @ a`."""
     return b @ a
 
 
-def do_rtruediv[X, Y](a: _c.CanRTruediv[X, Y], b: X) -> Y:
+def do_rtruediv(a: _c.CanRTruediv[_X, _Y], b: _X) -> _Y:
     """Same as `b / a`."""
     return b / a
 
 
-def do_rfloordiv[X, Y](a: _c.CanRFloordiv[X, Y], b: X) -> Y:
+def do_rfloordiv(a: _c.CanRFloordiv[_X, _Y], b: _X) -> _Y:
     """Same as `b // a`."""
     return b // a
 
 
-def do_rmod[X, Y](a: _c.CanRMod[X, Y], b: X) -> Y:
+def do_rmod(a: _c.CanRMod[_X, _Y], b: _X) -> _Y:
     """Same as `b % a`."""
     return b % a
 
 
-def do_rdivmod[X, Y](a: _c.CanRDivmod[X, Y], b: X) -> Y:
+def do_rdivmod(a: _c.CanRDivmod[_X, _Y], b: _X) -> _Y:
     """Same as `divmod(b, a)`."""
     return divmod(b, a)
 
 
-def do_rpow[X, Y](a: _c.CanRPow[X, Y], b: X) -> Y:
+def do_rpow(a: _c.CanRPow[_X, _Y], b: _X) -> _Y:
     """Same as `b ** a`."""
     return b ** a
 
 
-def do_rlshift[X, Y](a: _c.CanRLshift[X, Y], b: X) -> Y:
+def do_rlshift(a: _c.CanRLshift[_X, _Y], b: _X) -> _Y:
     """Same as `b << a`."""
     return b << a
 
 
-def do_rrshift[X, Y](a: _c.CanRRshift[X, Y], b: X) -> Y:
+def do_rrshift(a: _c.CanRRshift[_X, _Y], b: _X) -> _Y:
     """Same as `b >> a`."""
     return b >> a
 
 
-def do_rand[X, Y](a: _c.CanRAnd[X, Y], b: X) -> Y:
+def do_rand(a: _c.CanRAnd[_X, _Y], b: _X) -> _Y:
     """Same as `b & a`."""
     return b & a
 
 
-def do_rxor[X, Y](a: _c.CanRXor[X, Y], b: X) -> Y:
+def do_rxor(a: _c.CanRXor[_X, _Y], b: _X) -> _Y:
     """Same as `b ^ a`."""
     return b ^ a
 
 
-def do_ror[X, Y](a: _c.CanROr[X, Y], b: X) -> Y:
+def do_ror(a: _c.CanROr[_X, _Y], b: _X) -> _Y:
     """Same as `b | a`."""
     return b | a
 
 
 # augmented ops
 do_iadd: _d.DoesIAdd = _o.iadd
 do_isub: _d.DoesISub = _o.isub
```

### Comparing `optype-0.3.1/pyproject.toml` & `optype-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "optype"
-version = "0.3.1"
-description = "Building blocks for precise type hints in Python 3.12+"
+version = "0.4.0"
+description = "Building blocks for precise & flexible type hints"
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Operating System :: OS Independent",
+    "Typing :: Typed",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
+]
+repository = "https://github.com/jorenham/optype/"
+documentation = "https://github.com/jorenham/optype?tab=readme-ov-file#optype"
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/jorenham/optype/issues"
+"Changelog" = "https://github.com/jorenham/optype/releases"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
+typing-extensions = {version = ">=4.5", python = "<3.12"}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = '^3.7.0'
 
 [tool.poetry.group.lint.dependencies]
+basedpyright = "^1.10.1"
 codespell = "^2.2.6"
-basedpyright = "^1.8.0"
-ruff = "^0.3.5"
+ruff = "^0.3.7"
+typing-extensions = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
+typing-extensions = "*"
 
 [tool.poetry.group.test-github]
 optional = true
 [tool.poetry.group.test-github.dependencies]
 pytest-github-actions-annotate-failures = ">=0.2.0,<1.0"
 
 
@@ -51,20 +68,21 @@
     ".venv",
     ".vscode",
     "dist"
 ]
 stubPath = "."
 venvPath = "."
 venv = ".venv"
-pythonVersion = "3.12"
+pythonVersion = "3.10"
 pythonPlatform = "All"
 typeCheckingMode = "all"
-useLibraryCodeForTypes = false
 reportAny = false
 reportUnusedCallResult = false
+# because of `sys.version_info()` conditionals
+reportUnreachable = false
 
 
 [tool.pytest.ini_options]
 minversion = "8.0"
 testpaths = ["optype", "examples", "tests"]
 addopts = [
     "-ra",
@@ -76,16 +94,16 @@
     "ELLIPSIS",
 ]
 filterwarnings = ["error"]
 xfail_strict = true
 
 
 [tool.ruff]
-src = ["optype", "tests"]
-target-version = "py312"
+src = ["optype", "examples", "tests"]
+target-version = "py310"
 line-length = 79
 indent-width = 4
 show-fixes = true
 force-exclude = true
 extend-exclude = [".github", ".vscode"]
 
 [tool.ruff.lint]
@@ -146,58 +164,55 @@
     "LOG",      # flake8-logging
     "RUF",      # ruff
 ]
 extend-ignore = [
     # flake8-annotations
     "ANN001",   # missing-type-function-argument (deprecated)
     "ANN002",   # missing-type-args (deprecated)
-    "ANN401",   # any-type (unreasonable)
+    "ANN401",   # any-type
 
     # flake8-pyi
-    "PYI036",   # bad-exit-annotation (unreasonable)
+    "PYI036",   # bad-exit-annotation
 
     # refurb
-    "FURB118",  # reimplemented-operator (unreasonable)
+    "FURB118",  # reimplemented-operator
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "examples/*" = [
     # isort
     "I001",     # unsorted-imports
-
     # flake8-no-pep420
     "INP001",   # implicit-namespace-package
-
     # pylint
     "PLR2004",  # magic-value-comparison
 ]
 "tests/*" = [
     # flake8-annotations
     "ANN201",   # missing-return-type
-
     # flake8-self
     "SLF001",   # private-member-access
 ]
 
 [tool.ruff.lint.isort]
 case-sensitive = true
 combine-as-imports = true
 known-first-party = ["optype"]
-lines-between-types = 0
 lines-after-imports = 2
+lines-between-types = 0
 
 [tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
 [tool.ruff.lint.flake8-type-checking]
 strict = true
 
 [tool.ruff.lint.pylint]
 allow-dunder-method-names = [
-    "__replace__",  # used by `copy.replace` in Python 3.13+
+    "__replace__"   # used by `copy.replace` in Python 3.13+
 ]
 
 [tool.ruff.format]
 # keep in sync with .editorconfig
 line-ending = "lf"
 indent-style = "space"
 quote-style = "single"
```

### Comparing `optype-0.3.1/PKG-INFO` & `optype-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: optype
-Version: 0.3.1
-Summary: Building blocks for precise type hints in Python 3.12+
+Version: 0.4.0
+Summary: Building blocks for precise & flexible type hints
+Home-page: https://github.com/jorenham/optype/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Typing :: Typed
+Requires-Dist: typing-extensions (>=4.5) ; python_version < "3.12"
+Project-URL: Bug Tracker, https://github.com/jorenham/optype/issues
+Project-URL: Changelog, https://github.com/jorenham/optype/releases
+Project-URL: Documentation, https://github.com/jorenham/optype?tab=readme-ov-file#optype
+Project-URL: Repository, https://github.com/jorenham/optype/
 Description-Content-Type: text/markdown
 
 <h1 align="center">optype</h1>
 
 <p align="center">
     <i>One protocol, one method.</i>
 </p>
@@ -20,46 +32,46 @@
 <p align="center">
     Building blocks for precise & flexible type hints.
 </p>
 
 <p align="center">
     <a href="https://github.com/jorenham/optype/actions?query=workflow%3ACI">
         <img
-            alt="Continuous Integration"
+            alt="optype - CI"
             src="https://github.com/jorenham/optype/workflows/CI/badge.svg"
         />
     </a>
     <a href="https://pypi.org/project/optype/">
         <img
-            alt="PyPI"
+            alt="optype - PyPI"
             src="https://img.shields.io/pypi/v/optype?style=flat"
         />
     </a>
     <a href="https://github.com/jorenham/optype">
         <img
-            alt="Python Versions"
+            alt="optype - Python Versions"
             src="https://img.shields.io/pypi/pyversions/optype?style=flat"
         />
     </a>
     <a href="https://github.com/jorenham/optype">
         <img
-            alt="License"
+            alt="optype - license"
             src="https://img.shields.io/github/license/jorenham/optype?style=flat"
         />
     </a>
-    <a href="https://github.com/astral-sh/ruff">
+    <a href="https://detachhead.github.io/basedpyright">
         <img
-            alt="Ruff"
-            src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json"
+            alt="optype - basedpyright"
+            src="https://img.shields.io/badge/basedpyright-checked-42b983"
         />
     </a>
-    <a href="https://github.com/microsoft/pyright">
+    <a href="https://github.com/astral-sh/ruff">
         <img
-            alt="Checked with pyright"
-            src="https://microsoft.github.io/pyright/img/pyright_badge.svg"
+            alt="optype - ruff"
+            src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json"
         />
     </a>
 </p>
 
 ---
 
 ## Installation
@@ -87,34 +99,85 @@
 
 This is where `optype` comes in handy, which has single-method protocols for
 *all* the builtin special methods.
 For `twice`, we can use `optype.CanRMul[X, Y]`, which, as the name suggests,
 is a protocol with (only) the `def __rmul__(self, x: X) -> Y: ...` method.
 With this, the `twice` function can written as:
 
+<table>
+<tr>
+<th>Python 3.11</th>
+<th>Python 3.12</th>
+</tr>
+<tr>
+<td>
+
+```python
+from typing import Literal, TypeAlias, TypeVar
+from optype import CanRMul
+
+Y = TypeVar('Y')
+Two: TypeAlias = Literal[2]
+
+def twice(x: CanRMul[Two, Y]) -> Y:
+    return 2 * x
+```
+
+</td>
+<td>
+
 ```python
-import typing
-import optype
+from typing import Literal
+from optype import CanRMul
 
-type Two = typing.Literal[2]
 
-def twice[Y](x: optype.CanRMul[Two, Y], /) -> Y:
+type Two = Literal[2]
+
+def twice[Y](x: CanRMul[Two, Y]) -> Y:
     return 2 * x
 ```
 
+</td>
+</tr>
+</table>
+
 But what about types that implement `__add__` but not `__radd__`?
-In this case, we could return `x * 2` as fallback.
+In this case, we could return `x * 2` as fallback (assuming commutativity).
 Because the `optype.Can*` protocols are runtime-checkable, the revised
 `twice2` function can be compactly written as:
 
+<table>
+<tr>
+<th>Python 3.11</th>
+<th>Python 3.12</th>
+</tr>
+<tr>
+<td>
+
 ```python
-def twice2[Y](x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y:
-    return 2 * x if isinstance(x, optype.CanRMul) else x * 2
+from optype import CanMul
+
+def twice2(x: CanRMul[Two, Y] | CanMul[Two, Y]) -> Y:
+    return 2 * x if isinstance(x, CanRMul) else x * 2
 ```
 
+</td>
+<td>
+
+```python
+from optype import CanMul
+
+def twice2[Y](x: CanRMul[Two, Y] | CanMul[Two, Y]) -> Y:
+    return 2 * x if isinstance(x, CanRMul) else x * 2
+```
+
+</td>
+</tr>
+</table>
+
 See [`examples/twice.py`](examples/twice.py) for the full example.
 
 ## Overview
 
 The API of `optype` is flat; a single `import optype` is all you need.
 There are four flavors of things that live within `optype`,
 
@@ -1405,15 +1468,14 @@
 It can conveniently be used to check whether a type or instance is a
 dataclass, i.e. `isinstance(obj, optype.HasDataclassFields)`.
 
 [DC]: https://docs.python.org/3/library/dataclasses.html
 
 ## Future plans
 
-- Support for Python versions before 3.12 (#19).
 - [numpy][NP] interfaces for arrays-like types (no deps) (#24)
 - [array-api][API-ND] interfaces (no deps) (#25)
 - [dataframe-api][API-DF] interfaces (no deps) (#26)
 
 [NP]: https://github.com/numpy/numpy
 [API-ND]: https://data-apis.org/array-api/latest/
 [API-DF]: https://data-apis.org/dataframe-api/draft/index.html
```

#### html2text {}

```diff
@@ -1,57 +1,74 @@
-Metadata-Version: 2.1 Name: optype Version: 0.3.1 Summary: Building blocks for
-precise type hints in Python 3.12+ License: BSD-3-Clause Author: Joren
-Hammudoglu Author-email: jhammudoglu@gmail.com Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
+Metadata-Version: 2.1 Name: optype Version: 0.4.0 Summary: Building blocks for
+precise & flexible type hints Home-page: https://github.com/jorenham/optype/
+License: BSD-3-Clause Author: Joren Hammudoglu Author-email:
+jhammudoglu@gmail.com Requires-Python: >=3.10,<4.0 Classifier: Development
+Status :: 4 - Beta Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: 3.13 Classifier:
+Typing :: Typed Requires-Dist: typing-extensions (>=4.5) ; python_version <
+"3.12" Project-URL: Bug Tracker, https://github.com/jorenham/optype/issues
+Project-URL: Changelog, https://github.com/jorenham/optype/releases Project-
+URL: Documentation, https://github.com/jorenham/optype?tab=readme-ov-
+file#optype Project-URL: Repository, https://github.com/jorenham/optype/
 Description-Content-Type: text/markdown
                              ************ ooppttyyppee ************
                            One protocol, one method.
               Building blocks for precise & flexible type hints.
-  _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_C_h_e_c_k_e_d_ _w_i_t_h
-                                   _p_y_r_i_g_h_t_]
+_[_o_p_t_y_p_e_ _-_ _C_I_]_[_o_p_t_y_p_e_ _-_ _P_y_P_I_]_[_o_p_t_y_p_e_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_o_p_t_y_p_e_ _-_ _l_i_c_e_n_s_e_]_[_o_p_t_y_p_e
+                        _-_ _b_a_s_e_d_p_y_r_i_g_h_t_]_[_o_p_t_y_p_e_ _-_ _r_u_f_f_]
 --- ## Installation Optype is available as [`optype`][OPTYPE] on PyPI: ```shell
 pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Example
 Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
 Implementing it is trivial, but what about the type annotations? Because `twice
 (2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it might seem like a
 good idea to type it as `twice[T](x: T) -> T: ...`. However, that wouldn't
 include cases such as `twice(True) == 2` or `twice((42, True)) == (42, True,
 42, True)`, where the input- and output types differ. Moreover, `twice` should
 accept *any* type with a custom `__rmul__` method that accepts `2` as argument.
 This is where `optype` comes in handy, which has single-method protocols for
 *all* the builtin special methods. For `twice`, we can use `optype.CanRMul[X,
 Y]`, which, as the name suggests, is a protocol with (only) the `def __rmul__
 (self, x: X) -> Y: ...` method. With this, the `twice` function can written as:
-```python import typing import optype type Two = typing.Literal[2] def twice[Y]
-(x: optype.CanRMul[Two, Y], /) -> Y: return 2 * x ``` But what about types that
-implement `__add__` but not `__radd__`? In this case, we could return `x * 2`
-as fallback. Because the `optype.Can*` protocols are runtime-checkable, the
-revised `twice2` function can be compactly written as: ```python def twice2[Y]
-(x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y: return 2 * x if
-isinstance(x, optype.CanRMul) else x * 2 ``` See [`examples/twice.py`]
-(examples/twice.py) for the full example. ## Overview The API of `optype` is
-flat; a single `import optype` is all you need. There are four flavors of
-things that live within `optype`, - `optype.Can{}` types describe *what can be
-done* with it. For instance, any `CanAbs[T]` type can be used as argument to
-the `abs()` builtin function with return type `T`. Most `Can{}` implement a
-single special method, whose name directly matched that of the type. `CanAbs`
-implements `__abs__`, `CanAdd` implements `__add__`, etc. - `optype.Has{}` is
-the analogue of `Can{}`, but for special *attributes*. `HasName` has the
-`__name__: str` attribute, `HasDict` has a `__dict__`, etc. - `optype.Does{}`
-describe the *type of operators*. So `DoesAbs` is the type of the `abs({})`
-builtin function, and `DoesPos` the type of the `+{}` prefix operator. -
-`optype.do_{}` are the correctly-typed implementations of `Does{}`. For each
-`do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is the typed
-alias of `abs({})`, and `do_pos: DoesPos` is a typed version of `operator.pos`.
-The `optype.do_` operators are more complete than `operators`, has runtime-
-accessible type annotations, and uses a fully predictable naming scheme. ##
-Reference All [typing protocols][PC] here live in the root `optype` namespace.
-They are [runtime-checkable][RC] so that you can do e.g. `isinstance('snail',
-optype.CanAdd)`, in case you want to check whether `snail` implements
+PPyytthhoonn 33..1111                             PPyytthhoonn 33..1122
+```python from typing import Literal,   ```python from typing import Literal
+TypeAlias, TypeVar from optype import   from optype import CanRMul type Two =
+CanRMul Y = TypeVar('Y') Two: TypeAlias Literal[2] def twice[Y](x: CanRMul[Two,
+= Literal[2] def twice(x: CanRMul[Two,  Y]) -> Y: return 2 * x ```
+Y]) -> Y: return 2 * x ```
+But what about types that implement `__add__` but not `__radd__`? In this case,
+we could return `x * 2` as fallback (assuming commutativity). Because the
+`optype.Can*` protocols are runtime-checkable, the revised `twice2` function
+can be compactly written as:
+PPyytthhoonn 33..1111                             PPyytthhoonn 33..1122
+```python from optype import CanMul def ```python from optype import CanMul def
+twice2(x: CanRMul[Two, Y] | CanMul[Two, twice2[Y](x: CanRMul[Two, Y] | CanMul
+Y]) -> Y: return 2 * x if isinstance(x, [Two, Y]) -> Y: return 2 * x if
+CanRMul) else x * 2 ```                 isinstance(x, CanRMul) else x * 2 ```
+See [`examples/twice.py`](examples/twice.py) for the full example. ## Overview
+The API of `optype` is flat; a single `import optype` is all you need. There
+are four flavors of things that live within `optype`, - `optype.Can{}` types
+describe *what can be done* with it. For instance, any `CanAbs[T]` type can be
+used as argument to the `abs()` builtin function with return type `T`. Most
+`Can{}` implement a single special method, whose name directly matched that of
+the type. `CanAbs` implements `__abs__`, `CanAdd` implements `__add__`, etc. -
+`optype.Has{}` is the analogue of `Can{}`, but for special *attributes*.
+`HasName` has the `__name__: str` attribute, `HasDict` has a `__dict__`, etc. -
+`optype.Does{}` describe the *type of operators*. So `DoesAbs` is the type of
+the `abs({})` builtin function, and `DoesPos` the type of the `+{}` prefix
+operator. - `optype.do_{}` are the correctly-typed implementations of `Does{}`.
+For each `do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is
+the typed alias of `abs({})`, and `do_pos: DoesPos` is a typed version of
+`operator.pos`. The `optype.do_` operators are more complete than `operators`,
+has runtime-accessible type annotations, and uses a fully predictable naming
+scheme. ## Reference All [typing protocols][PC] here live in the root `optype`
+namespace. They are [runtime-checkable][RC] so that you can do e.g. `isinstance
+('snail', optype.CanAdd)`, in case you want to check whether `snail` implements
 `__add__`. > [!NOTE] > It is bad practice to use a [`typing.Protocol`][PC] as
 base class for your > implementation. Because of [`@typing.runtime_checkable`]
 [RC], you can use > `isinstance` either way. Unlike`collections.abc`,
 `optype`'s protocols aren't abstract base classes, i.e. they don't extend
 `abc.ABC`, only `typing.Protocol`. This allows the `optype` protocols to be
 used as building blocks for `.pyi` type stubs. [PC]: https://
 typing.readthedocs.io/en/latest/spec/protocol.html [RC]: https://
@@ -328,13 +345,12 @@
 __getnewargs_ex__ () -> tuple[tuple[*Args], dict
 __new__           [str, Kw]]                       CanGetnewargsEx[*Args, Kw]
                   (*Args, **dict[str, Kw]) -> Self
 ### `dataclasses` For the [`dataclasses`][DC] standard library, `optype`
 provides the `optype.HasDataclassFields` interface It can conveniently be used
 to check whether a type or instance is a dataclass, i.e. `isinstance(obj,
 optype.HasDataclassFields)`. [DC]: https://docs.python.org/3/library/
-dataclasses.html ## Future plans - Support for Python versions before 3.12
-(#19). - [numpy][NP] interfaces for arrays-like types (no deps) (#24) - [array-
-api][API-ND] interfaces (no deps) (#25) - [dataframe-api][API-DF] interfaces
-(no deps) (#26) [NP]: https://github.com/numpy/numpy [API-ND]: https://data-
-apis.org/array-api/latest/ [API-DF]: https://data-apis.org/dataframe-api/draft/
-index.html
+dataclasses.html ## Future plans - [numpy][NP] interfaces for arrays-like types
+(no deps) (#24) - [array-api][API-ND] interfaces (no deps) (#25) - [dataframe-
+api][API-DF] interfaces (no deps) (#26) [NP]: https://github.com/numpy/numpy
+[API-ND]: https://data-apis.org/array-api/latest/ [API-DF]: https://data-
+apis.org/dataframe-api/draft/index.html
```

