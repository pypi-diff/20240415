# Comparing `tmp/loggingpython-1.4.0.tar.gz` & `tmp/loggingpython-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.0.tar", last modified: Sun Apr  7 13:49:39 2024, max compression
+gzip compressed data, was "loggingpython-1.4.1.tar", last modified: Mon Apr 15 19:39:43 2024, max compression
```

## Comparing `loggingpython-1.4.0.tar` & `loggingpython-1.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.688949 loggingpython-1.4.0/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     3854 2024-04-07 13:49:39.687947 loggingpython-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2024-04-07 13:35:08.000000 loggingpython-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 13:49:39.688949 loggingpython-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1257 2024-04-07 13:34:41.000000 loggingpython-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.640448 loggingpython-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.648448 loggingpython-1.4.0/src/loggingpython/
--rw-rw-rw-   0        0        0     3689 2024-04-07 13:49:36.000000 loggingpython-1.4.0/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.678949 loggingpython-1.4.0/src/loggingpython/error/
--rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.0/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.0/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.0/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.0/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.0/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.0/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.0/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.685948 loggingpython-1.4.0/src/loggingpython/handler/
--rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.0/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     3992 2024-04-07 13:24:49.000000 loggingpython-1.4.0/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     4485 2024-04-07 13:12:35.000000 loggingpython-1.4.0/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     4393 2024-04-07 13:23:21.000000 loggingpython-1.4.0/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     1011 2024-04-07 13:13:28.000000 loggingpython-1.4.0/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     5508 2024-04-07 13:22:59.000000 loggingpython-1.4.0/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     5735 2024-04-07 13:22:38.000000 loggingpython-1.4.0/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    12754 2024-04-07 13:32:36.000000 loggingpython-1.4.0/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.0/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    16223 2024-04-05 13:07:38.000000 loggingpython-1.4.0/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.0/src/loggingpython/sys_procolls.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.686949 loggingpython-1.4.0/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3854 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.247328 loggingpython-1.4.1/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-15 19:39:43.246828 loggingpython-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 19:39:43.247829 loggingpython-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2024-04-15 19:39:35.000000 loggingpython-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.199828 loggingpython-1.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.208829 loggingpython-1.4.1/src/loggingpython/
+-rw-rw-rw-   0        0        0     3763 2024-04-15 19:39:30.000000 loggingpython-1.4.1/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.236828 loggingpython-1.4.1/src/loggingpython/error/
+-rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.1/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.1/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.1/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.1/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.1/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.1/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.1/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.243329 loggingpython-1.4.1/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.1/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     3422 2024-04-14 13:49:48.000000 loggingpython-1.4.1/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     3901 2024-04-14 16:01:40.000000 loggingpython-1.4.1/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     3777 2024-04-14 13:49:55.000000 loggingpython-1.4.1/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     1653 2024-04-14 13:50:01.000000 loggingpython-1.4.1/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     5518 2024-04-14 16:01:45.000000 loggingpython-1.4.1/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     4707 2024-04-14 16:03:19.000000 loggingpython-1.4.1/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    12186 2024-04-15 19:20:42.000000 loggingpython-1.4.1/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.1/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    16486 2024-04-14 14:44:12.000000 loggingpython-1.4.1/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.1/src/loggingpython/sys_procolls.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.244828 loggingpython-1.4.1/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/top_level.txt
```

### Comparing `loggingpython-1.4.0/LICENSE` & `loggingpython-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.0/README.md` & `loggingpython-1.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,82 @@
+Metadata-Version: 2.1
+Name: loggingpython
+Version: 1.4.1
+Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
+Home-page: https://github.com/loggingpython-Community/loggingpython
+Author: mrmajor.programmer
+Author-email: mrmajork.programmer@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Logging
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: colorama
+Requires-Dist: pandas
+
 # loggingpython
-## Version 1.4.0
 
-## This is not the whole new version, Docs still feel
+`loggingpython` is a Python library that provides a simple and extensible way to integrate logging into Python applications. In contrast to the standard logging library, `loggingpython` offers a completely independent implementation of handlers and loggers that have been specially developed for the requirements of modern applications.
 
-`loggingpython` is a Python package which provides a simple and extensible way to integrate logging into your applications. The package starts with a basic logger and can be extended with additional functions to meet the requirements of your application.
+## Features
 
----
+- **Simple Logger**: Begin with a basic logger and extend it with additional functions.
+- **Extensible**: Easily add more functionality to meet your application's logging needs.
+- **Customizable**: Tailor the logging system to your specific requirements.
 
 ## Installation
 
