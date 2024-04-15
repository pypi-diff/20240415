# Comparing `tmp/astutils-0.0.5.tar.gz` & `tmp/astutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astutils-0.0.5.tar", last modified: Tue Nov 28 12:27:21 2023, max compression
+gzip compressed data, was "astutils-0.0.6.tar", last modified: Mon Apr 15 17:15:33 2024, max compression
```

## Comparing `astutils-0.0.5.tar` & `astutils-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.786837 astutils-0.0.5/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1537 2023-11-28 12:12:52.000000 astutils-0.0.5/LICENSE
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      133 2023-11-28 12:12:52.000000 astutils-0.0.5/MANIFEST.in
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2071 2023-11-28 12:27:21.786837 astutils-0.0.5/PKG-INFO
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      960 2023-11-28 12:12:52.000000 astutils-0.0.5/README.md
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.782837 astutils-0.0.5/astutils/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      440 2023-11-28 12:12:52.000000 astutils-0.0.5/astutils/__init__.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       58 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils/_version.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2321 2023-11-28 12:12:52.000000 astutils-0.0.5/astutils/ast.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     6134 2023-11-28 12:12:52.000000 astutils-0.0.5/astutils/ply.py
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.786837 astutils-0.0.5/astutils.egg-info/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2071 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils.egg-info/PKG-INFO
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      437 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils.egg-info/SOURCES.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)        1 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils.egg-info/dependency_links.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       16 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils.egg-info/requires.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)        9 2023-11-28 12:27:21.000000 astutils-0.0.5/astutils.egg-info/top_level.txt
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.782837 astutils-0.0.5/examples/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      597 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/README.md
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.786837 astutils-0.0.5/examples/foo/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/foo/__init__.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1398 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/foo/ast.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      944 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/foo/backend.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2856 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/foo/lexyacc.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2456 2023-11-28 12:12:52.000000 astutils-0.0.5/examples/setup.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       38 2023-11-28 12:27:21.786837 astutils-0.0.5/setup.cfg
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2191 2023-11-28 12:25:58.000000 astutils-0.0.5/setup.py
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2023-11-28 12:27:21.786837 astutils-0.0.5/tests/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1339 2023-11-28 12:12:52.000000 astutils-0.0.5/tests/ast_test.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2011 2023-11-28 12:12:52.000000 astutils-0.0.5/tests/ply_test.py
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.081127 astutils-0.0.6/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1537 2024-04-15 17:14:11.000000 astutils-0.0.6/LICENSE
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      159 2024-04-15 17:14:11.000000 astutils-0.0.6/MANIFEST.in
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1682 2024-04-15 17:15:33.081127 astutils-0.0.6/PKG-INFO
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      960 2024-04-15 17:14:11.000000 astutils-0.0.6/README.md
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.077126 astutils-0.0.6/astutils/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      401 2024-04-15 17:14:11.000000 astutils-0.0.6/astutils/__init__.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       58 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils/_version.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2585 2024-04-15 17:14:11.000000 astutils-0.0.6/astutils/ast.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     6803 2024-04-15 17:14:11.000000 astutils-0.0.6/astutils/ply.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:14:11.000000 astutils-0.0.6/astutils/py.typed
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.077126 astutils-0.0.6/astutils.egg-info/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1682 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils.egg-info/PKG-INFO
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      455 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils.egg-info/SOURCES.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        1 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils.egg-info/dependency_links.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       16 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils.egg-info/requires.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        9 2024-04-15 17:15:33.000000 astutils-0.0.6/astutils.egg-info/top_level.txt
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.077126 astutils-0.0.6/examples/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      597 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/README.md
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.077126 astutils-0.0.6/examples/foo/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/foo/__init__.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1390 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/foo/ast.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      944 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/foo/backend.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2930 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/foo/lexyacc.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2214 2024-04-15 17:14:11.000000 astutils-0.0.6/examples/setup.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       38 2024-04-15 17:15:33.081127 astutils-0.0.6/setup.cfg
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1667 2024-04-15 17:14:11.000000 astutils-0.0.6/setup.py
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-15 17:15:33.077126 astutils-0.0.6/tests/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1339 2024-04-15 17:14:11.000000 astutils-0.0.6/tests/ast_test.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2017 2024-04-15 17:14:11.000000 astutils-0.0.6/tests/ply_test.py
```

### Comparing `astutils-0.0.5/LICENSE` & `astutils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astutils-0.0.5/PKG-INFO` & `astutils-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: astutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities for abstract syntax trees and parsing with PLY.
 Home-page: https://github.com/johnyf/astutils
 Author: Ioannis Filippidis
 Author-email: jfilippidis@gmail.com
 License: BSD
 Keywords: lexing,parsing,syntax tree,abstract syntax tree,AST,PLY,lex,yacc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply<=3.10,>=3.4
 
 [![Build Status][build_img]][ci]
