# Comparing `tmp/mloggers-1.1.6.tar.gz` & `tmp/mloggers-1.1.7.tar.gz`

## Comparing `mloggers-1.1.6.tar` & `mloggers-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.1.6/.taplo.toml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/_log_levels.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/console_logger.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/file_logger.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/logger.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/multi_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/progress.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.1.6/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.1.6/LICENSE
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mloggers-1.1.6/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mloggers-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 mloggers-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.1.7/.taplo.toml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/__init__.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/file_logger.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/logger.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/multi_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/progress.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.1.7/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.1.7/LICENSE
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mloggers-1.1.7/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 mloggers-1.1.7/PKG-INFO
```

### Comparing `mloggers-1.1.6/mloggers/console_logger.py` & `mloggers-1.1.7/mloggers/console_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class ConsoleLogger(Logger):
     """Logs to the console (i.e., standard I/O)."""
 
+    def __init__(self, default_level: LogLevel = LogLevel.INFO):  # type:ignore[reportArgumentType]
+        super().__init__(default_level)
+
     def log(
         self,
         message: str | dict[str, Any],
         level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
-        super(ConsoleLogger, self).log(message, level, *args, **kwargs)
+        if not super(ConsoleLogger, self).log(message, level, *args, **kwargs):
+            return
 
         time = "[" + datetime.now().strftime("%H:%M:%S") + "]"
 
         if level is None:
             level_str = ""
             level_clr = ""
         else:
@@ -30,15 +34,15 @@
             if isinstance(level, LogLevel):
                 level_str = "[" + level.name + "] "
             else:
                 level_str = "[" + str(level).upper() + "] "
 
             # Color the level string
             if isinstance(level, LogLevel):
-                level_clr = colored(level_str, level.value)
+                level_clr = colored(level_str, level.value["color"])
             else:
                 level_clr = colored(level_str, "green")
 
         # The first level of the dictionary is printed as a multiline
         # indented message.
         # The rest of the levels are printed as a single line
         # pretifyed depending on the type of the value.
```

### Comparing `mloggers-1.1.6/mloggers/file_logger.py` & `mloggers-1.1.7/mloggers/file_logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,35 @@
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class FileLogger(Logger):
     """Logs to a file."""
 
-    def __init__(self, file_path: str):
+    def __init__(self, file_path: str, default_level: LogLevel | int = LogLevel.INFO):  # type:ignore[reportArgumentType]
         """
         Initializes a file logger.
 
         ### Parameters
         ----------
         `file_path`: the path to the file to log to.
         - The file will be created if it does not exist. If it does, the logs will be appended to it.
+
+        `default_level`: the default log level to use.
         """
 
+        super().__init__(default_level)
+
         # Create the file if it does not exist
         if not os.path.exists(file_path):
             dir_path = os.path.dirname(file_path)
             try:
-                os.makedirs(dir_path)
+                # If dir path is empty, it means the file is in the current directory
+                if dir_path != "":
+                    os.makedirs(dir_path)
             except FileExistsError:
                 pass
             with open(file_path, "w") as file:
                 file.write("")
 
         print(f'{colored("[INFO]", "cyan")} [FileLogger] Logging to file {file_path}')
 
@@ -40,15 +46,16 @@
     def log(
         self,
         message: str | dict[str, Any],
         level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
-        super(FileLogger, self).log(message, level, *args, **kwargs)
+        if not super(FileLogger, self).log(message, level, *args, **kwargs):
+            return
 
         # Convert numpy's ndarrays to lists so that they are JSON serializable
         if isinstance(message, dict):
             for key, value in message.items():
                 if isinstance(value, np.ndarray):
                     message[key] = value.tolist()
         elif hasattr(message, "__str__") and callable(getattr(message, "__str__")):
```

### Comparing `mloggers-1.1.6/mloggers/multi_logger.py` & `mloggers-1.1.7/mloggers/multi_logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,48 @@
 class MultiLogger(Logger):
     """Logs to multiple loggers."""
 
     def __init__(
         self,
         loggers: list[Logger],
         default_mask: list[type[Logger]] = [],
+        default_level: LogLevel | int = LogLevel.INFO,  # type:ignore[reportArgumentType]
     ):
         """
         Initializes a multi-logger.
 
         ### Parameters
         ----------
         `loggers`: a list of the initialized loggers to use.
         `default_mask`: the default mask to use when logging.
+        `default_level`: the default log level to use.
         """
 
+        super().__init__(default_level)
+
         self._loggers = loggers
         self._default_mask = default_mask
 
+        for logger in self._loggers:
+            logger.set_level(self._log_level)
+
+    def set_level(self, level: LogLevel | int):
+        """
+        Sets the log level of the multi-logger.
+
+        ### Parameters
+        ----------
+        `level`: the level to set.
+        """
+
+        super(MultiLogger, self).set_level(level)
+
+        for logger in self._loggers:
+            logger.set_level(self._log_level)
+
     def log(
         self,
         message: str | dict[str, Any],
         level: LogLevel | str | None = None,
         mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
@@ -83,15 +104,15 @@
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.INFO, mask, *args, **kwargs)
+        self.log(message, LogLevel.INFO, mask, *args, **kwargs)  # type:ignore[reportArgumentType]
 
     def warn(
         self,
         message: str | dict[str, Any],
         mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
@@ -106,15 +127,18 @@
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.WARN, mask, *args, **kwargs)
+        self.log(message, LogLevel.WARN, mask, *args, **kwargs)  # type:ignore[reportArgumentType]
+
+    # Alias warning to warn
+    warning = warn
 
     def error(
         self,
         message: str | dict[str, Any],
         mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
@@ -129,15 +153,15 @@
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.ERROR, mask, *args, **kwargs)
+        self.log(message, LogLevel.ERROR, mask, *args, **kwargs)  # type:ignore[reportArgumentType]
 
     def debug(
         self,
         message: str | dict[str, Any],
         mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
@@ -152,8 +176,8 @@
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.DEBUG, mask, *args, **kwargs)
+        self.log(message, LogLevel.DEBUG, mask, *args, **kwargs)  # type:ignore[reportArgumentType]
```

### Comparing `mloggers-1.1.6/mloggers/progress.py` & `mloggers-1.1.7/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.6/mloggers/wandb_logger.py` & `mloggers-1.1.7/mloggers/wandb_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,39 +12,44 @@
     """Logs to Weights & Biases."""
 
     def __init__(
         self,
         project: str,
         group: str,
         experiment: str,
+        default_level: LogLevel | int = LogLevel.INFO,  # type:ignore[reportArgumentType]
         config: DictConfig | None = None,
     ):
         """
         Initializes a Weights & Biases logger.
 
         ### Parameters
         ----------
         `project`: the name of the project to log to.
         `group`: the name of the group to log to.
         `experiment`: the name of the experiment to log to.
+        `default_level`: the default log level to use.
         [optional] `config`: the configuration of the experiment.
         """
 
+        super().__init__(default_level)
+
         if config is not None:
             config = vars(config)
         wandb.init(project=project, group=group, name=experiment, config=config)
 
     def log(
         self,
         message: str | dict[str, Any],
         level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
-        super(WandbLogger, self).log(message, level, *args, **kwargs)
+        if not super(WandbLogger, self).log(message, level, *args, **kwargs):
+            return
 
         if isinstance(message, dict):
             log = message
         else:
             if level is not None:
                 level_str = (
                     level.name if isinstance(level, LogLevel) else str(level).upper()
```

### Comparing `mloggers-1.1.6/.gitignore` & `mloggers-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.6/LICENSE` & `mloggers-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.6/README.md` & `mloggers-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.6/pyproject.toml` & `mloggers-1.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
+    { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `mloggers-1.1.6/PKG-INFO` & `mloggers-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.1.6
+Version: 1.1.7
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
-Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>
+Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: aenum
 Requires-Dist: numpy
```

