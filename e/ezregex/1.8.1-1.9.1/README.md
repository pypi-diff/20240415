# Comparing `tmp/ezregex-1.8.1.tar.gz` & `tmp/ezregex-1.9.1.tar.gz`

## Comparing `ezregex-1.8.1.tar` & `ezregex-1.9.1.tar`

### file list

```diff
@@ -1,33 +1,42 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.8.1/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.8.1/MANIFEST.in
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 ezregex-1.8.1/generate_docs.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezregex-1.8.1/requirements.txt
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 ezregex-1.8.1/setup.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ezregex-1.8.1/todo.txt
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.8.1/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.8.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.8.1/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ezregex-1.8.1/.vscode/settings.json
--rw-r--r--   0        0        0    17630 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/EZRegex.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/__init__.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/api.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/api.pyi
--rw-r--r--   0        0        0    10221 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/generate.py
--rw-r--r--   0        0        0    24530 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/invert.py
--rw-r--r--   0        0        0    10146 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/invert_old.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/perl/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/perl/elements.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/python/__init__.py
--rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/python/elements.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 ezregex-1.8.1/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 ezregex-1.8.1/tests/_groups.py
--rw-r--r--   0        0        0    29621 2020-02-02 00:00:00.000000 ezregex-1.8.1/tests/_regexs.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ezregex-1.8.1/tests/test_generate.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.8.1/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    15150 2020-02-02 00:00:00.000000 ezregex-1.8.1/tests/tests.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.8.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.8.1/LICENSE
--rw-r--r--   0        0        0    23515 2020-02-02 00:00:00.000000 ezregex-1.8.1/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ezregex-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    23770 2020-02-02 00:00:00.000000 ezregex-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.1/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.1/MANIFEST.in
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ezregex-1.9.1/requirements.txt
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 ezregex-1.9.1/setup.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ezregex-1.9.1/todo.txt
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.1/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.1/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    18421 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/EZRegex.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/_dialects.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/_docs.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/generate.py
+-rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/invert.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/invert_old.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/elements.py
+-rw-r--r--   0        0        0    13333 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/interface.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/psuedonymns.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/psuedonymns.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/elements.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/psuedonymns.py
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/_groups.py
+-rw-r--r--   0        0        0    29505 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/_regexs.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/test_generate.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/tests.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.1/LICENSE
+-rw-r--r--   0        0        0    49171 2020-02-02 00:00:00.000000 ezregex-1.9.1/README.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ezregex-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    49406 2020-02-02 00:00:00.000000 ezregex-1.9.1/PKG-INFO
```

### Comparing `ezregex-1.8.1/setup.py` & `ezregex-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/todo.txt` & `ezregex-1.9.1/todo.txt`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/.github/FUNDING.yml` & `ezregex-1.9.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/.github/workflows/unit-tests.yml` & `ezregex-1.9.1/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/ezregex/EZRegex.py` & `ezregex-1.9.1/ezregex/EZRegex.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,132 +1,156 @@
+# pyright: reportArgumentType = false
+import colorsys
+import logging
 import re
 from copy import deepcopy
 from functools import partial
-from re import RegexFlag
-from typing import List
+from typing import Callable, List, Literal, LiteralString
 from warnings import warn
 
-from rich import print as rprint
-from rich.panel import Panel
-from rich.text import Text
-
-from .invert import invert
+from .api import api
 from .generate import *
+from .invert import invert
+from ._dialects import dialects
 
+# TODO: consider changing addFlags to "outer" or "end" or something
+# TODO: Seriously consider removing the debug functions
 
 class EZRegex:
     """ Represent parts of the Regex syntax. Should not be instantiated by the user directly."""
 
-    def __init__(self, funcs:List[partial], sanatize=True, init=True, replacement=False, flags=0):
-        """ The workhorse of the EZRegex library. This represents a regex pattern
-        that can be combined with other EZRegexs and strings.
-        Ideally, this should only be called internally, but it should still
-        work from the user's end """
-        self.flags = flags
+    def __init__(self,
+                 definition:List[partial[str]]|str|"EZRegex"|partial[str]|list[str],
+                 dialect: str,
+                 sanatize:bool=True,
+                 init:bool=True,
+                 replacement:bool=False,
+                 flags:str='',
+        ):
+        """
+        The workhorse of the EZRegex library. This represents a regex pattern that can be combined
+        with other EZRegexs and strings. Ideally, this should only be called internally, but it should
+        still work from the user's end
+        """
 
+        if dialect not in dialects.keys():
+            raise ValueError(f'Unsupported dialect `{dialect}` given. Supported dialects are: {list(dialects.keys())}')
+
+        self.flags = flags
         # Parse params
         # Add flags if it's another EZRegex
-        if isinstance(funcs, EZRegex):
-            self.flags = funcs.flags
-
-        if isinstance(funcs, (str, EZRegex)):
-            funcs = [str(funcs)]
-        elif not isinstance(funcs, (list, tuple)):
-            funcs = [funcs]
+        if isinstance(definition, EZRegex):
+            self.flags = definition.flags
+            if definition.dialect != dialect:
+                raise ValueError('Cannot mix regex dialects')
+
+        if isinstance(definition, (str, EZRegex)):
+            definition = [str(definition)]
+        elif not isinstance(definition, (list, tuple)):
+            definition = [definition]
 
         self.sanatize = sanatize
         self.replacement = replacement
-        self.funcList = list(funcs)
+        # This allows strings in the list now, but they get converted later in this function
+        self.funcList: list[str|partial[str]|Callable] = list(definition)
+        # Just some psuedonymns
         self.example = self.invert = self.inverse
+        self.dialect = dialect
+        # The dict that has the values
+        self._dialect = dialects[dialect]
+
 
         # The init parameter is not actually required, but it will make it more
         # efficient, so we don't have to check that the whole chain is callable
         if init:
             # Go through the chain (most likely of length 1) and parse any strings
             # This is for simplicity when defining all the members
             for i in range(len(self.funcList)):
                 if isinstance(self.funcList[i], str):
                     # I *hate* how Python handles lambdas
                     stringBecauseHatred = deepcopy(self.funcList[i])
                     self.funcList[i] = lambda cur=...: cur + stringBecauseHatred
                 elif not callable(self.funcList[i]) and self.funcList[i] is not None:
