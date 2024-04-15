# Comparing `tmp/itakello_logging-0.1.8.tar.gz` & `tmp/itakello_logging-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itakello_logging-0.1.8.tar", last modified: Thu Mar 28 22:41:29 2024, max compression
+gzip compressed data, was "itakello_logging-0.2.0.tar", last modified: Mon Apr 15 11:07:52 2024, max compression
```

## Comparing `itakello_logging-0.1.8.tar` & `itakello_logging-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.600225 itakello_logging-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 22:41:29.600225 itakello_logging-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/itakello_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/itakello_logging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/filters/custom_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/filters/ignore_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/itakello_logging/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/formatters/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/itakello_logging/test_logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 22:41:15.000000 itakello_logging-0.1.8/src/itakello_logging/test_logs/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 22:41:29.596225 itakello_logging-0.1.8/src/itakello_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-28 22:41:29.000000 itakello_logging-0.1.8/src/itakello_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 22:41:29.000000 itakello_logging-0.1.8/src/itakello_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 22:41:29.000000 itakello_logging-0.1.8/src/itakello_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 22:41:29.000000 itakello_logging-0.1.8/src/itakello_logging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.992027 itakello_logging-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/custom_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/ignore_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/formatters/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/loggers/confirmation_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/test_logs/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/top_level.txt
```

### Comparing `itakello_logging-0.1.8/LICENSE` & `itakello_logging-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.1.8/PKG-INFO` & `itakello_logging-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.1.8
+Version: 0.2.0
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.1.8/README.md` & `itakello_logging-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.1.8/setup.py` & `itakello_logging-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="itakello_logging",
-    version="0.1.8",
+    version="0.2.0",
     author="Itakello",
     author_email="maxste000@gmail.com",
     description="A custom logging library by Itakello",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Itakello/itakello_logging",
     package_dir={"": "src"},
```

### Comparing `itakello_logging-0.1.8/src/itakello_logging/core.py` & `itakello_logging-0.2.0/src/itakello_logging/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import pathlib
 from dataclasses import dataclass, field
 from datetime import datetime
+from typing import cast
 
 from .filters import CustomExcludeFilter, IgnoreRootFilter
 from .formatters import ConsoleFormatter
+from .loggers import ConfirmationLogger
 
 
 @dataclass
 class ItakelloLogging:
 
     debug_mode: bool = field(init=False)
     handlers: list[logging.Handler] = field(init=False)
@@ -16,19 +18,24 @@
 
     def __init__(
         self,
         excluded_modules: list[str] = [],
         debug: bool = False,
         exclude_root: bool = False,
     ) -> None:
+        logging.setLoggerClass(ConfirmationLogger)
         self.debug_mode = debug
         self.folder = self._create_folder("logs")
         handlers = self._get_handlers(excluded_modules, exclude_root)
         logging.basicConfig(level=logging.DEBUG, handlers=handlers, force=True)
 
+    @staticmethod
+    def get_logger(name: str) -> ConfirmationLogger:
+        return cast(ConfirmationLogger, logging.getLogger(name))
+
     def _create_folder(self, f_name: str) -> pathlib.Path:
         folder = pathlib.Path(f_name)
         folder.mkdir(exist_ok=True, parents=True)
         return folder
 
     def _get_handlers(
         self, excluded_loggers: list[str], exclude_root: bool
@@ -60,15 +67,15 @@
         )
         s_handler.setFormatter(console_formatter)
         return s_handler
 
     def _get_file_handler(self) -> logging.FileHandler:
         current_time = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         f_handler = logging.FileHandler(self.folder / f"{current_time}.log")
-        f_handler.setLevel(logging.DEBUG if self.debug_mode else logging.INFO)
+        f_handler.setLevel(logging.DEBUG)
         f_handler.setFormatter(
             logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         )
         return f_handler
 
 
 if __name__ == "__main__":
@@ -76,14 +83,15 @@
 
     ItakelloLogging(debug=True, excluded_modules=[], exclude_root=False)
     logging.debug("Test debug message from core.py with root logger")
     logging.info("Test info message from core.py with root logger")
     logging.warning("Test warning message from core.py with root logger")
     logging.error("Test error message from core.py with root logger")
     logging.critical("Test critical message from core.py with root logger")
-    logger = logging.getLogger(__name__)
+    logger = ItakelloLogging.get_logger(__name__)
     logger.debug("Test debug message from core.py with custom logger")
     logger.info("Test info message from core.py with custom logger")
+    logger.confirmation("Test confirmation message from core.py with custom logger")
     logger.warning("Test warning message from core.py with custom logger")
     logger.error("Test error message from core.py with custom logger")
     logger.critical("Test critical message from core.py with custom logger")
     test_func()
```

### Comparing `itakello_logging-0.1.8/src/itakello_logging.egg-info/PKG-INFO` & `itakello_logging-0.2.0/src/itakello_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.1.8
+Version: 0.2.0
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.1.8/src/itakello_logging.egg-info/SOURCES.txt` & `itakello_logging-0.2.0/src/itakello_logging.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 src/itakello_logging.egg-info/dependency_links.txt
 src/itakello_logging.egg-info/top_level.txt
 src/itakello_logging/filters/__init__.py
 src/itakello_logging/filters/custom_exclude.py
 src/itakello_logging/filters/ignore_root.py
 src/itakello_logging/formatters/__init__.py
 src/itakello_logging/formatters/console.py
+src/itakello_logging/loggers/__init__.py
+src/itakello_logging/loggers/confirmation_logger.py
 src/itakello_logging/test_logs/__init__.py
 src/itakello_logging/test_logs/test_logs.py
```

