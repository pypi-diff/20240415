# Comparing `tmp/py-irclib-0.3.0.tar.gz` & `tmp/py_irclib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-irclib-0.3.0.tar", last modified: Sun Aug 18 23:38:28 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `py-irclib-0.3.0.tar` & `py_irclib-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 23:38:28.000000 py-irclib-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2019-08-18 23:38:28.000000 py-irclib-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      413 2019-08-18 23:37:58.000000 py-irclib-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-18 23:38:28.000000 py-irclib-0.3.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 23:38:28.000000 py-irclib-0.3.0/irclib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6221 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 23:38:28.000000 py-irclib-0.3.0/irclib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/util/frozendict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      386 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/util/compare.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6770 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/util/numerics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14862 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-08-18 23:37:58.000000 py-irclib-0.3.0/irclib/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 23:38:28.000000 py-irclib-0.3.0/py_irclib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2019-08-18 23:38:28.000000 py-irclib-0.3.0/py_irclib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-18 23:38:28.000000 py-irclib-0.3.0/py_irclib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-08-18 23:38:28.000000 py-irclib-0.3.0/py_irclib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-08-18 23:38:28.000000 py-irclib-0.3.0/py_irclib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      782 2019-08-18 23:37:58.000000 py-irclib-0.3.0/setup.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/errors.py
+-rw-r--r--   0        0        0    17084 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/py.typed
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/commands.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/compare.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/frozendict.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/numerics.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 py_irclib-0.4.0/irclib/util/string.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 py_irclib-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 py_irclib-0.4.0/LICENSE
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 py_irclib-0.4.0/README.md
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 py_irclib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 py_irclib-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-irclib-0.3.0/irclib/string.py` & `py_irclib-0.4.0/irclib/util/string.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,296 @@
-# coding=utf-8
 """
 IRC string utils
 """
+
 import operator
-from functools import wraps
+import string
+from typing import (
+    Callable,
+    Dict,
+    List,
+    NamedTuple,
+    Optional,
+    Protocol,
+    SupportsIndex,
+    Tuple,
+    Union,
+)
+
+__all__ = ("Casemap", "RFC1459", "STRICT_RFC1459", "ASCII", "String")
 
-__all__ = ('Casemap', 'RFC1459', 'STRICT_RFC1459', 'ASCII', 'String')
 
+class Casemap(NamedTuple):
+    """String case-map
 
-class Casemap(tuple):
-    __slots__ = ()
+    Represents a mapping of lower to upper case letters
+    """
 
-    def __new__(cls, lower, upper):
-        return tuple.__new__(cls, (lower, upper))
+    lower: str
+    upper: str
 
     @property
-    def lower_table(self):
+    def lower_table(self) -> Dict[int, int]:
+        """The lower->upper translation table"""
         return str.maketrans(self.lower, self.upper)
 
     @property
-    def upper_table(self):
+    def upper_table(self) -> Dict[int, int]:
+        """The upper->lower table"""
         return str.maketrans(self.upper, self.lower)
 
-    @property
-    def lower(self):
-        return self[0]
-
-    @property
-    def upper(self):
-        return self[1]
-
-
-RFC1459 = Casemap("".join(map(chr, range(65, 95))), "".join(map(chr, range(97, 127))))
-STRICT_RFC1459 = Casemap("".join(map(chr, range(65, 94))), "".join(map(chr, range(97, 126))))
-ASCII = Casemap("".join(map(chr, range(65, 91))), "".join(map(chr, range(97, 123))))
-
-sentinel = object()
-
-
-class cached_property:
-    def __init__(self, wrapped):
-        self.wrapped = wrapped
-        try:
-            self.__doc__ = wrapped.__doc__
-        except AttributeError:  # pragma: no cover
-            self.__doc__ = ""
-
-        self.name = wrapped.__name__
-
-    def __get__(self, inst, owner, _sentinel=sentinel):
-        if inst is None:
-            return self
 
-        val = inst._cache.get(self.name, _sentinel)
-        if val is not _sentinel:
-            return val
+RFC1459 = Casemap(
+    "".join(map(chr, range(65, 95))), "".join(map(chr, range(97, 127)))
+)
+STRICT_RFC1459 = Casemap(
+    "".join(map(chr, range(65, 94))), "".join(map(chr, range(97, 126)))
+)
+ASCII = Casemap(
+    "".join(map(chr, range(65, 91))), "".join(map(chr, range(97, 123)))
+)
 
-        inst._cache[self.name] = val = self.wrapped(inst)
-        return val
 