-                    raise TypeError(f"Invalid type {type(self.funcList[i])} passed to EZRegex constructor")
+                    raise ValueError(f"Invalid type {type(self.funcList[i])} passed to EZRegex constructor")
+
+
+    def _escape(self, pattern:str):
+        """ This function was modified from the one in /usr/lib64/python3.12/re/__init__.py line 255 """
+        _special_chars_map = {i: '\\' + chr(i) for i in self._dialect['escape_chars']}
+        return pattern.translate(_special_chars_map)
+
 
     def _sanitizeInput(self, i, addFlags=False):
-        """ Instead of rasising an error if passed a strange datatype, it now
-            trys to cast it to a string """
+        """ Instead of rasising an error if passed a strange datatype, it now trys to cast it to a string """
         i = deepcopy(i)
 
         # Don't sanatize anything if this is a replacement string
         if self.replacement:
             return str(i)
 
         # If it's another chain, compile it
         if isinstance(i, EZRegex):
             return i._compile(addFlags=addFlags)
         # It's a string (so we need to escape it)
         elif isinstance(i, str):
-            i = re.escape(i)
-            return i
+            return self._escape(i)
         # A couple of singletons use bools and None as kwargs, just ignore them and move on
         elif i is None or isinstance(i, bool):
             return i
         # A couple singletons use ints as input, just cast it to a string and don't throw a warning
         elif isinstance(i, int):
             return str(i)
         # It's something we don't know, but try to cast it to a string anyway
         else:
             try:
-                s = str(i)
-                msg = f"Type {type(i)} passed to EZRegex, auto-casting to a string. Special characters will will not be escaped."
-                try:
-                    from Cope import debug
-                except:
-                    warn(msg)
-                else:
-                    debug(msg, color=-1, calls=3)
-                return s
+                logging.warning(f"Type {type(i)} passed to EZRegex, auto-casting to a string. Special characters will will not be escaped.")
+                return str(i)
             except:
-                raise TypeError(f'Incorrect type {type(i)} given to EZRegex parameter: Must be string or another EZRegex chain.')
+                raise ValueError(f'Incorrect type {type(i)} given to EZRegex parameter: Must be string or another EZRegex chain.')
 
     def __call__(self, *args, **kwargs):
-        """ This should be called by the user to specify the specific parameters
-            of this instance
-            i.e. anyof('a', 'b') """
+        """ This should be called by the user to specify the specific parameters of this instance i.e. anyof('a', 'b') """
         # If this is being called without parameters, just compile the chain.
         # If it's being called *with* parameters, then it better be a fundemental
         # member, otherwise that doesn't make any sense.
         if len(self.funcList) > 1:
             if not len(args) and not len(kwargs):
                 return self._compile()
             else:
-                raise TypeError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
+                raise ValueError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
 
         # Sanatize the arguments
         args = list(map(self._sanitizeInput if self.sanatize else deepcopy, args))
 
         _kwargs = {}
         for key, val in kwargs.items():
             _kwargs[key] = self._sanitizeInput(val) if self.sanatize else deepcopy(val)
 
-        return EZRegex([partial(self.funcList[0], *args, **_kwargs)], init=False, sanatize=self.sanatize, replacement=self.replacement, flags=self.flags)
+        return EZRegex(
+            [partial(self.funcList[0], *args, **_kwargs)],
+            dialect=self.dialect,
+            init=False,
+            sanatize=self.sanatize,
+            replacement=self.replacement,
+            flags=self.flags
+        )
 
     # Magic Functions
     def __str__(self, addFlags=True):
         return self._compile(addFlags)
 
     def __repr__(self):
         return 'EZRegex("' + self._compile() + '")'
 
     def __eq__(self, thing):
         return self._sanitizeInput(thing, addFlags=True) == self._compile()
 
     def __mul__(self, amt):
         if amt is Ellipsis:
-            return EZRegex(f'(?{self})*', sanatize=False)
+            return EZRegex(f'(?{self})*', self.dialect, sanatize=False)
         rtn = self
         # This isn't optimal, but it's unlikely anyone will use this with large numbers
         for i in range(amt-1):
             # This doesn't work
             # rtn += self
             # But this does??
             rtn = rtn + self
@@ -136,39 +160,41 @@
         return self * amt
 
     def __imul__(self, amt):
         return self * amt
 
     def __add__(self, thing):
         return EZRegex(self.funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
+            dialect=self.dialect,
             init=False,
             sanatize=self.sanatize or thing.sanatize if isinstance(thing, EZRegex) else self.sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
-            flags=(self.flags | thing.flags) if isinstance(thing, EZRegex) else self.flags
+            flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __radd__(self, thing):
         return EZRegex([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self.funcList,
+            dialect=self.dialect,
             init=False,
             sanatize=self.sanatize or thing.sanatize if isinstance(thing, EZRegex) else self.sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
-            flags=(self.flags | thing.flags) if isinstance(thing, EZRegex) else self.flags
+            flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __iadd__(self, thing):
         # return self + self._sanitizeInput(thing)
         return self + thing
 
     def __and__(self, thing):
         warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={self}){thing}', sanatize=False)
+        return EZRegex(fr'(?={self}){thing}', self.dialect, sanatize=False)
 
     def __rand__(self, thing):
         warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={thing}){self}', sanatize=False)
+        return EZRegex(fr'(?={thing}){self}', self.dialect, sanatize=False)
 
     # The shift operators just shadow the add operators
     def __lshift__(self, thing):
         return self.__add__(thing)
 
     def __rlshift__(self, thing):
         return self.__radd__(thing)
@@ -190,33 +216,32 @@
         return self.invert()
 
     def __not__(self):
         raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
 
     def __pos__(self):
         comp = self._compile()
-        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', sanatize=False)
+        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self.dialect, sanatize=False)
 
     def __ror__(self, thing):
         print('ror called')
