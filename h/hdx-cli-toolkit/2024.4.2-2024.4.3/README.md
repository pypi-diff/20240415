# Comparing `tmp/hdx_cli_toolkit-2024.4.2.tar.gz` & `tmp/hdx_cli_toolkit-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx_cli_toolkit-2024.4.2.tar", last modified: Fri Apr 12 09:53:20 2024, max compression
+gzip compressed data, was "hdx_cli_toolkit-2024.4.3.tar", last modified: Mon Apr 15 07:01:25 2024, max compression
```

## Comparing `hdx_cli_toolkit-2024.4.2.tar` & `hdx_cli_toolkit-2024.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.711656 hdx_cli_toolkit-2024.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.441929 hdx_cli_toolkit-2024.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.441929 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15286 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.4.2/LICENSE` & `hdx_cli_toolkit-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/PKG-INFO` & `hdx_cli_toolkit-2024.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.2/README.md` & `hdx_cli_toolkit-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/pyproject.toml` & `hdx_cli_toolkit-2024.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hdx_cli_toolkit"
-version = "2024.4.2"
+version = "2024.4.3"
 description = "HDX CLI tool kit for commandline interaction with HDX"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 authors = [
   {email = "ian.hopkinson@un.org"},
   {name = "Ian Hopkinson"}
```

### Comparing `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/cli.py` & `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     get_users_from_hdx,
     update_values_in_hdx,
     configure_hdx_connection,
     update_resource_in_hdx,
     get_filtered_datasets,
     decorate_dataset_with_extras,
     download_hdx_datasets,
+    get_approved_tag_list,
 )
 
 
 @click.group()
 def hdx_toolkit() -> None:
     """Tools for Commandline interactions with HDX"""
 
@@ -290,16 +291,27 @@
             print(
                 f"{a_user['name']:<50.50}: {a_user['id']}",
                 flush=True,
             )
 
 
 @hdx_toolkit.command(name="configuration")
-def show_configuration():
+@click.option(
+    "--approved_tag_list",
+    is_flag=True,
+    default=False,
+    help="if present then print the list of approved tags",
+)
+def show_configuration(approved_tag_list: bool = False):
     """Print configuration information to terminal"""
+    if approved_tag_list:
+        approved_tags = get_approved_tag_list()
+        for approved_tag in approved_tags:
+            print(approved_tag, flush=True)
+        return
     print_banner("configuration")
     # Check files
     user_hdx_config_yaml = os.path.join(os.path.expanduser("~"), ".hdx_configuration.yaml")
     default_hdx_config_yaml = script_dir_plus_file(
         "hdx_base_configuration.yaml", ConfigurationError
     )
```

### Comparing `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/hdx_utilities.py` & `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/hdx_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 
 import fnmatch
 import functools
 import json
 import os
 import time
 import traceback
+import urllib3
 
 from pathlib import Path
 
 import click
+import urllib3.util
 import yaml
 
 from hdx.api.configuration import Configuration, ConfigurationError
 from hdx.data.organization import Organization
 from hdx.data.resource_view import ResourceView
 from hdx.data.hdxobject import HDXError
 from hdx.data.dataset import Dataset
 from hdx.data.showcase import Showcase
 from hdx.data.resource import Resource
 from hdx.data.user import User
+from hdx.utilities.path import script_dir_plus_file
 
 from hdx_cli_toolkit.utilities import read_attributes
 
 
 def hdx_error_handler(f):
     @functools.wraps(f)
     def inner(*args, **kwargs):
@@ -412,7 +415,31 @@
             hdx_site=hdx_site,
             hdx_read_only=False,
         )
         if verbose:
             print(f"Connected to HDX site {Configuration.read().get_hdx_site_url()}", flush=True)
     except ConfigurationError:
         pass
+
+
+def get_approved_tag_list() -> list[str]:
+    approved_tag_list = []
+    default_hdx_config_yaml = script_dir_plus_file(
+        "hdx_base_configuration.yaml", ConfigurationError
+    )
+
+    with open(default_hdx_config_yaml, "r", encoding="utf-8") as file_handle:
+        hdx_config_dict = yaml.safe_load(file_handle)
+
+    tags_list_url = hdx_config_dict["tags_list_url"]
+
+    response = urllib3.request(
+        "GET", tags_list_url, timeout=60, retries=urllib3.util.Retry(90, backoff_factor=1.0)
+    )
+    if response.status == 200:
+        response_str = response.data.decode("utf-8")
+        approved_tag_list = response_str.split("\n")
+    else:
+        print("Could not retrieve approved tag list", flush=True)
+        print(f"The tag list url {tags_list_url} returned status {response.status}", flush=True)
+
+    return approved_tag_list
```

### Comparing `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/utilities.py` & `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/PKG-INFO` & `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/SOURCES.txt` & `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/tests/test_cli.py` & `hdx_cli_toolkit-2024.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/tests/test_cli_integration.py` & `hdx_cli_toolkit-2024.4.3/tests/test_cli_integration.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities.py` & `hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities_integration.py` & `hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from hdx_cli_toolkit.hdx_utilities import (
     update_resource_in_hdx,
     configure_hdx_connection,
     update_values_in_hdx,
     add_showcase,
     add_quickcharts,
+    get_approved_tag_list,
 )
 
 from hdx_cli_toolkit.utilities import make_conversion_func
 
 
 DATASET_NAME = "hdx_cli_toolkit_test"
 TEST_RESOURCE_NAME = "test_resource_1"
@@ -196,7 +197,12 @@
                     quickchart_dict["hxl_preview_config"] = json.loads(
                         quickchart_dict["hxl_preview_config"]
                     )
                 quickchart_dicts.append(quickchart_dict)
 
     assert len(quickchart_dicts) == 2
     assert quickchart_dicts[1]["title"] == "Quick Charts"
+
+
+def test_get_approved_tag_list():
+    approved_tags = get_approved_tag_list()
+    assert len(approved_tags) == 140
```

### Comparing `hdx_cli_toolkit-2024.4.2/tests/test_utilities.py` & `hdx_cli_toolkit-2024.4.3/tests/test_utilities.py`

 * *Files identical despite different names*

