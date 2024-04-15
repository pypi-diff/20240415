# Comparing `tmp/watson_poetry-0.1.8.tar.gz` & `tmp/watson_poetry-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watson_poetry-0.1.8.tar", max compression
+gzip compressed data, was "watson_poetry-0.1.9.tar", max compression
```

## Comparing `watson_poetry-0.1.8.tar` & `watson_poetry-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.8/README.md
--rw-r--r--   0        0        0      620 2024-04-14 22:01:13.407803 watson_poetry-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3007 2024-04-14 22:01:04.054160 watson_poetry-0.1.8/src/watson_poetry/plugin.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.9/README.md
+-rw-r--r--   0        0        0      620 2024-04-14 22:05:03.934745 watson_poetry-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2947 2024-04-14 22:04:58.176420 watson_poetry-0.1.9/src/watson_poetry/plugin.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.9/PKG-INFO
```

### Comparing `watson_poetry-0.1.8/src/watson_poetry/plugin.py` & `watson_poetry-0.1.9/src/watson_poetry/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
         io = event.io
 
         verbose_level= Verbosity(io.is_verbose() + io.is_very_verbose() + io.is_debug())
-        print(verbose_level)
         
         if self.is_active:
             self._run_command(io, verbose_level)
         elif verbose_level >= Verbosity.VERBOSE:
             io.write_line("Watson not set to run any command.")
 
     def read_pyproject_toml(self) -> None:
@@ -64,14 +63,14 @@
             if verbosity is Verbosity.DEBUG:
                 io.write_line(f"Adding prefix to activate venv: source {self.venv_path}/bin/activate &&")
             prefix = f"source {self.venv_path}/bin/activate && "
         else: 
             if verbosity is Verbosity.DEBUG:
                 io.write_line("No prefix to activate venv.")
             prefix = ""
-        if verbosity is Verbosity.DEBUG:
-            io.write_line(f"Running command: {prefix}{self.__command}")
+
+        io.write_line(f"<info>Running command: {prefix}{self.__command}</info>")
         process = subprocess.run(f"{prefix}{self.__command}", capture_output=True, shell=True, text=True)
         if process.returncode != 0:
             if verbosity is Verbosity.DEBUG:
                 io.write_line(f"Command failed with return code {process.returncode}.")
             raise subprocess.CalledProcessError(process.returncode, process.args)
```

