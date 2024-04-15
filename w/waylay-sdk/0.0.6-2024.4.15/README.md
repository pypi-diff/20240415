# Comparing `tmp/waylay-sdk-0.0.6.tar.gz` & `tmp/waylay_sdk-2024.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-0.0.6.tar", last modified: Mon Apr  8 08:05:16 2024, max compression
+gzip compressed data, was "waylay_sdk-2024.4.15.tar", last modified: Mon Apr 15 12:57:09 2024, max compression
```

## Comparing `waylay-sdk-0.0.6.tar` & `waylay_sdk-2024.4.15.tar`

### file list

```diff
@@ -1,47 +1,11 @@
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.766450 waylay-sdk-0.0.6/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-03-26 14:02:35.000000 waylay-sdk-0.0.6/LICENSE.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-04-08 08:05:16.763467 waylay-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     7018 2024-03-28 11:04:55.000000 waylay-sdk-0.0.6/README.md
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1663 2024-04-08 08:03:16.000000 waylay-sdk-0.0.6/pyproject.toml
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-08 08:05:16.766523 waylay-sdk-0.0.6/setup.cfg
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.711405 waylay-sdk-0.0.6/src/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.710230 waylay-sdk-0.0.6/src/waylay/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.715760 waylay-sdk-0.0.6/src/waylay/sdk/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      754 2024-03-28 08:55:26.000000 waylay-sdk-0.0.6/src/waylay/sdk/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       60 2024-04-08 08:03:17.000000 waylay-sdk-0.0.6/src/waylay/sdk/_version.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.719756 waylay-sdk-0.0.6/src/waylay/sdk/api/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      661 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     6130 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/_models.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4423 2024-03-28 08:55:26.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2298 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2299 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/http.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    10842 2024-03-29 09:16:21.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/serialization.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.736117 waylay-sdk-0.0.6/src/waylay/sdk/auth/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      523 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     5972 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/interactive.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    11539 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/parse.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4243 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/provider.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1880 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/client.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.739325 waylay-sdk-0.0.6/src/waylay/sdk/config/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      341 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     3106 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    13667 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2809 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/exceptions.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.748324 waylay-sdk-0.0.6/src/waylay/sdk/plugin/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      229 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4401 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/base.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2373 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      206 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/loader.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2480 2024-03-28 11:04:55.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/type_stubs.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       80 2024-02-13 14:44:08.000000 waylay-sdk-0.0.6/src/waylay/sdk/py.typed
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.748875 waylay-sdk-0.0.6/src/waylay/sdk/services/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4887 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/services/gateway.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.761854 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1071 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       64 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/entry_points.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      441 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/requires.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 12:57:09.446366 waylay_sdk-2024.4.15/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     8303 2024-04-15 12:57:09.446013 waylay_sdk-2024.4.15/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     6769 2024-04-09 09:16:22.000000 waylay_sdk-2024.4.15/README.md
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1190 2024-04-15 12:56:18.000000 waylay_sdk-2024.4.15/pyproject.toml
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 12:57:09.446411 waylay_sdk-2024.4.15/setup.cfg
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 12:57:09.445173 waylay_sdk-2024.4.15/waylay_sdk.egg-info/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     8303 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      193 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      513 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/requires.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 12:57:09.000000 waylay_sdk-2024.4.15/waylay_sdk.egg-info/top_level.txt
```

### Comparing `waylay-sdk-0.0.6/PKG-INFO` & `waylay_sdk-2024.4.15/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,77 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 0.0.6
+Version: 2024.4.15
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
-License: ISC License (ISC)
-        Copyright 2020, Waylay
-        
-        Permission to use, copy, modify, and/or distribute this software for any purpose 
-        with or without fee is hereby granted, provided that the above copyright notice 
-        and this permission notice appear in all copies.
-        
-        THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
-        REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
-        FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
-        OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
-        DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
-        ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
-        
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/
-Project-URL: Repository, https://github.com/waylayio/waylay-sdk-py.git
+Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
+Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
 Keywords: waylay,sdk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: httpx