-    def __set__(self, inst, value):
-        raise AttributeError("cached property is read-only")
-
-
-class cached_method(cached_property):
-    def __get__(self, inst, owner, _sentinel=sentinel):
-        return lambda: cached_property.__get__(self, inst, owner, _sentinel)
-
-
-def type_wrap(super_index, wrap_out=True):
-    def _decorate(func):
-        @wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(args[super_index], String):
-                args = list(args)
-                args[super_index] = self._wrap(args[super_index])
-
-            if wrap_out:
-                return self._wrap(func(self, *args, **kwargs))
+class TranslateTable(Protocol):
+    def __getitem__(self, item: int, /) -> Union[str, int, None]:
+        raise NotImplementedError
 
-            return func(self, *args, **kwargs)
 
-        return wrapper
+class String(str):
+    """Case-insensitive string"""
 
-    return lambda func: _decorate(func)
+    __slots__ = ("_casemap",)
 
+    _casemap: Casemap
 
-class String(str):
-    __slots__ = ("_casemap", "_cache")
+    def _wrap(self, value: str) -> "String":
+        return self.__class__.__new__(self.__class__, value, self.casemap)
 
-    def _wrap(self, value):
-        return self.__class__(value, self.casemap)
+    def __new__(
+        cls, value: str = "", casemap: Optional[Casemap] = None
+    ) -> "String":
+        o = str.__new__(cls, value)
+        o._casemap = casemap or ASCII  # noqa: SLF001
+        return o
 
-    @cached_method
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(str(self.lower()))
 
-    def __new__(cls, value='', casemap=None):
-        return str.__new__(cls, value)
-
-    def __init__(self, value='', casemap=None):
-        super().__init__()
-        self._cache = dict(casemap=casemap)
-
-    def __internal_cmp(self, other, cmp):
+    def __internal_cmp(
+        self, other: object, cmp: Callable[[str, str], bool]
+    ) -> bool:
         if isinstance(other, String):
             return cmp(str(self.casefold()), str(other.casefold()))
 
-        return cmp(self, self._wrap(other))
+        if isinstance(other, str):
+            return cmp(self, self._wrap(other))
+
+        return NotImplemented
 
-    def __lt__(self, other):
+    def __lt__(self, other: str) -> bool:
         return self.__internal_cmp(other, operator.lt)
 
-    def __le__(self, other):
+    def __le__(self, other: str) -> bool:
         return self.__internal_cmp(other, operator.le)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return self.__internal_cmp(other, operator.eq)
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return self.__internal_cmp(other, operator.ne)
 
-    def __gt__(self, other):
+    def __gt__(self, other: str) -> bool:
         return self.__internal_cmp(other, operator.gt)
 
-    def __ge__(self, other):
+    def __ge__(self, other: str) -> bool:
         return self.__internal_cmp(other, operator.ge)
 
-    @type_wrap(0, False)
-    def __contains__(self, item):
-        return item.casefold() in str(self.casefold())
+    def __contains__(self, item: object) -> bool:
+        if not isinstance(item, str):
+            return False
 
-    def __getitem__(self, item):
+        return self._wrap(item).casefold() in str(self.casefold())
+
+    def __getitem__(self, item: Union[SupportsIndex, slice]) -> "String":
         return self._wrap(super().__getitem__(item))
 
-    def translate(self, table):
+    def translate(self, table: TranslateTable) -> "String":
         return self._wrap(super().translate(table))
 
-    @cached_method
-    def capitalize(self):
+    @property
+    def _capitalize(self) -> "String":
         return self[:1].upper() + self[1:].lower()
 
-    @cached_method
-    def casefold(self):
+    def __add__(self, other: str) -> "String":
+        return self._wrap(str(self) + other)
+
+    def capitalize(self) -> "String":
+        return self._capitalize
+
+    @property
+    def _casefold(self) -> "String":
         return self.lower()
 
-    @cached_method
-    def lower(self):
+    def casefold(self) -> "String":
+        return self._casefold
+
+    @property
+    def _lower(self) -> "String":
         return self.translate(self.casemap.lower_table)
 
-    @cached_method
-    def upper(self):
+    def lower(self) -> "String":
+        return self._lower
+
+    @property
+    def _upper(self) -> "String":
         return self.translate(self.casemap.upper_table)
 
