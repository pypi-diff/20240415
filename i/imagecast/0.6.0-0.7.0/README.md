# Comparing `tmp/imagecast-0.6.0.tar.gz` & `tmp/imagecast-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagecast-0.6.0.tar", last modified: Tue Dec 19 23:58:46 2023, max compression
+gzip compressed data, was "imagecast-0.7.0.tar", last modified: Mon Apr 15 21:01:23 2024, max compression
```

## Comparing `imagecast-0.6.0.tar` & `imagecast-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-12-19 23:58:46.077594 imagecast-0.6.0/
--rw-r--r--   0 amo        (501) staff       (20)    32386 2021-03-06 10:22:35.000000 imagecast-0.6.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)     5666 2023-12-19 23:58:46.077206 imagecast-0.6.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3257 2023-12-19 23:57:45.000000 imagecast-0.6.0/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-12-19 23:58:46.073035 imagecast-0.6.0/imagecast/
--rw-r--r--   0 amo        (501) staff       (20)      152 2023-12-19 23:58:35.000000 imagecast-0.6.0/imagecast/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     3312 2021-03-06 10:55:16.000000 imagecast-0.6.0/imagecast/api.py
--rw-r--r--   0 amo        (501) staff       (20)     3399 2023-12-19 23:57:45.000000 imagecast-0.6.0/imagecast/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     3593 2023-12-19 23:57:45.000000 imagecast-0.6.0/imagecast/core.py
--rw-r--r--   0 amo        (501) staff       (20)     1129 2021-03-06 10:55:16.000000 imagecast-0.6.0/imagecast/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-12-19 23:58:46.076378 imagecast-0.6.0/imagecast.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     5666 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      384 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       48 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-03-06 10:26:56.000000 imagecast-0.6.0/imagecast.egg-info/not-zip-safe
--rw-r--r--   0 amo        (501) staff       (20)      138 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       10 2023-12-19 23:58:46.000000 imagecast-0.6.0/imagecast.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)      182 2023-01-17 22:09:54.000000 imagecast-0.6.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-12-19 23:58:46.077691 imagecast-0.6.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     2908 2023-12-19 23:58:35.000000 imagecast-0.6.0/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-12-19 23:58:46.075959 imagecast-0.6.0/test/
--rw-r--r--   0 amo        (501) staff       (20)     3056 2023-12-19 23:57:45.000000 imagecast-0.6.0/test/test_core.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-15 21:01:23.542398 imagecast-0.7.0/
+-rw-r--r--   0 amo        (501) staff       (20)    32386 2021-03-06 10:22:35.000000 imagecast-0.7.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     6338 2024-04-15 21:01:23.541961 imagecast-0.7.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3862 2024-04-15 02:12:08.000000 imagecast-0.7.0/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-15 21:01:23.535543 imagecast-0.7.0/imagecast/
+-rw-r--r--   0 amo        (501) staff       (20)      152 2024-04-15 21:01:17.000000 imagecast-0.7.0/imagecast/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     3605 2024-04-15 21:00:32.000000 imagecast-0.7.0/imagecast/api.py
+-rw-r--r--   0 amo        (501) staff       (20)     3409 2024-04-15 02:12:08.000000 imagecast-0.7.0/imagecast/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     3704 2024-04-15 02:12:08.000000 imagecast-0.7.0/imagecast/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     1129 2021-03-06 10:55:16.000000 imagecast-0.7.0/imagecast/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-15 21:01:23.540887 imagecast-0.7.0/imagecast.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     6338 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      418 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       48 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2021-03-06 10:26:56.000000 imagecast-0.7.0/imagecast.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (501) staff       (20)      208 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       10 2024-04-15 21:01:23.000000 imagecast-0.7.0/imagecast.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)      206 2024-04-15 02:12:08.000000 imagecast-0.7.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-15 21:01:23.542485 imagecast-0.7.0/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     2954 2024-04-15 21:01:17.000000 imagecast-0.7.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-15 21:01:23.540495 imagecast-0.7.0/test/
+-rw-r--r--   0 amo        (501) staff       (20)     1759 2024-04-15 02:12:08.000000 imagecast-0.7.0/test/test_api.py
+-rw-r--r--   0 amo        (501) staff       (20)     1706 2024-04-15 02:12:08.000000 imagecast-0.7.0/test/test_cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     2909 2024-04-15 00:28:38.000000 imagecast-0.7.0/test/test_core.py
```

### Comparing `imagecast-0.6.0/LICENSE` & `imagecast-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imagecast-0.6.0/PKG-INFO` & `imagecast-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: imagecast
-Version: 0.6.0
+Version: 0.7.0
 Summary: Imagecast is like ImageMagick but for Pythonistas. Optionally provides its features via HTTP API.
 Home-page: https://github.com/panodata/imagecast
 Author: Andreas Motl
 Author-email: andreas.motl@panodata.org
 License: AGPL 3, EUPL 1.2
 Keywords: image conversion http api proxy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -38,49 +37,60 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