-        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', sanatize=False)
+        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self.dialect, sanatize=False)
 
     def __or__(self, thing):
         warn('The or operator is unstable and likely to fail, if used more than twice. Use anyof() instead, for now.')
-        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', sanatize=False)
+        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self.dialect, sanatize=False)
 
     def __xor__(self, thing):
         return NotImplemented
 
     def __rxor__(self, thing):
         return NotImplemented
 
     def __mod__(self, other):
-        """ I would prefer __rmod__(), but it doesn't work on strings, since
-            __mod__() is already specified for string formmating. """
+        """ I would prefer __rmod__(), but it doesn't work on strings, since __mod__() is already specified for string formmating. """
         # I don't need to check this, re will do it for me
         # if not isisntance(other, str):
             # raise TypeError(f"Can't search type {type(other)} ")
         return re.search(other, self._compile())
 
     def __hash__(self):
         if len(self.funcList) > 1:
@@ -261,78 +286,60 @@
             # assert digit[...:'foo'] == digit[None:'foo'] == digit[,'foo'] ==
             pass
         elif type(args) is not tuple or len(args) == 1:
             if type(args) is tuple:
                 args = args[0]
             if args is None or args is Ellipsis or args == 0:
                 # at_least_0(self)
-                return EZRegex(fr'(?:{self._compile()})*', sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
             elif args == 1:
                 # at_least_1(self)
-                return EZRegex(fr'(?:{self._compile()})+', sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
             else:
                 # match_at_least(args, self)
-                return EZRegex(fr'(?:{self._compile()}){{{args},}}', sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self.dialect, sanatize=False)
         else:
             start, end = args
             if start is None or start is Ellipsis:
                 # match_at_most(2, self)
-                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self.dialect, sanatize=False)
             elif end is None or end is Ellipsis:
                 if start == 0:
                     # at_least_0(self)
-                    return EZRegex(fr'(?:{self._compile()})*', sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
                 elif start == 1:
                     # at_least_1(self)
-                    return EZRegex(fr'(?:{self._compile()})+', sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
                 else:
                     # match_at_least(start, self)
-                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self.dialect, sanatize=False)
             else:
                 # match_range(start, end, self)
-                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self.dialect, sanatize=False)
 
     def __reversed__(self):
         return self.inverse()
 
     def __rich__(self):
         return self._compile()
 
     def __pretty__(self):
         return self._compile()
 
     # Regular functions
     def _compile(self, addFlags=True):
         regex = ''
         for func in self.funcList:
-            regex = func(cur=regex)
+            regex = func(cur=regex) # type: ignore
 
         # Add the flags
-        _flags = ''
         if addFlags:
-            if self.flags & RegexFlag.ASCII:
-                _flags += 'a'
-            if self.flags & RegexFlag.DEBUG:
-                pass
-            if self.flags & RegexFlag.DOTALL:
-                _flags += 's'
-            if self.flags & RegexFlag.IGNORECASE:
-                _flags += 'i'
-            if self.flags & RegexFlag.LOCALE:
-                _flags += 'L'
-            if self.flags & RegexFlag.MULTILINE:
-                _flags += 'm'
-            if self.flags & RegexFlag.TEMPLATE:
-                pass
-            if self.flags & RegexFlag.UNICODE:
-                _flags += 'u'
-            if self.flags & RegexFlag.VERBOSE:
-                _flags += 'x'
-            if len(_flags):
-                regex = fr'(?{_flags})' + regex
+            regex = self._dialect['beginning'] + regex + self._dialect['end']
+            if len(self.flags):
+                regex = self._dialect['flag_func'](regex, self.flags)
         return regex
 
     def compile(self, addFlags=True):
         return re.compile(self._compile(addFlags))
 
     def str(self):
         return self.__str__()
@@ -345,90 +352,93 @@
         else:
             debug(self, name='Compiled ezregex string', calls=2)
         return self
 
     def debugStr(self):
         return self.debug().str()
 
-    def copy(self):
+    def copy(self, addFlags=True):
         try:
-            from clipboard import copy
+            from clipboard import copy  # type: ignore
         except ImportError as err:
             raise ModuleNotFoundError('Please install the clipboard module in order to auto copy '
                                       'ezregex expressions (i.e. pip install clipboard)') from err
         else:
-            copy(self._compile())
+            copy(self._compile(addFlags=addFlags))
 
-    # def test(self, testString=None, show=True, context=True) -> bool:
-    #     """ Tests the current regex expression to see if it's in @param testString.
-    #         Returns the match objects (None if there was no match)"""
-    #     # json = self._matchJSON(testString=testString)
-    #     json = api(self, test_string=testString)
-    #     if not show:
-    #         return bool(len(json['matches']))
-
-    #     _cope = False
-    #     if context:
-    #         # Use the nice context function in the Cope library
-    #         try:   from Cope import get_context, get_metadata
-    #         except ImportError: pass
-    #         else:  _cope = True
-
-    #     st = Text()  # String
-    #     gt = Text()  # Groups (all the group-related text)
-    #     defaultColor = 'bold'
-    #     textColor = ''
-
-    #     st.append("Testing expression", style=defaultColor)
-    #     # Add the context line
-    #     if _cope:
-    #         st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
-    #     st.append(':\n', style=defaultColor)
-
-    #     # The expression we're testing
-    #     st.append(f'\t{json["regex"]}\n', style=textColor)
-    #     st.append("for matches in:\n\t", style=defaultColor)
-
-    #     # Add the main string
-    #     for color, background, part in json['parts']:
-    #         st.append(part, style=color if background is None else f'{color} on {background}')
-    #     st.append('\n')
-
-    #     # Add all the matches and groups
-    #     for m in json['matches']:
-    #         gt.append('Match = "')
-    #         for color, background, part in m['match']['parts']:
-    #             gt.append(part, style=color if background is None else f'{color} on {background}')
-    #         gt.append('" ')
-    #         gt.append(f"({m['match']['start']}:{m['match']['end']})", style='italic bright_black')
-    #         gt.append('\n')
-    #         if len(m['unnamedGroups']):
-    #             gt.append('Unnamed Groups:\n')
-    #         for cnt, group in enumerate(m['unnamedGroups']):
-    #             gt.append(f'\t{cnt+1}: "')
-    #             gt.append(group['string'], style=group['color'])
-    #             gt.append('" ')
-    #             gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
-    #             gt.append('\n')
-    #         if len(m['namedGroups']):
-    #             gt.append('Named Groups:\n')
-    #         for name, group in m['namedGroups'].items():
-    #             gt.append(f'\t{name}: "')
-    #             gt.append(group['string'], style=group['color'])
-    #             gt.append('" ')
-    #             gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
-    #             gt.append('\n')
-    #         gt.append('\n')
-
-    #     # Assemble everything into a panel
-    #     rprint(Panel(Text.assemble(*st, '\n', *gt),
-    #         title='Testing Regex',
-    #         subtitle=Text('Found\n', style='blue') if len(json['matches'])
-    #             else Text('Not Found\n', style='red')))  #, border_style='dim green')
+    def test(self, testString=None, show=True, context=True) -> bool:
+        """ Tests the current regex expression to see if it's in @param testString.
+            Returns the match objects (None if there was no match)"""
+        from rich import print as rprint
+        from rich.panel import Panel
+        from rich.text import Text
+
+        # json = self._matchJSON(testString=testString)
+        json = api(self, test_string=testString)
+        if not show:
+            return bool(len(json['matches']))
+
+        _cope = False
+        if context:
+            # Use the nice context function in the Cope library
+            try:   from Cope import get_context, get_metadata
+            except ImportError: pass
+            else:  _cope = True
+
+        st = Text()  # String
+        gt = Text()  # Groups (all the group-related text)
+        defaultColor = 'bold'
+        textColor = ''
+
+        st.append("Testing expression", style=defaultColor)
+        # Add the context line
+        if _cope:
+            st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
+        st.append(':\n', style=defaultColor)
+
+        # The expression we're testing
+        st.append(f'\t{json["regex"]}\n', style=textColor)
+        st.append("for matches in:\n\t", style=defaultColor)
+
+        # Add the main string
+        for color, background, part in json['parts']:
+            st.append(part, style=color if background is None else f'{color} on {background}')
+        st.append('\n')
+
+        # Add all the matches and groups
+        for m in json['matches']:
+            gt.append('Match = "')
+            for color, background, part in m['match']['parts']:
+                gt.append(part, style=color if background is None else f'{color} on {background}')
+            gt.append('" ')
+            gt.append(f"({m['match']['start']}:{m['match']['end']})", style='italic bright_black')
+            gt.append('\n')
+            if len(m['unnamed groups']):
+                gt.append('Unnamed Groups:\n')
+            for id, group in m['unnamed groups'].items():
+                gt.append(f'\t{id}: "')
+                gt.append(['string'], style=group['color'])
+                gt.append('" ')
+                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
+                gt.append('\n')
+            if len(m['named groups']):
+                gt.append('Named Groups:\n')
+            for name, group in m['named groups'].items():
+                gt.append(f'\t{name}: "')
+                gt.append(group['string'], style=group['color'])
+                gt.append('" ')
+                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
+                gt.append('\n')
+            gt.append('\n')
+
+        # Assemble everything into a panel
+        rprint(Panel(Text.assemble(*st, '\n', *gt),
+            title='Testing Regex',
+            subtitle=Text('Found\n', style='blue') if len(json['matches'])
+                else Text('Not Found\n', style='red')))  #, border_style='dim green')
 
-    #     return bool(len(json['matches']))
+        return bool(len(json['matches']))
 
     def inverse(self, amt=1, **kwargs):
-        """ "Inverts" the current Regex expression to give an example of a string
-            it would match.
+        """ "Inverts" the current Regex expression to give an example of a string it would match.
             Useful for debugging purposes. """
         return '\n'.join([invert(self._compile(), **kwargs) for _ in range(amt)])
```

### Comparing `ezregex-1.8.1/ezregex/api.py` & `ezregex-1.9.1/ezregex/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import re
 import colorsys
+import re
 
 foreground_s = .75
-foreground_v = 1
+foreground_v = 1.
 background_v_bias = .5
 background_s_bias = .9
 
 # These functions comprise the color algorithm
 def toHtml(r, g, b):
             return f'#{r:02x}{g:02x}{b:02x}'
 
 def toRgb(html: str) -> tuple:
     hex_color = html.lstrip('#')
     rgb = tuple(int(hex_color[i:i+2], 16) for i in (0, 2, 4))
     return rgb
 
-def generate_colors(amt, s=1, v=1, offset=0):
+def generate_colors(amt, s:float=1, v:float=1, offset:int=0):
     """ Generate `amt` number of colors evenly spaced around the color wheel
         with a given saturation and value
     """
     amt += 1
     return [toHtml(*map(lambda c: round(c*255), colorsys.hsv_to_rgb(*((offset + ((1/amt) * (i + 1))) % 1.001, s, v)))) for i in range(amt-1)]
 
-def furthest_colors(html, amt=5, v_bias=0, s_bias=0):
+def furthest_colors(html, amt:int=5, v_bias:float=0, s_bias:float=0):
     """ Gets the `amt` number of colors evenly spaced around the color wheel from the given color
         `v_bias` and `s_bias` are between 0-1 and offset the colors
     """
     amt += 1
     h, s, v = colorsys.rgb_to_hsv(*map(lambda c: c/255, toRgb(html)))
 
     return [toHtml(*map(lambda c: round(c*255), colorsys.hsv_to_rgb(*((h + ((1/amt) * (i + 1))) % 1.001, (s+s_bias) % 1.001, (v+v_bias) % 1.001)))) for i in range(amt-1)]
@@ -53,16 +53,26 @@
     allMatches = [m.span() for m in matches]
     # Map match spans to unique colors
     _colors = generate_colors(len(allMatches), s=foreground_s, v=foreground_v)
     matchColors = dict(zip(allMatches, _colors))
 
     for match in matches:
         allGroups = {match.span(i+1) for i in range(len(match.groups()))}
-        namedGroups = dict({(i, match.span(i)) for i in match.groupdict().keys()})
-        unnamedGroups = allGroups - set(namedGroups.values())
+        namedGroups = {i: match.span(i) for i in match.groupdict().keys()}
+        # TODO: have named groups show their name and number instead of just their name
+        # namedGroups = {
+        #     (cnt+1, ): match.span(cnt+1)
+        #     for cnt, i in enumerate(match.groups())
+        #     if i in match.groupdict().values()
+        # }
+        unnamedGroups = {
+            cnt+1: match.span(cnt+1)
+            for cnt, i in enumerate(match.groups())
+            if i not in match.groupdict().values()
+        }
         # Map group spans to unique colors
         # This gets equally spaced colors from the given color, so they're differentiable
         # and readable on a dark background
         colors = dict(zip(allGroups, furthest_colors(
             matchColors[match.span()],
             amt=len(allGroups),
             v_bias=background_v_bias,
@@ -101,25 +111,25 @@
                 'string': match.group(),
                 'string HTML': match_html,
                 'parts': match_parts,
                 'end': match.end(),
                 'start': match.start(),
                 "color": matchColors[match.span()],
             },
-            "unnamed groups":[],
+            "unnamed groups":{},
             "named groups":{},
         }
 
-        for i in range(len(unnamedGroups)):
-            match_json['unnamed groups'].append({
-                'string': match.group(i+1) or '',
-                'end': match.end(i+1),
-                'start': match.start(i+1),
-                "color": colors[match.span(i+1)],
-            })
+        for num, span in unnamedGroups.items():
+            match_json['unnamed groups'][num] = {
+                'string': match.group(num) or '',
+                'end': span[1],
+                'start': span[0],
+                "color": colors[span],
+            }
 
         for name, span in namedGroups.items():
             match_json['named groups'][name] = {
                 'string': match.group(name) or '',
                 'end': span[1],
                 'start': span[0],
                 "color": colors[span],
@@ -130,9 +140,11 @@
     html_string += test_string[globalCursor:]
     parts.append([None, None, test_string[globalCursor:]])
     html_string += '</span></p>'
     json['string HTML'] = html_string
     json['parts'] = parts
     if replacement_pattern is not None:
         json['replaced'] = re.sub(pattern.str(), replacement_pattern.str(), test_string, replacement_count)
+    else:
+        json['replaced'] = None
     json['split'] = re.split(pattern.str(), test_string, split_count)
     return json
```

### Comparing `ezregex-1.8.1/ezregex/api.pyi` & `ezregex-1.9.1/ezregex/api.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import TypedDict
+
 from ezregex.EZRegex import EZRegex
 
 Group = TypedDict(
     'Group',
     {
         'string': str,
         'end': int,
@@ -40,8 +41,14 @@
         'parts': list[list[str|None]],
         'matches': list[Matches],
         'replaced': str | None,
         'split': list[str] | None,
     }
 )
 
-def api(pattern:EZRegex, replacement_pattern:EZRegex|str|None=None, test_string:str|None=None, *, replacement_count:int=0, split_count:int=0) -> APIStructure: ...
+def api(
+    pattern:EZRegex,
+    replacement_pattern:EZRegex|str|None=None,
+    test_string:str|None=None, *,
+    replacement_count:int=0,
+    split_count:int=0
+) -> APIStructure: ...
```

### Comparing `ezregex-1.8.1/ezregex/generate.py` & `ezregex-1.9.1/ezregex/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 https://nbviewer.ipython.org/url/norvig.com/ipython/xkcd1313.ipynb
 and
 https://nbviewer.jupyter.org/url/norvig.com/ipython/xkcd1313-part2.ipynb
 (if the links don't work, try them through the wayback machine)
 Credit goes to Peter Norvig and Stefan Pochmann.
 """
 
-from collections import Counter, defaultdict
-import re
 import itertools
 import random
+import re
+from collections import Counter, defaultdict
 
 Set = frozenset # Data will be frozensets, so they can't be mutated.
 
 
 cat = ''.join  # Join a sequence of strings with nothing between them
 
 def OR(*regexes):
@@ -128,20 +128,20 @@
             covers.pop(best)
             # Try with and without the greedy-best part
             self.search({c:covers[c]-covered for c in covers}, OR(partial, best))
             self.search(covers, partial)
         return self.cheapest
 
 # TODO: Reimplement this eventually
-def consider_negative_lookahead(W, L):
-    "Return either SOLUTION[W, L] or negative lookup of SOLUTION[L, W], whichever is shorter."
-    solution = min(SOLUTION[W, L], '^(?!.*(' + SOLUTION[L, W] + '))',
-                   key=len)
-    assert not mistakes(solution, W, L)
-    return solution
+# def consider_negative_lookahead(W, L):
+#     "Return either SOLUTION[W, L] or negative lookup of SOLUTION[L, W], whichever is shorter."
+#     solution = min(SOLUTION[W, L], '^(?!.*(' + SOLUTION[L, W] + '))',
+#                    key=len)
+#     assert not mistakes(solution, W, L)
+#     return solution
 
 class BranchBoundRandomRestart(BranchBound):
     def search(self, covers, partial=None):
         """Recursively extend partial regex until it matches all winners in covers.
         Try all reasonable combinations until we run out of calls."""
         if self.calls <= 0:
             return partial, covers
```

### Comparing `ezregex-1.8.1/ezregex/invert.py` & `ezregex-1.9.1/ezregex/invert.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from typing import Literal, Union
 
 from random_word.services.local import Local
 
 from ezregex import *
 
 if version_info.minor <= 10:
-    from re import sre_parse as sre
+    from re import sre_parse as sre  # type: ignore
 else:
-    from re import _parser as sre
+    from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
 
 with open(Local().source) as f:
     words = json.load(f).keys()
@@ -86,25 +86,25 @@
         _tried = tries
 
     # If we get an error in the actual inversion part, just handle it as though
     # we generated a bad string that doesn't match, and continue recusing
     try:
         match backend:
             case 'xeger':
-                from xeger import Xeger
+                from xeger import Xeger  # type: ignore
                 rtn = Xeger().xeger(expr)
             case 'regex':
                 # Tries already gets implemented in this function
                 try:
                     rtn = invertRegex(expr, 1)
                 except NotImplementedError:
                     # Handle the error ourselves
                     rtn = None
             case 'sre_yield':
-                import sre_yield
+                import sre_yield  # type: ignore
                 for i in sre_yield.AllStrings(expr):
                     rtn = i
             case 're_parser':
                 groups = {}
                 def handle(pattern, amt=1, opposite=False):
                     if _verbose:
                         print(f'Handling {pattern} * {amt}')
```

### Comparing `ezregex-1.8.1/ezregex/invert_old.py` & `ezregex-1.9.1/ezregex/invert_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from copy import copy
 from dataclasses import dataclass
 from random import choice, choices, randint
 from warnings import warn
 
+
 def unsanitize(string):
     return re.sub(r'\\([' + re.escape(')([]{}+*$^-\\?| ,') + r'])', '\g<1>', string)
 
 def randbool():
     return bool(randint(0, 1))
 
 def _randWord(randomlyGenerate=False):
```

### Comparing `ezregex-1.8.1/ezregex/python/psuedonymns.py` & `ezregex-1.9.1/ezregex/javascript/psuedonymns.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 from .elements import *
 
-match_max = matchMax
-match_at_most = atMost = at_most = matchAtMost
-match_num = matchAmt = match_amt = amt = num = matchNum
-match_range = matchRange
-match_more_than = match_greater_than = matchGreaterThan = moreThan = more_than = matchMoreThan
-match_at_least = match_min = matchMin = atLeast = at_least = matchAtLeast
-line_starts_with = line_start = lineStart = lineStartsWith
-string_starts_with = string_start = stringStart = stringStartsWith
-line_ends_with = line_end = lineEnd = lineEndsWith
-string_ends_with = string_end = stringEnd = stringEndsWith
+matchMax = match_max
+matchAtMost = atMost = at_most = match_at_most
+matchNum = matchAmt = match_amt = amt = num = match_num
+matchRange = match_range
+matchMoreThan = match_greater_than = matchGreaterThan = moreThan = more_than = match_more_than
+matchAtLeast = match_min = matchMin = atLeast = at_least = match_at_least
+lineStartsWith = line_start = lineStart = line_starts_with
+stringStartsWith = string_start = stringStart = string_starts_with
+lineEndsWith = line_end = lineEnd = line_ends_with
+stringEndsWith = string_end = stringEnd = string_ends_with
 stuff      = chunk
 whiteChunk = whitechunk
 anychar    = anything
 anyChar    = anything
 char       = anything
 alpha      = letter
-alphanum   = alpha_num = alphaNum
+alphanum   = alpha_num = alpha_num
 white      = whitechunk
 
-anyAmt = any_amt = zeroOrMore = zero_or_more = atLeastNone
-any_between = anyBetween
-word_char = wordChar
-hex_digit = hex
-oct_digit = octDigit
-newline = newLine
-space_or_tab = spaceOrTab
-carriage_return = carriageReturn
-vertical_tab = verticalTab
-form_feed = formFeed
+anyAmt = any_amt = zeroOrMore = zero_or_more = at_least_none
+anyBetween = any_between
+wordChar = word_char
+hexDigit = hex
+octDigit = oct_digit
+newline = newLine = new_line
+spaceOrTab = space_or_tab
+carriageReturn = carriage_return
+verticalTab = vertical_tab
+formFeed = form_feed
 dot = period
 intOrFloat = int_or_float
-not_whitespace = notWhitespace
-not_digit = notDigit
-not_word = notWord
-anyof = any_of = oneOf = one_of = anyOf
-any_except = anyExcept
-any_char_except = anyCharExcept
-printable_and_space = printableAndSpace
-ifFollowedBy = if_followed_by = ifProcededBy
-if_exists = ifExists
-ifNotFollowedBy = if_not_followed_by = ifNotProcededBy
-if_preceded_by = ifPrecededBy
-if_not_preceded_by = ifNotPrecededBy
-if_enclosed_with = if_enclosed_by = ifEnclosedBy = ifEnclosedWith
-if_proceded_by = ifProcededBy
-if_not_proceded_by = ifNotProcededBy
-passive_group = passiveGroup
-named_group = namedGroup
-sameAs = same_as = earlier_group = sameAsGroup = same_as_group = earlierGroup
-exactly = is_exactly = isExactly
+notWhitespace = not_whitespace
+notDigit = not_digit
+notWord = not_word
+anyof = any_of = anyOf = oneOf = one_of = any_of
+anyExcept = any_except
+anyCharExcept = any_char_except
+printableAndSpace = printable_and_space
+ifFollowedBy = if_followed_by = if_proceded_by
+ifExists = if_exists
+ifNotFollowedBy = if_not_followed_by = if_not_proceded_by
+ifPrecededBy = if_preceded_by
+ifNotPrecededBy = if_not_preceded_by
+ifEnclosedWith = if_enclosed_by = ifEnclosedBy = if_enclosed_with
+ifProcededBy = if_proceded_by
+ifNotProcededBy = if_not_proceded_by
+passiveGroup = passive_group
+sameAs = same_as = earlierGroup = sameAsGroup = same_as_group = earlier_group
+exactly = isExactly = is_exactly
 oneOrNone = one_or_none = opt = optional
-oneOrMore = one_or_more = at_least_one = atLeast1 = at_least_1 = atLeastOne
-noneOrMore = none_or_more = at_least_none = at_least_0 = atLeast0 = atLeastNone
+oneOrMore = one_or_more = atLeastOne = atLeast1 = at_least_1 = at_least_one
+noneOrMore = none_or_more = atLeastNone = at_least_0 = atLeast0 = at_least_none
 ascii = a = ASCII
 dotall = s = DOTALL
 ignorecase = i = ignoreCase = ignore_case = IGNORECASE
 locale = L = LOCALE
 multiline = m = MULTILINE
-unicode = u = UNICODE
-# Useful Combinations
+# Useful combinations
 integer = signed
-literally_anything = literallyAnything
-word_boundary = wordBoundary
-not_word_boundary = notWordBoundary
+literallyAnything = literally_anything
+wordBoundary = word_boundary
+notWordBoundary = not_word_boundary
 
 replaceGroup = replace_group = rgroup
-replace_all = replaceAll = replace_entire = replaceEntire
+replaceAll = replace_all = replaceEntire = replace_entire
```

### Comparing `ezregex-1.8.1/tests/_groups.py` & `ezregex-1.9.1/tests/_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+
 # from builtins import __builtin__
 
 Set = frozenset # Data will be frozensets, so they can't be mutated.
 
 def words(text):
     "All space-separated words in text."
     return Set(text.split())
```

### Comparing `ezregex-1.8.1/tests/_regexs.py` & `ezregex-1.9.1/tests/_regexs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-
-import re
 from inspect import currentframe, getframeinfo
 
-from rich import print as rprint
-from rich.table import Table
-from rich.text import Text
+from _regexs import *
 
 import ezregex.python as er
-from ezregex.python import *
 from ezregex.invert import *
-
-import random
-
-from _regexs import *
-
+from ezregex.python import *
 
 # This goes (regex,                                                                         (things it should match),                                    (things it shouldnt match))
 _regexsLine = getframeinfo(currentframe()).lineno + 2
 regexs = (
     ('stuff' + ' ' + optional(comma) + space + ifFollowedBy('*'),                           ['stuff , *', 'stuff  *'],                                              None),
     ('stuff' + anyof('a', 'b', 'c') + ' ' + optional(comma) + space + ifFollowedBy('*'),    ['stuffa , *', 'stuffb  *'],                                            None),
     (anyof('a', 'b', 'c') + ' ' + optional(comma) + space + ifFollowedBy('*'),              ['a , *', 'b  *'],                                                      None),
@@ -99,15 +90,15 @@
     (whitespace,                                                                            (' ', '\t', '\t  ', '\n'),                                              ('dfsd',)),
     (whitechunk,                                                                            (' ', '\t', '\t  ', '\n'),                                              ('dfsd',)),
     (white,                                                                                 (' ', '\t', '\t  ', '\n'),                                              ('dfsd',)),
     (digit,                                                                                 ('6',),                                                                 ('_', '-', 'a')),
     (number,                                                                                ('6', '69'),                                                            ('-a', 'A')),
     (punctuation,                                                                           '@#$%^&*()'.split(),                                                    '12345678sdfsdf'.split()),
     (wordChar,                                                                              ('w',),                                                                 ('-',)),
-    (hexDigit,                                                                              ('A', 'a', '0'),                                                        ('g', 'G')),
+    (hex_digit,                                                                              ('A', 'a', '0'),                                                        ('g', 'G')),
     (octDigit,                                                                              ('7',),                                                                 ('9', 'a', 'A', '8')),
     (chunk,                                                                                 ('wordssdf   asdf\n',),                                                 ('\n',)),
     (spaceOrTab,                                                                            (' ', '\t', ' \t  '),                                                   ('\n',)),
     (newLine,                                                                               ('\n',),                                                                ('\r',)),
     (carriageReturn,                                                                        ('\r',),                                                                ('\n',)),
     (tab,                                                                                   ('\t',),                                                                (' ',)),
     (space,                                                                                 (' ',),                                                                 ('\t',)),
```

### Comparing `ezregex-1.8.1/tests/test_generate.py` & `ezregex-1.9.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/tests/testing_color_algorithm.ipynb` & `ezregex-1.9.1/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/tests/tests.py` & `ezregex-1.9.1/tests/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+import random
 import re
 from inspect import currentframe, getframeinfo
 
 from rich import print as rprint
 from rich.table import Table
 from rich.text import Text
+from test_generate import *
 
 import ezregex.python as er
-from ezregex.python import *
-from ezregex.invert import *
+from ezregex import api
 from ezregex.generate import *
-from test_generate import *
-
-import random
+from ezregex.invert import *
+from ezregex.python import *
 
 try:
     from Cope import debug
 except ImportError:
     pass
 
-from _regexs import *
 from _groups import *
-from _groups import _winners, _losers
+from _groups import _losers, _winners
+from _regexs import *
+from _regexs import _regexsLine
 
-from ezregex import api
 
-def runTests(singletons=True, _invert=True, replacement=True, _generate=True, testMethod=False, _api=False, operators=True, strictness=20, dontIncludePassed=True, invertBackend='re_parser', invert_tries=1):
+def runTests(singletons=True, _invert=True, replacement=True, _generate=True, testMethod=False, internal=False, operators=True, strictness=20, dontIncludePassed=True, invertBackend='re_parser', invert_tries=1):
     global ow
     if singletons:
         print("Testing EZRegex singletons...")
         # Test the various parameters of anyof()
         assert er.anyof('aiLmsux', split=True, chars=True)._compile(False) == "[aiLmsux]",                  f"Was supposed to be '[aiLmsux]', was actually '{er.anyof('aiLmsux', split=True, chars=True)._compile(False)}'"
         # assert er.anyof('aiLmsux', split=False, chars=True)._compile(False) == Error,                     f"Was supposed to be 'Error', was actually '{er.anyof('aiLmsux', split=False, chars=True)._compile(False)}'"
         assert er.anyof('aiLmsux', split=None, chars=True)._compile(False) == "[aiLmsux]",                  f"Was supposed to be '[aiLmsux]', was actually '{er.anyof('aiLmsux', split=None, chars=True)._compile(False)}'"
@@ -55,37 +55,37 @@
         # Test flags
         assert str(word + ASCII + stuff)      == r'(?a)\w+.+', fr"{word + ASCII + stuff}      != (?a)\w+.+"
         assert str(word) == r'\w+', f'{word}'
         assert str(word + DOTALL + stuff)     == r'(?s)\w+.+', fr"{word + DOTALL + stuff}     != (?s)\w+.+"
         assert str(word + IGNORECASE + stuff) == r'(?i)\w+.+', fr"{word + IGNORECASE + stuff} != (?i)\w+.+"
         assert str(word + LOCALE + stuff)     == r'(?L)\w+.+', fr"{word + LOCALE + stuff}     != (?L)\w+.+"
         assert str(word + MULTILINE + stuff)  == r'(?m)\w+.+', fr"{word + MULTILINE + stuff}  != (?m)\w+.+"
-        assert str(word + UNICODE + stuff)    == r'(?u)\w+.+', fr"{word + UNICODE + stuff}    != (?u)\w+.+"
+        # assert str(word + UNICODE + stuff)    == r'(?u)\w+.+', fr"{word + UNICODE + stuff}    != (?u)\w+.+"
 
         a = word + ow
-        b = stuff + UNICODE
+        # b = stuff + UNICODE
         c = IGNORECASE + '9'
-        assert a + b + c == word + ow + stuff + UNICODE + IGNORECASE + '9', f"{a + b + c} != {word + ow + stuff + UNICODE + IGNORECASE + '9'}"
+        assert a + c == word + ow + IGNORECASE + '9', f"{a + b + c} != {word + ow + IGNORECASE + '9'}"
 
         for cnt, r in enumerate(regexs):
             regex, match, dontMatch = r
             try:
                 if match is not None:
                     for m in match:
                         assert m in regex, f"{regex} does not match '{m}' (approx. {__file__}, line {_regexsLine+cnt})"
                 if dontMatch is not None:
                     for m in dontMatch:
                         assert m not in regex, f"{regex} DOES match '{m}' (approx. {__file__}, line {_regexsLine+cnt})"
             except Exception as err:
                 print(regex)
                 print(f'Error @ approx. {__file__}, line {_regexsLine+cnt}: \nregex = `{regex}`, match = `{match}`, dontMatch = `{dontMatch}`')
-                raise err.with_traceback(None)
+                raise err#.with_traceback(None)
 
-        a = str(EZRegex(r'\s+'))
-        b = str(EZRegex(raw(r'\s+')))
+        a = str(EZRegex(r'\s+', 'python'))
+        b = str(EZRegex(raw(r'\s+'), 'python'))
         c = r'\s+'
         d = str(raw(r'\s+'))
         # e = str(whitespace + matchMax)
         assert a == b == c == d, f'\na: {a}\n b: {b}\n c: {c}\n d: {d}\n e: {e}'
         # assert (word + ow + anything + ':').test('word    d:', show=False)
         # assert not (word + ow + anything + ':').test('word', show=False)
         assert 'word    d:' in (word + ow + anything + ':')
@@ -159,23 +159,23 @@
         # This is actually accurate, if you think about it.
         # ifFollowedBy(word).test("literal(hllow) + isExactly('thing')")# fails in _matchJSON()
 
         ('(' + +(anything + optional(group(comma))) + ')').test()# -- empty groups print as None
 
         group(+group(number) + group(anyof('98'))).test('999')
 
-    if _api:
+    if internal:
         # rprint((word + number)._matchJSON())
         # rprint((word + whitechunk + group('func') + ':' + namedGroup('test', anyof('8', '7')))._matchJSON())
-        rprint(api(ifFollowedBy(word)))
-        rprint(api(word))
-        rprint(api(number, test_string='word'))
+        rprint(ifFollowedBy(word)._matchJSON())
+        rprint(word._matchJSON())
+        rprint(number._matchJSON('word'))
         r = 'group 1' + ':' + ow + group('stuff') + ' | ' + 'group ' + number + ': ' + group('things') + ' | ' + 'named group "' + word + '": '  + named_group('foo', 'bar')
         s = 'random stuff! and then group 1: stuff | group 2: things | named group "foo": bar  \t oh and then more random stuff'
-        rprint(api(r, rgroup(1) + 'replaced', test_string=s))
+        rprint(r._matchJSON(s))
 
     if operators:
         print('Testing operators...')
         # The ~ operator
         for r in random.choices(regexs, k=strictness):
             regex, match, dontMatch = r
             assert re.search(regex.str(), ~regex), f"Invertting with ~ failed to find {regex} in {~regex}"
@@ -248,21 +248,21 @@
 
     print('All Tests Passed!')
 
 # From 1-100, 1 is easy, 100 is hard
 difficulty = 1
 runTests(
     # These should remain on, for the GitHub automated tests
-    singletons=False,
+    singletons=True,
     _invert=False,
-    replacement=False,
-    operators=False,
-    _generate=False,
+    replacement=True,
+    operators=True,
+    _generate=True,
     # These display for you to check that they look correct
     testMethod=False,
-    _api=True,
+    _api=False,
     # Settings
     strictness=difficulty,
     invert_tries=101-difficulty,
     dontIncludePassed=True,
     invertBackend='re_parser',
 )
```

### Comparing `ezregex-1.8.1/.gitignore` & `ezregex-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/LICENSE` & `ezregex-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.8.1/pyproject.toml` & `ezregex-1.9.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 python_version = ['3.10', '3.11', '3.12', 'pypy', 'pypy3']
 
 [tool.hatch.commands]
 prerelease = 'hatch build'
 
 [project]
 name = 'ezregex'
-version = '1.8.1'
+version = '1.9.1'
 description = 'A readable and intuitive way to generate Regular Expressions'
-dependencies = ['rich', 'random_word']
+dependencies = ['random_word']
 readme = "README.md"
 requires-python = ">=3.10"
```