-### With pip
-
-For a simple installation via pip, run the following command:
+You can install `loggingpython` using pip:
 ```bash
 pip install loggingpython
 ```
 
-### With GitHub
-
-To install the latest development of `loggingpython` directly from the GitHub repository, follow these steps:
-
-1. Clone the repository:
+Alternatively, you can install the latest development version directly from GitHub:
 ```bash
 git clone https://github.com/loggingpython-Community/loggingpython.git
-```
-
-2. Change into the cloned directory:
-```bash
 cd loggingpython
-```
-
-3. Install the package:
-```bash
 pip install .
 ```
 
----
-
-## Simple Example
+## Quick start
 
-In this section, we show how to configure and use a basic logger with `loggingpython`. First, we import the package and create a logger:
+To use `loggingpython`, you first need to import the package and create a logger:
 ```python
 import loggingpython as lp
 
-# Create a basic logger
+# Create a simple logger with a file handler and a console handler
 logger = lp.getBasicLogger()
 ```
 
-This creates a logger with a Filehandler and a Consolehandler, the Consolehandler has colors in the message.
-
-Now, we can use the logger to generate various types of log messages:
-
+You can add various handlers to your logger to customize how log messages are handled:
 ```python
-# Logging messages at different levels
+# Log messages at different levels
 logger.debug("This is a debug message.")
 logger.info("This is an info message.")
 logger.warning("This is a warning.")
 logger.error("This is an error.")
 logger.critical("This is a critical error.")
-
-# Log message with an exception
-try:
-    1 / 0 
-except ZeroDivisionError as e:
-    logger.error(f"An exception occurred: {e}")
 ```
 
-The file handler saves the logs in the `logs/file.log` directory.
+## Contributing
 