-Requires-Dist: appdirs
-Requires-Dist: python-jose
-Requires-Dist: python_dateutil
-Requires-Dist: typing_extensions>=4.10.0
-Requires-Dist: typeguard
-Requires-Dist: jsonpath-ng
-Requires-Dist: pydantic>=2.6.0
-Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Requires-Dist: waylay-sdk-alarms
 Requires-Dist: waylay-sdk-data
 Requires-Dist: waylay-sdk-registry
 Requires-Dist: waylay-sdk-resources
 Requires-Dist: waylay-sdk-rules
 Requires-Dist: waylay-sdk-storage
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-mock; extra == "dev"
-Requires-Dist: pytest-httpx; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: starlette; extra == "dev"
-Requires-Dist: syrupy; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: types-python-jose; extra == "dev"
-Requires-Dist: types-appdirs; extra == "dev"
-Requires-Dist: types-python-dateutil; extra == "dev"
-Requires-Dist: docformatter; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: types-alarms
+Requires-Dist: waylay-sdk-alarms-types; extra == "types-alarms"
+Provides-Extra: types-data
+Requires-Dist: waylay-sdk-data-types; extra == "types-data"
+Provides-Extra: types-registry
+Requires-Dist: waylay-sdk-registry-types; extra == "types-registry"
+Provides-Extra: types-resources
+Requires-Dist: waylay-sdk-resources-types; extra == "types-resources"
+Provides-Extra: types-rules
+Requires-Dist: waylay-sdk-rules-types; extra == "types-rules"
+Provides-Extra: types-storage
+Requires-Dist: waylay-sdk-storage-types; extra == "types-storage"
+Provides-Extra: types
+Requires-Dist: waylay-sdk-alarms-types; extra == "types"
+Requires-Dist: waylay-sdk-data-types; extra == "types"
+Requires-Dist: waylay-sdk-registry-types; extra == "types"
+Requires-Dist: waylay-sdk-resources-types; extra == "types"
+Requires-Dist: waylay-sdk-rules-types; extra == "types"
+Requires-Dist: waylay-sdk-storage-types; extra == "types"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
-This `waylay-sdk` package provides a basic SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs). 
+This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
 
