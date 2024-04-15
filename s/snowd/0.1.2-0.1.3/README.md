# Comparing `tmp/snowd-0.1.2.tar.gz` & `tmp/snowd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowd-0.1.2.tar", max compression
+gzip compressed data, was "snowd-0.1.3.tar", max compression
```

## Comparing `snowd-0.1.2.tar` & `snowd-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2073 2023-12-05 15:40:02.163706 snowd-0.1.2/README.md
--rw-r--r--   0        0        0      700 2023-12-06 13:14:36.298589 snowd-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      141 2023-12-05 15:40:02.171706 snowd-0.1.2/snowd/__init__.py
--rw-r--r--   0        0        0      467 2023-12-05 15:40:02.171706 snowd-0.1.2/snowd/__main__.py
--rw-r--r--   0        0        0     6379 2023-12-05 15:40:02.171706 snowd-0.1.2/snowd/client.py
--rw-r--r--   0        0        0      575 2023-12-05 15:40:02.171706 snowd-0.1.2/snowd/envvars.py
--rw-r--r--   0        0        0     5553 2023-12-06 13:14:36.298589 snowd-0.1.2/snowd/git.py
--rw-r--r--   0        0        0      871 2023-12-05 15:40:02.175706 snowd-0.1.2/snowd/polling.py
--rw-r--r--   0        0        0     1770 2023-12-05 15:40:02.175706 snowd-0.1.2/snowd/state.py
--rw-r--r--   0        0        0     3592 2023-12-06 12:56:53.428734 snowd-0.1.2/snowd/utils.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 snowd-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2073 2024-04-15 14:17:34.592230 snowd-0.1.3/README.md
+-rw-r--r--   0        0        0      700 2024-04-15 14:17:34.596230 snowd-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-04-15 14:17:34.596230 snowd-0.1.3/snowd/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-15 14:17:34.596230 snowd-0.1.3/snowd/__main__.py
+-rw-r--r--   0        0        0     6222 2024-04-15 14:17:34.596230 snowd-0.1.3/snowd/client.py
+-rw-r--r--   0        0        0      575 2024-04-15 14:17:34.600231 snowd-0.1.3/snowd/envvars.py
+-rw-r--r--   0        0        0     5553 2024-04-15 14:17:34.600231 snowd-0.1.3/snowd/git.py
+-rw-r--r--   0        0        0      871 2024-04-15 14:17:34.600231 snowd-0.1.3/snowd/polling.py
+-rw-r--r--   0        0        0     1489 2024-04-15 14:17:34.600231 snowd-0.1.3/snowd/state.py
+-rw-r--r--   0        0        0     3592 2024-04-15 14:17:34.600231 snowd-0.1.3/snowd/utils.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 snowd-0.1.3/PKG-INFO
```

### Comparing `snowd-0.1.2/README.md` & `snowd-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `snowd-0.1.2/pyproject.toml` & `snowd-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snowd"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "snowd", from="."}]
 
 # [tool.poetry.scripts]
 # snowd = "snowd.__main__:main"
```

### Comparing `snowd-0.1.2/snowd/client.py` & `snowd-0.1.3/snowd/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,44 +118,40 @@
 def get_client(
     instance=None,
     user=None,
     password=None,
     /,
     client_id=None,
     client_secret=None,
-    use_env_variables=False,
 ):
-    if use_env_variables:
-        instance = instance or SNOW_INSTANCE
-        user = user or SNOW_USER
-        password = password or SNOW_PASSWORD
-        client_id = client_id or SNOW_CLIENT_ID
-        client_secret = client_secret or SNOW_CLIENT_SECRET
+    instance = instance or SNOW_INSTANCE
+    user = user or SNOW_USER
+    password = password or SNOW_PASSWORD
+    client_id = client_id or SNOW_CLIENT_ID
+    client_secret = client_secret or SNOW_CLIENT_SECRET
     if client_id and client_secret:
         return _get_oauth_client(instance, user, password, client_id, client_secret)
     return pysnow.Client(instance=instance, user=user, password=password)
 
 
 class Client:
     def __init__(
         self,
         instance=None,
         user=None,
         password=None,
         client_id=None,
         client_secret=None,
-        use_env_variables=False,
     ):
         self._client = get_client(
             instance,
             user,
             password,
             client_id=client_id,
             client_secret=client_secret,
-            use_env_variables=use_env_variables,
         )
         self._user = None
         self._tz_name = None
         self._tz = None
         self._utcoffset = None
 
     @property
```

### Comparing `snowd-0.1.2/snowd/envvars.py` & `snowd-0.1.3/snowd/envvars.py`

 * *Files identical despite different names*

### Comparing `snowd-0.1.2/snowd/git.py` & `snowd-0.1.3/snowd/git.py`

 * *Files identical despite different names*

### Comparing `snowd-0.1.2/snowd/polling.py` & `snowd-0.1.3/snowd/polling.py`

 * *Files identical despite different names*

### Comparing `snowd-0.1.2/snowd/state.py` & `snowd-0.1.3/snowd/state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 
-import click
-
 log = logging.getLogger(__name__)
 
 
 def timestampfilestate(filename):
     file = Path(filename)
 
     lastrun = datetime.fromtimestamp(0)
@@ -32,15 +30,15 @@
         file.write_text(str(int(lastrun.timestamp())))
 
     return get, save
 
 
 @contextmanager
 def timestampfile(filename):
-    now = datetime.utcnow()
+    now = datetime.now(datetime.UTC)
     file = Path(filename)
 
     lastrun = now
     if file.is_file():
         try:
             timestamp = int(file.read_text())
             lastrun = datetime.fromtimestamp(timestamp)
@@ -54,19 +52,7 @@
     with open(file, "w") as f:
         f.write(str(int(now.timestamp())))
     try:
         yield lastrun, savelast
     finally:
         with open(file, "w") as f:
             f.write(str(int(now.timestamp())))
-
-
-@click.command("hello")
-@click.argument("name", default="(anonymous person)")
-@click.option(
-    "-a",
-    "--adjective",
-    type=click.Choice(["handsome", "smart"]),
-    default="handsome",
-)
-def main(name, adjective):
-    print(f"hello {adjective} {name}")
```

### Comparing `snowd-0.1.2/snowd/utils.py` & `snowd-0.1.3/snowd/utils.py`

 * *Files identical despite different names*

### Comparing `snowd-0.1.2/PKG-INFO` & `snowd-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowd
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: David Gallay
 Author-email: david.gallay@nagra.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