-This example shows how to configure and use a basic logger to generate various types of log messages.
-
----
-
-We welcome your contributions to the development of loggingpython. If you have feedback, suggestions or would like to contribute to the development, please visit our [GitHub repository](https://github.com/loggingpython-Community/loggingpython) for more information. You can also find more details in our [wiki](https://github.com/loggingpython-Community/loggingpython/wiki) or in the folder `Docs`. For more detailed information, please also visit our package page on [PyPi](https://pypi.org/project/loggingpython).
-
----
+We welcome contributions to `loggingpython`. If you have feedback, suggestions, or would like to contribute, please visit our [GitHub repository](https://github.com/loggingpython-Community/loggingpython).
 
 ## License
 
 `loggingpython` is licensed under the [MIT License](https://opensource.org/licenses/MIT).
 
-## Further resources
+## Further Resources
 
+- [Documentation](https://github.com/loggingpython-Community/loggingpython/wiki)
 - [GitHub Repository](https://github.com/loggingpython-Community/loggingpython)
 - [Issue Tracker](https://github.com/loggingpython-Community/loggingpython/issues)
 - [Changelog](https://github.com/loggingpython-Community/loggingpython/blob/main/CHANGELOG.md)
 - [PyPi](https://pypi.org/project/loggingpython/)
 
-## Social media
+## Social Media
 
 - [GitHub](https://github.com/loggingpython-Community)
-
----
```

### Comparing `loggingpython-1.4.0/setup.py` & `loggingpython-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.0',
+    version='1.4.1',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.4.0/src/loggingpython/__init__.py` & `loggingpython-1.4.1/src/loggingpython/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .error.server_method_call_error import ServerMethodCallError
 from .error.client_method_call_error import ClientMethodCallError
 from .error.invalid_log_level_error import InvalidLogLevelError
 from .error.invalid_handler_method_error import InvalidHandlerMethodError
 from .error.handler_not_found_error import HandlerNotFoundError
 
 
-__version__ = "1.3.2"
+__version__ = "1.4.1"
 __all__ = [
     # Bacis
     "Logger",
 
     # Enum
     "LogLevel",
     "SysProtocolls",
@@ -60,30 +60,37 @@
 
 
 def hello_from_loggingpython() -> None:
     """
     Outputs a welcome message containing information about the
     loggingpython community.
     """
-    print(f"""Hello from the loggingpython-community.
+    print(f"""
+Hello from the loggingpython-community.
 We also use other libs, for a list of all libs look here: \
 https://github.com/loggingpython-Community/loggingpython/wiki/Lib-List
 Version: {__version__}
-PyPi: https://pypi.org/project/loggingpython
-GitHub: https://github.com/loggingpython-Community/loggingpython""")
+GitHub: https://github.com/loggingpython-Community/loggingpython
+""")
 
 
-def getLogger(name: str = "Root-Logger") -> Logger:
+def getLogger(name: str = "Root-Logger",
+              time_format: str = None,
+              min_loglevel: LogLevel = None,
+              max_loglevel: LogLevel = None) -> Logger:
     """
-        Creates and returns an instance of the logger.
+    Creates and returns an instance of the logger.
 
-        Returns:
-            Logger: An instance of the logger.
-        """
-    return Logger(name)
+    Returns:
+        Logger: An instance of the logger.
+    """
+    return Logger(name=name,
+                  time_format=time_format,
+                  min_loglevel=min_loglevel,
+                  max_loglevel=max_loglevel)
 
 
 def getBasicLogger() -> Logger:
     """
     Creates a logger with predefined handlers for file and console output.
         console output.
 
@@ -103,18 +110,16 @@
     Returns:
         dict: A dictionary where keys are the handler names and values are
             the handler classes.
     """
     handlers = {}
     for handler_name in __all__:
         if handler_name.endswith("Handler"):
-            # Adjust the module name to correctly resolve the import path
             module_name = f"{__name__}.handler.{handler_name.lower()}"
             try:
-                # Use importlib.import_module for dynamic import
                 handler_module = importlib.import_module(module_name)
                 handler_class = getattr(handler_module, handler_name)
                 handlers[handler_name] = handler_class
             except ModuleNotFoundError as e:
                 print(f"Failed to import {handler_name}: {e}")
     return handlers
```

### Comparing `loggingpython-1.4.0/src/loggingpython/error/__init__.py` & `loggingpython-1.4.1/src/loggingpython/error/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.0/src/loggingpython/error/invalid_handler_method_error.py` & `loggingpython-1.4.1/src/loggingpython/error/invalid_handler_method_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.1/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.1/src/loggingpython/handler/filehandler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from typing import TextIO
-from colorama import Fore, Style
-import sys
+import os
+from datetime import datetime
 
-from ..log_levels import LogLevel
 from .handler import Handler
 
 
-class ConsoleHandler(Handler):
+class FileHandler(Handler):
     """
-    A class for handling log messages in the console.
+    A class for handling log messages in files.
 
     This class inherits from the Handler class and implements specific
-    methods for formatting and outputting log messages in the console.
-    It supports the coloring of log messages based on their
-    severity and allows customization of the formatting string.
+    methods for formatting and outputting log messages to files. It supports
+    the creation of log files in a specified directory, automatic file rotation
+    based on the current date, and allows customization of the formatting
+    string. The FileHandler ensures that log messages are stored persistently
+    and can be reviewed later for debugging or auditing purposes.
     """
-
-    def __init__(self, stream: TextIO = sys.stdout,
+    def __init__(self, name: str, path: str = "logs",
                  logformat_string: str = "%(asctime)s: [%(loggername)s]: \
 [%(loglevel)s]: %(message)s") -> None:
         """
-        Initializes the ConsoleHandler with an optional stream and an optional
-        optional formatting string for log messages.
+        Initializes the FileHandler with the given name, log path, and log
+            format string.
 
         Args:
-            stream (TextIO, optional): The stream into which the log messages
-                are to be written. By default, this is sys.stdout.
-            logformat_string (str, optional): The formatting string for the
-                log messages. By default, it contains the timestamp,
-                logger name, log level and the message itself.
-        """
-        self.stream: TextIO = stream
-        self.logformat_string: str = logformat_string
+            name (str): The name of the log file.
+            path (str, optional): The path where the log files will be
+                stored. Defaults to "logs".
+            logformat_string (str, optional): The format string for the log
+                messages. Defaults to "%(asctime)s: [%(loggername)s]:
+                [%(loglevel)s]: %(message)s".
+        """
+        self._mk_logdir(path)
+        self.name: str = name
+        self.path: str = path
+        self._current_date: str = datetime.now().strftime("%Y-%m-%d")
+        self.file: str = f"{self.path}/{self.name}_{self._current_date}.log"
+        self._mk_logfile(self.file)
+        self.file = open(self.file, "a")
 
-        self.color_map: dict = {
-            LogLevel.DEBUG.name: Fore.GREEN,
-            LogLevel.INFO.name: Fore.CYAN,
-            LogLevel.WARNING.name: Fore.YELLOW,
-            LogLevel.ERROR.name: Fore.RED,
-            LogLevel.CRITICAL.name: Fore.MAGENTA,
-        }
+        self.logformat_string: str = logformat_string
 
     def emit(self, record: dict) -> None:
         """
-        Outputs a formatted log message based on the transferred
-        log data record log data set.
+        Writes a log record to the file.
 
         Args:
-            record (dict): A dictionary with the details of the log message,
-                including timestamp, logger name, log level and message.
+            record (dict): A dictionary containing the log record details.
         """
-        formatted_message = self._format_message(record)
-        color = self._get_color_for_level(record["loglevel"])
-        self.stream.write(color + formatted_message + Style.RESET_ALL + '\n')
-        self.stream.flush()
+        formatted_message_values = self._format_message(record)
+        formatted_message = self.logformat_string % formatted_message_values
 
-    def set_colors_for_levels(self, color_map: dict) -> None:
-        """
-        Sets colors for the different log levels.
+        self._update_file()
+        self.file.write(formatted_message + "\n")
+        self.file.flush()
 
-        Args:
-            color_map (dict): A dictionary that assigns log levels (as strings)
-                to the corresponding colors from colorama.
+    def _update_file(self) -> None:
         """
-        for level in color_map.keys():
-            if level not in LogLevel.__members__:
-                raise ValueError(f"Invalid log level: {level}")
+        Updates the log file if the current date has changed.
+        """
+        current_date = datetime.now().strftime("%Y-%m-%d")
+        if current_date != self._current_date:
+            self.current_date = current_date
+            self._close_file()
+            filename = f"{self.logpath}/{self.name}_{self._current_date}.log"
+            self.file = open(filename, "a")
 
-        self.color_map.update(color_map)
+    def _close_file(self) -> None:
+        """
+        Closes the current log file.
+        """
+        if self.file:
+            self.file.close()
 
-    def _get_color_for_level(self, loglevel: str) -> str:
+    def _mk_logdir(self, logpath: str) -> None:
         """
-        Returns the color for a specific log level.
+        Creates the log directory if it does not exist.
 
         Args:
-            loglevel (str): The log level for which the color is to
-                be retrieved.
-
-        Returns:
-            str: The color for the given log level.
+            logpath (str): The path of the log directory.
         """
-        return self.color_map.get(loglevel, Fore.WHITE)
+        if not os.path.exists(logpath):
+            os.makedirs(logpath)
 
-    def _format_message(self, record: dict) -> str:
+    def _mk_logfile(self, file: str) -> None:
         """
-        Formats a log message based on the transferred log data set.
+        Creates the log file if it does not exist.
 
         Args:
-            record (dict): A dictionary with the details of the log message.
+            file (str): The path of the log file.
+        """
+        if not os.path.exists(file):
+            os.open(file, os.O_CREAT)
 
-        Returns:
-            str: The formatted log message.
+    def _get_datestemp(self) -> str:
         """
-        values = {
-            "loggername": record.get("loggername", ""),
-            "iso_8601_time": record.get("iso_8601_time", ""),
-            "asctime": record.get("asctime", ""),
-            "loglevel": record.get("loglevel", ""),
-            "message": record.get("message", ""),
-        }
+        Returns the current date in the format "YYYY-MM-DD".
 
-        logformat_string = self.logformat_string
-        return logformat_string % values
+        Returns:
+            str: The current date.
+        """
+        return datetime.now().strftime("%Y-%m-%d")
 
     def __repr__(self) -> str:
-        return f"ConsoleHandler({self.name}, {self.logformat_string})"
+        return f"FileHandler({self.name}, {self.path}, \
+{self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"ConsoleHandler with: {self.name} and {self.logformat_string}"
+        return f"FileHandler with: {self.name}, {self.path} and \
+{self.logformat_string}"
```

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.1/src/loggingpython/handler/csvhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,22 @@
     def emit(self, record: dict) -> None:
         """
         Writes a log record to the file.
 
         Args:
             record (dict): A dictionary containing the log record details.
         """
-        formatted_message = self._format_message(record)
+        formatted_message_values = self._format_message(record)
+
+        df = pd.DataFrame([formatted_message_values])
+
+        formatted_message = df.to_csv(index=False, header=False, sep=";",
+                                      lineterminator="\n")
+
+        return formatted_message
         self._update_file()
         self.file.write(formatted_message)
         self.file.flush()
 
     def _update_file(self):
         """
         Updates the log file if the current date has changed.
@@ -96,38 +103,13 @@
         Returns the current date in the format "YYYY-MM-DD".
 
         Returns:
             str: The current date.
         """
         return datetime.now().strftime("%Y-%m-%d")
 
-    def _format_message(self, record: dict) -> str:
-        """
-        Formats a log message based on the provided log data.
-
-        Args:
-            record (dict): A dictionary containing the log message details.
-
-        Returns:
-            str: The formatted log message.
-        """
-        values = {
-            "loggername": record.get("loggername", ""),
-            "iso_8601_time": record.get("iso_8601_time", ""),
-            "asctime": record.get("asctime", ""),
-            "loglevel": record.get("loglevel", ""),
-            "message": record.get("message", ""),
-        }
-
-        df = pd.DataFrame([values])
-
-        formatted_message = df.to_csv(index=False, header=False, sep=";",
-                                      lineterminator="\n")
-
-        return formatted_message
-
     def __repr__(self) -> str:
         return f"CSVHandler({self.name}, {self.path}, {self.logformat_string})"
 
     def __str__(self) -> str:
         return f"CSVHandler with: {self.name}, {self.path} and \
 {self.logformat_string}"
```

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.1/src/loggingpython/handler/jsonhandler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 import os
+import json
 from datetime import datetime
 
 from .handler import Handler
 
 
-class FileHandler(Handler):
+class JSONHandler(Handler):
     """
-    A class for handling log messages in files.
+    A class for handling log messages in JSON format.
 
     This class inherits from the Handler class and implements specific
-    methods for formatting and outputting log messages to files. It supports
-    the creation of log files in a specified directory, automatic file rotation
-    based on the current date, and allows customization of the formatting
-    string. The FileHandler ensures that log messages are stored persistently
-    and can be reviewed later for debugging or auditing purposes.
+    methods for formatting and outputting log messages in JSON files. It
+    supports the creation of new log files based on the current date and
+    allows customization of the log format string. The JSONHandler ensures
+    that log messages are stored in a structured and easily accessible format,
+    making it suitable for further analysis or review. It also includes
+    features for hashing log messages for unique identification and updating
+    the log file if the current date has changed.
     """
-    def __init__(self, name: str, path: str = "logs",
-                 logformat_string: str = "%(asctime)s: [%(loggername)s]: \
-[%(loglevel)s]: %(message)s") -> None:
+    def __init__(self, name: str, path: str = "logs") -> None:
         """
-        Initializes the FileHandler with the given name, log path, and log
+        Initializes the JSONHandler with the given name, log path, and log
             format string.
 
         Args:
             name (str): The name of the log file.
             path (str, optional): The path where the log files will be
                 stored. Defaults to "logs".
             logformat_string (str, optional): The format string for the log
                 messages. Defaults to "%(asctime)s: [%(loggername)s]:
                 [%(loglevel)s]: %(message)s".
         """
         self._mk_logdir(path)
         self.name: str = name
         self.path: str = path
         self._current_date: str = datetime.now().strftime("%Y-%m-%d")
-        self.file: str = f"{self.path}/{self.name}_{self._current_date}.log"
+        self.file: str = f"{self.path}/{self.name}_{self._current_date}.json"
         self._mk_logfile(self.file)
-        self.file = open(self.file, "a")
-
-        self.logformat_string: str = logformat_string
+        self.log_data: dict[str, str] = {}
 
     def emit(self, record: dict) -> None:
         """
-        Writes a log record to the file.
-
+        Adds a log message to the JSON object and checks whether the
+            date has been changed.
         Args:
-            record (dict): A dictionary containing the log record details.
+            record (dict): A dictionary containing the details of the log
+                entry. contains the details of the log entry.
         """
-        formatted_message = self._format_message(record)
+        formatted_message_values = self._format_message(record)
+        formatted_message = self._format_in_json(formatted_message_values)
+        message_hash = hash(str(formatted_message))
+
+        self.log_data[str(message_hash)] = formatted_message
         self._update_file()
-        self.file.write(formatted_message + "\n")
-        self.file.flush()
+        self._write_log_data_to_file()
+
+    def _write_log_data_to_file(self) -> None:
+        """
+        Writes the JSON object to the file.
+        """
+        with open(self.file, 'w') as file:
+            file.write(json.dumps(self.log_data, indent=4))
 
     def _update_file(self) -> None:
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
-            self.current_date = current_date
+            self._current_date = current_date
             self._close_file()
-            filename = f"{self.logpath}/{self.name}_{self._current_date}.log"
-            self.file = open(filename, "a")
+            file: str = f"{self.path}/{self.name}_{self._current_date}.json"
+            self.file = open(file, "a")
+            self.log_data: dict[str, str] = {}
 
     def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
@@ -113,17 +124,35 @@
             "loggername": record.get("loggername", ""),
             "iso_8601_time": record.get("iso_8601_time", ""),
             "asctime": record.get("asctime", ""),
             "loglevel": record.get("loglevel", ""),
             "message": record.get("message", ""),
         }
 
-        logformat_string = self.logformat_string
-        return logformat_string % values
+        return values
+
+    def _format_in_json(self, record: dict) -> dict:
+        """
+        Formats a log message based on the provided log data into a JSON
+            object with hashed keys.
+
+        Args:
+            record (dict): A dictionary containing the log message details.
+
+        Returns:
+            dict: The formatted log message as a JSON object with hashed keys.
+        """
+        sorted_keys = sorted(record.keys())
+        string_representation = str({key: record[key] for key in sorted_keys})
+        message_hash = hash(string_representation)
+        values = {
+            message_hash: record,
+        }
+        return values
 
     def __repr__(self) -> str:
-        return f"FileHandler({self.name}, {self.path}, \
+        return f"JSONHandler({self.name}, {self.path}, \
 {self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"FileHandler with: {self.name}, {self.path} and \
+        return f"JSONHandler with: {self.name}, {self.path} and \
 {self.logformat_string}"
```

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.1/src/loggingpython/handler/sqlhandler.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,23 +42,21 @@
     def emit(self, record: dict) -> None:
         """
         Writes a log record to the database.
 
         Args:
             record (dict): A dictionary containing the log record details.
         """
-        # Extrahieren Sie die Werte aus dem Log-Record
         hash_message = hash(str(record))
         message = record.get("message", "")
         loglevel = record.get("loglevel", "")
         asctime = record.get("asctime", "")
         iso_8601_time = record.get("iso_8601_time", "")
         loggername = record.get("loggername", "")
 
-        # Fügen Sie die Log-Nachricht in die Datenbank ein
         with sqlite3.connect(self.file) as conn:
             cursor = conn.cursor()
             cursor.execute(
                 """
                 INSERT INTO logs (hash_message, message, loglevel, asctime, \
 iso_8601_time, loggername)
                 VALUES (?, ?, ?, ?, ?, ?)
@@ -87,20 +85,16 @@
     def _update_file(self) -> None:
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
             self._current_date = current_date
-            # Therefore, no explicit closing action is required here
-            # Update the file name for the new database file
             self.file = f"{self.path}/{self.name}_{self._current_date}.db"
-            # Create the new database file if it does not yet exist
             self._mk_logfile(self.file)
-            # Create the table in the new db file if it does not yet exist
             self._creat_db()
 
     def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
@@ -131,32 +125,12 @@
         Returns the current date in the format "YYYY-MM-DD".
 
         Returns:
             str: The current date.
         """
         return datetime.now().strftime("%Y-%m-%d")
 
-    def _format_message(self, record: dict) -> str:
-        """
-        Formats a log message based on the provided log data.
-
-        Args:
-            record (dict): A dictionary containing the log message details.
-
-        Returns:
-            str: The formatted log message.
-        """
-        values = {
-            "loggername": record.get("loggername", ""),
-            "iso_8601_time": record.get("iso_8601_time", ""),
-            "asctime": record.get("asctime", ""),
-            "loglevel": record.get("loglevel", ""),
-            "message": record.get("message", ""),
-        }
-
-        return values
-
     def __repr__(self) -> str:
         return f"SQLHandler({self.name}, {self.path})"
 
     def __str__(self) -> str:
         return f"SQLHandler with:{self.name} and {self.path}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `loggingpython-1.4.0/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.1/src/loggingpython/handler/syshandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import socket
 import json
 from functools import partial
 
-from ..logger import Logger
 from .handler import Handler
 from ..sys_procolls import SysProtocolls
 from ..error.server_unreachable_error import ServerUnreachableError
 from ..error.server_method_call_error import ServerMethodCallError
 from ..error.client_method_call_error import ClientMethodCallError
 
+
 class SysHandler(Handler):
     """
     A class for handling log messages over a network connection.
 
     This class inherits from the Handler class and implements specific methods
     for sending and receiving log messages over a network connection. It
     supports both client and server modes, allowing for the establishment of
@@ -26,15 +26,15 @@
                  name: str = "client",
                  client: bool = True,
                  protocoll: SysProtocolls = SysProtocolls.TCP,
                  server_name: str = "localhost",
                  port: int = 8080,
                  logformat_string: str = "%(asctime)s: [%(client_name)s] \
 [%(client_addr)i] [%(loggername)s] [%(loglevel)s]: %(message)s",
-                 logger: Logger = None) -> None:
+                 logger=None) -> None:
         """
         Initializes a SysHandler instance.
 
         Args:
             name (str): The name of the handler. Default is "client".
             client (bool): Whether the handler is a client. Default is True.
             protocoll (SysProtocolls): The protocol to use (TCP or UDP).
@@ -53,37 +53,37 @@
         address, and initializes the handler based on the provided parameters.
         """
         self.name = name
         self.client = client
         self.protocoll = protocoll
         self.server_name = server_name
         self.port = port
-        self.syssocket = socket.socket(socket.AF_INET,
-                                       self.protocoll.value)
+        self._syssocket = socket.socket(socket.AF_INET,
+                                        self.protocoll.value)
         self.server_addr = (self.server_name, self.port)
         self.logformat_string = logformat_string
 
         if self.protocoll == SysProtocolls.TCP:
             self._connect_client = partial(self._connect_client_tcp)
-            self._start_server = partial(self._start_server_tcp)
+            self._run_server = partial(self._run_server_tcp)
             self.handle_client_connection = partial(
                 self._handle_client_connection_tcp)
             self.emit = partial(self._emit_tcp)
         elif self.protocoll == SysProtocolls.UDP:
             self._connect_client = partial(self._connect_client_udp)
-            self._client_onlystart_server = partial(self._start_server_udp)
+            self._run_server = partial(self._run_server_udp)
             self.handle_client_connection = partial(
                 self._handle_client_connection_udp)
             self.emit = partial(self._emit_udp)
 
         if self.client:
             self._connect_client()
         else:
-            self._start_server()
-            self.logger = logger
+            self._logger = logger
+            self._run_server()
 
     @staticmethod
     def _client_only(func):
         """
         Decorator to ensure a method can only be called by a client.
 
         This decorator checks if the handler is in client mode before allowing
@@ -129,15 +129,15 @@
         """
         Establishes a TCP connection to the server as a client.
 
         This method connects the client socket to the server's address and port
         using TCP.
         """
         try:
-            self.syssocket.connect(self.server_addr)
+            self._syssocket.connect(self.server_addr)
         except ConnectionRefusedError:
             raise ServerUnreachableError(servername=self.server_name,
                                          port=self.port)
         except TimeoutError:
             raise ServerUnreachableError(servername=self.server_name,
                                          port=self.port)
 
@@ -148,46 +148,48 @@
 
         This method connects the client socket to the server's address and port
         using UDP.
         """
         ...
 
     @_client_only
-    def _start_server(self) -> None:
+    def _run_server(self) -> None:
         """
         Starts a server that listens for incoming connections.
 
-        This method is dynamically set to either `_start_server_tcp` or
-        `_start_server_udp` based on the protocol specified during the
+        This method is dynamically set to either `_run_server_tcp` or
+        `_run_server_udp` based on the protocol specified during the
         initialization of the SysHandler instance.
         """
         ...
 
     @_server_only
-    def _start_server_tcp(self) -> None:
+    def _run_server_tcp(self) -> None:
         """
         Starts a TCP server that listens for incoming connections.
 
         This method binds the server socket to the specified address and port,
         listens for incoming TCP connections, and accepts them.
         """
-        self.syssocket.bind(self.server_addr)
-        self.syssocket.listen(1)
-        print(f"TCP server listens in {self.server_addr}")
+        self._logger.info("Server is running")
+        self._syssocket.bind(self.server_addr)
+        self._syssocket.listen(1)
+        print(f"TCP server listens to {self.server_addr}")
 
     @_server_only
-    def _start_server_udp(self) -> None:
+    def _run_server_udp(self) -> None:
         """
         Starts a UDP server that listens for incoming connections.
 
         This method binds the server socket to the specified address and port,
         and listens for incoming UDP messages.
         """
-        self.syssocket.bind(self.server_addr)
-        print(f"UCP server listens in {self.server_addr}")
+        self._logger.info("Server is running")
+        self._syssocket.bind(self.server_addr)
+        print(f"UDP server listens to {self.server_addr}")
 
     @_client_only
     def emit(self, record: dict[str]) -> None:
         """
         Sends a log message to the server.
 
         This method is dynamically set to either `_emit_tcp` or `_emit_udp`
@@ -208,22 +210,23 @@
         it to the server using TCP. It also listens for a response from the
         server.
 
         Args:
             record (dict): A dictionary containing the log message details.
         """
         formatted_message = self._format_message(record)
+        formatted_message["client_name"] = self.name
 
         message_str = json.dumps(formatted_message)
 
         message_bytes = message_str.encode('utf-8')
 
-        self.syssocket.sendall(message_bytes)
+        self._syssocket.sendall(message_bytes)
 
-        data = self.syssocket.recv(1024)
+        data = self._syssocket.recv(1024)
         print(f"Received response: {data} from server")
 
     @_client_only
     def _emit_udp(self, record: dict[str]) -> None:
         """
         Sends a log message to the server over UDP.
 
@@ -231,19 +234,20 @@
         it to the server using UDP. It also listens for a response from the
         server.
 
         Args:
             record (dict): A dictionary containing the log message details.
         """
         formatted_message = self._format_message(record)
+        formatted_message["client_name"] = self.name
 
         message_str = json.dumps(formatted_message)
 
         message_bytes = message_str.encode('utf-8')
-        self.syssocket.sendto(message_bytes, self.server_addr)
+        self._syssocket.sendto(message_bytes, self.server_addr)
 
     @_server_only
     def _handle_client_connection(self) -> None:
         """
         Handles incoming connections from clients.
 
         This method is dynamically set to either
@@ -255,19 +259,19 @@
 
     @_server_only
     def _handle_client_connection_tcp(self) -> None:
         """
         Handles incoming TCP connections from clients.
 
         This method accepts incoming TCP connections, receives log messages,
-        decodes them, and logs the received log messages using `self.logger` if
-        available. It also sends a confirmation message back to the client.
+        decodes them, and logs the received log messages using `self._logger`
+        if available. It also sends a confirmation message back to the client.
         """
         while True:
-            client_socket, addr = self.syssocket.accept()
+            client_socket, addr = self._syssocket.accept()
             print(f"Connection from {addr} accepted")
 
             while True:
                 data = client_socket.recv(1024)
                 if not data:
                     print(f"Connection from {addr} was closed.")
                     break
@@ -275,64 +279,41 @@
                 received_dict = json.loads(received_str)
 
                 print(f"Received message: '{received_dict}' from {addr}")
                 received_dict["client_addr"] = addr
                 logformat_string = self.logformat_string
                 log_message = logformat_string % received_dict
 
-                self.logger.info(log_message)
+                self._logger.info(log_message)
 
                 client_socket.sendall(b"Receive message")
 
-            client_socket.close()
-
     @_server_only
     def _handle_client_connection_udp(self) -> None:
         """
         Handles incoming UDP connections from clients.
 
         This method listens for incoming UDP messages, decodes them, and logs
-        the received log messages using `self.logger` if available. It also
+        the received log messages using `self._logger` if available. It also
         sends a confirmation message back to the client.
         """
         while True:
-            data, addr = self.syssocket.recvfrom(1024)
+            data, addr = self._syssocket.recvfrom(1024)
             received_str = data.decode('utf-8')
             received_dict = json.loads(received_str)
 
             print(f"Received message: '{received_dict}' from {addr}")
 
             received_dict["client_addr"] = addr
             logformat_string = self.logformat_string
             log_message = logformat_string % received_dict
 
-            self.logger.info(log_message)
-
-            self.syssocket.sendto(b"Receive message", addr)
-
-    def _format_message(self, record: dict[str]) -> dict[str]:
-        """
-        Formats a log message based on the provided log data.
-
-        Args:
-            record (dict): A dictionary containing the log message details.
-
-        Returns:
-            str: The formatted log message.
-        """
-        values = {
-            "client_name": self.name,
-            "loggername": record.get("loggername", ""),
-            "iso_8601_time": record.get("iso_8601_time", ""),
-            "asctime": record.get("asctime", ""),
-            "loglevel": record.get("loglevel", ""),
-            "message": record.get("message", ""),
-        }
+            self._logger.info(log_message)
 
-        return values
+            self._syssocket.sendto(b"Receive message", addr)
 
     def __repr__(self) -> str:
         return f"SysHandler({self.client}, {self.protocoll}, \
 {self.server_name}, {self.port})"
 
     def __str__(self) -> str:
         return f"SysHandler with: {self.client}, {self.protocoll}, \
```

### Comparing `loggingpython-1.4.0/src/loggingpython/logger.py` & `loggingpython-1.4.1/src/loggingpython/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,7 +429,15 @@
 
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except except_type as e:
                 self.critical(f"{func.__name__} failed with error: {str(e)}")
         return wrapper
+
+    def __repr__(self) -> str:
+        return f"Logger({self.name}, {self.time_format}, {self.min_loglevel}, \
+{self.max_loglevel})"
+
+    def __str__(self) -> str:
+        return f"Logger with: {self.name}, {self.min_loglevel} and \
+{self.max_loglevel}"
```

### Comparing `loggingpython-1.4.0/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.1/src/loggingpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