```

### Comparing `astutils-0.0.5/README.md` & `astutils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `astutils-0.0.5/astutils/ast.py` & `astutils-0.0.6/astutils/ast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,116 @@
 """Abstract syntax tree nodes."""
 # Copyright 2014-2022 by California Institute of Technology
 # All rights reserved. Licensed under 3-clause BSD.
 #
 
 
-class Terminal(object):
+class Terminal:
     """Nullary symbol."""
 
     def __init__(
             self,
-            value,
-            dtype='terminal'):
+            value:
+                str,
+            dtype:
+                str='terminal'
+            ) -> None:
         try:
             value + 's'
         except TypeError:
             raise TypeError(
                 'value must be a string, '
-                'got: {v}'.format(
-                    v=value))
+                f'got: {value}')
         self.type = dtype
         self.value = value
 
-    def __hash__(self):
+    def __hash__(
+            self
+            ) -> int:
         return id(self)
 
-    def __repr__(self):
-        return '{cls}({v}, {t})'.format(
-            cls=type(self).__name__,
-            t=repr(self.type),
-            v=repr(self.value))
+    def __repr__(
+            self
+            ) -> str:
+        class_name = type(self).__name__
+        return (
+            f'{class_name}('
+                f'{self.value!r}, '
+                f'{self.type!r})')
 
-    def __str__(self, *arg, **kw):
+    def __str__(
+            self,
+            *arg,
+            **kw
+            ) -> str:
         return self.value
 
-    def __len__(self):
+    def __len__(
+            self
+            ) -> int:
         return 1
 
-    def __eq__(self, other):
-        try:
-            return (
-                self.type == other.type and
-                self.value == other.value)
-        except AttributeError:
-            return False
+    def __eq__(
+            self,
+            other
+            ) -> bool:
+        return (
+            hasattr(other, 'type') and
+            hasattr(other, 'value') and
+            self.type == other.type and
+            self.value == other.value)
 
-    def flatten(self, *arg, **kw):
+    def flatten(
+            self,
+            *arg,
+            **kw):
         return self.value
 
 
-class Operator(object):
+class Operator:
     """Operator with arity > 0."""
 
     def __init__(
             self,
-            operator,
-            *operands):
+            operator:
+                str,
+            *operands
+            ) -> None:
         try:
             operator + 'a'
         except TypeError:
             raise TypeError(
                 'operator must be string, '
-                'got: {op}'.format(
-                    op=operator))
+                f'got: {operator}')
         self.type = 'operator'
         self.operator = operator
         self.operands = list(operands)
 
-    def __repr__(self):
-        return '{cls}({op}, {xyz})'.format(
-            cls=type(self).__name__,
-            op=repr(self.operator),
-            xyz=', '.join(
-                repr(x)
-                for x in self.operands))
-
-    def __str__(self):
-        return '({op} {xyz})'.format(
-            op=self.operator,
-            xyz=' '.join(
-                x.__str__()
-                for x in self.operands))
-
-    def __len__(self):
-        return 1 + sum(
-            len(x) for x in self.operands)
-
-    def flatten(self, *arg, **kw):
-        return ' '.join([
-            '(',
-            self.operator,
-            ', '.join(
-                x.flatten(*arg, **kw)
-                for x in self.operands),
-            ')'])
+    def __repr__(
+            self
+            ) -> str:
+        class_name = type(self).__name__
+        xyz = ', '.join(map(repr, self.operands))
+        return (
+            f'{class_name}('
+                f'{self.operator!r}, '
+                f'{xyz})')
+
+    def __str__(
+            self
+            ) -> str:
+        xyz = ' '.join(map(str, self.operands))
+        return f'({self.operator} {xyz})'
+
+    def __len__(
+            self
+            ) -> int:
+        return 1 + sum(map(len, self.operands))
+
+    def flatten(
+            self,
+            *arg,
+            **kw):
+        csv = ', '.join(
+            x.flatten(*arg, **kw)
+            for x in self.operands)
+        return f'( {self.operator} {csv} )'
```

### Comparing `astutils-0.0.5/astutils/ply.py` & `astutils-0.0.6/astutils/ply.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Utilities for Python lex-yacc (PLY)."""
 # Copyright 2014-2022 by California Institute of Technology
 # All rights reserved. Licensed under 3-clause BSD.
 #
