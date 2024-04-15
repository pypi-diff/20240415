# Comparing `tmp/gremlinpython-3.7.0.tar.gz` & `tmp/gremlinpython-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gremlinpython-3.7.0.tar", last modified: Fri Aug  4 19:45:55 2023, max compression
+gzip compressed data, was "gremlinpython-3.7.1.tar", last modified: Mon Dec  4 20:18:47 2023, max compression
```

## Comparing `gremlinpython-3.7.0.tar` & `gremlinpython-3.7.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.107662 gremlinpython-3.7.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      814 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      170 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6055 2023-08-04 19:45:55.107930 gremlinpython-3.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5553 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.048563 gremlinpython-3.7.0/gremlin_python/
--rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/gremlin_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-08-04 19:45:54.000000 gremlinpython-3.7.0/gremlin_python/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.070649 gremlinpython-3.7.0/gremlin_python/driver/
--rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/gremlin_python/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.082456 gremlinpython-3.7.0/gremlin_python/driver/aiohttp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/gremlin_python/driver/aiohttp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6228 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/gremlin_python/driver/aiohttp/transport.py
--rw-r--r--   0 root         (0) root         (0)     7399 2023-08-04 19:44:07.000000 gremlinpython-3.7.0/gremlin_python/driver/client.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/connection.py
--rw-r--r--   0 root         (0) root         (0)     8695 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/driver_remote_connection.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/protocol.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/remote_connection.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/request.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/resultset.py
--rw-r--r--   0 root         (0) root         (0)    10009 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/driver/transport.py
--rw-r--r--   0 root         (0) root         (0)     1588 2023-08-04 19:45:53.000000 gremlinpython-3.7.0/gremlin_python/driver/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.091388 gremlinpython-3.7.0/gremlin_python/process/
--rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/anonymous_traversal.py
--rw-r--r--   0 root         (0) root         (0)    61785 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/graph_traversal.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/strategies.py
--rw-r--r--   0 root         (0) root         (0)     6159 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/translator.py
--rw-r--r--   0 root         (0) root         (0)    22924 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/process/traversal.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/statics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.094066 gremlinpython-3.7.0/gremlin_python/structure/
--rw-r--r--   0 root         (0) root         (0)      852 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.101001 gremlinpython-3.7.0/gremlin_python/structure/io/
--rw-r--r--   0 root         (0) root         (0)      852 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37195 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/io/graphbinaryV1.py
--rw-r--r--   0 root         (0) root         (0)    21389 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/io/graphsonV2d0.py
--rw-r--r--   0 root         (0) root         (0)    24709 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/io/graphsonV3d0.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/gremlin_python/structure/io/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:45:55.106619 gremlinpython-3.7.0/gremlinpython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6055 2023-08-04 19:45:54.000000 gremlinpython-3.7.0/gremlinpython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2023-08-04 19:45:55.000000 gremlinpython-3.7.0/gremlinpython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:45:54.000000 gremlinpython-3.7.0/gremlinpython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2023-08-04 19:45:54.000000 gremlinpython-3.7.0/gremlinpython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-04 19:45:54.000000 gremlinpython-3.7.0/gremlinpython.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-08-04 19:45:55.109008 gremlinpython-3.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3092 2023-08-04 19:44:08.000000 gremlinpython-3.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.607256 gremlinpython-3.7.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      814 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      170 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-12-04 20:18:47.608882 gremlinpython-3.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.247181 gremlinpython-3.7.1/gremlin_python/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlin_python/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.304576 gremlinpython-3.7.1/gremlin_python/driver/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.318717 gremlinpython-3.7.1/gremlin_python/driver/aiohttp/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/aiohttp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10842 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/aiohttp/transport.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/client.py
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)     8695 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/driver_remote_connection.py
+-rw-r--r--   0 root         (0) root         (0)    11549 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/remote_connection.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/request.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/resultset.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/driver/transport.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-12-04 20:18:44.000000 gremlinpython-3.7.1/gremlin_python/driver/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.374421 gremlinpython-3.7.1/gremlin_python/process/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/anonymous_traversal.py
+-rw-r--r--   0 root         (0) root         (0)    68433 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/graph_traversal.py
+-rw-r--r--   0 root         (0) root         (0)     9474 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/strategies.py
+-rw-r--r--   0 root         (0) root         (0)    11147 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/translator.py
+-rw-r--r--   0 root         (0) root         (0)    23119 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/process/traversal.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/statics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.490498 gremlinpython-3.7.1/gremlin_python/structure/
+-rw-r--r--   0 root         (0) root         (0)      852 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.551344 gremlinpython-3.7.1/gremlin_python/structure/io/
+-rw-r--r--   0 root         (0) root         (0)      852 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37292 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/io/graphbinaryV1.py
+-rw-r--r--   0 root         (0) root         (0)    21389 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/io/graphsonV2d0.py
+-rw-r--r--   0 root         (0) root         (0)    24710 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/io/graphsonV3d0.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/gremlin_python/structure/io/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 20:18:47.602137 gremlinpython-3.7.1/gremlinpython.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlinpython.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlinpython.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlinpython.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlinpython.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-12-04 20:18:47.000000 gremlinpython-3.7.1/gremlinpython.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-12-04 20:18:47.616888 gremlinpython-3.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3092 2023-12-04 20:06:10.000000 gremlinpython-3.7.1/setup.py
```

### Comparing `gremlinpython-3.7.0/LICENSE` & `gremlinpython-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/MANIFEST.in` & `gremlinpython-3.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/PKG-INFO` & `gremlinpython-3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.7.0
+Version: 3.7.1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.7.0/README.rst` & `gremlinpython-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/__init__.py` & `gremlinpython-3.7.1/gremlin_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/__version__.py` & `gremlinpython-3.7.1/gremlin_python/__version__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 '''
-version   = '3.7.0'
-timestamp = 1691178354
+version   = '3.7.1'
+timestamp = 1701721127
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/__init__.py` & `gremlinpython-3.7.1/gremlin_python/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/aiohttp/__init__.py` & `gremlinpython-3.7.1/gremlin_python/driver/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/aiohttp/transport.py` & `gremlinpython-3.7.1/gremlin_python/driver/aiohttp/transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -134,7 +134,103 @@
             # Close the event loop.
             self._loop.close()
 
     @property
     def closed(self):
         # Connection is closed if either the websocket or the client session is closed.
         return self._websocket.closed or self._client_session.closed
+
+
+class AiohttpHTTPTransport(AbstractBaseTransport):
+    nest_asyncio_applied = False
+
+    def __init__(self, call_from_event_loop=None, read_timeout=None, write_timeout=None, **kwargs):
+        if call_from_event_loop is not None and call_from_event_loop and not AiohttpTransport.nest_asyncio_applied:
+            """ 
+                The AiohttpTransport implementation uses the asyncio event loop. Because of this, it cannot be called 
+                within an event loop without nest_asyncio. If the code is ever refactored so that it can be called 
+                within an event loop this import and call can be removed. Without this, applications which use the 
+                event loop to call gremlin-python (such as Jupyter) will not work.
+            """
+            import nest_asyncio
+            nest_asyncio.apply()
+            AiohttpTransport.nest_asyncio_applied = True
+
+        # Start event loop and initialize client session and response to None
+        self._loop = asyncio.new_event_loop()
+        self._client_session = None
+        self._http_req_resp = None
+        self._enable_ssl = False
+
+        # Set all inner variables to parameters passed in.
+        self._aiohttp_kwargs = kwargs
+        self._write_timeout = write_timeout
+        self._read_timeout = read_timeout
+        if "ssl_options" in self._aiohttp_kwargs:
+            self._ssl_context = self._aiohttp_kwargs.pop("ssl_options")
+            self._enable_ssl = True
+
+    def __del__(self):
+        # Close will only actually close if things are left open, so this is safe to call.
+        # Clean up any connection resources and close the event loop.
+        self.close()
+
+    def connect(self, url, headers=None):
+        # Inner function to perform async connect.
+        async def async_connect():
+            # Start client session and use it to send all HTTP requests. Base url is the endpoint, headers are set here
+            # Base url can only parse basic url with no path, see https://github.com/aio-libs/aiohttp/issues/6647
+            if self._enable_ssl:
+                # ssl context is established through tcp connector
+                tcp_conn = aiohttp.TCPConnector(ssl_context=self._ssl_context)
+                self._client_session = aiohttp.ClientSession(connector=tcp_conn,
+                                                             base_url=url, headers=headers, loop=self._loop)
+            else:
+                self._client_session = aiohttp.ClientSession(base_url=url, headers=headers, loop=self._loop)
+
+        # Execute the async connect synchronously.
+        self._loop.run_until_complete(async_connect())
+
+    def write(self, message):
+        # Inner function to perform async write.
+        async def async_write():
+            basic_auth = None
+            # basic password authentication for https connections
+            if message['auth']:
+                basic_auth = aiohttp.BasicAuth(message['auth']['username'], message['auth']['password'])
+            async with async_timeout.timeout(self._write_timeout):
+                self._http_req_resp = await self._client_session.post(url="/gremlin",
+                                                                      auth=basic_auth,
+                                                                      data=message['payload'],
+                                                                      headers=message['headers'],
+                                                                      **self._aiohttp_kwargs)
+
+        # Execute the async write synchronously.
+        self._loop.run_until_complete(async_write())
+
+    def read(self):
+        # Inner function to perform async read.
+        async def async_read():
+            async with async_timeout.timeout(self._read_timeout):
+                return await self._http_req_resp.read()
+
+        return self._loop.run_until_complete(async_read())
+
+    def close(self):
+        # Inner function to perform async close.
+        async def async_close():
+            if self._client_session is not None and not self._client_session.closed:
+                await self._client_session.close()
+                self._client_session = None
+
+        # If the loop is not closed (connection hasn't already been closed)
+        if not self._loop.is_closed():
+            # Execute the async close synchronously.
+            self._loop.run_until_complete(async_close())
+
+            # Close the event loop.
+            self._loop.close()
+
+    @property
+    def closed(self):
+        # Connection is closed when client session is closed.
+        return self._client_session.closed
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/client.py` & `gremlinpython-3.7.1/gremlin_python/driver/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import logging
 import warnings
 import queue
+import re
 from concurrent.futures import ThreadPoolExecutor
 
 from gremlin_python.driver import connection, protocol, request, serializer
 from gremlin_python.process import traversal
 
 log = logging.getLogger("gremlinpython")
 
@@ -41,47 +42,61 @@
 
     def __init__(self, url, traversal_source, protocol_factory=None,
                  transport_factory=None, pool_size=None, max_workers=None,
                  message_serializer=None, username="", password="",
                  kerberized_service="", headers=None, session=None,
                  enable_user_agent_on_connect=True, **transport_kwargs):
         log.info("Creating Client with url '%s'", url)
+
+        # check via url that we are using http protocol
+        self._use_http = re.search('^http', url)
+
         self._closed = False
         self._url = url
         self._headers = headers
         self._enable_user_agent_on_connect = enable_user_agent_on_connect
         self._traversal_source = traversal_source
-        if "max_content_length" not in transport_kwargs:
+        if not self._use_http and "max_content_length" not in transport_kwargs:
             transport_kwargs["max_content_length"] = 10 * 1024 * 1024
         if message_serializer is None:
             message_serializer = serializer.GraphBinarySerializersV1()
 
         self._message_serializer = message_serializer
         self._username = username
         self._password = password
         self._session = session
         self._session_enabled = (session is not None and session != "")
         if transport_factory is None:
             try:
                 from gremlin_python.driver.aiohttp.transport import (
-                    AiohttpTransport)
+                    AiohttpTransport, AiohttpHTTPTransport)
             except ImportError:
                 raise Exception("Please install AIOHTTP or pass "
                                 "custom transport factory")
             else:
                 def transport_factory():
-                    return AiohttpTransport(**transport_kwargs)
+                    if self._use_http:
+                        return AiohttpHTTPTransport(**transport_kwargs)
+                    else:
+                        return AiohttpTransport(**transport_kwargs)
         self._transport_factory = transport_factory
         if protocol_factory is None:
-            def protocol_factory(): return protocol.GremlinServerWSProtocol(
-                self._message_serializer,
-                username=self._username,
-                password=self._password,
-                kerberized_service=kerberized_service,
-                max_content_length=transport_kwargs["max_content_length"])
+            def protocol_factory():
+                if self._use_http:
+                    return protocol.GremlinServerHTTPProtocol(
+                        self._message_serializer,
+                        username=self._username,
+                        password=self._password)
+                else:
+                    return protocol.GremlinServerWSProtocol(
+                        self._message_serializer,
+                        username=self._username,
+                        password=self._password,
+                        kerberized_service=kerberized_service,
+                        max_content_length=transport_kwargs["max_content_length"])
         self._protocol_factory = protocol_factory
         if self._session_enabled:
             if pool_size is None:
                 pool_size = 1
             elif pool_size != 1:
                 raise Exception("PoolSize must be 1 on session mode!")
         if pool_size is None:
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/connection.py` & `gremlinpython-3.7.1/gremlin_python/driver/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     def write(self, request_message):
         if not self._inited:
             self.connect()
         request_id = str(uuid.uuid4())
         if request_message.args.get("requestId"):
             request_id = request_message.args.get("requestId")
+            uuid.UUID(request_id) # Checks for proper UUID or else server will return an error.
         result_set = resultset.ResultSet(queue.Queue(), request_id)
         self._results[request_id] = result_set
         # Create write task
         future = Future()
         future_write = self._executor.submit(
             self._protocol.write, request_id, request_message)
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/driver_remote_connection.py` & `gremlinpython-3.7.1/gremlin_python/driver/driver_remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/protocol.py` & `gremlinpython-3.7.1/gremlin_python/driver/protocol.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
+import json
 import logging
 import abc
 import base64
 import struct
 
 # import kerberos    Optional dependency imported in relevant codeblock
 
 from gremlin_python.driver import request
 from gremlin_python.driver.resultset import ResultSet
+from gremlin_python.process.translator import Translator
+from gremlin_python.process.traversal import Bytecode
 
 log = logging.getLogger("gremlinpython")
 
 __author__ = 'David M. Brown (davebshow@gmail.com)'
 
 
 class GremlinServerError(Exception):
@@ -59,15 +62,14 @@
 
     @abc.abstractmethod
     def write(self, request_id, request_message):
         pass
 
 
 class GremlinServerWSProtocol(AbstractBaseProtocol):
-
     QOP_AUTH_BIT = 1
     _kerberos_context = None
     _max_content_length = 10 * 1024 * 1024
 
     def __init__(self,
                  message_serializer,
                  username='', password='',
@@ -129,15 +131,15 @@
                 result_set.status_attributes = message['status']['attributes']
                 del results_dict[request_id]
             return status_code
         else:
             # This message is going to be huge and kind of hard to read, but in the event of an error,
             # it can provide invaluable info, so space it out appropriately.
             log.error("\r\nReceived error message '%s'\r\n\r\nWith results dictionary '%s'",
-                          str(message), str(results_dict))
+                      str(message), str(results_dict))
             del results_dict[request_id]
             raise GremlinServerError(message['status'])
 
     def _kerberos_received(self, message):
         # Inspired by: https://github.com/thobbs/pure-sasl/blob/0.6.2/puresasl/mechanisms.py
         #              https://github.com/thobbs/pure-sasl/blob/0.6.2/LICENSE
         try:
@@ -181,12 +183,75 @@
         word, = struct.unpack('!I', plaintext_data)
         qop_bits = word >> 24
         assert self.QOP_AUTH_BIT & qop_bits, "Unexpected sasl qop level received from gremlin server"
 
         name_length = len(self._username)
         fmt = '!I' + str(name_length) + 's'
         word = self.QOP_AUTH_BIT << 24 | self._max_content_length
-        out = struct.pack(fmt, word, self._username.encode("utf-8"),)
+        out = struct.pack(fmt, word, self._username.encode("utf-8"), )
         encoded = base64.b64encode(out).decode('ascii')
         kerberos.authGSSClientWrap(self._kerberos_context, encoded)
         auth = kerberos.authGSSClientResponse(self._kerberos_context)
         return request.RequestMessage('', 'authentication', {'sasl': auth})
+
+
+class GremlinServerHTTPProtocol(AbstractBaseProtocol):
+
+    def __init__(self,
+                 message_serializer,
+                 username='', password=''):
+        self._message_serializer = message_serializer
+        self._username = username
+        self._password = password
+
+    def connection_made(self, transport):
+        super(GremlinServerHTTPProtocol, self).connection_made(transport)
+
+    def write(self, request_id, request_message):
+
+        basic_auth = {}
+        if self._username and self._password:
+            basic_auth['username'] = self._username
+            basic_auth['password'] = self._password
+
+        content_type = str(self._message_serializer.version, encoding='utf-8')
+        message = {
+            'headers': {'CONTENT-TYPE': content_type,
+                        'ACCEPT': content_type},
+            'payload': self._message_serializer.serialize_message(request_id, request_message),
+            'auth': basic_auth
+        }
+
+        self._transport.write(message)
+
+    def data_received(self, message, results_dict):
+        # if Gremlin Server cuts off then we get a None for the message
+        if message is None:
+            log.error("Received empty message from server.")
+            raise GremlinServerError({'code': 500,
+                                      'message': 'Server disconnected - please try to reconnect', 'attributes': {}})
+
+        message = self._message_serializer.deserialize_message(message)
+        request_id = message['requestId']
+        result_set = results_dict[request_id] if request_id in results_dict else ResultSet(None, None)
+        status_code = message['status']['code']
+        aggregate_to = message['result']['meta'].get('aggregateTo', 'list')
+        data = message['result']['data']
+        result_set.aggregate_to = aggregate_to
+
+        if status_code == 204:
+            result_set.stream.put_nowait([])
+            del results_dict[request_id]
+            return status_code
+        elif status_code in [200, 206]:
+            result_set.stream.put_nowait(data)
+            if status_code == 200:
+                result_set.status_attributes = message['status']['attributes']
+                del results_dict[request_id]
+            return status_code
+        else:
+            # This message is going to be huge and kind of hard to read, but in the event of an error,
+            # it can provide invaluable info, so space it out appropriately.
+            log.error("\r\nReceived error message '%s'\r\n\r\nWith results dictionary '%s'",
+                      str(message), str(results_dict))
+            del results_dict[request_id]
+            raise GremlinServerError(message['status'])
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/remote_connection.py` & `gremlinpython-3.7.1/gremlin_python/driver/remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/request.py` & `gremlinpython-3.7.1/gremlin_python/driver/request.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/resultset.py` & `gremlinpython-3.7.1/gremlin_python/driver/resultset.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/serializer.py` & `gremlinpython-3.7.1/gremlin_python/driver/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
+import base64
 import logging
 import struct
 import uuid
 import io
 try:
     import ujson as json
     if int(json.__version__[0]) < 2:
@@ -152,15 +153,16 @@
 
     def finalize_message(self, message, mime_len, mime_type):
         message = json.dumps(message)
         message = b''.join([mime_len, mime_type, message.encode('utf-8')])
         return message
 
     def deserialize_message(self, message):
-        msg = json.loads(message.decode('utf-8'))
+        # for parsing string message via HTTP connections
+        msg = json.loads(message if isinstance(message, str) else message.decode('utf-8'))
         return self._graphson_reader.to_object(msg)
 
 
 class GraphSONSerializersV2d0(GraphSONMessageSerializer):
     """Message serializer for GraphSON 2.0"""
     def __init__(self):
         reader = graphsonV2d0.GraphSONReader()
@@ -264,15 +266,16 @@
                 ba.extend(v)
             else:
                 self._graphbinary_writer.to_dict(v, ba)
 
         return bytes(ba)
 
     def deserialize_message(self, message):
-        b = io.BytesIO(message)
+        # for parsing string message via HTTP connections
+        b = io.BytesIO(base64.b64decode(message) if isinstance(message, str) else message)
 
         b.read(1)  # version
 
         request_id = str(self._graphbinary_reader.to_object(b, graphbinaryV1.DataType.uuid))
         status_code = self.int32_unpack(b.read(4))[0]
         status_msg = self._graphbinary_reader.to_object(b, graphbinaryV1.DataType.string)
         status_attrs = self._graphbinary_reader.to_object(b, graphbinaryV1.DataType.map, nullable=False)
```

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/transport.py` & `gremlinpython-3.7.1/gremlin_python/driver/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/driver/useragent.py` & `gremlinpython-3.7.1/gremlin_python/driver/useragent.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import platform
 
-gremlin_version = "3.7.0"  # DO NOT MODIFY - Configured automatically by Maven Replacer Plugin
+gremlin_version = "3.7.1"  # DO NOT MODIFY - Configured automatically by Maven Replacer Plugin
 
 def _generate_user_agent():
     application_name = "NotAvailable"
     runtime_version = platform.python_version().replace(" ", "_")
     os_name = platform.system().replace(" ", "_")
     os_version = platform.release().replace(" ", "_")
     architecture = platform.machine().replace(" ", "_")
```

### Comparing `gremlinpython-3.7.0/gremlin_python/process/__init__.py` & `gremlinpython-3.7.1/gremlin_python/process/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/process/anonymous_traversal.py` & `gremlinpython-3.7.1/gremlin_python/process/anonymous_traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/process/graph_traversal.py` & `gremlinpython-3.7.1/gremlin_python/process/graph_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         warnings.warn(
             "gremlin_python.process.GraphTraversalSource.withComputer will be replaced by "
             "gremlin_python.process.GraphTraversalSource.with_computer.",
             DeprecationWarning)
         return self.with_computer(graph_computer, workers, result, persist, vertices, edges, configuration)
 
     def with_computer(self, graph_computer=None, workers=None, result=None, persist=None, vertices=None,
-                  edges=None, configuration=None):
+                      edges=None, configuration=None):
         return self.with_strategies(
             VertexProgramStrategy(graph_computer, workers, result, persist, vertices, edges, configuration))
 
     def E(self, *args):
         traversal = self.get_graph_traversal()
         traversal.bytecode.add_step("E", *args)
         return traversal
@@ -305,22 +305,38 @@
         self.bytecode.add_step("addV", *args)
         return self
 
     def aggregate(self, *args):
         self.bytecode.add_step("aggregate", *args)
         return self
 
+    def all_(self, *args):
+        self.bytecode.add_step("all", *args)
+        return self
+
     def and_(self, *args):
         self.bytecode.add_step("and", *args)
         return self
 
+    def any_(self, *args):
+        self.bytecode.add_step("any", *args)
+        return self
+
     def as_(self, *args):
         self.bytecode.add_step("as", *args)
         return self
 
+    def as_date(self, *args):
+        self.bytecode.add_step("asDate", *args)
+        return self
+
+    def as_string(self, *args):
+        self.bytecode.add_step("asString", *args)
+        return self
+
     def barrier(self, *args):
         self.bytecode.add_step("barrier", *args)
         return self
 
     def both(self, *args):
         self.bytecode.add_step("both", *args)
         return self
@@ -371,18 +387,26 @@
         self.bytecode.add_step("coalesce", *args)
         return self
 
     def coin(self, *args):
         self.bytecode.add_step("coin", *args)
         return self
 
+    def combine(self, *args):
+        self.bytecode.add_step("combine", *args)
+        return self
+
     def concat(self, *args):
         self.bytecode.add_step("concat", *args)
         return self
 
+    def conjoin(self, *args):
+        self.bytecode.add_step("conjoin", *args)
+        return self
+
     def connectedComponent(self, *args):
         warnings.warn(
             "gremlin_python.process.GraphTraversalSource.connectedComponent will be replaced by "
             "gremlin_python.process.GraphTraversalSource.connected_component.",
             DeprecationWarning)
         return self.connected_component(*args)
 
@@ -405,18 +429,34 @@
             DeprecationWarning)
         return self.cyclic_path(*args)
 
     def cyclic_path(self, *args):
         self.bytecode.add_step("cyclicPath", *args)
         return self
 
+    def date_add(self, *args):
+        self.bytecode.add_step("dateAdd", *args)
+        return self
+
+    def date_diff(self, *args):
+        self.bytecode.add_step("dateDiff", *args)
+        return self
+
     def dedup(self, *args):
         self.bytecode.add_step("dedup", *args)
         return self
 
+    def difference(self, *args):
+        self.bytecode.add_step("difference", *args)
+        return self
+
+    def disjunct(self, *args):
+        self.bytecode.add_step("disjunct", *args)
+        return self
+
     def drop(self, *args):
         self.bytecode.add_step("drop", *args)
         return self
 
     def element(self, *args):
         self.bytecode.add_step("element", *args)
         return self
@@ -455,14 +495,18 @@
         self.bytecode.add_step("flatMap", *args)
         return self
 
     def fold(self, *args):
         self.bytecode.add_step("fold", *args)
         return self
 
+    def format_(self, *args):
+        self.bytecode.add_step("format", *args)
+        return self
+
     def from_(self, *args):
         self.bytecode.add_step("from", *args)
         return self
 
     def group(self, *args):
         self.bytecode.add_step("group", *args)
         return self
@@ -575,38 +619,50 @@
         self.bytecode.add_step("index", *args)
         return self
 
     def inject(self, *args):
         self.bytecode.add_step("inject", *args)
         return self
 
+    def intersect(self, *args):
+        self.bytecode.add_step("intersect", *args)
+        return self
+
     def is_(self, *args):
         self.bytecode.add_step("is", *args)
         return self
 
     def key(self, *args):
         self.bytecode.add_step("key", *args)
         return self
 
     def label(self, *args):
         self.bytecode.add_step("label", *args)
         return self
 
+    def length(self, *args):
+        self.bytecode.add_step("length", *args)
+        return self
+
     def limit(self, *args):
         self.bytecode.add_step("limit", *args)
         return self
 
     def local(self, *args):
         self.bytecode.add_step("local", *args)
         return self
 
     def loops(self, *args):
         self.bytecode.add_step("loops", *args)
         return self
 
+    def lTrim(self, *args):
+        self.bytecode.add_step("lTrim", *args)
+        return self
+
     def map(self, *args):
         self.bytecode.add_step("map", *args)
         return self
 
     def match(self, *args):
         self.bytecode.add_step("match", *args)
         return self
@@ -619,14 +675,18 @@
         self.bytecode.add_step("max", *args)
         return self
 
     def mean(self, *args):
         self.bytecode.add_step("mean", *args)
         return self
 
+    def merge(self, *args):
+        self.bytecode.add_step("merge", *args)
+        return self
+
     def merge_e(self, *args):
         self.bytecode.add_step("mergeE", *args)
         return self
 
     def merge_v(self, *args):
         self.bytecode.add_step("mergeV", *args)
         return self
@@ -718,14 +778,18 @@
             DeprecationWarning)
         return self.peer_pressure(*args)
 
     def peer_pressure(self, *args):
         self.bytecode.add_step("peerPressure", *args)
         return self
 
+    def product(self, *args):
+        self.bytecode.add_step("product", *args)
+        return self
+
     def profile(self, *args):
         self.bytecode.add_step("profile", *args)
         return self
 
     def program(self, *args):
         self.bytecode.add_step("program", *args)
         return self
@@ -761,14 +825,26 @@
         self.bytecode.add_step("read", *args)
         return self
 
     def repeat(self, *args):
         self.bytecode.add_step("repeat", *args)
         return self
 
+    def replace(self, *args):
+        self.bytecode.add_step("replace", *args)
+        return self
+
+    def reverse(self, *args):
+        self.bytecode.add_step("reverse", *args)
+        return self
+
+    def rTrim(self, *args):
+        self.bytecode.add_step("rTrim", *args)
+        return self
+
     def sack(self, *args):
         self.bytecode.add_step("sack", *args)
         return self
 
     def sample(self, *args):
         self.bytecode.add_step("sample", *args)
         return self
@@ -810,22 +886,30 @@
         self.bytecode.add_step("simplePath", *args)
         return self
 
     def skip(self, *args):
         self.bytecode.add_step("skip", *args)
         return self
 
+    def split(self, *args):
+        self.bytecode.add_step("split", *args)
+        return self
+
     def store(self, *args):
         self.bytecode.add_step("store", *args)
         return self
 
     def subgraph(self, *args):
         self.bytecode.add_step("subgraph", *args)
         return self
 
+    def substring(self, *args):
+        self.bytecode.add_step("substring", *args)
+        return self
+
     def sum_(self, *args):
         self.bytecode.add_step("sum", *args)
         return self
 
     def tail(self, *args):
         self.bytecode.add_step("tail", *args)
         return self
@@ -856,14 +940,22 @@
             DeprecationWarning)
         return self.to_e(*args)
 
     def to_e(self, *args):
         self.bytecode.add_step("toE", *args)
         return self
 
+    def to_lower(self, *args):
+        self.bytecode.add_step("toLower", *args)
+        return self
+
+    def to_upper(self, *args):
+        self.bytecode.add_step("toUpper", *args)
+        return self
+
     def toV(self, *args):
         warnings.warn(
             "gremlin_python.process.GraphTraversalSource.toV will be replaced by "
             "gremlin_python.process.GraphTraversalSource.to_v.",
             DeprecationWarning)
         return self.to_v(*args)
 
@@ -871,14 +963,18 @@
         self.bytecode.add_step("toV", *args)
         return self
 
     def tree(self, *args):
         self.bytecode.add_step("tree", *args)
         return self
 
+    def trim(self, *args):
+        self.bytecode.add_step("trim", *args)
+        return self
+
     def unfold(self, *args):
         self.bytecode.add_step("unfold", *args)
         return self
 
     def union(self, *args):
         self.bytecode.add_step("union", *args)
         return self
@@ -972,22 +1068,38 @@
         return cls.graph_traversal(None, None, Bytecode()).add_v(*args)
 
     @classmethod
     def aggregate(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).aggregate(*args)
 
     @classmethod
+    def all_(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).all_(*args)
+
+    @classmethod
     def and_(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).and_(*args)
 
     @classmethod
+    def any_(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).any_(*args)
+
+    @classmethod
     def as_(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).as_(*args)
 
     @classmethod
+    def as_date(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).as_date(*args)
+
+    @classmethod
+    def as_string(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).as_string(*args)
+
+    @classmethod
     def barrier(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).barrier(*args)
 
     @classmethod
     def both(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).both(*args)
 
@@ -1036,18 +1148,26 @@
         return cls.graph_traversal(None, None, Bytecode()).coalesce(*args)
 
     @classmethod
     def coin(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).coin(*args)
 
     @classmethod
+    def combine(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).combine(*args)
+
+    @classmethod
     def concat(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).concat(*args)
 
     @classmethod
+    def conjoin(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).conjoin(*args)
+
+    @classmethod
     def constant(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).constant(*args)
 
     @classmethod
     def count(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).count(*args)
 
@@ -1060,18 +1180,34 @@
         return cls.cyclic_path(*args)
 
     @classmethod
     def cyclic_path(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).cyclic_path(*args)
 
     @classmethod
+    def date_add(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).date_add(*args)
+
+    @classmethod
+    def date_diff(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).date_diff(*args)
+
+    @classmethod
     def dedup(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).dedup(*args)
 
     @classmethod
+    def difference(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).difference(*args)
+
+    @classmethod
+    def disjunct(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).disjunct(*args)
+
+    @classmethod
     def drop(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).drop(*args)
 
     @classmethod
     def element(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).element(*args)
 
@@ -1112,14 +1248,18 @@
         return cls.graph_traversal(None, None, Bytecode()).flat_map(*args)
 
     @classmethod
     def fold(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).fold(*args)
 
     @classmethod
+    def format_(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).format_(*args)
+
+    @classmethod
     def group(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).group(*args)
 
     @classmethod
     def groupCount(cls, *args):
         warnings.warn(
             "gremlin_python.process.__.groupCount will be replaced by "
@@ -1236,38 +1376,50 @@
         return cls.graph_traversal(None, None, Bytecode()).index(*args)
 
     @classmethod
     def inject(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).inject(*args)
 
     @classmethod
+    def intersect(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).intersect(*args)
+
+    @classmethod
     def is_(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).is_(*args)
 
     @classmethod
     def key(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).key(*args)
 
     @classmethod
     def label(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).label(*args)
 
     @classmethod
+    def length(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).length(*args)
+
+    @classmethod
     def limit(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).limit(*args)
 
     @classmethod
     def local(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).local(*args)
 
     @classmethod
     def loops(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).loops(*args)
 
     @classmethod
+    def ltrim(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).ltrim(*args)
+
+    @classmethod
     def map(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).map(*args)
 
     @classmethod
     def match(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).match(*args)
 
@@ -1280,14 +1432,18 @@
         return cls.graph_traversal(None, None, Bytecode()).max_(*args)
 
     @classmethod
     def mean(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).mean(*args)
 
     @classmethod
+    def merge(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).merge(*args)
+
+    @classmethod
     def merge_e(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).merge_e(*args)
 
     @classmethod
     def merge_v(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).merge_v(*args)
 
@@ -1352,14 +1508,18 @@
         return cls.graph_traversal(None, None, Bytecode()).out_v(*args)
 
     @classmethod
     def path(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).path(*args)
 
     @classmethod
+    def product(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).product(*args)
+
+    @classmethod
     def project(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).project(*args)
 
     @classmethod
     def properties(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).properties(*args)
 
@@ -1384,14 +1544,26 @@
         return cls.graph_traversal(None, None, Bytecode()).range_(*args)
 
     @classmethod
     def repeat(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).repeat(*args)
 
     @classmethod
+    def replace(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).replace(*args)
+
+    @classmethod
+    def reverse(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).reverse(*args)
+
+    @classmethod
+    def rTrim(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).rTrim(*args)
+
+    @classmethod
     def sack(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).sack(*args)
 
     @classmethod
     def sample(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).sample(*args)
 
@@ -1424,22 +1596,30 @@
         return cls.graph_traversal(None, None, Bytecode()).simple_path(*args)
 
     @classmethod
     def skip(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).skip(*args)
 
     @classmethod
+    def split(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).split(*args)
+
+    @classmethod
     def store(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).store(*args)
 
     @classmethod
     def subgraph(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).subgraph(*args)
 
     @classmethod
+    def substring(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).substring(*args)
+
+    @classmethod
     def sum_(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).sum_(*args)
 
     @classmethod
     def tail(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).tail(*args)
 
@@ -1472,14 +1652,22 @@
         return cls.to_e(*args)
 
     @classmethod
     def to_e(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).to_e(*args)
 
     @classmethod
+    def to_lower(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).to_lower(*args)
+
+    @classmethod
+    def to_upper(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).to_upper(*args)
+
+    @classmethod
     def toV(cls, *args):
         warnings.warn(
             "gremlin_python.process.__.toV will be replaced by "
             "gremlin_python.process.__.to_v.",
             DeprecationWarning)
         return cls.to_v(*args)
 
@@ -1488,14 +1676,18 @@
         return cls.graph_traversal(None, None, Bytecode()).to_v(*args)
 
     @classmethod
     def tree(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).tree(*args)
 
     @classmethod
+    def trim(cls, *args):
+        return cls.graph_traversal(None, None, Bytecode()).trim(*args)
+
+    @classmethod
     def unfold(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).unfold(*args)
 
     @classmethod
     def union(cls, *args):
         return cls.graph_traversal(None, None, Bytecode()).union(*args)
 
@@ -1635,14 +1827,22 @@
     return __.and_(*args)
 
 
 def as_(*args):
     return __.as_(*args)
 
 
+def as_date(*args):
+    return __.as_date(*args)
+
+
+def as_string(*args):
+    return __.as_string(*args)
+
+
 def barrier(*args):
     return __.barrier(*args)
 
 
 def both(*args):
     return __.both(*args)
 
@@ -1703,14 +1903,22 @@
     return __.cyclic_path(*args)
 
 
 def cyclic_path(*args):
     return __.cyclic_path(*args)
 
 
+def date_add(*args):
+    return __.date_add(*args)
+
+
+def date_diff(*args):
+    return __.date_diff(*args)
+
+
 def dedup(*args):
     return __.dedup(*args)
 
 
 def drop(*args):
     return __.drop(*args)
 
@@ -1747,14 +1955,18 @@
     return __.flat_map(*args)
 
 
 def fold(*args):
     return __.fold(*args)
 
 
+def format_(*args):
+    return __.format_(*args)
+
+
 def group(*args):
     return __.group(*args)
 
 
 def groupCount(*args):
     return __.group_count(*args)
 
@@ -1851,26 +2063,34 @@
     return __.key(*args)
 
 
 def label(*args):
     return __.label(*args)
 
 
+def length(*args):
+    return __.length(*args)
+
+
 def limit(*args):
     return __.limit(*args)
 
 
 def local(*args):
     return __.local(*args)
 
 
 def loops(*args):
     return __.loops(*args)
 
 
+def ltrim(*args):
+    return __.ltrim(*args)
+
+
 def map(*args):
     return __.map(*args)
 
 
 def match(*args):
     return __.match(*args)
 
@@ -1971,14 +2191,26 @@
     return __.range_(*args)
 
 
 def repeat(*args):
     return __.repeat(*args)
 
 
+def replace(*args):
+    return __.replace(*args)
+
+
+def reverse(*args):
+    return __.reverse(*args)
+
+
+def rTrim(*args):
+    return __.rTrim(*args)
+
+
 def sack(*args):
     return __.sack(*args)
 
 
 def sample(*args):
     return __.sample(*args)
 
@@ -2003,22 +2235,30 @@
     return __.simple_path(*args)
 
 
 def skip(*args):
     return __.skip(*args)
 
 
+def split(*args):
+    return __.split(*args)
+
+
 def store(*args):
     return __.store(*args)
 
 
 def subgraph(*args):
     return __.subgraph(*args)
 
 
+def substring(*args):
+    return __.substring(*args)
+
+
 def sum_(*args):
     return __.sum_(*args)
 
 
 def tail(*args):
     return __.tail(*args)
 
@@ -2043,26 +2283,38 @@
     return __.to_e(*args)
 
 
 def to_e(*args):
     return __.to_e(*args)
 
 
+def to_lower(*args):
+    return __.to_lower(*args)
+
+
+def to_upper(*args):
+    return __.to_upper(*args)
+
+
 def toV(*args):
     return __.to_v(*args)
 
 
 def to_v(*args):
     return __.to_v(*args)
 
 
 def tree(*args):
     return __.tree(*args)
 
 
+def trim(*args):
+    return __.trim(*args)
+
+
 def unfold(*args):
     return __.unfold(*args)
 
 
 def union(*args):
     return __.union(*args)
 
@@ -2103,14 +2355,18 @@
 
 statics.add_static('aggregate', aggregate)
 
 statics.add_static('and_', and_)
 
 statics.add_static('as_', as_)
 
+statics.add_static('as_date', as_date)
+
+statics.add_static('as_string', as_string)
+
 statics.add_static('barrier', barrier)
 
 statics.add_static('both', both)
 
 statics.add_static('bothE', bothE)
 
 statics.add_static('both_e', both_e)
@@ -2137,14 +2393,18 @@
 
 statics.add_static('count', count)
 
 statics.add_static('cyclicPath', cyclicPath)
 
 statics.add_static('cyclicpath', cyclic_path)
 
+statics.add_static('date_add', date_add)
+
+statics.add_static('date_diff', date_diff)
+
 statics.add_static('dedup', dedup)
 
 statics.add_static('drop', drop)
 
 statics.add_static('element', element)
 
 statics.add_static('elementMap', elementMap)
@@ -2159,14 +2419,16 @@
 
 statics.add_static('flatMap', flatMap)
 
 statics.add_static('flat_map', flat_map)
 
 statics.add_static('fold', fold)
 
+statics.add_static('format_', format_)
+
 statics.add_static('group', group)
 
 statics.add_static('groupCount', groupCount)
 
 statics.add_static('group_count', group_count)
 
 statics.add_static('has', has)
@@ -2209,20 +2471,24 @@
 
 statics.add_static('is_', is_)
 
 statics.add_static('key', key)
 
 statics.add_static('label', label)
 
+statics.add_static('length', length)
+
 statics.add_static('limit', limit)
 
 statics.add_static('local', local)
 
 statics.add_static('loops', loops)
 
+statics.add_static('ltrim', ltrim)
+
 statics.add_static('map', map)
 
 statics.add_static('match', match)
 
 statics.add_static('math', math)
 
 statics.add_static('max_', max_)
@@ -2269,14 +2535,20 @@
 
 statics.add_static('property_map', property_map)
 
 statics.add_static('range_', range_)
 
 statics.add_static('repeat', repeat)
 
+statics.add_static('replace', replace)
+
+statics.add_static('reverse', reverse)
+
+statics.add_static('rTrim', rTrim)
+
 statics.add_static('sack', sack)
 
 statics.add_static('sample', sample)
 
 statics.add_static('select', select)
 
 statics.add_static('sideEffect', sideEffect)
@@ -2285,18 +2557,22 @@
 
 statics.add_static('simplePath', simplePath)
 
 statics.add_static('simple_path', simple_path)
 
 statics.add_static('skip', skip)
 
+statics.add_static('split', split)
+
 statics.add_static('store', store)
 
 statics.add_static('subgraph', subgraph)
 
+statics.add_static('substring', substring)
+
 statics.add_static('sum_', sum_)
 
 statics.add_static('tail', tail)
 
 statics.add_static('timeLimit', timeLimit)
 
 statics.add_static('time_limit', time_limit)
@@ -2307,18 +2583,24 @@
 
 statics.add_static('toE', toE)
 
 statics.add_static('to_e', to_e)
 
 statics.add_static('toV', toV)
 
+statics.add_static('to_lower', to_lower)
+
+statics.add_static('to_upper', to_upper)
+
 statics.add_static('to_v', to_v)
 
 statics.add_static('tree', tree)
 
+statics.add_static('trim', trim)
+
 statics.add_static('unfold', unfold)
 
 statics.add_static('union', union)
 
 statics.add_static('until', until)
 
 statics.add_static('value', value)
```

### Comparing `gremlinpython-3.7.0/gremlin_python/process/strategies.py` & `gremlinpython-3.7.1/gremlin_python/process/strategies.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/process/traversal.py` & `gremlinpython-3.7.1/gremlin_python/process/traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,21 @@
 statics.add_static('V3_0', GraphSONVersion.V3_0)
 
 GryoVersion = Enum('GryoVersion', ' V1_0 V3_0')
 
 statics.add_static('V1_0', GryoVersion.V1_0)
 statics.add_static('V3_0', GryoVersion.V3_0)
 
+DT = Enum('DT', ' second minute hour day')
+
+statics.add_static('second', DT.second)
+statics.add_static('minute', DT.minute)
+statics.add_static('hour', DT.hour)
+statics.add_static('day', DT.day)
+
 Merge = Enum('Merge', ' on_create on_match out_v in_v')
 
 statics.add_static('on_create', Merge.on_create)
 statics.add_static('on_match', Merge.on_match)
 statics.add_static('in_v', Merge.in_v)
 statics.add_static('out_v', Merge.out_v)
```

### Comparing `gremlinpython-3.7.0/gremlin_python/statics.py` & `gremlinpython-3.7.1/gremlin_python/statics.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/__init__.py` & `gremlinpython-3.7.1/gremlin_python/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/graph.py` & `gremlinpython-3.7.1/gremlin_python/structure/graph.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/io/__init__.py` & `gremlinpython-3.7.1/gremlin_python/structure/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/io/graphbinaryV1.py` & `gremlinpython-3.7.1/gremlin_python/structure/io/graphbinaryV1.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from struct import pack, unpack
 from aenum import Enum
 from datetime import timedelta
 from gremlin_python import statics
 from gremlin_python.statics import FloatType, BigDecimal, FunctionType, ShortType, IntType, LongType, BigIntType, \
                                    TypeType, DictType, ListType, SetType, SingleByte, ByteBufferType, GremlinType, \
                                    SingleChar
-from gremlin_python.process.traversal import Barrier, Binding, Bytecode, Cardinality, Column, Direction, Merge, \
+from gremlin_python.process.traversal import Barrier, Binding, Bytecode, Cardinality, Column, Direction, DT, Merge, \
                                              Operator, Order, Pick, Pop, P, Scope, TextP, Traversal, Traverser, \
                                              TraversalStrategy, T
 from gremlin_python.process.graph_traversal import GraphTraversal
 from gremlin_python.structure.graph import Graph, Edge, Property, Vertex, VertexProperty, Path
 from gremlin_python.structure.io.util import HashableDict, SymbolUtil
 
 log = logging.getLogger(__name__)
@@ -93,14 +93,15 @@
     textp = 0x28
     traversalstrategy = 0x29
     bulkset = 0x2a
     tree = 0x2b                   # not supported - no tree object in Python yet
     metrics = 0x2c
     traversalmetrics = 0x2d
     merge = 0x2e
+    dt = 0x2f
     char = 0x80
     duration = 0x81
     inetaddress = 0x82            # todo
     instant = 0x83                # todo
     localdate = 0x84              # todo
     localdatetime = 0x85          # todo
     localtime = 0x86              # todo
@@ -915,14 +916,19 @@
         to_extend.extend(int32_pack(len(args)))
         for a in args:
             writer.to_dict(a, to_extend)
 
         return to_extend
 
 
+class DTIO(_EnumIO):
+    graphbinary_type = DataType.dt
+    python_type = DT
+
+
 class MergeIO(_EnumIO):
     graphbinary_type = DataType.merge
     python_type = Merge
 
 
 class ScopeIO(_EnumIO):
     graphbinary_type = DataType.scope
```

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/io/graphsonV2d0.py` & `gremlinpython-3.7.1/gremlin_python/structure/io/graphsonV2d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/io/graphsonV3d0.py` & `gremlinpython-3.7.1/gremlin_python/structure/io/graphsonV3d0.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+
 import calendar
 import datetime
 import json
 import uuid
 import math
 from collections import OrderedDict
 from decimal import *
```

### Comparing `gremlinpython-3.7.0/gremlin_python/structure/io/util.py` & `gremlinpython-3.7.1/gremlin_python/structure/io/util.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/gremlinpython.egg-info/PKG-INFO` & `gremlinpython-3.7.1/gremlinpython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.7.0
+Version: 3.7.1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.7.0/gremlinpython.egg-info/SOURCES.txt` & `gremlinpython-3.7.1/gremlinpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.7.0/setup.py` & `gremlinpython-3.7.1/setup.py`

 * *Files identical despite different names*

