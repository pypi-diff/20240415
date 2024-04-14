# Comparing `tmp/watson_poetry-0.1.6.tar.gz` & `tmp/watson_poetry-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watson_poetry-0.1.6.tar", max compression
+gzip compressed data, was "watson_poetry-0.1.7.tar", max compression
```

## Comparing `watson_poetry-0.1.6.tar` & `watson_poetry-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.6/README.md
--rw-r--r--   0        0        0      620 2024-04-14 21:56:13.250323 watson_poetry-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3042 2024-04-14 21:55:59.415691 watson_poetry-0.1.6/src/watson_poetry/plugin.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.7/README.md
+-rw-r--r--   0        0        0      620 2024-04-14 21:58:09.629649 watson_poetry-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3018 2024-04-14 21:57:56.360784 watson_poetry-0.1.7/src/watson_poetry/plugin.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.7/PKG-INFO
```

### Comparing `watson_poetry-0.1.6/pyproject.toml` & `watson_poetry-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "watson-poetry"
-version = "0.1.6"
+version = "0.1.7"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `watson_poetry-0.1.6/src/watson_poetry/plugin.py` & `watson_poetry-0.1.7/src/watson_poetry/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def read_pyproject_toml(self) -> None:
         try:
             with open("pyproject.toml", "rb") as file:
                 config = toml.load(file)
 
                 self.is_needed =  config.get("tool", {}).get("watson", {}).get("always_compile_before_running", False)
-                self.compile_command = config.get("tool", {}).get("watsong", {}).get("command", self.command)
+                self.command = config.get("tool", {}).get("watsong", {}).get("command", self.command)
                 self.run_in_venv = config.get("tool", {}).get("watson", {}).get("run_in_venv", self.run_in_venv)
                 self.venv_path = config.get("tool", {}).get("watson", {}).get("venv_path", self.venv_path)
 
         except FileNotFoundError:
             self.is_needed = False
 
     def _run_command(self, io: IO, verbosity: Verbosity):
@@ -65,13 +65,13 @@
                 io.write_line(f"Adding prefix to activate venv: source {self.venv_path}/bin/activate &&")
             prefix = f"source {self.venv_path}/bin/activate && "
         else: 
             if verbosity is Verbosity.DEBUG:
                 io.write_line("No prefix to activate venv.")
             prefix = ""
         if verbosity is Verbosity.DEBUG:
-            io.write_line(f"Running command: {prefix}{self.compile_command}")
-        process = subprocess.run(f"{prefix}{self.compile_command}", capture_output=True, shell=True, text=True)
+            io.write_line(f"Running command: {prefix}{self.command}")
+        process = subprocess.run(f"{prefix}{self.command}", capture_output=True, shell=True, text=True)
         if process.returncode != 0:
             if verbosity is Verbosity.DEBUG:
                 io.write_line(f"Command failed with return code {process.returncode}.")
             raise subprocess.CalledProcessError(process.returncode, process.args)
```