-from __future__ import absolute_import
 import logging
 import os
 import textwrap as _tw
+import typing as _ty
 import warnings
 
 import ply.lex
 import ply.yacc
 
 import astutils.ast as _ast
 
 
 logger = logging.getLogger(__name__)
 
 
-class Lexer(object):
+class Lexer:
     """Init and build methods."""
 
-    def __init__(self, debug=False):
+    def __init__(
+            self,
+            debug:
+                bool=False
+            ) -> None:
         self.reserved = getattr(
             self, 'reserved', dict())
         self.delimiters = getattr(
             self, 'delimiters', list())
         self.operators = getattr(
             self, 'operators', list())
         self.misc = getattr(
@@ -34,45 +38,50 @@
         self.tokens = (
             self.delimiters +
             self.operators +
             self.misc +
             sorted(set(self.reserved.values())))
         self.build(debug=debug)
 
-    def t_error(self, t):
-        raise Exception(
-            'Illegal character "{t}"'.format(
-                t=t.value[0]))
+    def t_error(
+            self,
+            t
+            ) -> _ty.NoReturn:
+        raise RuntimeError(
+            f'Illegal character "{t.value[0]}"')
 
     def build(
             self,
-            debug=False,
+            debug:
+                bool=False,
             debuglog=None,
-            **kwargs):
+            **kwargs
+            ) -> None:
         """Create a lexer."""
         if debug and debuglog is None:
             debuglog = self.logger
         self.lexer = ply.lex.lex(
             module=self,
             debug=debug,
             debuglog=debuglog,
             **kwargs)
 
 
-class Parser(object):
+class Parser:
     """Init, build and parse methods.
 
     To subclass, overwrite the class attributes
     defined below, and add production rules.
     """
 
     def __init__(
             self,
             nodes=None,
-            lexer=None):
+            lexer=None
+            ) -> None:
         self.tabmodule = getattr(
             self, 'tabmodule', None)
         self.start = getattr(
             self, 'start', 'expr')
         # low to high
         self.precedence = getattr(
             self, 'precedence', tuple())
@@ -102,19 +111,25 @@
                 'pass argument `lexer` to '
                 '`Parser.__init__()`')
         self.tokens = self._lexer.tokens
         self.parser = None
 
     def build(
             self,
-            tabmodule=None,
-            outputdir='',
-            write_tables=False,
-            debug=False,
-            debuglog=None):
+            tabmodule:
+                str |
+                None=None,
+            outputdir:
+                str='',
+            write_tables:
+                bool=False,
+            debug:
+                bool=False,
+            debuglog=None
+            ) -> None:
         """Build parser using `ply.yacc`."""
         if tabmodule is None:
             tabmodule = self.tabmodule
         if debug and debuglog is None:
             debuglog = self.logger
         self.parser = ply.yacc.yacc(
             method='LALR',
@@ -124,56 +139,79 @@
             outputdir=outputdir,
             write_tables=write_tables,
             debug=debug,
             debuglog=debuglog)
 
     def parse(
             self,
-            formula,
-            debuglog=None):
+            formula:
+                str,
+            debuglog=None
+            ) -> _ty.Any:
         """Parse string `formula`.
 
         @param formula:
             input to the parser
-        @type formula:
-            `str`
         @return:
             what the parser returns
             (many parsers return a syntax tree)
         """
         if self.parser is None:
             self.build()
         root = self.parser.parse(
             input=formula,
             lexer=self._lexer.lexer,
             debug=debuglog)
+        self._clear_lr_stack()
         if root is not None:
             return root
-        raise Exception(
-            'failed to parse:\n\t{f}'.format(
-                f=formula))
+        raise RuntimeError(
+            f'failed to parse:\n\t{formula}')
 
-    def p_error(self, p):
+    def _clear_lr_stack(
+            self
+            ) -> None:
+        """Ensure no references remain.
+
+        Otherwise, references can prevent `gc` from
+        collecting objects that are expected to
+        have become unreachable.
+        """
+        has_lr_stack = (
+            self.parser is not None and
+            hasattr(self.parser, 'statestack') and
+            hasattr(self.parser, 'symstack'))
+        if not has_lr_stack:
+            return
+        self.parser.restart()
+
+    def p_error(
+            self,
+            p
+            ) -> _ty.NoReturn:
         s = list()
         while True:
             tok = self.parser.token()
             if tok is None:
                 break
             s.append(tok.value)
