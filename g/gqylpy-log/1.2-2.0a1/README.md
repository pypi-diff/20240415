# Comparing `tmp/gqylpy_log-1.2.tar.gz` & `tmp/gqylpy_log-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_log-1.2.tar", last modified: Fri Feb  9 10:05:32 2024, max compression
+gzip compressed data, was "gqylpy_log-2.0a1.tar", last modified: Mon Apr 15 00:53:09 2024, max compression
```

## Comparing `gqylpy_log-1.2.tar` & `gqylpy_log-2.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:05:32.907374 gqylpy_log-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-02-09 10:05:16.000000 gqylpy_log-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-09 10:05:32.907374 gqylpy_log-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-09 10:05:16.000000 gqylpy_log-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:05:32.907374 gqylpy_log-1.2/gqylpy_log/
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-02-09 10:05:16.000000 gqylpy_log-1.2/gqylpy_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-09 10:05:16.000000 gqylpy_log-1.2/gqylpy_log/g log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:05:32.907374 gqylpy_log-1.2/gqylpy_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-09 10:05:32.000000 gqylpy_log-1.2/gqylpy_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-09 10:05:32.000000 gqylpy_log-1.2/gqylpy_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 10:05:32.000000 gqylpy_log-1.2/gqylpy_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-09 10:05:32.000000 gqylpy_log-1.2/gqylpy_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 10:05:32.907374 gqylpy_log-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-09 10:05:16.000000 gqylpy_log-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/gqylpy_log/
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/gqylpy_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/gqylpy_log/g log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/gqylpy_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/setup.py
```

### Comparing `gqylpy_log-1.2/LICENSE` & `gqylpy_log-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_log-1.2/gqylpy_log/g log.py` & `gqylpy_log-2.0a1/gqylpy_log/g log.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,101 +13,156 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys
 import logging
 
-from typing import TypeVar, Optional, Literal, Callable, Union
+from logging import handlers as logging_handlers
 
-Logger     = TypeVar("Logger", str, logging.Logger)
-Closure    = TypeVar("Closure", bound=Callable)
-OutputMode = Literal["stream", "file", "stream,file"]
+from types import ModuleType
 
-__first__: logging.Logger
+from typing import (
+    TypeVar, Type, Final, Optional, TypedDict, Union, Callable, Mapping, Dict,
+    List, Any
+)
 
-gpack = sys.modules[__package__]
-gcode = sys.modules[__name__]
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+else:
+    class Annotated(metaclass=type('', (type,), {
+        '__new__': lambda *a: type.__new__(*a)()
+    })):
+        def __getitem__(self, *a): ...
+
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    TypeAlias = TypeVar("TypeAlias")
+
+Logger:  TypeAlias = TypeVar("Logger", str, logging.Logger)
+Level:   TypeAlias = TypeVar("Level", int, str)
+Closure: TypeAlias = TypeVar("Closure", bound=Callable)
+
+
+class DictFormatter(TypedDict, total=False):
+    fmt:      str
+    datefmt:  str
+    style:    str
+    validate: bool
+
+    if sys.version_info >= (3, 10):
+        defaults: Mapping[str, Any]
+
+
+class Options(TypedDict, total=False):
+    onlyRecordCurrentLevel: bool
+
+
+Formatter: TypeAlias = Union[DictFormatter, logging.Formatter]
+
+Filter: TypeAlias = Union[
+    Callable[[logging.LogRecord], bool], logging.Filter, logging.Filterer
+]
+
+Handler: TypeAlias = Union[Dict[str, Any], logging.Handler]
+
+default: Annotated[logging.Logger, "built-in default logger"]
+
+gpack: Final[ModuleType] = sys.modules[__package__]
+gcode: Final[ModuleType] = sys.modules[__name__]
+
+logging_handlers.Handler       = logging.Handler
+logging_handlers.StreamHandler = logging.StreamHandler
+logging_handlers.FileHandler   = logging.FileHandler
 
 
 def __init__(
-        name:    str,
+        name:      str,
         *,
-        level:   Union[int, str] = "NOTSET",
-        output:  OutputMode      = "stream",
-        logfmt:  Optional[str]   = None,
-        datefmt: Optional[str]   = None,
-        logfile: Optional[str]   = None,
-        gname:   Optional[str]   = None
+        level:     Level         = 0,
+        formatter: Formatter     = logging.Formatter(),
+        filters:   List[Filter]  = [],
+        options:   Options       = {},
+        handlers:  List[Handler] = [],
+        gname:     Optional[str] = None
 ) -> logging.Logger:
-    if output.replace(" ", "") not in \
-            ("stream", "file", "stream,file", "file,stream"):
-        raise TypeError(
-            "parameter 'output' can only be 'stream', 'file', or "
-            f"'stream,file', not '{output}'."
-        )
+    logger = logging.Logger(name, level)
 
-    logger    = logging.Logger(name, level)
-    formatter = logging.Formatter(logfmt, datefmt)
+    if formatter.__class__ is dict:
+        formatter = logging.Formatter(**formatter)
 
