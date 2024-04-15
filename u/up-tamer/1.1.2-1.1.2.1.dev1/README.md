# Comparing `tmp/up_tamer-1.1.2.tar.gz` & `tmp/up_tamer-1.1.2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_tamer-1.1.2.tar", last modified: Fri Feb 23 16:58:20 2024, max compression
+gzip compressed data, was "up_tamer-1.1.2.1.dev1.tar", last modified: Mon Apr 15 08:13:22 2024, max compression
```

## Comparing `up_tamer-1.1.2.tar` & `up_tamer-1.1.2.1.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:58:20.599544 up_tamer-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 16:58:18.000000 up_tamer-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-23 16:58:20.599544 up_tamer-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-02-23 16:58:18.000000 up_tamer-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 16:58:20.599544 up_tamer-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-23 16:58:18.000000 up_tamer-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:58:20.599544 up_tamer-1.1.2/up_tamer/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-23 16:58:18.000000 up_tamer-1.1.2/up_tamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-02-23 16:58:18.000000 up_tamer-1.1.2/up_tamer/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30020 2024-02-23 16:58:18.000000 up_tamer-1.1.2/up_tamer/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:58:20.599544 up_tamer-1.1.2/up_tamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-23 16:58:20.000000 up_tamer-1.1.2/up_tamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-23 16:58:20.000000 up_tamer-1.1.2/up_tamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 16:58:20.000000 up_tamer-1.1.2/up_tamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-23 16:58:20.000000 up_tamer-1.1.2/up_tamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 16:58:20.000000 up_tamer-1.1.2/up_tamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.210898 up_tamer-1.1.2.1.dev1/up_tamer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30614 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/top_level.txt
```

### Comparing `up_tamer-1.1.2/LICENSE` & `up_tamer-1.1.2.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2/README.md` & `up_tamer-1.1.2.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2/setup.py` & `up_tamer-1.1.2.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2/up_tamer/__init__.py` & `up_tamer-1.1.2.1.dev1/up_tamer/__init__.py`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2/up_tamer/converter.py` & `up_tamer-1.1.2.1.dev1/up_tamer/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,26 +138,32 @@
     def walk_int_constant(self, expression: 'FNode',
                           args: List[pytamer.tamer_expr]) -> pytamer.tamer_expr:
         assert len(args) == 0
         return pytamer.tamer_expr_make_integer_constant(self._env, expression.constant_value())
 
     def walk_plus(self, expression: 'FNode',
                   args: List[pytamer.tamer_expr]) -> pytamer.tamer_expr:
-        assert len(args) == 2
-        return pytamer.tamer_expr_make_plus(self._env, args[0], args[1])
+        assert len(args) > 0
+        res = args[0]
+        for i in range(1, len(args)):
+            res = pytamer.tamer_expr_make_plus(self._env, res, args[i])
+        return res
 
     def walk_minus(self, expression: 'FNode',
                    args: List[pytamer.tamer_expr]) -> pytamer.tamer_expr:
         assert len(args) == 2
         return pytamer.tamer_expr_make_minus(self._env, args[0], args[1])
 
     def walk_times(self, expression: 'FNode',
                    args: List[pytamer.tamer_expr]) -> pytamer.tamer_expr:
-        assert len(args) == 2
-        return pytamer.tamer_expr_make_times(self._env, args[0], args[1])
+        assert len(args) > 0
+        res = args[0]
+        for i in range(1, len(args)):
+            res = pytamer.tamer_expr_make_times(self._env, res, args[i])
+        return res
 
     def walk_div(self, expression: 'FNode',
                  args: List[pytamer.tamer_expr]) -> pytamer.tamer_expr:
         assert len(args) == 2
         return pytamer.tamer_expr_make_div(self._env, args[0], args[1])
 
     def walk_le(self, expression: 'FNode',
```

### Comparing `up_tamer-1.1.2/up_tamer/engine.py` & `up_tamer-1.1.2.1.dev1/up_tamer/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,17 +400,25 @@
                 for c in lc:
                     expr = pytamer.tamer_expr_make_temporal_expression(self._env,
                                                                        self._convert_interval(i),
                                                                        converter.convert(c))
                     expressions.append(expr)
             for t, le in action.effects.items():
                 for e in le:
-                    assert not e.is_conditional() and e.is_assignment()
-                    ass = pytamer.tamer_expr_make_assign(self._env, converter.convert(e.fluent),
-                                                         converter.convert(e.value))
+                    assert not e.is_conditional()
+                    if e.is_assignment():
+                        ass = pytamer.tamer_expr_make_assign(self._env, converter.convert(e.fluent), converter.convert(e.value))
+                    elif e.is_increase():
+                        val = pytamer.tamer_expr_make_plus(self._env, converter.convert(e.fluent), converter.convert(e.value))
+                        ass = pytamer.tamer_expr_make_assign(self._env, converter.convert(e.fluent), val)
+                    elif e.is_decrease():
+                        val = pytamer.tamer_expr_make_minus(self._env, converter.convert(e.fluent), converter.convert(e.value))
+                        ass = pytamer.tamer_expr_make_assign(self._env, converter.convert(e.fluent), val)
+                    else:
+                        raise NotImplementedError
                     expr = pytamer.tamer_expr_make_temporal_expression(self._env,
                                                                        self._convert_timing(t),
                                                                        ass)
                     expressions.append(expr)
             for t, se in action.simulated_effects.items():
                 simulated_effects.append(self._convert_simulated_effect(converter, problem, action, t, se))
             expressions.append(self._convert_duration(converter, action.duration))
```