-See [Waylay Docs](https://docs.waylay.io/#/api/sdk/python) for documentation.
+It includes api support for the most relevant services, as extensions for the `waylay-sdk-core` base SDK client.
+
+Alternatively:
+* use the [`waylay-sdk-core`](https://pypi.org/project/waylay-sdk-core) package for a minimal SDK client
+* use any of the `waylay-sdk-{service}` packages to install an SDK client that has api support for the selected service(s) only.
+
+
+See [Waylay Docs](https://docs.waylay.io/#/api/sdk/python) for extensive documentation.
 
 ## Installation
 
 This package requires a python runtime `3.9` or higher.
 
-The basic client can be installed with
+The basic client with api support for the [common services](#service-packages), can be installed with
 ```bash
 pip install waylay-sdk
 ```
 
-This client provides basic configuration, authorization and plugin features for the SDK.
-
-It includes a generic http client to make authenticated calls to the services available on your _Waylay_ gateway endpoint.
-
-Support for specific Waylay services or tools is provided by separate [service](#service-packages) and [tool](#tool-packages) packages.
-
-## Basic usage
-
-### In webscripts and plugins
-
-The SDK client can be used in the _python_ webscripts and plugins of the Waylay platform.
-
-In that case, the webscript or plugin _runtime_ will configure and authenticate a client, and 
-provide it as a `waylay` parameter to the _webscript_ or _plugin_ callback function.
-
-You just need to state the required SDK package dependencies when authoring the _webscript_ or _plugin_.
-
-```python
-async def execute(request: Request, waylay: WaylayClient):
-    # list templates with the query as specified in the request body
-    template_query = request.json()
-
-    # with only the 'waylay-sdk' package:
-    templates = await waylay.api_client('GET', '/rules/v1/templates', query=template_query)
-
-    # with the 'waylay-sdk-rules' service plugin package
-    # templates = await waylay.rules.templates.list(query=template_query)
-    return templates
+To additionally [typing](#service-packages) support for a given service, e.g. for the `alarms` service:
+```bash
+pip install waylay-sdk[types-alarms]
 ```
-
-### Interactive Authentication
-When used outside the Waylay platform (e.g. in a _python notebook_) the client requires you to provide
-* the gateway endpoint: `api.waylay.io` for Enterprise users,
-* an API key-secret pair: see [Waylay Console](console.waylay.io) at _>Settings>Authentication keys_.
-
-```python
-from waylay.sdk import WaylayClient
-
-# this will interactively request the gateway and credentials on first usage.
-client = WaylayClient.from_profile()
-
-# list the available service packages
-client.services
-
-# use the generic api client to see the status page of the 'registry' service.
-resp = await client.api_client.request('GET', '/registry/v2')
+... or for all services:
+```bash
+pip install waylay-sdk[types]
 ```
 
-Credentials and endpoints are stored in a local _profile_ file (you can have multiple such profiles).
-Other authentication methods are available (JWToken, pass apiKey/Secret directly)
-
 ## Service packages
 
 Support for a specific Waylay REST api comes as a separate _service package_.
 Each _service_ provides two packages:
 * an _api_ package `waylay-<service>-sdk` that describes all resources and actions for that service. JSON request and responses are represented as basic python data (_dict_, _list_, primitives)
 * a _types_ package `waylay-<service>-sdk-types` that provides [pydantic](https://docs.pydantic.dev/) models to represent JSON request and responses.
 
@@ -136,97 +81,80 @@
 
 Use the _types_ package for interactive cases (python notebooks), or solutions that are regularly tested and maintained. 
 
 When not installed, the SDK client does not interfere with the json representations of requests and responses, and you should check the [API documentation](https://docs.waylay.io/#/api/?id=openapi-docs) of the service for exact specifications.
 
 The Service plugs are _generated_ from their [openapi description](https://docs.waylay.io/#/api/?id=openapi-docs).
 
-### `waylay-sdk-alarms` _Alarms_ api package
+#### Included dependencies
 
-The [waylay-sdk-alarms](https://pypi.org/project/waylay-sdk-alarms) package provides the client bindings for the [Alarms](https://docs.waylay.io/#/api/alarms/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/alarms.html) specification.
+This release of `waylay-sdk` includes the following _api_ and (optional) _types_ packages
 
-```bash
-## with types
-pip install waylay-sdk-alarms[types]
+| name | package | api endpoint | docs | types package 
+| ------- | ------------------ | ------- | --| --|
+| `alarms` | [`waylay-sdk-alarms`](https://pypi.org/project/waylay-sdk-alarms) | `/alarms/v1` | [doc](https://docs.waylay.io/#/api/alarms/) [openapi](https://docs.waylay.io/openapi/public/redocly/alarms.html) | [`waylay-sdk-alarms-types`](https://pypi.org/project/waylay-sdk-alarms-types/) |
+| `data` | [`waylay-sdk-data`](https://pypi.org/project/waylay-sdk-data) | `/data/v1` | [doc](https://docs.waylay.io/#/api/broker/) [openapi](https://docs.waylay.io/openapi/public/redocly/data.html) | [`waylay-sdk-data-types`](https://pypi.org/project/waylay-sdk-data-types/) |
+| `registry` | [`waylay-sdk-registry`](https://pypi.org/project/waylay-sdk-registry) | `/registry/v2` | [doc](https://docs.waylay.io/#/api/registry/) [openapi](https://docs.waylay.io/openapi/public/redocly/registry.html) | [`waylay-sdk-registry-types`](https://pypi.org/project/waylay-sdk-registry-types/) |
+| `resources` | [`waylay-resources-alarms`](https://pypi.org/project/waylay-sdk-resources) | `/resources/v1` | [doc](https://docs.waylay.io/#/api/resources/) [openapi](https://docs.waylay.io/openapi/public/resources/alarms.html) | [`waylay-sdk-resources-types`](https://pypi.org/project/waylay-sdk-resources-types/) |
+| `rules` | [`waylay-sdk-rules`](https://pypi.org/project/waylay-sdk-rules) | `/rules/v1` | [doc](https://docs.waylay.io/#/api/rules/) [openapi](https://docs.waylay.io/openapi/public/redocly/rules.html) | [`waylay-sdk-rules-types`](https://pypi.org/project/waylay-sdk-rules-types/) |
+| `storage` | [`waylay-sdk-storage`](https://pypi.org/project/waylay-sdk-storage) | `/storage/v1` | [doc](https://docs.waylay.io/#/api/storage/) [openapi](https://docs.waylay.io/openapi/public/redocly/storage.html) | [`waylay-sdk-storage-types`](https://pypi.org/project/waylay-sdk-storage-types/) |
 
-## without types
-pip install waylay-sdk-alarms
-```
 
-### `waylay-sdk-data` _Data_ (broker) api package
 
-The [waylay-sdk-data](https://pypi.org/project/waylay-sdk-data) package provides the client bindings for the `data` api of the [broker](https://docs.waylay.io/#/api/broker/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/broker.html) specification.
+## Basic usage
 
-```bash
-## with types
-pip install waylay-sdk-data[types]
+### In webscripts and plugins
 
-## without types
-pip install waylay-sdk-data
-```
+The SDK client can be used in the _python_ webscripts and plugins of the Waylay platform.
 
-### `waylay-sdk-resources` _Resources_ (digital twin) api package
+In that case, the webscript or plugin _runtime_ will configure and authenticate a client, and 
+provide it as a `waylay` parameter to the _webscript_ or _plugin_ callback function.
 
-The [waylay-sdk-resources](https://pypi.org/project/waylay-sdk-resources) package provides the client bindings for the [resources](https://docs.waylay.io/#/api/resources/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/resources.html) specification.
+You just need to state the `waylay-sdk` dependency when authoring the _webscript_ or _plugin_.
 
-```bash
-## with types
-pip install waylay-sdk-resources[types]
 
-## without types
-pip install waylay-sdk-resources
+#### webscript example
+```python
+async def execute(request: Request, waylay: WaylayClient):
+    # list templates with the query as specified in the request body
+    template_query = request.json()
+    templates = await waylay.rules.templates.list(query=template_query)
+    return templates
 ```
 
-### `waylay-sdk-rules` _Rules_ (rules engine) api package
-
-The [waylay-sdk-rules](https://pypi.org/project/waylay-sdk-rules) package provides the client bindings for the [rules](https://docs.waylay.io/#/api/rules/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/rules.html) specification.
-
-```bash
-## with types
-pip install waylay-sdk-rules[types]
-
-## without types
-pip install waylay-sdk-rules
+#### plug example
+```python
+from csv import DictReader
+from io import StringIO
+async def execute(path: str, waylay: WaylayClient):
+    """Return the CSV data from a file in assets storage."""
+    # use the _List Objects_ operation, using the `path` plug property
+    sign_resp = await waylay.storage.objects.list('assets', path, query={"sign": "GET"})
+    content_url = sign_resp._links.get_object.href
+    # fetch the csv data with the generic rest client, disable waylay auth for this signed url
+    csv_data = await waylay.api_client.request('GET', content_url, auth=None)
+    # parse as csv and return as a (state, rawData) tuple
+    return ('OK', data=[
+        record for record in DictReader(StringIO(csv_data))
+    ])
 ```
 
-### `waylay-sdk-storage` _Storage_ (file object storage) api package
-
-The [waylay-sdk-storage](https://pypi.org/project/waylay-sdk-storage) package provides the client bindings for the [storage](https://docs.waylay.io/#/api/storage/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/storage.html) specification.
-
-```bash
-## with types
-pip install waylay-sdk-storage[types]
-
-## without types
-pip install waylay-sdk-storage
-```
+### Interactive Authentication
+When used outside the Waylay platform (e.g. in a _python notebook_) the client requires you to provide
+* the gateway endpoint: `api.waylay.io` for Enterprise users,
+* an API key-secret pair: see [Waylay Console](console.waylay.io) at _>Settings>Authentication keys_.
 
-### `waylay-sdk-registry` _Function Registry V2_ api package
+```python
+from waylay.sdk import WaylayClient
 
-The [waylay-sdk-registry](https://pypi.org/project/waylay-sdk-registry) package provides the client bindings for the [registry v2](https://docs.waylay.io/#/api/registry/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/registry.html) specification.
+# this will interactively request the gateway and credentials on first usage.
+client = WaylayClient.from_profile()
 
-```bash
-## with types
-pip install waylay-sdk-registry[types]
+# list the available service packages
+client.services
 
-## without types
-pip install waylay-sdk-registry
+# use the generic api client to see the status page of the 'registry' service.
+resp = await client.api_client.request('GET', '/registry/v2')
 ```
 
-
-## Tool packages
-
-Tool packages provide SDK extensions for specific use cases.
-
-
-### `waylay-sdk-ml-adapter` _ML Adapter_ tool package
-
-The [waylay-sdk-ml-adapter](https://pypi.org/project/waylay-sdk-ml-adapter) package provides utilities for using and deploying Machine Learning models in plugs and webscripts.
-
-```bash
-## basic install
-pip install waylay-sdk-ml-adapter
-
-## install with support for pytorch models
-pip install waylay-sdk-ml-adapter[pytorch]
-
-```
+Credentials and endpoints are stored in a local _profile_ file (you can have multiple such profiles).
+Other authentication methods are available (JWToken, pass apiKey/Secret directly)
```

### Comparing `waylay-sdk-0.0.6/README.md` & `waylay_sdk-2024.4.15/waylay_sdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,77 @@
+Metadata-Version: 2.1
+Name: waylay-sdk
+Version: 2024.4.15
+Summary: Waylay Python SDK.
+Author-email: Waylay <info@waylay.io>
+Project-URL: Homepage, https://www.waylay.io/
+Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
+Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
+Keywords: waylay,sdk
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: waylay-sdk-alarms
+Requires-Dist: waylay-sdk-data
+Requires-Dist: waylay-sdk-registry
+Requires-Dist: waylay-sdk-resources
+Requires-Dist: waylay-sdk-rules
+Requires-Dist: waylay-sdk-storage
+Provides-Extra: types-alarms
+Requires-Dist: waylay-sdk-alarms-types; extra == "types-alarms"
+Provides-Extra: types-data
+Requires-Dist: waylay-sdk-data-types; extra == "types-data"
+Provides-Extra: types-registry
+Requires-Dist: waylay-sdk-registry-types; extra == "types-registry"
+Provides-Extra: types-resources
+Requires-Dist: waylay-sdk-resources-types; extra == "types-resources"
+Provides-Extra: types-rules
+Requires-Dist: waylay-sdk-rules-types; extra == "types-rules"
+Provides-Extra: types-storage
+Requires-Dist: waylay-sdk-storage-types; extra == "types-storage"
+Provides-Extra: types
+Requires-Dist: waylay-sdk-alarms-types; extra == "types"
+Requires-Dist: waylay-sdk-data-types; extra == "types"
+Requires-Dist: waylay-sdk-registry-types; extra == "types"
+Requires-Dist: waylay-sdk-resources-types; extra == "types"
+Requires-Dist: waylay-sdk-rules-types; extra == "types"
+Requires-Dist: waylay-sdk-storage-types; extra == "types"
+
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
-This `waylay-sdk` package provides a basic SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs). 
+This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
+
+It includes api support for the most relevant services, as extensions for the `waylay-sdk-core` base SDK client.
+
+Alternatively:
+* use the [`waylay-sdk-core`](https://pypi.org/project/waylay-sdk-core) package for a minimal SDK client
+* use any of the `waylay-sdk-{service}` packages to install an SDK client that has api support for the selected service(s) only.
 
-See [Waylay Docs](https://docs.waylay.io/#/api/sdk/python) for documentation.
+
+See [Waylay Docs](https://docs.waylay.io/#/api/sdk/python) for extensive documentation.
 
 ## Installation
 
 This package requires a python runtime `3.9` or higher.
 
-The basic client can be installed with
+The basic client with api support for the [common services](#service-packages), can be installed with
 ```bash
 pip install waylay-sdk
 ```
 
-This client provides basic configuration, authorization and plugin features for the SDK.
-
-It includes a generic http client to make authenticated calls to the services available on your _Waylay_ gateway endpoint.
-
-Support for specific Waylay services or tools is provided by separate [service](#service-packages) and [tool](#tool-packages) packages.
-
-## Basic usage
-
-### In webscripts and plugins
-
-The SDK client can be used in the _python_ webscripts and plugins of the Waylay platform.
-
-In that case, the webscript or plugin _runtime_ will configure and authenticate a client, and 
-provide it as a `waylay` parameter to the _webscript_ or _plugin_ callback function.
-
-You just need to state the required SDK package dependencies when authoring the _webscript_ or _plugin_.
-
-```python
-async def execute(request: Request, waylay: WaylayClient):
-    # list templates with the query as specified in the request body
-    template_query = request.json()
-
-    # with only the 'waylay-sdk' package:
-    templates = await waylay.api_client('GET', '/rules/v1/templates', query=template_query)
-
-    # with the 'waylay-sdk-rules' service plugin package
-    # templates = await waylay.rules.templates.list(query=template_query)
-    return templates
+To additionally [typing](#service-packages) support for a given service, e.g. for the `alarms` service:
+```bash
+pip install waylay-sdk[types-alarms]
 ```
-
-### Interactive Authentication
-When used outside the Waylay platform (e.g. in a _python notebook_) the client requires you to provide
-* the gateway endpoint: `api.waylay.io` for Enterprise users,
-* an API key-secret pair: see [Waylay Console](console.waylay.io) at _>Settings>Authentication keys_.
-
-```python
-from waylay.sdk import WaylayClient
-
-# this will interactively request the gateway and credentials on first usage.
-client = WaylayClient.from_profile()
-
-# list the available service packages
-client.services
-
-# use the generic api client to see the status page of the 'registry' service.
-resp = await client.api_client.request('GET', '/registry/v2')
+... or for all services:
+```bash
+pip install waylay-sdk[types]
 ```
 
-Credentials and endpoints are stored in a local _profile_ file (you can have multiple such profiles).
-Other authentication methods are available (JWToken, pass apiKey/Secret directly)
-
 ## Service packages
 
 Support for a specific Waylay REST api comes as a separate _service package_.
 Each _service_ provides two packages:
 * an _api_ package `waylay-<service>-sdk` that describes all resources and actions for that service. JSON request and responses are represented as basic python data (_dict_, _list_, primitives)
 * a _types_ package `waylay-<service>-sdk-types` that provides [pydantic](https://docs.pydantic.dev/) models to represent JSON request and responses.
 
@@ -79,97 +81,80 @@
 
 Use the _types_ package for interactive cases (python notebooks), or solutions that are regularly tested and maintained. 
 
 When not installed, the SDK client does not interfere with the json representations of requests and responses, and you should check the [API documentation](https://docs.waylay.io/#/api/?id=openapi-docs) of the service for exact specifications.
 
 The Service plugs are _generated_ from their [openapi description](https://docs.waylay.io/#/api/?id=openapi-docs).
 
-### `waylay-sdk-alarms` _Alarms_ api package
+#### Included dependencies
 
-The [waylay-sdk-alarms](https://pypi.org/project/waylay-sdk-alarms) package provides the client bindings for the [Alarms](https://docs.waylay.io/#/api/alarms/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/alarms.html) specification.
+This release of `waylay-sdk` includes the following _api_ and (optional) _types_ packages
 
-```bash
-## with types
-pip install waylay-sdk-alarms[types]
+| name | package | api endpoint | docs | types package 
+| ------- | ------------------ | ------- | --| --|
+| `alarms` | [`waylay-sdk-alarms`](https://pypi.org/project/waylay-sdk-alarms) | `/alarms/v1` | [doc](https://docs.waylay.io/#/api/alarms/) [openapi](https://docs.waylay.io/openapi/public/redocly/alarms.html) | [`waylay-sdk-alarms-types`](https://pypi.org/project/waylay-sdk-alarms-types/) |
+| `data` | [`waylay-sdk-data`](https://pypi.org/project/waylay-sdk-data) | `/data/v1` | [doc](https://docs.waylay.io/#/api/broker/) [openapi](https://docs.waylay.io/openapi/public/redocly/data.html) | [`waylay-sdk-data-types`](https://pypi.org/project/waylay-sdk-data-types/) |
+| `registry` | [`waylay-sdk-registry`](https://pypi.org/project/waylay-sdk-registry) | `/registry/v2` | [doc](https://docs.waylay.io/#/api/registry/) [openapi](https://docs.waylay.io/openapi/public/redocly/registry.html) | [`waylay-sdk-registry-types`](https://pypi.org/project/waylay-sdk-registry-types/) |
+| `resources` | [`waylay-resources-alarms`](https://pypi.org/project/waylay-sdk-resources) | `/resources/v1` | [doc](https://docs.waylay.io/#/api/resources/) [openapi](https://docs.waylay.io/openapi/public/resources/alarms.html) | [`waylay-sdk-resources-types`](https://pypi.org/project/waylay-sdk-resources-types/) |
+| `rules` | [`waylay-sdk-rules`](https://pypi.org/project/waylay-sdk-rules) | `/rules/v1` | [doc](https://docs.waylay.io/#/api/rules/) [openapi](https://docs.waylay.io/openapi/public/redocly/rules.html) | [`waylay-sdk-rules-types`](https://pypi.org/project/waylay-sdk-rules-types/) |
+| `storage` | [`waylay-sdk-storage`](https://pypi.org/project/waylay-sdk-storage) | `/storage/v1` | [doc](https://docs.waylay.io/#/api/storage/) [openapi](https://docs.waylay.io/openapi/public/redocly/storage.html) | [`waylay-sdk-storage-types`](https://pypi.org/project/waylay-sdk-storage-types/) |
 
-## without types
-pip install waylay-sdk-alarms
-```
 
-### `waylay-sdk-data` _Data_ (broker) api package
 
-The [waylay-sdk-data](https://pypi.org/project/waylay-sdk-data) package provides the client bindings for the `data` api of the [broker](https://docs.waylay.io/#/api/broker/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/broker.html) specification.
+## Basic usage
 
-```bash
-## with types
-pip install waylay-sdk-data[types]
+### In webscripts and plugins
 
-## without types
-pip install waylay-sdk-data
-```
+The SDK client can be used in the _python_ webscripts and plugins of the Waylay platform.
 
-### `waylay-sdk-resources` _Resources_ (digital twin) api package
+In that case, the webscript or plugin _runtime_ will configure and authenticate a client, and 
+provide it as a `waylay` parameter to the _webscript_ or _plugin_ callback function.
 
-The [waylay-sdk-resources](https://pypi.org/project/waylay-sdk-resources) package provides the client bindings for the [resources](https://docs.waylay.io/#/api/resources/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/resources.html) specification.
+You just need to state the `waylay-sdk` dependency when authoring the _webscript_ or _plugin_.
 
-```bash
-## with types
-pip install waylay-sdk-resources[types]
 
-## without types
-pip install waylay-sdk-resources
+#### webscript example
+```python
+async def execute(request: Request, waylay: WaylayClient):
+    # list templates with the query as specified in the request body
+    template_query = request.json()
+    templates = await waylay.rules.templates.list(query=template_query)
+    return templates
 ```
 
-### `waylay-sdk-rules` _Rules_ (rules engine) api package
-
-The [waylay-sdk-rules](https://pypi.org/project/waylay-sdk-rules) package provides the client bindings for the [rules](https://docs.waylay.io/#/api/rules/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/rules.html) specification.
-
-```bash
-## with types
-pip install waylay-sdk-rules[types]
-
-## without types
-pip install waylay-sdk-rules
+#### plug example
+```python
+from csv import DictReader
+from io import StringIO
+async def execute(path: str, waylay: WaylayClient):
+    """Return the CSV data from a file in assets storage."""
+    # use the _List Objects_ operation, using the `path` plug property
+    sign_resp = await waylay.storage.objects.list('assets', path, query={"sign": "GET"})
+    content_url = sign_resp._links.get_object.href
+    # fetch the csv data with the generic rest client, disable waylay auth for this signed url
+    csv_data = await waylay.api_client.request('GET', content_url, auth=None)
+    # parse as csv and return as a (state, rawData) tuple
+    return ('OK', data=[
+        record for record in DictReader(StringIO(csv_data))
+    ])
 ```
 
-### `waylay-sdk-storage` _Storage_ (file object storage) api package
-
-The [waylay-sdk-storage](https://pypi.org/project/waylay-sdk-storage) package provides the client bindings for the [storage](https://docs.waylay.io/#/api/storage/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/storage.html) specification.
-
-```bash
-## with types
-pip install waylay-sdk-storage[types]
-
-## without types
-pip install waylay-sdk-storage
-```
+### Interactive Authentication
+When used outside the Waylay platform (e.g. in a _python notebook_) the client requires you to provide
+* the gateway endpoint: `api.waylay.io` for Enterprise users,
+* an API key-secret pair: see [Waylay Console](console.waylay.io) at _>Settings>Authentication keys_.
 
-### `waylay-sdk-registry` _Function Registry V2_ api package
+```python
+from waylay.sdk import WaylayClient
 
-The [waylay-sdk-registry](https://pypi.org/project/waylay-sdk-registry) package provides the client bindings for the [registry v2](https://docs.waylay.io/#/api/registry/) service, based on its [openapi](https://docs.waylay.io/openapi/public/redocly/registry.html) specification.
+# this will interactively request the gateway and credentials on first usage.
+client = WaylayClient.from_profile()
 
-```bash
-## with types
-pip install waylay-sdk-registry[types]
+# list the available service packages
+client.services
 
-## without types
-pip install waylay-sdk-registry
+# use the generic api client to see the status page of the 'registry' service.
+resp = await client.api_client.request('GET', '/registry/v2')
 ```
 
-
-## Tool packages
-
-Tool packages provide SDK extensions for specific use cases.
-
-
-### `waylay-sdk-ml-adapter` _ML Adapter_ tool package
-
-The [waylay-sdk-ml-adapter](https://pypi.org/project/waylay-sdk-ml-adapter) package provides utilities for using and deploying Machine Learning models in plugs and webscripts.
-
-```bash
-## basic install
-pip install waylay-sdk-ml-adapter
-
-## install with support for pytorch models
-pip install waylay-sdk-ml-adapter[pytorch]
-
-```
+Credentials and endpoints are stored in a local _profile_ file (you can have multiple such profiles).
+Other authentication methods are available (JWToken, pass apiKey/Secret directly)
```