-        raise Exception(
-            'Syntax error at "{p}"\n'.format(
-                p=p.value) +
-            'remaining input:\n{s}\n'.format(
-                s=' '.join(s)))
+        s = ' '.join(s)
+        raise RuntimeError(
+            f'Syntax error at "{p.value}"\n'
+            f'remaining input:\n{s}\n')
 
 
 def rewrite_tables(
-        parser_class,
-        tabmodule,
-        outputdir):
+        parser_class:
+            type[Parser],
+        tabmodule:
+            str,
+        outputdir:
+            str
+        ) -> None:
     """Write the parser table file.
 
     Overwrites any preexisting parser file.
 
     The module name (after last dot) in `tabmodule`
     is appended to `outputdir` to form the path.
 
@@ -192,36 +230,28 @@
         rewrite_tables(Parser, _TABMODULE, outputdir)
     ```
 
     @param parser_class:
         PLY production rules
     @param tabmodule:
         module name for table file
-    @type tabmodule:
-        `str`
     @param outputdir:
         dump parser file
         in this directory
-    @type outputdir:
-        `str`
     """
     if outputdir is None:
         raise ValueError(
             '`outputdir` must be `str`.')
-    table = tabmodule.rpartition('.')[-1]
+    *_, table = tabmodule.rpartition('.')
     for ext in ('.py', '.pyc'):
         path = outputdir + table + ext
         if os.path.isfile(path):
-            logger.info(
-                'found file `{path}`'.format(
-                    path=path))
+            logger.info(f'found file `{path}`')
             os.remove(path)
-            logger.info(
-                'removed file `{path}`'.format(
-                    path=path))
+            logger.info(f'removed file `{path}`')
     parser = parser_class()
     debugfile = ply.yacc.debug_file
     path = os.path.join(outputdir, debugfile)
     with open(path, 'w') as debuglog_file:
         debuglog = ply.yacc.PlyLogger(debuglog_file)
         parser.build(
             write_tables=True,
```

### Comparing `astutils-0.0.5/astutils.egg-info/PKG-INFO` & `astutils-0.0.6/astutils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: astutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities for abstract syntax trees and parsing with PLY.
 Home-page: https://github.com/johnyf/astutils
 Author: Ioannis Filippidis
 Author-email: jfilippidis@gmail.com
 License: BSD
 Keywords: lexing,parsing,syntax tree,abstract syntax tree,AST,PLY,lex,yacc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply<=3.10,>=3.4
 
 [![Build Status][build_img]][ci]
```

### Comparing `astutils-0.0.5/examples/README.md` & `astutils-0.0.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `astutils-0.0.5/examples/foo/ast.py` & `astutils-0.0.6/examples/foo/ast.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 be used with different backends. Each backend is
 created by subclassing the below classes, then
 overriding the `flatten` method.
 """
 import astutils
 
 
-class Nodes(object):
+class Nodes:
     """Namespace of AST node classes."""
 
     Terminal = astutils.Terminal
     Operator = astutils.Operator
 
     class Var(astutils.Terminal):
         """Variable identifier."""
```

### Comparing `astutils-0.0.5/examples/foo/backend.py` & `astutils-0.0.6/examples/foo/backend.py`

 * *Files identical despite different names*

### Comparing `astutils-0.0.5/examples/foo/lexyacc.py` & `astutils-0.0.6/examples/foo/lexyacc.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,44 +23,47 @@
             'NOT', 'AND', 'OR', 'XOR',
             'IMP', 'BIMP',
             'EQUALS', 'NEQUALS']
         self.misc = ['NAME', 'NUMBER']
         super(Lexer, self).__init__(**kw)
 
     def t_NAME(self, t):
-        r'[A-Za-z_][A-za-z0-9]*'
+        r"""
+        [A-Za-z_]
+        [A-Za-z0-9]*
+        """
         t.type = self.reserved.get(
             t.value, 'NAME')
         return t
 
     def t_AND(self, t):
-        r'\&\&'
+        r' \& \& '
         t.value = '&'
         return t
 
     def t_OR(self, t):
-        r'\|\|'
+        r' \| \| '
         t.value = '|'
         return t
 
-    t_NOT = r'\!'
-    t_XOR = r'\^'
-    t_LPAREN = r'\('
-    t_RPAREN = r'\)'
-    t_NUMBER = r'\d+'
-    t_IMP = '->'
-    t_BIMP = r'\<->'
-    t_ignore = ' \t'
+    t_NOT = r' \! '
+    t_XOR = r' \^ '
+    t_LPAREN = r' \( '
+    t_RPAREN = r' \) '
+    t_NUMBER = r' \d+ '
+    t_IMP = ' -> '
+    t_BIMP = r' \< -> '
+    t_ignore = ''.join(['\x20', '\t'])
 
     def t_comment(self, t):
