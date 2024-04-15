# Comparing `tmp/pypeline_runner-0.2.0.tar.gz` & `tmp/pypeline_runner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeline_runner-0.2.0.tar", max compression
+gzip compressed data, was "pypeline_runner-0.2.1.tar", max compression
```

## Comparing `pypeline_runner-0.2.0.tar` & `pypeline_runner-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-04-14 16:33:24.497637 pypeline_runner-0.2.0/LICENSE
--rw-r--r--   0        0        0     5929 2024-04-14 16:33:24.497637 pypeline_runner-0.2.0/README.md
--rw-r--r--   0        0        0     3925 2024-04-14 16:33:25.293635 pypeline_runner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-14 16:33:25.293635 pypeline_runner-0.2.0/src/pypeline/__init__.py
--rw-r--r--   0        0        0      350 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/__run.py
--rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/artifacts.py
--rw-r--r--   0        0        0     1491 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/config.py
--rw-r--r--   0        0        0     1101 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/execution_context.py
--rw-r--r--   0        0        0      980 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/pipeline.py
--rw-r--r--   0        0        0      894 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/project_slurper.py
--rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/__init__.py
--rw-r--r--   0        0        0     2235 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/create.py
--rw-r--r--   0        0        0     5772 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
--rw-r--r--   0        0        0    15971 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
--rw-r--r--   0        0        0       13 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/.gitignore
--rw-r--r--   0        0        0       34 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/poetry.toml
--rw-r--r--   0        0        0       36 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pypeline.ps1
--rw-r--r--   0        0        0      219 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pypeline.yaml
--rw-r--r--   0        0        0      225 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/scoopfile.json
--rw-r--r--   0        0        0      651 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/steps/my_step.py
--rw-r--r--   0        0        0     3382 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/main.py
--rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/py.typed
--rw-r--r--   0        0        0     4359 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/pypeline.py
--rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/__init__.py
--rw-r--r--   0        0        0     1954 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/create_venv.py
--rw-r--r--   0        0        0     3356 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/scoop_install.py
--rw-r--r--   0        0        0     1930 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/west_install.py
--rw-r--r--   0        0        0     7168 1970-01-01 00:00:00.000000 pypeline_runner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 17:48:20.206606 pypeline_runner-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5929 2024-04-14 17:48:20.206606 pypeline_runner-0.2.1/README.md
+-rw-r--r--   0        0        0     3925 2024-04-14 17:48:20.958601 pypeline_runner-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-14 17:48:20.958601 pypeline_runner-0.2.1/src/pypeline/__init__.py
+-rw-r--r--   0        0        0      350 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/__run.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/__init__.py
+-rw-r--r--   0        0        0     1355 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/artifacts.py
+-rw-r--r--   0        0        0     1663 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/config.py
+-rw-r--r--   0        0        0     1101 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/execution_context.py
+-rw-r--r--   0        0        0      980 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/pipeline.py
+-rw-r--r--   0        0        0      894 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/domain/project_slurper.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/__init__.py
+-rw-r--r--   0        0        0     2235 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/create.py
+-rw-r--r--   0        0        0     5772 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
+-rw-r--r--   0        0        0    15971 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0       13 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/.gitignore
+-rw-r--r--   0        0        0       34 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/poetry.toml
+-rw-r--r--   0        0        0       36 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/pypeline.ps1
+-rw-r--r--   0        0        0      219 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/pypeline.yaml
+-rw-r--r--   0        0        0      225 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/scoopfile.json
+-rw-r--r--   0        0        0      651 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/steps/my_step.py
+-rw-r--r--   0        0        0     3227 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/main.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/py.typed
+-rw-r--r--   0        0        0     4359 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/pypeline.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/steps/__init__.py
+-rw-r--r--   0        0        0     1954 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/steps/create_venv.py
+-rw-r--r--   0        0        0     3356 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/steps/scoop_install.py
+-rw-r--r--   0        0        0     1930 2024-04-14 17:48:20.210606 pypeline_runner-0.2.1/src/pypeline/steps/west_install.py
+-rw-r--r--   0        0        0     7168 1970-01-01 00:00:00.000000 pypeline_runner-0.2.1/PKG-INFO
```

### Comparing `pypeline_runner-0.2.0/LICENSE` & `pypeline_runner-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/README.md` & `pypeline_runner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/pyproject.toml` & `pypeline_runner-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypeline-runner"
-version = "0.2.0"
+version = "0.2.1"
 description = "Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines)."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/pypeline"
 documentation = "https://pypeline-runner.readthedocs.io"
 classifiers = [
```

### Comparing `pypeline_runner-0.2.0/src/pypeline/domain/artifacts.py` & `pypeline_runner-0.2.1/src/pypeline/domain/artifacts.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/domain/config.py` & `pypeline_runner-0.2.1/src/pypeline/domain/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,21 +16,24 @@
     # This field is intended to keep track of where configuration was loaded from and
     # it is automatically added when configuration is loaded from file
     file: Optional[Path] = None
 
     @classmethod
     def from_file(cls, config_file: Path) -> "ProjectConfig":
         config_dict = cls.parse_to_dict(config_file)
-        return cls.from_dict(config_dict)
+        try:
+            return cls.from_dict(config_dict)
+        except Exception as e:
+            raise UserNotificationException(f"Invalid configuration file '{config_file}'. \nError: {e}") from None
 
     @staticmethod
     def parse_to_dict(config_file: Path) -> Dict[str, Any]:
         try:
             with open(config_file) as fs:
                 config_dict = yaml.safe_load(fs)
                 # Add file name to config to keep track of where configuration was loaded from
                 config_dict["file"] = config_file
             return config_dict
         except ScannerError as e:
-            raise UserNotificationException(f"Failed scanning configuration file '{config_file}'. \nError: {e}") from e
+            raise UserNotificationException(f"Failed scanning configuration file '{config_file}'. \nError: {e}") from None
         except ParserError as e:
-            raise UserNotificationException(f"Failed parsing configuration file '{config_file}'. \nError: {e}") from e
+            raise UserNotificationException(f"Failed parsing configuration file '{config_file}'. \nError: {e}") from None
```

### Comparing `pypeline_runner-0.2.0/src/pypeline/domain/execution_context.py` & `pypeline_runner-0.2.1/src/pypeline/domain/execution_context.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/domain/pipeline.py` & `pypeline_runner-0.2.1/src/pypeline/domain/pipeline.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/domain/project_slurper.py` & `pypeline_runner-0.2.1/src/pypeline/domain/project_slurper.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/kickstart/create.py` & `pypeline_runner-0.2.1/src/pypeline/kickstart/create.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1` & `pypeline_runner-0.2.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py` & `pypeline_runner-0.2.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/steps/my_step.py` & `pypeline_runner-0.2.1/src/pypeline/kickstart/templates/project/steps/my_step.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/main.py` & `pypeline_runner-0.2.1/src/pypeline/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from pathlib import Path
-from typing import List, Optional
+from typing import Optional
 
 import typer
 from py_app_dev.core.exceptions import UserNotificationException
 from py_app_dev.core.logging import logger, setup_logger, time_it
 
 from pypeline import __version__
 from pypeline.domain.project_slurper import ProjectSlurper
@@ -82,21 +82,14 @@
             raise UserNotificationException(f"Step '{step}' not found in the pipeline.")
         logger.info("No steps to run.")
         return
 
     PipelineStepsExecutor(project_slurper.artifacts_locator, steps_references, force_run, dry_run).run()
 
 
-def main(args: Optional[List[str]] = None) -> int:
+if __name__ == "__main__":
     try:
         setup_logger()
-        if args is None:
-            args = sys.argv[1:]
-        app(args)
-        return 0
+        app()
     except UserNotificationException as e:
         logger.error(f"{e}")
-        return 1
-
-
-if __name__ == "__main__":
-    sys.exit(main())
+        sys.exit(1)
```

### Comparing `pypeline_runner-0.2.0/src/pypeline/pypeline.py` & `pypeline_runner-0.2.1/src/pypeline/pypeline.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/steps/create_venv.py` & `pypeline_runner-0.2.1/src/pypeline/steps/create_venv.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/steps/scoop_install.py` & `pypeline_runner-0.2.1/src/pypeline/steps/scoop_install.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/src/pypeline/steps/west_install.py` & `pypeline_runner-0.2.1/src/pypeline/steps/west_install.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.0/PKG-INFO` & `pypeline_runner-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-runner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines).
 Home-page: https://github.com/cuinixam/pypeline
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypeline-runner Version: 0.2.0 Summary: Configure
+Metadata-Version: 2.1 Name: pypeline-runner Version: 0.2.1 Summary: Configure
 and execute pipelines with Python (similar to GitHub workflows or Jenkins
 pipelines). Home-page: https://github.com/cuinixam/pypeline License: MIT
 Author: cuinixam Author-email: me@cuinixam.com Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

