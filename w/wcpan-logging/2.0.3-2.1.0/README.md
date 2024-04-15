# Comparing `tmp/wcpan_logging-2.0.3.tar.gz` & `tmp/wcpan_logging-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcpan_logging-2.0.3.tar", max compression
+gzip compressed data, was "wcpan_logging-2.1.0.tar", max compression
```

## Comparing `wcpan_logging-2.0.3.tar` & `wcpan_logging-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2023-03-11 01:17:55.637995 wcpan_logging-2.0.3/LICENSE.txt
--rw-r--r--   0        0        0      416 2023-03-12 03:26:11.579014 wcpan_logging-2.0.3/README.md
--rw-r--r--   0        0        0      721 2023-12-09 06:48:27.547579 wcpan_logging-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      170 2023-12-09 06:38:18.377577 wcpan_logging-2.0.3/wcpan/logging/__init__.py
--rw-r--r--   0        0        0     2398 2023-12-09 06:46:14.337579 wcpan_logging-2.0.3/wcpan/logging/builder.py
--rw-r--r--   0        0        0      351 2023-03-11 01:17:55.637995 wcpan_logging-2.0.3/wcpan/logging/const.py
--rw-r--r--   0        0        0     2253 2023-03-11 01:17:55.637995 wcpan_logging-2.0.3/wcpan/logging/formatter.py
--rw-r--r--   0        0        0        0 2023-12-09 06:40:01.327579 wcpan_logging-2.0.3/wcpan/logging/py.typed
--rw-r--r--   0        0        0      370 2023-03-11 01:17:55.637995 wcpan_logging-2.0.3/wcpan/logging/types.py
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 wcpan_logging-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-03-11 01:17:55.637995 wcpan_logging-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      416 2024-04-14 15:47:32.511542 wcpan_logging-2.1.0/README.md
+-rw-r--r--   0        0        0      726 2024-04-15 02:28:18.191540 wcpan_logging-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-15 02:21:55.901540 wcpan_logging-2.1.0/wcpan/logging/__init__.py
+-rw-r--r--   0        0        0     2548 2024-04-15 02:28:06.561540 wcpan_logging-2.1.0/wcpan/logging/builder.py
+-rw-r--r--   0        0        0      351 2024-04-15 02:21:55.901540 wcpan_logging-2.1.0/wcpan/logging/const.py
+-rw-r--r--   0        0        0     2253 2024-04-15 02:21:55.901540 wcpan_logging-2.1.0/wcpan/logging/formatter.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:47:32.511542 wcpan_logging-2.1.0/wcpan/logging/py.typed
+-rw-r--r--   0        0        0      370 2024-04-15 02:21:55.901540 wcpan_logging-2.1.0/wcpan/logging/types.py
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 wcpan_logging-2.1.0/PKG-INFO
```

### Comparing `wcpan_logging-2.0.3/LICENSE.txt` & `wcpan_logging-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wcpan_logging-2.0.3/pyproject.toml` & `wcpan_logging-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wcpan-logging"
-version = "2.0.3"
+version = "2.1.0"
 description = "Configuration generator for builtin logging module."
 authors = ["Wei-Cheng Pan <legnaleurc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legnaleurc/wcpan.logging"
 packages = [{include = "wcpan"}]
 classifiers = [
@@ -16,12 +16,12 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = ">=23.1,<25.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wcpan_logging-2.0.3/wcpan/logging/builder.py` & `wcpan_logging-2.1.0/wcpan/logging/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 class ConfigBuilder:
     def __init__(
         self,
         *,
         level: LevelName | None = None,
         path: StrPath | None = None,
         rotate: bool = False,
+        rotate_when: str = "h",
         processes: bool = False,
         threads: bool = False
     ) -> None:
         self._level: LevelName | None = level
         self._path = path
         self._rotate = rotate
+        self._rotate_when = rotate_when
         self._processes = processes
         self._threads = threads
         self._loggers: dict[str, LevelName | None] = {}
 
     def add(self, *names: str, level: LevelName | None = None) -> Self:
         for name in names:
             self._loggers[name] = level
         return self
 
     def to_dict(self) -> AnyDict:
-        handler = create_handler(path=self._path, rotate=self._rotate)
+        handler = create_handler(
+            path=self._path, rotate=self._rotate, rotate_when=self._rotate_when
+        )
         handler["formatter"] = FORMATTER_ID
         root = create_root(level=self._level)
         root["handlers"] = [HANDLER_ID]
         return {
             "version": 1,
             "formatters": {
                 FORMATTER_ID: {
@@ -55,24 +59,24 @@
 def create_root(*, level: LevelName | None) -> AnyDict:
     root: AnyDict = {}
     if level:
         root["level"] = LEVEL_TABLE[level]
     return root
 
 
-def create_handler(*, path: StrPath | None, rotate: bool) -> AnyDict:
+def create_handler(*, path: StrPath | None, rotate: bool, rotate_when: str) -> AnyDict:
     if not path:
         return {
             "class": "logging.StreamHandler",
         }
     elif rotate:
         return {
             "class": "logging.handlers.TimedRotatingFileHandler",
             "filename": str(path),
-            "when": "w6",
+            "when": rotate_when,
         }
     else:
         return {
             "class": "logging.FileHandler",
             "filename": str(path),
         }
```

### Comparing `wcpan_logging-2.0.3/wcpan/logging/formatter.py` & `wcpan_logging-2.1.0/wcpan/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `wcpan_logging-2.0.3/PKG-INFO` & `wcpan_logging-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcpan-logging
-Version: 2.0.3
+Version: 2.1.0
 Summary: Configuration generator for builtin logging module.
 Home-page: https://github.com/legnaleurc/wcpan.logging
 License: MIT
 Author: Wei-Cheng Pan
 Author-email: legnaleurc@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

