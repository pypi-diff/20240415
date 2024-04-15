# Comparing `tmp/privates_py-0.1.0.tar.gz` & `tmp/privates_py-0.2.0.tar.gz`

## Comparing `privates_py-0.1.0.tar` & `privates_py-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privates_py-0.1.0/src/privates/__about__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 privates_py-0.1.0/src/privates/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 privates_py-0.1.0/src/privates/_util.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 privates_py-0.1.0/src/privates/exceptions.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 privates_py-0.1.0/src/privates/modifiers.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privates_py-0.1.0/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 privates_py-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 privates_py-0.1.0/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 privates_py-0.1.0/hatch.toml
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 privates_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 privates_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privates_py-0.2.0/src/privates/__about__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 privates_py-0.2.0/src/privates/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 privates_py-0.2.0/src/privates/_util.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 privates_py-0.2.0/src/privates/exceptions.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 privates_py-0.2.0/src/privates/modifiers.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privates_py-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 privates_py-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 privates_py-0.2.0/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 privates_py-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 privates_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 privates_py-0.2.0/PKG-INFO
```

### Comparing `privates_py-0.1.0/src/privates/_util.py` & `privates_py-0.2.0/src/privates/_util.py`

 * *Files identical despite different names*

### Comparing `privates_py-0.1.0/src/privates/modifiers.py` & `privates_py-0.2.0/src/privates/modifiers.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,29 +42,35 @@
 
     return False
 
 
 def _ensure_access(
     protected: Iterable[str],
     privates: Iterable[str],
+    readonly: Iterable[str],
     subclasses: set[type],
     friends: set[type | FunctionType],
     tp: type,
     name: str,
 ) -> None:
-    if name in protected:
+    if (name in protected) or (name in readonly):
         frame = get_back_frame()
         co_name = frame.f_code.co_name
 
         for subclass in subclasses:
             if _check_access(co_name, subclass, frame):
                 return
 
+        for friend in friends:
+            if _check_access(co_name, friend, frame):
+                return
+
+        msg = "protected" if name in protected else "read-only"
         raise AccessError(
-            f"attempted to access protected attribute {name!r} outside of subclass to {tp.__name__}"  # noqa
+            f"attempted to access {msg} attribute {name!r} outside of subclass to {tp.__name__}"  # noqa
         )
 
     if (name.startswith("_") and (not name.endswith("__"))) or (
         name in privates
     ):
         frame = get_back_frame()
         co_name = frame.f_code.co_name
@@ -89,39 +95,69 @@
     """
     old_getattribute = tp.__getattribute__
     old_setattribute = tp.__setattr__
     old_delattribute = tp.__delattr__
     tp.__friends__ = set()  # type: ignore
     privates: Iterable[str] = getattr(tp, "__private__", set())
     protected: Iterable[str] = getattr(tp, "__protected__", set())
+    readonly: Iterable[str] = getattr(tp, "__readonly__", set())
     old_init_subclass = tp.__init_subclass__
     subclasses: set[type] = {tp}
     friends: set[type | FunctionType] = tp.__friends__  # type: ignore
 
     def subclass_wrapper(cls, *args, **kwargs) -> None:
         subclasses.add(cls)
         old_init_subclass(*args, **kwargs)  # type: ignore
 
     tp.__init_subclass__ = classmethod(subclass_wrapper)  # type: ignore
 
     def get_wrapper(self, name: str) -> Any:
-        _ensure_access(protected, privates, subclasses, friends, tp, name)
+        if name in readonly:
+            # public get access for readonly attributes
+            return old_getattribute(self, name)  # type: ignore
+
+        _ensure_access(
+            protected,
+            privates,
+            set(),
+            subclasses,
+            friends,
+            tp,
+            name,
+        )
         return old_getattribute(self, name)  # type: ignore
 
     def set_wrapper(self, name: str, value: Any) -> Any:
-        _ensure_access(protected, privates, subclasses, friends, tp, name)
+        _ensure_access(
+            protected,
+            privates,
+            readonly,
+            subclasses,
+            friends,
+            tp,
+            name,
+        )
         return old_setattribute(self, name, value)  # type: ignore
 
     def del_wrapper(self, name: str) -> None:
-        _ensure_access(protected, privates, subclasses, friends, tp, name)
+        _ensure_access(
+            protected,
+            privates,
+            readonly,
+            subclasses,
+            friends,
+            tp,
+            name,
+        )
         return old_delattribute(self, name)  # type: ignore
 
     tp.__getattribute__ = get_wrapper  # type: ignore
     tp.__setattr__ = set_wrapper  # type: ignore
     tp.__delattr__ = del_wrapper  # type: ignore
+
     return tp
 
 
 def class_modifier(
     target: type[T],
 ) -> type[T]:
     """Modify the access rules for a class.
@@ -139,23 +175,42 @@
     frame = get_back_frame()
 
     if not isinstance(target, type):
         raise TypeError(
             "class_modifier() can only be applied to classes. use function_modifier() instead"  # noqa
         )
     supports_private(target)
+    friends: set[type | FunctionType] = target.__friends__  # type: ignore
 
     init = target.__init__
 
     def inner(*args: Any, **kwargs: Any) -> None:
         caller_frame = get_back_frame()
         if caller_frame.f_locals != frame.f_locals:
-            raise AccessError(
-                f"attempted to access {target} outside of it's module"
-            )
+            ok: bool = False
+
+            for friend in friends:
+                if isinstance(friend, type):
+                    for attr_name in dir(friend):
+                        func = getattr(friend, attr_name)
+
+                        if not isinstance(func, FunctionType):
+                            continue
+
+                        if func.__code__ == caller_frame.f_code:
+                            ok = True
+                            break
+                elif friend.__code__ == caller_frame.f_code:
+                    ok = True
+                    break
+
+            if not ok:
+                raise AccessError(
+                    f"attempted to access {target} outside of it's scope"
+                )
 
         init(*args, **kwargs)
 
     target.__init__ = inner  # type: ignore
     return target
```

### Comparing `privates_py-0.1.0/LICENSE.txt` & `privates_py-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `privates_py-0.1.0/hatch.toml` & `privates_py-0.2.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `privates_py-0.1.0/pyproject.toml` & `privates_py-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "privates.py"
 dynamic = ["version"]
 description = 'Stop others from touching your privates.'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "ZeroIntensity", email = "zintensitydev@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["typing_extensions"]
 
 [project.urls]
 Documentation = "https://privates.zintensity.dev"
```

