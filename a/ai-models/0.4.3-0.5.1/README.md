# Comparing `tmp/ai-models-0.4.3.tar.gz` & `tmp/ai-models-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-models-0.4.3.tar", last modified: Mon Feb 26 16:44:21 2024, max compression
+gzip compressed data, was "ai-models-0.5.1.tar", last modified: Mon Apr 15 13:14:47 2024, max compression
```

## Comparing `ai-models-0.4.3.tar` & `ai-models-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:44:21.610633 ai-models-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 16:44:12.000000 ai-models-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-02-26 16:44:21.610633 ai-models-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-02-26 16:44:12.000000 ai-models-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:44:21.610633 ai-models-0.4.3/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:44:21.610633 ai-models-0.4.3/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:44:21.610633 ai-models-0.4.3/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-26 16:44:12.000000 ai-models-0.4.3/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:44:21.610633 ai-models-0.4.3/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:44:21.000000 ai-models-0.4.3/ai_models.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 16:44:21.610633 ai-models-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-26 16:44:12.000000 ai-models-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 13:14:36.000000 ai-models-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 13:14:47.752941 ai-models-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-15 13:14:36.000000 ai-models-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.752941 ai-models-0.5.1/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-15 13:14:36.000000 ai-models-0.5.1/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:47.748941 ai-models-0.5.1/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:14:47.000000 ai-models-0.5.1/ai_models.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:14:47.752941 ai-models-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-15 13:14:36.000000 ai-models-0.5.1/setup.py
```

### Comparing `ai-models-0.4.3/LICENSE` & `ai-models-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-models-0.4.3/PKG-INFO` & `ai-models-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.4.3
+Version: 0.5.1
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.4.3/README.md` & `ai-models-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ai-models-0.4.3/ai_models/__main__.py` & `ai-models-0.5.1/ai_models/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,27 +81,27 @@
         help=("Dump information for tracking provenance."),
     )
 
     parser.add_argument(
         "--input",
         default="mars",
         help="Source to use",
-        choices=available_inputs(),
+        choices=sorted(available_inputs()),
     )
 
     parser.add_argument(
         "--file",
         help="Source to use if source=file",
     )
 
     parser.add_argument(
         "--output",
         default="file",
         help="Where to output the results",
-        choices=available_outputs(),
+        choices=sorted(available_outputs()),
     )
 
     parser.add_argument(
         "--date",
         default="-1",
         help="For which analysis date to start the inference (default: yesterday)",
     )
@@ -212,30 +212,42 @@
         help="Model version",
     )
 
     if "--models" not in argv:
         parser.add_argument(
             "model",
             metavar="MODEL",
-            choices=available_models(),
+            choices=available_models() if "--remote" not in argv else None,
             help="The model to run",
         )
 
     parser.add_argument(
         "--remote",
         help="Enable remote execution, read url and token from ~/.config/ai-models/api.yaml",
         action="store_true",
         dest="remote_execution",
         default=(os.environ.get("AI_MODELS_REMOTE", "0") == "1"),
     )
 
     args, unknownargs = parser.parse_known_args(argv)
 
     if args.models:
-        for p in sorted(available_models()):
+        if args.remote_execution:
+            from .remote import RemoteAPI
+
+            api = RemoteAPI()
+            models = api.models()
+            if len(models) == 0:
+                print(f"No remote models available on {api.url}")
+                sys.exit(0)
+            print(f"Models available on remote server {api.url}")
+        else:
+            models = available_models()
+
+        for p in sorted(models):
             print(p)
         sys.exit(0)
 
     if args.assets_sub_directory:
         args.assets = os.path.join(args.assets, args.model)
 
     if args.path is None:
@@ -267,15 +279,20 @@
                 "You need to specify --retrieve-requests or --archive-requests"
             )
 
     run(vars(args), unknownargs)
 
 
 def run(cfg: dict, model_args: list):
-    model = load_model(cfg["model"], **cfg, model_args=model_args)
+    if cfg["remote_execution"]:
+        from .remote import RemoteModel
+
+        model = RemoteModel(**cfg, model_args=model_args)
+    else:
+        model = load_model(cfg["model"], **cfg, model_args=model_args)
 
     if cfg["fields"]:
         model.print_fields()
         sys.exit(0)
 
     # This logic is a bit convoluted, but it is for backwards compatibility.
     if cfg["retrieve_requests"] or (
@@ -285,18 +302,15 @@
         sys.exit(0)
 
     if cfg["assets_list"]:
         model.print_assets_list()
         sys.exit(0)
 
     try:
-        if cfg["remote_execution"]:
-            model.remote(cfg, model_args)
-        else:
-            model.run()
+        model.run()
     except FileNotFoundError as e:
         LOG.exception(e)
         LOG.error(
             "It is possible that some files requited by %s are missing.",
             cfg["model"],
         )
         LOG.error("Rerun the command as:")
```

### Comparing `ai-models-0.4.3/ai_models/checkpoint.py` & `ai-models-0.5.1/ai_models/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.4.3/ai_models/inputs/__init__.py` & `ai-models-0.5.1/ai_models/inputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 import logging
 from functools import cached_property
 
 import climetlab as cml
+import entrypoints
 
 LOG = logging.getLogger(__name__)
 
 
 class RequestBasedInput:
     def __init__(self, owner, **kwargs):
         self.owner = owner
@@ -195,21 +196,16 @@
         return self.all_fields.sel(levtype="ml")
 
     @cached_property
     def all_fields(self):
         return cml.load_source("file", self.file)
 
 
-INPUTS = dict(
-    mars=MarsInput,
-    file=FileInput,
-    cds=CdsInput,
-    opendata=OpenDataInput,
-)
-
-
 def get_input(name, *args, **kwargs):
-    return INPUTS[name](*args, **kwargs)
+    return available_inputs()[name].load()(*args, **kwargs)
 
 
 def available_inputs():
-    return sorted(INPUTS.keys())
+    result = {}
+    for e in entrypoints.get_group_all("ai_models.input"):
+        result[e.name] = e
+    return result
```

### Comparing `ai-models-0.4.3/ai_models/model.py` & `ai-models-0.5.1/ai_models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 # nor does it submit to any jurisdiction.
 
 import datetime
 import json
 import logging
 import os
 import sys
-import tempfile
 import time
 from collections import defaultdict
 from functools import cached_property
 
 import climetlab as cml
 import entrypoints
 import numpy as np
 from climetlab.utils.humanize import seconds
 from multiurl import download
 
 from .checkpoint import peek
 from .inputs import get_input
 from .outputs import get_output
-from .remote import RemoteClient
 from .stepper import Stepper
 
 LOG = logging.getLogger(__name__)
 
 
 class Timer:
     def __init__(self, title):
@@ -454,31 +452,14 @@
                         startStep=0,
                         endStep=0,
                         date=int(self.start_datetime.strftime("%Y%m%d")),
                         time=int(self.start_datetime.strftime("%H%M")),
                         check=True,
                     )
 
