# Comparing `tmp/saucelabs_visual-0.0.5.tar.gz` & `tmp/saucelabs_visual-0.0.6.tar.gz`

## Comparing `saucelabs_visual-0.0.5.tar` & `saucelabs_visual-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/build.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/dev.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/user.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/client.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/regions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/__init__.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/robot.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/.gitignore
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/README.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/requirements/build.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/requirements/dev.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/requirements/user.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/__init__.py
+-rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/client.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/regions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/frameworks/__init__.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/src/saucelabs_visual/frameworks/robot.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/.gitignore
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.6/PKG-INFO
```

### Comparing `saucelabs_visual-0.0.5/src/saucelabs_visual/client.py` & `saucelabs_visual-0.0.6/src/saucelabs_visual/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import environ
 from typing import List, Union
 
 from gql import Client, gql
-from gql.transport.aiohttp import AIOHTTPTransport, BasicAuth
+from gql.transport.requests import RequestsHTTPTransport
+from requests.auth import HTTPBasicAuth
 
 from saucelabs_visual.regions import Region
 from saucelabs_visual.typing import IgnoreRegion, FullPageConfig
 
 
 class SauceLabsVisual:
     client: Client = None
@@ -23,15 +24,15 @@
         if username is None or access_key is None:
             raise Exception(
                 'Sauce Labs credentials not set. Please check that you set correctly your '
                 '`SAUCE_USERNAME` and `SAUCE_ACCESS_KEY` environment variables.'
             )
 
         region_url = Region.from_name(environ.get("SAUCE_REGION") or 'us-west-1').graphql_endpoint
-        transport = AIOHTTPTransport(url=region_url, auth=BasicAuth(username, access_key))
+        transport = RequestsHTTPTransport(url=region_url, auth=HTTPBasicAuth(username, access_key))
         self.client = Client(transport=transport, execute_timeout=90)
 
     def get_client(self) -> Client:
         return self.client
 
     def create_build(
             self,
```

### Comparing `saucelabs_visual-0.0.5/src/saucelabs_visual/regions.py` & `saucelabs_visual-0.0.6/src/saucelabs_visual/regions.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/robot.py` & `saucelabs_visual-0.0.6/src/saucelabs_visual/frameworks/robot.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.5/.gitignore` & `saucelabs_visual-0.0.6/.gitignore`

 * *Files identical despite different names*