-        r'\#.*'
+        r' \#.* '
         return
 
     def t_newline(self, t):
-        r'\n+'
+        r' \n+ '
         t.lexer.lineno += t.value.count('\n')
 
 
 class Parser(astutils.Parser):
     """Parser for Boolean formulae."""
 
     def __init__(self, **kw):
```

### Comparing `astutils-0.0.5/examples/setup.py` & `astutils-0.0.6/examples/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,31 +19,22 @@
 import sys
 
 import setuptools
 
 
 PACKAGE_NAME = 'foo'
 DESCRIPTION = 'foo is very useful.'
-PACKAGE_URL = 'https://example.org/{name}'.format(
-    name=PACKAGE_NAME)
+PACKAGE_URL = f'https://example.org/{PACKAGE_NAME}'
 README = 'README.md'
-VERSION_FILE = '{name}/_version.py'.format(
-    name=PACKAGE_NAME)
-MAJOR = 0
-MINOR = 0
-MICRO = 1
-VERSION = '{major}.{minor}.{micro}'.format(
-    major=MAJOR, minor=MINOR, micro=MICRO)
+VERSION_FILE = f'{PACKAGE_NAME}/_version.py'
+VERSION = '0.0.1'
 VERSION_FILE_TEXT = (
     '# This file was generated from setup.py\n'
-    "version = '{version}'\n").format(
-        version=VERSION)
-PYTHON_REQUIRES = (
-    '>=2.7, '
-    '!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*')
+    f"version = '{VERSION}'\n")
+PYTHON_REQUIRES = '>=3.10'
 PLY_REQUIRED = 'ply >= 3.4, <= 3.10'
 INSTALL_REQUIRES = [PLY_REQUIRED]
 TESTS_REQUIRE = [
     'pytest >= 4.6.11']
 
 
 def run_setup():
```

### Comparing `astutils-0.0.5/setup.py` & `astutils-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 """Installation script."""
 import setuptools
 
 
 PACKAGE_NAME = 'astutils'
 DESCRIPTION = 'Utilities for abstract syntax trees and parsing with PLY.'
-PACKAGE_URL = 'https://github.com/johnyf/{name}'.format(name=PACKAGE_NAME)
+PACKAGE_URL = f'https://github.com/johnyf/{PACKAGE_NAME}'
 README = 'README.md'
-VERSION_FILE = '{name}/_version.py'.format(name=PACKAGE_NAME)
-MAJOR = 0
-MINOR = 0
-MICRO = 5
-VERSION = '{major}.{minor}.{micro}'.format(
-    major=MAJOR, minor=MINOR, micro=MICRO)
+VERSION_FILE = f'{PACKAGE_NAME}/_version.py'
+VERSION = '0.0.6'
 VERSION_FILE_TEXT = (
     '# This file was generated from setup.py\n'
-    "version = '{version}'\n").format(version=VERSION)
-PYTHON_REQUIRES = (
-    '>=2.7, '
-    '!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*')
+    f"version = '{VERSION}'\n")
+PYTHON_REQUIRES = '>=3.10'
 TESTS_REQUIRE = ['pytest >= 4.6.11']
 KEYWORDS = [
     'lexing', 'parsing', 'syntax tree', 'abstract syntax tree',
     'AST', 'PLY', 'lex', 'yacc']
 CLASSIFIERS = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 2.7',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3 :: Only',
     'Topic :: Software Development']
 
 
 def run_setup():
     """Install."""
     with open(VERSION_FILE, 'w') as f:
         f.write(VERSION_FILE_TEXT)
```

### Comparing `astutils-0.0.5/tests/ast_test.py` & `astutils-0.0.6/tests/ast_test.py`

 * *Files identical despite different names*

### Comparing `astutils-0.0.5/tests/ply_test.py` & `astutils-0.0.6/tests/ply_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,23 +62,23 @@
     assert r is True, r
 
 
 def test_illegal_character():
     parser = Parser()
     parser.names = {'True': True}
     s = '( True'
-    with pytest.raises(Exception):
+    with pytest.raises(RuntimeError):
         parser.parse(s)
 
 
 def test_syntax_error():
     parser = Parser()
     parser.names = {'True': True}
     s = 'True True'
-    with pytest.raises(Exception):
+    with pytest.raises(RuntimeError):
         parser.parse(s)
 
 
 def test_rewrite_tables():
     prefix = 'foo'
     outputdir = './'
     for ext in ('.py', '.pyc'):
```