-Requires-Dist: docopt<1,>=0.6
+Requires-Dist: typing-extensions<5; python_version < "3.9"
+Requires-Dist: docopt-ng<1,>=0.6
 Requires-Dist: munch<5,>=2.3
 Requires-Dist: Pillow<11,>=8
-Requires-Dist: playwright<1.41
+Requires-Dist: playwright<1.44
 Requires-Dist: requests<3,>=2.23
 Requires-Dist: requests-cache<2,>=0.5
 Provides-Extra: service
-Requires-Dist: fastapi<0.106; extra == "service"
-Requires-Dist: uvicorn<0.25; extra == "service"
+Requires-Dist: fastapi<0.111; extra == "service"
+Requires-Dist: pydantic-settings<3; extra == "service"
+Requires-Dist: uvicorn<0.30; extra == "service"
 
-.. image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
+#########
+Imagecast
+#########
+
+|
+
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/panodata/imagecast/actions/workflows/tests.yml
 
-.. image:: https://img.shields.io/pypi/pyversions/imagecast.svg
+.. |ci-coverage| image:: https://codecov.io/gh/panodata/imagecast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/panodata/imagecast
+    :alt: Test suite code coverage
+
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/imagecast.svg
     :target: https://python.org
 
-.. image:: https://img.shields.io/pypi/v/imagecast.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/status/imagecast.svg
+.. |status| image:: https://img.shields.io/pypi/status/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/l/imagecast.svg
+.. |license| image:: https://img.shields.io/pypi/l/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://static.pepy.tech/badge/imagecast/month
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/imagecast/month
     :target: https://pepy.tech/project/imagecast
 
-|
-
-.. imagecast-readme:
-
-#########
-Imagecast
-#########
+.. end-badges
 
 
 *****
 About
 *****
 
 Imagecast is like ImageMagick but for Pythonistas. Optionally provides its
@@ -179,14 +189,18 @@
     You should not run the service without restricting the
     list of allowed remote hosts on the public internet.
 
     To do that, invoke the service like::
 
         imagecast service --allowed-hosts=unsplash.com,media.example.org
 
+    By default, no host will be allowed. If you really need to enable access
+    to all upstream hosts, use ``--allowed-hosts=*``. All host names must be
+    listed explicitly, wildcard notations like ``*.iana.org`` are not permitted.
+
 
 **************
 Other projects
 **************
 
 - https://github.com/DictGet/ecce-homo
 - https://github.com/agschwender/pilbox
```

### Comparing `imagecast-0.6.0/README.rst` & `imagecast-0.7.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-.. image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
+#########
+Imagecast
+#########
+
+|
+
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/panodata/imagecast/actions/workflows/tests.yml
 
-.. image:: https://img.shields.io/pypi/pyversions/imagecast.svg
+.. |ci-coverage| image:: https://codecov.io/gh/panodata/imagecast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/panodata/imagecast
+    :alt: Test suite code coverage
+
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/imagecast.svg
     :target: https://python.org
 
