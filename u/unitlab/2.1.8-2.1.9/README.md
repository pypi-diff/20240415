# Comparing `tmp/unitlab-2.1.8.tar.gz` & `tmp/unitlab-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-2.1.8.tar", last modified: Tue Apr  9 12:43:14 2024, max compression
+gzip compressed data, was "unitlab-2.1.9.tar", last modified: Mon Apr 15 06:05:00 2024, max compression
```

## Comparing `unitlab-2.1.8.tar` & `unitlab-2.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 12:43:14.358066 unitlab-2.1.8/
--rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.8/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-09 12:43:14.358066 unitlab-2.1.8/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1450 2024-04-09 12:41:44.000000 unitlab-2.1.8/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-09 12:43:14.358066 unitlab-2.1.8/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-09 12:42:35.000000 unitlab-2.1.8/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 12:43:14.354066 unitlab-2.1.8/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 12:43:14.358066 unitlab-2.1.8/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.8/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.8/src/unitlab/__main__.py
--rw-rw-r--   0 me        (1000) me        (1000)    12067 2024-04-09 12:04:07.000000 unitlab-2.1.8/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.8/src/unitlab/dataset.py
--rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.8/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4560 2024-04-09 10:15:52.000000 unitlab-2.1.8/src/unitlab/main.py
--rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.8/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 12:43:14.358066 unitlab-2.1.8/src/unitlab.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-09 12:43:14.000000 unitlab-2.1.8/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/
+-rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.9/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-15 06:05:00.721197 unitlab-2.1.9/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1450 2024-04-09 12:41:44.000000 unitlab-2.1.9/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-15 06:05:00.721197 unitlab-2.1.9/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-15 06:01:52.000000 unitlab-2.1.9/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.9/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.9/src/unitlab/__main__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11952 2024-04-15 05:57:27.000000 unitlab-2.1.9/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.9/src/unitlab/dataset.py
+-rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.9/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4547 2024-04-15 05:56:37.000000 unitlab-2.1.9/src/unitlab/main.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1888 2024-04-15 06:00:14.000000 unitlab-2.1.9/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/unitlab.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-2.1.8/LICENSE.md` & `unitlab-2.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.8/PKG-INFO` & `unitlab-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.8
+Version: 2.1.9
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-2.1.8/README.md` & `unitlab-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.8/setup.py` & `unitlab-2.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="2.1.8",
+    version="2.1.9",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-2.1.8/src/unitlab/client.py` & `unitlab-2.1.9/src/unitlab/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import urllib.parse
 
 import aiofiles
 import aiohttp
 import requests
 import tqdm
 
-from . import exceptions, utils
+from . import exceptions
 from .dataset import DatasetUploadHandler
+from .utils import handle_exceptions
 
 logger = logging.getLogger(__name__)
 
 
 class UnitlabClient:
     """A client with a connection to the Unitlab.ai platform.
 
@@ -44,20 +45,15 @@
 
     Args:
         api_key: Your Unitlab.ai API key. If no API key given, reads ``UNITLAB_API_KEY`` from the environment. Defaults to :obj:`None`.
     Raises:
         :exc:`~unitlab.exceptions.AuthenticationError`: If an invalid API key is used or (when not passing the API key directly) if ``UNITLAB_API_KEY`` is not found in your environment.
     """
 
-    def __init__(self, api_key: str = None, api_url: str = None):
-        if api_key is None:
-            api_key = utils.get_api_key()
-        if api_url is None:
-            api_url = utils.get_api_url()
-
+    def __init__(self, api_key, api_url: str = "https://api.unitlab.ai"):
         self.api_key = api_key
         self.api_url = api_url
         self.api_session = requests.Session()
         adapter = requests.adapters.HTTPAdapter(max_retries=3)
         self.api_session.mount("http://", adapter)
         self.api_session.mount("https://", adapter)
 
@@ -91,21 +87,21 @@
         traceback,
     ) -> None:
         self.close()
 
     def _get_headers(self):
         return {"Authorization": f"Api-Key {self.api_key}"}
 
-    @utils.handle_exceptions
+    @handle_exceptions
     def _get(self, endpoint):
         return self.api_session.get(
             urllib.parse.urljoin(self.api_url, endpoint), headers=self._get_headers()
         )
 
-    @utils.handle_exceptions
+    @handle_exceptions
     def _post(self, endpoint, data=None):
         return self.api_session.post(
             urllib.parse.urljoin(self.api_url, endpoint),
             json=data or {},
             headers=self._get_headers(),
         )
```

### Comparing `unitlab-2.1.8/src/unitlab/dataset.py` & `unitlab-2.1.9/src/unitlab/dataset.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.8/src/unitlab/exceptions.py` & `unitlab-2.1.9/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.8/src/unitlab/main.py` & `unitlab-2.1.9/src/unitlab/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from pathlib import Path
 from uuid import UUID
 
 import typer
 import validators
 from typing_extensions import Annotated
 
+from . import utils
 from .client import UnitlabClient
-from .utils import get_api_key, write_config
 
 app = typer.Typer()
 project_app = typer.Typer()
 dataset_app = typer.Typer()
 
 app.add_typer(project_app, name="project", help="Project commands")
 app.add_typer(dataset_app, name="dataset", help="Dataset commands")
 
 
 API_KEY = Annotated[
     str,
     typer.Option(
-        default_factory=get_api_key, help="The api-key obtained from unitlab.ai"
+        default_factory=utils.get_api_key, help="The api-key obtained from unitlab.ai"
     ),
 ]
 
 
 class DownloadType(str, Enum):
     annotation = "annotation"
     files = "files"
@@ -42,15 +42,15 @@
 @app.command(help="Configure the credentials")
 def configure(
     api_key: Annotated[str, typer.Option(help="The api-key obtained from unitlab.ai")],
     api_url: Annotated[str, typer.Option()] = "https://api.unitlab.ai",
 ):
     if not validators.url(api_url, simple_host=True):
         raise typer.BadParameter("Invalid api url")
-    write_config(api_key=api_key, api_url=api_url)
+    utils.write_config(api_key=api_key, api_url=api_url)
 
 
 def get_client(api_key: str) -> UnitlabClient:
     return UnitlabClient(api_key=api_key)
 
 
 @project_app.command(name="list", help="Project list")
```

### Comparing `unitlab-2.1.8/src/unitlab/utils.py` & `unitlab-2.1.9/src/unitlab/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 def get_api_key() -> str:
     config = read_config()
     try:
         return config.get("default", "api_key")
     except Exception:
         raise exceptions.ConfigurationError(
-            f"Key `api_key` not found in {CONFIG_FILE_PATH}. Please run `unitlab configure` or provide one"
+            f"Key `api_key` not found in {CONFIG_FILE_PATH}. Please run `unitlab configure` or provide the api-key using the --api-key option."
         )
 
 
 def get_api_url() -> str:
     config = read_config()
     try:
         return config.get("default", "api_url")
```

### Comparing `unitlab-2.1.8/src/unitlab.egg-info/PKG-INFO` & `unitlab-2.1.9/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.8
+Version: 2.1.9
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