-    def remote(self, cfg: dict, model_args: list):
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            input_file = os.path.join(tmpdirname, "input.grib")
-            output_file = os.path.join(tmpdirname, "output.grib")
-            self.all_fields.save(input_file)
-
-            client = RemoteClient(
-                input_file=input_file,
-                output_file=output_file,
-            )
-
-            client.run(cfg, model_args)
-
-            ds = cml.load_source("file", output_file)
-            for field in ds:
-                self.write(None, template=field)
-
 
 def load_model(name, **kwargs):
     return available_models()[name].load()(**kwargs)
 
 
 def available_models():
     result = {}
```

### Comparing `ai-models-0.4.3/ai_models/outputs/__init__.py` & `ai-models-0.5.1/ai_models/outputs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # nor does it submit to any jurisdiction.
 
 import itertools
 import logging
 from functools import cached_property
 
 import climetlab as cml
+import entrypoints
 import numpy as np
 
 LOG = logging.getLogger(__name__)
 
 
 class FileOutput:
     def __init__(self, owner, path, metadata, **kwargs):
@@ -113,22 +114,19 @@
     def __init__(self, *args, **kwargs):
         LOG.info("Results will not be written.")
 
     def write(self, *args, **kwargs):
         pass
 
 
-OUTPUTS = dict(
-    file=FileOutput,
-    none=NoneOutput,
-)
-
-
 def get_output(name, owner, *args, **kwargs):
-    result = OUTPUTS[name](owner, *args, **kwargs)
+    result = available_outputs()[name].load()(owner, *args, **kwargs)
     if kwargs.get("hindcast_reference_year") is not None:
         result = HindcastReLabel(owner, result, **kwargs)
     return result
 
 
 def available_outputs():
-    return sorted(OUTPUTS.keys())
+    result = {}
+    for e in entrypoints.get_group_all("ai_models.output"):
+        result[e.name] = e
+    return result
```

### Comparing `ai-models-0.4.3/ai_models/stepper.py` & `ai-models-0.5.1/ai_models/stepper.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,10 +37,13 @@
             seconds(now - self.last),
             step,
             seconds(eta),
         )
         self.last = now
 
     def __exit__(self, *args):
+        if self.num_steps == 0:
+            return
+
         elapsed = time.time() - self.start
         LOG.info("Elapsed: %s.", seconds(elapsed))
         LOG.info("Average: %s per step.", seconds(elapsed / self.num_steps))
```

### Comparing `ai-models-0.4.3/ai_models.egg-info/PKG-INFO` & `ai-models-0.5.1/ai_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.4.3
+Version: 0.5.1
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.4.3/setup.py` & `ai-models-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 
 
 import io
 import os
 
 import setuptools
+from setuptools.command.install import install
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return io.open(file_path, encoding="utf-8").read()
 
 
@@ -25,45 +26,69 @@
     if line.startswith("__version__"):
         version = line.split("=")[-1].strip()[1:-1]
 
 
 assert version
 
 
+class PostInstall(install):
+    def run(self):
+        from ai_models.remote.config import config_exists, create_config
+
+        if not config_exists():
+            create_config()
+
+        install.run(self)
+
+
 setuptools.setup(
     name="ai-models",
     version=version,
     description="A package to run AI weather models",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
     author_email="software.support@ecmwf.int",
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf-lab/ai-models",
     packages=setuptools.find_packages(),
     include_package_data=True,
+    cmdclass={
+        "install": PostInstall,
+    },
     install_requires=[
         "entrypoints",
         "climetlab>=0.20.11",
         "multiurl",
         "ecmwflibs>=0.6.1",
         "gputil",
         "earthkit-meteo",
         "pyyaml",
+        "tqdm",
     ],
     extras_require={
         "provenance": [
             "nvsmi",
             "GitPython",
         ]
     },
     zip_safe=True,
     keywords="tool",
     entry_points={
         "console_scripts": ["ai-models=ai_models.__main__:main"],
+        "ai_models.input": [
+            "file=ai_models.inputs:FileInput",
+            "mars=ai_models.inputs:MarsInput",
+            "cds=ai_models.inputs:CdsInput",
+            "opendata=ai_models.inputs:OpenDataInput",
+        ],
+        "ai_models.output": [
+            "file=ai_models.outputs:FileOutput",
+            "none=ai_models.outputs:NoneOutput",
+        ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
```