-.. image:: https://img.shields.io/pypi/v/imagecast.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/status/imagecast.svg
+.. |status| image:: https://img.shields.io/pypi/status/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/l/imagecast.svg
+.. |license| image:: https://img.shields.io/pypi/l/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://static.pepy.tech/badge/imagecast/month
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/imagecast/month
     :target: https://pepy.tech/project/imagecast
 
-|
-
-.. imagecast-readme:
-
-#########
-Imagecast
-#########
+.. end-badges
 
 
 *****
 About
 *****
 
 Imagecast is like ImageMagick but for Pythonistas. Optionally provides its
@@ -125,14 +134,18 @@
     You should not run the service without restricting the
     list of allowed remote hosts on the public internet.
 
     To do that, invoke the service like::
 
         imagecast service --allowed-hosts=unsplash.com,media.example.org
 
+    By default, no host will be allowed. If you really need to enable access
+    to all upstream hosts, use ``--allowed-hosts=*``. All host names must be
+    listed explicitly, wildcard notations like ``*.iana.org`` are not permitted.
+
 
 **************
 Other projects
 **************
 
 - https://github.com/DictGet/ecce-homo
 - https://github.com/agschwender/pilbox
```

### Comparing `imagecast-0.6.0/imagecast/api.py` & `imagecast-0.7.0/imagecast/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 # -*- coding: utf-8 -*-
 # (c) 2020-2021 Andreas Motl <andreas@terkin.org>
 # License: GNU Affero General Public License, Version 3
 import logging
+import sys
 from dataclasses import dataclass
+from functools import lru_cache
 from typing import List
 from urllib.parse import urlparse
 
 from fastapi import Depends, FastAPI, HTTPException, Query
 from fastapi.responses import HTMLResponse, PlainTextResponse, Response
 from PIL import Image
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 from starlette.status import HTTP_403_FORBIDDEN
 
 from imagecast import __appname__, __version__
 from imagecast.core import process
 
 
+if sys.version_info < (3, 9):
+    from typing_extensions import Annotated
+else:
+    from typing import Annotated
+
+
 # https://fastapi.tiangolo.com/advanced/settings/
 class Settings(BaseSettings):
     allowed_hosts: List[str] = []
 
 
-settings = Settings()
+@lru_cache
+def get_settings():
+    return Settings()
+
+
 app = FastAPI()
 
 log = logging.getLogger(__name__)
 
 
 # Using pydantic models for GET request query params.
 # https://github.com/tiangolo/fastapi/issues/318#issuecomment-584020926
 @dataclass
 class QueryOptions:
     uri: str = Query(default=None)
+    element: str = Query(default=None)
     monochrome: int = Query(default=None)
     grayscale: bool = Query(default=False)
     crop: str = Query(default=None)
     width: int = Query(default=None)
     height: int = Query(default=None)
     dpi: int = Query(default=72)
     format: str = Query(default=None)
     cache_ttl: int = Query(default=300)
 
 
 @app.get("/")
-def index(options: QueryOptions = Depends(QueryOptions)):
+def index(settings: Annotated[Settings, Depends(get_settings)], options: QueryOptions = Depends(QueryOptions)):
     appname = f"{__appname__} {__version__}"
     about = "Imagecast is like ImageMagick but for Pythonistas. Optionally provides its features via HTTP API."
 
     if options.uri:
 
         # Protect the service from accessing arbitrary remote URIs.
         uri_parsed = urlparse(options.uri.encode("utf-8"))