-    @type_wrap(0)
-    def count(self, c, start=None, end=None):
-        return str(self.casefold()).count(c.casefold(), start, end)
-
-    @type_wrap(0)
-    def startswith(self, prefix, start=None, end=None):
-        return str(self.casefold()).startswith(prefix.lower(), start, end)
-
-    @type_wrap(0)
-    def endswith(self, suffix, start=None, end=None):
-        return str(self.casefold()).endswith(suffix.casefold(), start, end)
-
-    @type_wrap(0)
-    def find(self, sub, start=None, end=None):
-        return str(self.casefold()).find(sub.casefold(), start, end)
-
-    @type_wrap(0)
-    def rfind(self, sub, start=None, end=None):
-        return str(self.casefold()).rfind(sub.casefold(), start, end)
-
-    @type_wrap(0)
-    def index(self, sub, start=None, end=None):
-        return str(self.casefold()).index(sub.casefold(), start, end)
-
-    @type_wrap(0)
-    def rindex(self, sub, start=None, end=None):
-        return str(self.casefold()).rindex(sub.casefold(), start, end)
+    def upper(self) -> "String":
+        return self._upper
 
-    @type_wrap(0, False)
-    def partition(self, sep):
+    def count(
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> int:
+        return str(self.casefold()).count(
+            self._wrap(sub).casefold(), start, end
+        )
+
+    def startswith(
+        self,
+        prefix: Union[str, Tuple[str, ...]],
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> bool:
+        prefix_list: Tuple[str, ...]
+        prefix_list = (prefix,) if isinstance(prefix, str) else prefix
+
+        mapped_list = tuple(self._wrap(p).casefold() for p in prefix_list)
+
+        return str(self.casefold()).startswith(mapped_list, start, end)
+
+    def endswith(
+        self,
+        suffix: Union[str, Tuple[str, ...]],
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> bool:
+        suffix_list: Tuple[str, ...]
+        suffix_list = (suffix,) if isinstance(suffix, str) else suffix
+
+        mapped_list = tuple(self._wrap(p).casefold() for p in suffix_list)
+
+        return str(self.casefold()).endswith(mapped_list, start, end)
+
+    def find(
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> int:
+        return str(self.casefold()).find(self._wrap(sub).casefold(), start, end)
+
+    def rfind(
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> int:
+        return str(self.casefold()).rfind(
+            self._wrap(sub).casefold(), start, end
+        )
+
+    def index(
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> int:
+        return str(self.casefold()).index(
+            self._wrap(sub).casefold(), start, end
+        )
+
+    def rindex(
+        self,
+        sub: str,
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
+    ) -> int:
+        return str(self.casefold()).rindex(
+            self._wrap(sub).casefold(), start, end
+        )
+
+    def partition(self, sep: str) -> Tuple["String", "String", "String"]:
         pos = self.find(sep)
         if pos < 0:
             return self, self._wrap(""), self._wrap("")
 
-        return self[:pos], self[pos:pos + len(sep)], self[pos + len(sep):]
+        return self[:pos], self[pos : pos + len(sep)], self[pos + len(sep) :]
 
-    @type_wrap(0, False)
-    def rpartition(self, sep):
+    def rpartition(self, sep: str) -> Tuple["String", "String", "String"]:
         pos = self.rfind(sep)
         if pos < 0:
             return self._wrap(""), self._wrap(""), self
 
-        return self[:pos], self[pos:pos + len(sep)], self[pos + len(sep):]
+        return self[:pos], self[pos : pos + len(sep)], self[pos + len(sep) :]
 
-    def replace(self, old, new, count=-1):
+    def replace(
+        self, old: str, new: str, count: SupportsIndex = -1
+    ) -> "String":
         raise NotImplementedError
 
-    def strip(self, chars=None):
+    def strip(self, chars: Optional[str] = None) -> "String":
         return self.lstrip(chars).rstrip(chars)
 
-    def lstrip(self, chars=None):
-        raise NotImplementedError
+    def lstrip(self, chars: Optional[str] = None) -> "String":
+        if chars is None:
+            chars = string.whitespace
 
-    def rstrip(self, chars=None):
-        raise NotImplementedError
+        chars = self._wrap(chars)
+
+        start = 0
+        while start < len(self) and self[start] in chars:
+            start += 1
+
+        return self[start:]
+
+    def rstrip(self, chars: Optional[str] = None) -> "String":
+        if chars is None:
+            chars = string.whitespace
+
+        chars = self._wrap(chars)
 
-    @cached_method
-    def swapcase(self):
-        tr = self.casemap.lower_table + self.casemap.upper_table
+        end = len(self)
+        while end > 0 and self[end - 1] in chars:
+            end -= 1
 
-        return self.translate(tr)
+        return self[:end]
 
-    def title(self):
+    @property
+    def _swapcase(self) -> "String":
+        trans = self.casemap.lower_table.copy()
+        trans.update(self.casemap.upper_table)
+
+        return self.translate(trans)
+
+    def swapcase(self) -> "String":
+        return self._swapcase
+
+    def title(self) -> str:
         raise NotImplementedError
 
-    def split(self, sep=None, maxsplit=-1):
+    def split(
+        self, sep: Optional[str] = None, maxsplit: SupportsIndex = -1
+    ) -> List[str]:
         raise NotImplementedError
 
-    def rsplit(self, sep=None, maxsplit=-1):
+    def rsplit(
+        self, sep: Optional[str] = None, maxsplit: SupportsIndex = -1
+    ) -> List[str]:
         raise NotImplementedError
 
-    @cached_property
-    def casemap(self):
-        raise RuntimeError("String.casefold property not properly cached")
+    @property
+    def casemap(self) -> Casemap:
+        """Casemap associated with this string"""
+        return self._casemap
```

### Comparing `py-irclib-0.3.0/irclib/parser.py` & `py_irclib-0.4.0/irclib/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,279 +2,291 @@
 Simple IRC line parser
 
 Backported from async-irc (https://github.com/snoonetIRC/async-irc.git)
 """
 
 import re
 from abc import ABCMeta, abstractmethod
+from typing import (
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
+
+from typing_extensions import Self
 
 from irclib.errors import ParseError
 
 __all__ = (
-    'Cap', 'CapList', 'MessageTag', 'TagList', 'Prefix', 'ParamList', 'Message'
+    "Cap",
+    "CapList",
+    "MessageTag",
+    "TagList",
+    "Prefix",
+    "ParamList",
+    "Message",
 )
+MsgTagList = Optional["TagList"]
+MsgPrefix = Optional["Prefix"]
+MessageTuple = Tuple[MsgTagList, MsgPrefix, str, "ParamList"]
+
+TAGS_SENTINEL = "@"
+TAGS_SEP = ";"
+TAG_VALUE_SEP = "="
+
+PREFIX_SENTINEL = ":"
+PREFIX_USER_SEP = "!"
+PREFIX_HOST_SEP = "@"
 
-TAGS_SENTINEL = '@'
-TAGS_SEP = ';'
-TAG_VALUE_SEP = '='
-
-PREFIX_SENTINEL = ':'
-PREFIX_USER_SEP = '!'
-PREFIX_HOST_SEP = '@'
+PARAM_SEP = " "
+TRAIL_SENTINEL = ":"
 
-PARAM_SEP = ' '
-TRAIL_SENTINEL = ':'
+CAP_SEP = " "
+CAP_VALUE_SEP = "="
 
-CAP_SEP = ' '
-CAP_VALUE_SEP = '='
-
-PREFIX_RE = re.compile(r'^:?(?P<nick>.*?)(?:!(?P<user>.*?))?(?:@(?P<host>.*?))?$')
+PREFIX_RE = re.compile(
+    r"^:?(?P<nick>.*?)(?:!(?P<user>.*?))?(?:@(?P<host>.*?))?$"
+)
 
 TAG_VALUE_ESCAPES = {
-    '\\s': ' ',
-    '\\:': ';',
-    '\\r': '\r',
-    '\\n': '\n',
-    '\\\\': '\\',
+    "\\s": " ",
+    "\\:": ";",
+    "\\r": "\r",
+    "\\n": "\n",
+    "\\\\": "\\",
 }
 
 TAG_VALUE_UNESCAPES = {
-    unescaped: escaped
-    for escaped, unescaped in TAG_VALUE_ESCAPES.items()
+    unescaped: escaped for escaped, unescaped in TAG_VALUE_ESCAPES.items()
 }
 
+SelfT = TypeVar("SelfT")
+
 
 class Parseable(metaclass=ABCMeta):
     """Abstract class for parseable objects"""
 
     @abstractmethod
-    def __str__(self):
+    def __str__(self) -> str:
         raise NotImplementedError
 
-    @staticmethod
+    @classmethod
     @abstractmethod
-    def parse(text):
-        """Parse the object from a string
-        :type text: str
-        """
+    def parse(cls, text: str) -> Self:
+        """Parse the object from a string"""
         raise NotImplementedError
 
 
 class Cap(Parseable):
     """Represents a CAP entity as defined in IRCv3.2"""
 
-    def __init__(self, name, value=None):
+    def __init__(self, name: str, value: Optional[str] = None) -> None:
         self._name = name
         self._value = value
 
     @property
-    def name(self):
+    def name(self) -> str:
+        """CAP name"""
         return self._name
 
     @property
-    def value(self):
+    def value(self) -> Optional[str]:
+        """CAP value"""
         return self._value
 
-    @property
-    def _data(self):
+    def as_tuple(self) -> Tuple[str, Optional[str]]:
+        """Get data as a tuple of values"""
         return self.name, self.value
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
             return self == self.parse(other)
 
         if isinstance(other, Cap):
-            return tuple(self) == tuple(other)
+            return self.as_tuple() == other.as_tuple()
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, str):
             return self != self.parse(other)
 
         if isinstance(other, Cap):
-            return tuple(self) != tuple(other)
+            return self.as_tuple() != other.as_tuple()
 
         return NotImplemented
 
-    def __str__(self):
-        """
-        :rtype: str
-        """
+    def __str__(self) -> str:
         if self.value:
-            return CAP_VALUE_SEP.join(self)
+            return CAP_VALUE_SEP.join((self.name, self.value))
 
         return self.name
 
-    def __iter__(self):
-        """
-        Allow unpacking as a tuple
-        """
-        return iter(self._data)
-
-    @staticmethod
-    def parse(text):
-        """Parse a CAP entity from a string
-        :type text: str
-        """
+    @classmethod
+    def parse(cls, text: str) -> "Cap":
+        """Parse a CAP entity from a string"""
         name, _, value = text.partition(CAP_VALUE_SEP)
         return Cap(name, value or None)
 
 
-class CapList(Parseable, list):
+class CapList(Parseable, List[Cap]):
     """Represents a list of CAP entities"""
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
             return self == self.parse(other)
 
         if isinstance(other, list):
             return list(self) == list(other)
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, str):
             return self != self.parse(other)
 
         if isinstance(other, list):
             return list(self) != list(other)
 
         return NotImplemented
 
-    def __str__(self):
-        """
-        :rtype: str
-        """
+    def __str__(self) -> str:
         return CAP_SEP.join(map(str, self))
 
-    @staticmethod
-    def parse(text):
-        """Parse a list of CAPs from a string
-        :type text: str
-        """
-        if text.startswith(':'):
+    @classmethod
+    def parse(cls, text: str) -> "CapList":
+        """Parse a list of CAPs from a string"""
+        if text.startswith(":"):
             text = text[1:]  # Remove leading colon
 
         # We want to strip any leading or trailing whitespace
         # Some networks (ie: freenode) send a trailing space in a CAP ACK
         stripped = text.strip()
 
-        if not text:
-            caps = []
-        else:
-            caps = (
-                Cap.parse(s)
-                for s in stripped.split(CAP_SEP)
-            )
+        caps: Iterable[Cap]
+        caps = (
+            [] if not text else (Cap.parse(s) for s in stripped.split(CAP_SEP))
+        )
 
         return CapList(caps)
 
 
 class MessageTag(Parseable):
     """
     Basic class to wrap a message tag
     """
 
-    def __init__(self, name, value=None):
+    def __init__(
+        self, name: str, value: str = "", *, has_value: bool = False
+    ) -> None:
         self._name = name
-        self._value = value
+        self._value = value or ""
+        self._has_value = has_value
 
     @property
-    def name(self):
+    def name(self) -> str:
+        """Message tag name"""
         return self._name
 
     @property
-    def value(self):
+    def value(self) -> str:
+        """Message tag value"""
         return self._value
 
-    def __iter__(self):
-        return iter((self.name, self.value))
-
     @staticmethod
-    def unescape(value):
+    def unescape(value: str) -> str:
         """
         Replace the escaped characters in a tag value with their literals
+
         :param value: Escaped string
         :return: Unescaped string
         """
         new_value = ""
         escaped = False
-        for i, c in enumerate(value):
+        for char in value:
             if escaped:
-                new_value += TAG_VALUE_ESCAPES.get('\\{}'.format(c), c)
+                new_value += TAG_VALUE_ESCAPES.get(f"\\{char}", char)
                 escaped = False
-            elif c == '\\':
+            elif char == "\\":
                 escaped = True
             else:
-                new_value += c
+                new_value += char
 
         return new_value
 
     @staticmethod
-    def escape(value):
+    def escape(value: str) -> str:
         """
         Replace characters with their escaped variants
+
         :param value: The raw string
         :return: The escaped string
         """
         return "".join(TAG_VALUE_UNESCAPES.get(c, c) for c in value)
 
-    def __str__(self):
-        if self.value:
-            return "{}{}{}".format(
-                self.name, TAG_VALUE_SEP, self.escape(self.value)
-            )
+    def __repr__(self) -> str:
+        return f"MessageTag(name={self.name!r}, value={self.value!r})"
+
+    def __str__(self) -> str:
+        if self.value or self._has_value:
+            return f"{self.name}{TAG_VALUE_SEP}{self.escape(self.value)}"
 
         return self.name
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
             return self == self.parse(other)
 
         if isinstance(other, MessageTag):
-            return tuple(self) == tuple(other)
+            return self.name == other.name and self.value == other.value
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, str):
             return self != self.parse(other)
 
         if isinstance(other, MessageTag):
-            return tuple(self) != tuple(other)
+            return not (self.name == other.name and self.value == other.value)
 
         return NotImplemented
 
-    @staticmethod
-    def parse(text):
+    @classmethod
+    def parse(cls, text: str) -> "MessageTag":
         """
         Parse a tag from a string
-        :type text: str
+
         :param text: The basic tag string
         :return: The MessageTag object
         """
         name, sep, value = text.partition(TAG_VALUE_SEP)
         if value:
             value = MessageTag.unescape(value)
 
-        return MessageTag(name, value if sep else None)
+        return MessageTag(name, value, has_value=bool(sep))
 
 
-class TagList(Parseable, dict):
+class TagList(Parseable, Dict[str, MessageTag]):
     """Object representing the list of message tags on a line"""
 
-    def __init__(self, tags=()):
+    def __init__(self, tags: Iterable[MessageTag] = ()) -> None:
         super().__init__((tag.name, tag) for tag in tags)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return TAGS_SEP.join(map(str, self.values()))
 
     @staticmethod
-    def _cmp_type_map(obj):
+    def _cmp_type_map(obj: object) -> Dict[str, MessageTag]:
         if isinstance(obj, str):
             return TagList.parse(obj)
 
         if isinstance(obj, dict):
             sample = next(iter(obj.values()), None)
             if obj and (sample is None or isinstance(sample, str)):
                 # Handle str -> str dict
@@ -284,200 +296,215 @@
             return dict(obj)
 
         if isinstance(obj, list):
             return TagList(obj)
 
         return NotImplemented
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         obj = self._cmp_type_map(other)
         if obj is NotImplemented:
             return NotImplemented
 
         return dict(self) == dict(obj)
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         obj = self._cmp_type_map(other)
         if obj is NotImplemented:
             return NotImplemented
 
         return dict(self) != dict(obj)
 
-    @staticmethod
-    def parse(text):
+    @classmethod
+    def parse(cls, text: str) -> "TagList":
         """
         Parse the list of tags from a string
-        :type text: str
+
         :param text: The string to parse
         :return: The parsed object
         """
         return TagList(
             map(MessageTag.parse, filter(None, text.split(TAGS_SEP)))
         )
 
     @staticmethod
-    def from_dict(tags):
-        return TagList(
-            MessageTag(k, v) for k, v in tags.items()
-        )
+    def from_dict(tags: Dict[str, str]) -> "TagList":
+        """Create a TagList from a dict of tags"""
+        return TagList(MessageTag(k, v) for k, v in tags.items())
 
 
 class Prefix(Parseable):
     """
     Object representing the prefix of a line
     """
 
-    def __init__(self, nick=None, user=None, host=None):
-        self._nick = nick or ''
-        self._user = user or ''
-        self._host = host or ''
+    def __init__(
+        self,
+        nick: Optional[str] = None,
+        user: Optional[str] = None,
+        host: Optional[str] = None,
+    ) -> None:
+        self._nick = nick or ""
+        self._user = user or ""
+        self._host = host or ""
 
     @property
-    def nick(self):
+    def nick(self) -> str:
+        """IRC nickname"""
         return self._nick
 
     @property
-    def user(self):
+    def user(self) -> str:
+        """IRC ident/username"""
         return self._user
 
     @property
-    def ident(self):
-        return self._user
+    def ident(self) -> str:
+        """IRC ident. Alias for `user`."""
+        return self.user
 
     @property
-    def host(self):
+    def host(self) -> str:
+        """Hostname"""
         return self._host
 
     @property
-    def mask(self):
+    def mask(self) -> str:
         """
         The complete n!u@h mask
         """
         mask = self.nick
         if self.user:
             mask += PREFIX_USER_SEP + self.user
 
         if self.host:
             mask += PREFIX_HOST_SEP + self.host
 
         return mask
 
     @property
-    def _data(self):
+    def _data(self) -> Tuple[str, str, str]:
         return self.nick, self.user, self.host
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         return iter(self._data)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.mask
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return any(self)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
             return self == self.parse(other)
 
         if isinstance(other, Prefix):
             return self._data == other._data
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, str):
             return self != self.parse(other)
 
         if isinstance(other, Prefix):
             return self._data != other._data
 
         return NotImplemented
 
-    @staticmethod
-    def parse(text):
+    @classmethod
+    def parse(cls, text: str) -> "Prefix":
         """
         Parse the prefix from a string
-        :type text: str
+
         :param text: String to parse
         :return: Parsed Object
         """
         if not text:
             return Prefix()
 
         match = PREFIX_RE.match(text)
         if not match:  # pragma: no cover
             # This should never trip, we are pretty lenient with prefixes
-            raise ParseError("Invalid IRC prefix format")
+            msg = "Invalid IRC prefix format"
+            raise ParseError(msg)
 
         nick, user, host = match.groups()
         return Prefix(nick, user, host)
 
 
-class ParamList(Parseable, list):
+class ParamList(Parseable, List[str]):
     """
     An object representing the parameter list from a line
     """
 
-    def __init__(self, *params, has_trail=False):
+    def __init__(self, *params: str, has_trail: bool = False) -> None:
         super().__init__(params)
         self._has_trail = has_trail
 
     @property
-    def has_trail(self):
+    def has_trail(self) -> bool:
+        """Does the parameter list end with a trailing parameter"""
         return self._has_trail
 
-    def __str__(self):
+    def __str__(self) -> str:
         if not self:
-            return ''
+            return ""
 
-        needs_trail = PARAM_SEP in self[-1] or self[-1].startswith(TRAIL_SENTINEL) or not self[-1]
+        needs_trail = (
+            PARAM_SEP in self[-1]
+            or self[-1].startswith(TRAIL_SENTINEL)
+            or not self[-1]
+        )
 
         if self.has_trail or needs_trail:
             return PARAM_SEP.join(self[:-1] + [TRAIL_SENTINEL + self[-1]])
 
         return PARAM_SEP.join(self)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
             return self == self.parse(other)
 
         if isinstance(other, list):
             return list(self) == list(self.from_list(other))
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, str):
             return self != self.parse(other)
 
         if isinstance(other, list):
             return list(self) != list(other)
 
         return NotImplemented
 
     @staticmethod
-    def from_list(data):
+    def from_list(data: Sequence[str]) -> "ParamList":
+        """Create a ParamList from a Sequence of strings."""
         if not data:
             return ParamList()
 
         args = list(data[:-1])
         if data[-1].startswith(TRAIL_SENTINEL) or not data[-1]:
             has_trail = True
             args.append(data[-1])
         else:
             has_trail = False
             args.append(data[-1])
 
         return ParamList(*args, has_trail=has_trail)
 
-    @staticmethod
-    def parse(text):
+    @classmethod
+    def parse(cls, text: str) -> "ParamList":
         """
         Parse a list of parameters
-        :type text: str
+
         :param text: The list of parameters
         :return: The parsed object
         """
         args = []
         has_trail = False
         while text:
             if text[0] == TRAIL_SENTINEL:
@@ -488,119 +515,147 @@
             arg, _, text = text.partition(PARAM_SEP)
             if arg:
                 args.append(arg)
 
         return ParamList(*args, has_trail=has_trail)
 
 
+def _parse_tags(
+    tags: Union[TagList, Dict[str, str], str, None, List[str]],
+) -> MsgTagList:
+    if isinstance(tags, TagList):
+        return tags
+
+    if isinstance(tags, dict):
+        return TagList.from_dict(cast(Dict[str, str], tags))
+
+    if isinstance(tags, str):
+        return TagList.parse(tags)
+
+    if tags is None:
+        return None
+
+    return TagList(MessageTag.parse(str(tag)) for tag in tags)
+
+
+def _parse_prefix(prefix: Union[Prefix, str, None, Iterable[str]]) -> MsgPrefix:
+    if isinstance(prefix, Prefix):
+        return prefix
+
+    if isinstance(prefix, str):
+        return Prefix.parse(prefix)
+
+    if prefix is None:
+        return None
+
+    return Prefix(*prefix)
+
+
+def _parse_params(
+    parameters: Tuple[Union[str, List[str], ParamList], ...],
+) -> ParamList:
+    if len(parameters) == 1 and not isinstance(parameters[0], str):
+        # This seems to be a list
+        if isinstance(parameters[0], ParamList):
+            return parameters[0]
+
+        return ParamList.from_list(parameters[0])
+
+    return ParamList.from_list(cast(Tuple[str, ...], parameters))
+
+
 class Message(Parseable):
     """
     An object representing a parsed IRC line
     """
 
-    def __init__(self, tags, prefix, command, *parameters):
-        if isinstance(tags, TagList):
-            self._tags = tags
-        elif isinstance(tags, dict):
-            self._tags = TagList.from_dict(tags)
-        elif isinstance(tags, str):
-            self._tags = TagList.parse(tags)
-        elif tags is None:
-            self._tags = None
-        else:
-            self._tags = TagList(MessageTag.parse(str(tag)) for tag in tags)
-
-        if isinstance(prefix, Prefix):
-            self._prefix = prefix
-        elif isinstance(prefix, str):
-            self._prefix = Prefix.parse(prefix)
-        elif prefix is None:
-            self._prefix = None
-        else:
-            self._prefix = Prefix(*prefix)
-
+    def __init__(
+        self,
+        tags: Union[TagList, Dict[str, str], str, None, List[str]],
+        prefix: Union[str, Prefix, None, Iterable[str]],
+        command: str,
+        *parameters: Union[str, List[str], ParamList],
+    ) -> None:
+        self._tags = _parse_tags(tags)
+        self._prefix = _parse_prefix(prefix)
         self._command = command
-
-        if len(parameters) == 1 and not isinstance(parameters[0], str):
-            # This seems to be a list
-            if isinstance(parameters[0], ParamList):
-                self._parameters = parameters[0]
-            else:
-                self._parameters = ParamList.from_list(parameters[0])
-        else:
-            self._parameters = ParamList.from_list(parameters)
+        self._parameters = _parse_params(parameters)
 
     @property
-    def tags(self):
+    def tags(self) -> MsgTagList:
+        """IRC tag list"""
         return self._tags
 
     @property
-    def prefix(self):
+    def prefix(self) -> MsgPrefix:
+        """IRC prefix"""
         return self._prefix
 
     @property
-    def command(self):
+    def command(self) -> str:
+        """IRC command"""
         return self._command
 
     @property
-    def parameters(self):
+    def parameters(self) -> ParamList:
+        """Command parameter list"""
         return self._parameters
 
-    def __iter__(self):
-        return iter((self.tags, self.prefix, self.command, self.parameters))
-
-    def __str__(self):
-        tag_str = '' if self.tags is None else TAGS_SENTINEL + str(self.tags)
-        prefix_str = '' if self.prefix is None else PREFIX_SENTINEL + str(self.prefix)
+    def as_tuple(self) -> MessageTuple:
+        """Get the message object as a tuple of values"""
+        return self.tags, self.prefix, self.command, self.parameters
+
+    def __str__(self) -> str:
+        tag_str = "" if self.tags is None else TAGS_SENTINEL + str(self.tags)
+        prefix_str = (
+            "" if self.prefix is None else PREFIX_SENTINEL + str(self.prefix)
+        )
 
         return PARAM_SEP.join(
-            str(s) for s in (
-                tag_str, prefix_str, self.command, self.parameters
-            )
+            str(s)
+            for s in (tag_str, prefix_str, self.command, self.parameters)
             if s
         )
 
-    def __bool__(self):
-        return any(self)
+    def __bool__(self) -> bool:
+        return any(self.as_tuple())
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, (str, bytes)):
             return self == Message.parse(other)
 
         if isinstance(other, Message):
-            return tuple(self) == tuple(other)
+            return self.as_tuple() == other.as_tuple()
 
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         if isinstance(other, (str, bytes)):
             return self != Message.parse(other)
 
         if isinstance(other, Message):
-            return tuple(self) != tuple(other)
+            return self.as_tuple() != other.as_tuple()
 
         return NotImplemented
 
-    @staticmethod
-    def parse(text):
-        """Parse an IRC message in to objects
-        :type text: str
-        """
+    @classmethod
+    def parse(cls, text: Union[str, bytes]) -> "Message":
+        """Parse an IRC message in to objects"""
         if isinstance(text, bytes):
             text = text.decode(errors="ignore")
 
-        tags = ''
-        prefix = ''
+        tags = ""
+        prefix = ""
         if text.startswith(TAGS_SENTINEL):
             tags, _, text = text.partition(PARAM_SEP)
 
         if text.startswith(PREFIX_SENTINEL):
             prefix, _, text = text.partition(PARAM_SEP)
 
         command, _, params = text.partition(PARAM_SEP)
         # Differentiate empty tags '@ CMD' from no tags 'CMD'
-        tags = TagList.parse(tags[1:]) if tags else None
+        tags_obj = TagList.parse(tags[1:]) if tags else None
         # Differentiate empty prefix ': CMD' from no prefix 'CMD'
-        prefix = Prefix.parse(prefix[1:]) if prefix else None
+        prefix_obj = Prefix.parse(prefix[1:]) if prefix else None
         command = command.upper()
-        params = ParamList.parse(params)
-        return Message(tags, prefix, command, params)
+        param_obj = ParamList.parse(params)
+        return Message(tags_obj, prefix_obj, command, param_obj)
```