-    if "stream" in output:
-        handler = logging.StreamHandler()
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
+    for handler_or_params in handlers:
+        if isinstance(handler_or_params, logging.Handler):
+            logger.addHandler(handler_or_params)
+            continue
+
+        if "formatter" in handler_or_params:
+            the_formatter: Formatter = handler_or_params.pop("formatter")
+            if the_formatter.__class__ is dict:
+                the_formatter = logging.Formatter(**the_formatter)
+        else:
+            the_formatter = formatter
 
-    if "file" in output:
-        if logfile is None:
-            starter: str = os.path.basename(sys.argv[0])
-            logfile: str = f"/var/log/{starter[:-3]}.log"
+        the_level:   Level         = handler_or_params.pop("level", level)
+        the_filters: List[Filter]  = handler_or_params.pop("filters", filters)
+        the_options: Options       = handler_or_params.pop("options", options)
+
+        handler_type: Type[logging.Handler] = \
+            getattr(logging_handlers, handler_or_params.pop("name"))
+
+        if issubclass(handler_type, logging.FileHandler):
+            filename: str = handler_or_params["filename"]
+            logdir:   str = os.path.dirname(os.path.abspath(filename))
+            os.makedirs(logdir, exist_ok=True)
+
+        handler: logging.Handler = handler_type(**handler_or_params)
+        handler.setLevel(the_level)
+        handler.setFormatter(the_formatter)
+        handler.filters.extend(
+            x for x in the_filters if x not in handler.filters
+        )
 
-        logdir: str = os.path.dirname(os.path.abspath(logfile))
-        os.path.isdir(logdir) or os.makedirs(logdir)
+        if the_options.get("onlyRecordCurrentLevel"):
+            handler.addFilter(only_record_current_level(handler.level))
 
-        handler = logging.FileHandler(logfile, encoding="utf8")
-        handler.setFormatter(formatter)
         logger.addHandler(handler)
 
     if gname:
-        if not hasattr(gcode, "__first__") or \
-                gcode.__first__.name == "builtin":
-            gcode.__first__ = logger
+        if not hasattr(gcode, "default") or gcode.default.name == "default":
+            gcode.default = logger
         setattr(gpack, gname, logger)
 
     return logger
 
 
+def only_record_current_level(
+        levelno: int
+) -> Callable[[logging.LogRecord], bool]:
+    return lambda record: record.levelno == levelno
+
+
 def __getattr__(method: str) -> Closure:
     if not hasattr(logging.Logger, method):
         raise AttributeError(
             f"module '{__package__}' has no attribute '{method}'"
         )
 
     def logger(
             *msg,
-            sep:     str           = " ",
-            oneline: bool          = False,
-            linesep: str           = "; ",
-            gname:   Union[Logger] = None,
+            sep:     str              = " ",
+            oneline: bool             = False,
+            linesep: str              = "; ",
+            gname:   Optional[Logger] = None,
             **kw
     ) -> None:
         if gname is None:
-            if not hasattr(gcode, "__first__"):
-                gobj: logging.Logger = __init__(
-                    name="builtin",
-                    level=gpack.level,
-                    output=gpack.output,
-                    logfmt=gpack.logfmt,
-                    datefmt=gpack.datefmt,
-                    **({"logfile": gpack.logfile} if gpack.logfile !=
-                        "/var/log/{default is your startup filename}.log"
-                       else {}),
-                    gname="builtin"
-                )
-                setattr(gcode, "__first__", gobj)
-            gobj: logging.Logger = __first__
+            if not hasattr(gcode, "default"):
+                __init__("default", **gpack.default, gname="default")
+            gobj: logging.Logger = default
         elif gname.__class__ is str:
             gobj: logging.Logger = getattr(gpack, gname, None)
             if gobj.__class__ is not logging.Logger:
                 raise NameError(f"gname '{gname}' not in '{__package__}'.")
         elif gname.__class__ is logging.Logger:
             gobj: logging.Logger = gname
         else:
```

### Comparing `gqylpy_log-1.2/setup.py` & `gqylpy_log-2.0a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,20 +14,24 @@
     name=g.__name__,
     version=version,
     author=author,
     author_email=email,
     license="Apache 2.0",
     url="http://gqylpy.com",
     project_urls={"Source": source},
-    description="二次封装 logging，更方便快捷的创建日志记录器。使用 gqylpy_log 模块可以"
-                "快速创建 logging.Logger 实例并完成一系列的日志配置，使你的代码更简洁。",
+    description="""
+        Secondary encapsulation `logging`, more convenient and fast to create
+        the logger. Use this module can quickly create instances of
+        `logging.Logger` and complete a series of log configuration,make your
+        code cleaner.
+    """,
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     packages=[g.__name__],
-    python_requires=">=3.8, <4",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: Chinese (Simplified)",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -35,10 +39,11 @@
         "Topic :: Artistic Software",
         "Topic :: Internet :: Log Analysis",
         "Topic :: Text Processing",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12"
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13"
     ]
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