```

### Comparing `imagecast-0.6.0/imagecast/cli.py` & `imagecast-0.7.0/imagecast/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def run():
     """
     Imagecast modifies images, optionally serving them via HTTP API.
 
     Usage:
-      imagecast --uri=<uri> [--element=] [--monochrome=<threshold>] [--grayscale] [--width=<width>] [--height=<height>] [--crop=<cropbox>] [--display] [--format=<format>] [--dpi=<dpi>] [--save=<save>]
+      imagecast --uri=<uri> [--element=] [--monochrome=<threshold>] [--grayscale] [--width=<width>] [--height=<height>] [--crop=<cropbox>] [--display] [--format=<format>] [--dpi=<dpi>] [--save=<save>] [--debug]
       imagecast service [--listen=<listen>] [--allowed-hosts=<allowed-hosts>] [--reload]
       imagecast --version
       imagecast (-h | --help)
 
     Options:
       --uri=<uri>                       URI to image
       --element=<selector>              When URI points to a HTML resource, use this expression as DOM element selector
```

### Comparing `imagecast-0.6.0/imagecast/core.py` & `imagecast-0.7.0/imagecast/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # -*- coding: utf-8 -*-
 # (c) 2020-2021 Andreas Motl <andreas@hiveeyes.org>
 # License: GNU Affero General Public License, Version 3
 import io
+import logging
 import tempfile
 
 import requests
 from PIL import Image
 from requests_cache import CachedSession
 
 
+logger = logging.getLogger(__name__)
+
+
 class ImageEngine:
 
     http = None
 
     def __init__(self, cache_ttl=300):
         self.response: requests.Response = None
         self.data = None
@@ -94,14 +98,17 @@
         buffer = io.BytesIO()
         self.image.save(buffer, format=format, dpi=(dpi, dpi))
         return buffer.getvalue()
 
 
 def process(options):
     ie = ImageEngine(cache_ttl=options.cache_ttl)
+
+    logger.info(f"Acquiring image from {options.uri}")
+
     ie.acquire(options.uri, options.element)
     ie.read()
 
     if options.monochrome:
         ie.monochrome(int(options.monochrome))
 
     if options.grayscale:
```

### Comparing `imagecast-0.6.0/imagecast/util.py` & `imagecast-0.7.0/imagecast/util.py`

 * *Files identical despite different names*

### Comparing `imagecast-0.6.0/imagecast.egg-info/PKG-INFO` & `imagecast-0.7.0/imagecast.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: imagecast
-Version: 0.6.0
+Version: 0.7.0
 Summary: Imagecast is like ImageMagick but for Pythonistas. Optionally provides its features via HTTP API.
 Home-page: https://github.com/panodata/imagecast
 Author: Andreas Motl
 Author-email: andreas.motl@panodata.org
 License: AGPL 3, EUPL 1.2
 Keywords: image conversion http api proxy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -38,49 +37,60 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
-Requires-Dist: docopt<1,>=0.6
+Requires-Dist: typing-extensions<5; python_version < "3.9"
+Requires-Dist: docopt-ng<1,>=0.6
 Requires-Dist: munch<5,>=2.3
 Requires-Dist: Pillow<11,>=8
-Requires-Dist: playwright<1.41
+Requires-Dist: playwright<1.44
 Requires-Dist: requests<3,>=2.23
 Requires-Dist: requests-cache<2,>=0.5
 Provides-Extra: service
-Requires-Dist: fastapi<0.106; extra == "service"
-Requires-Dist: uvicorn<0.25; extra == "service"
+Requires-Dist: fastapi<0.111; extra == "service"
+Requires-Dist: pydantic-settings<3; extra == "service"
+Requires-Dist: uvicorn<0.30; extra == "service"
 
-.. image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
+#########
+Imagecast
+#########
+
+|
+
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/panodata/imagecast/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/panodata/imagecast/actions/workflows/tests.yml
 
-.. image:: https://img.shields.io/pypi/pyversions/imagecast.svg
+.. |ci-coverage| image:: https://codecov.io/gh/panodata/imagecast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/panodata/imagecast
+    :alt: Test suite code coverage
+
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/imagecast.svg
     :target: https://python.org
 
-.. image:: https://img.shields.io/pypi/v/imagecast.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/status/imagecast.svg
+.. |status| image:: https://img.shields.io/pypi/status/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://img.shields.io/pypi/l/imagecast.svg
+.. |license| image:: https://img.shields.io/pypi/l/imagecast.svg
     :target: https://pypi.org/project/imagecast/
 
-.. image:: https://static.pepy.tech/badge/imagecast/month
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/imagecast/month
     :target: https://pepy.tech/project/imagecast
 
-|
-
-.. imagecast-readme:
-
-#########
-Imagecast
-#########
+.. end-badges
 
 
 *****
 About
 *****
 
 Imagecast is like ImageMagick but for Pythonistas. Optionally provides its
@@ -179,14 +189,18 @@
     You should not run the service without restricting the
     list of allowed remote hosts on the public internet.
 
     To do that, invoke the service like::
 
         imagecast service --allowed-hosts=unsplash.com,media.example.org
 
+    By default, no host will be allowed. If you really need to enable access
+    to all upstream hosts, use ``--allowed-hosts=*``. All host names must be
+    listed explicitly, wildcard notations like ``*.iana.org`` are not permitted.
+
 
 **************
 Other projects
 **************
 
 - https://github.com/DictGet/ecce-homo
 - https://github.com/agschwender/pilbox
```

### Comparing `imagecast-0.6.0/setup.py` & `imagecast-0.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst")).read()
 
 setup(name="imagecast",
-      version="0.6.0",
+      version="0.7.0",
       description="Imagecast is like ImageMagick but for Pythonistas. Optionally provides its features via HTTP API.",
       long_description=README,
       license="AGPL 3, EUPL 1.2",
       classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: GNU Affero General Public License v3",
@@ -52,25 +51,27 @@
       keywords="image conversion http api proxy",
       packages=find_packages(),
       include_package_data=True,
       package_data={
       },
       zip_safe=False,
       install_requires=[
-          "docopt>=0.6,<1",
+          "typing-extensions<5; python_version<'3.9'",
+          "docopt-ng>=0.6,<1",
           "munch>=2.3,<5",
           "Pillow>=8,<11",
-          "playwright<1.41",
+          "playwright<1.44",
           "requests>=2.23,<3",
           "requests-cache>=0.5,<2",
       ],
       extras_require={
           "service": [
-              "fastapi<0.106",
-              "uvicorn<0.25",
+              "fastapi<0.111",
+              "pydantic-settings<3",
+              "uvicorn<0.30",
           ],
       },
       entry_points={
           "console_scripts": [
               "imagecast = imagecast.cli:run",
           ],
       },
```

### Comparing `imagecast-0.6.0/test/test_core.py` & `imagecast-0.7.0/test/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,39 +98,34 @@
 
 def test_to_bytes(ie: ImageEngine):
 
     ie.read()
     ie.crop((50, 50, 100, 100))
     buffer = ie.to_bytes()
 
-    assert False \
-        or buffer.startswith(b"\x80") \
-        or buffer.startswith(b"\x7f") \
-        or buffer.startswith(b"{")
+    assert isinstance(buffer, bytes)
 
 
 def test_acquire_html_full():
     """
     Acquire image from HTML, using Playwright/Firefox.
     """
     ie = ImageEngine()
 
     ie.acquire("https://example.org/")
     ie.read()
-    buffer = ie.to_bytes()
+    buffer = ie.to_buffer("png", dpi=72)
 
-    # TODO: Why doesn't this employ a PNG header?
-    assert buffer.startswith(b"\xf0\xf0\xf2\xff\xf0\xf0\xf2")
+    assert buffer.startswith(b"\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR")
 
 
 def test_acquire_html_partial():
     """
     Acquire image from HTML, with DOM selector.
     """
     ie = ImageEngine()
 
     ie.acquire("https://example.org/", dom_selector="h1")
     ie.read()
-    buffer = ie.to_bytes()
+    buffer = ie.to_buffer("png", dpi=72)
 
-    # TODO: Why doesn't this employ a PNG header?
-    assert buffer.startswith(b"\xfd\xfd\xff\xff\xfd")
+    assert buffer.startswith(b"\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR")
```

