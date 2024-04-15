# Comparing `tmp/nacl_middleware-0.0.7.tar.gz` & `tmp/nacl_middleware-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacl_middleware-0.0.7.tar", last modified: Mon Apr 15 15:19:52 2024, max compression
+gzip compressed data, was "nacl_middleware-0.0.8.tar", last modified: Mon Apr 15 17:26:27 2024, max compression
```

## Comparing `nacl_middleware-0.0.7.tar` & `nacl_middleware-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8442 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6825 2024-04-15 15:18:08.000000 nacl_middleware-0.0.7/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.339354 nacl_middleware-0.0.7/nacl_middleware/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.7/nacl_middleware/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/nacl_middleware/nacl_middleware.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3086 2024-04-15 10:14:26.000000 nacl_middleware-0.0.7/nacl_middleware/nacl_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/nacl_middleware/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/nacl_middleware.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8442 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-15 15:19:40.000000 nacl_middleware-0.0.7/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/tests/test_server.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 17:26:27.904315 nacl_middleware-0.0.8/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8135 2024-04-15 17:26:27.904315 nacl_middleware-0.0.8/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6518 2024-04-15 17:26:12.000000 nacl_middleware-0.0.8/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 17:26:27.894315 nacl_middleware-0.0.8/nacl_middleware/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.8/nacl_middleware/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.8/nacl_middleware/nacl_middleware.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3128 2024-04-15 17:26:12.000000 nacl_middleware-0.0.8/nacl_middleware/nacl_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.8/nacl_middleware/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 17:26:27.904315 nacl_middleware-0.0.8/nacl_middleware.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8135 2024-04-15 17:26:27.000000 nacl_middleware-0.0.8/nacl_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-15 17:26:27.000000 nacl_middleware-0.0.8/nacl_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-15 17:26:27.000000 nacl_middleware-0.0.8/nacl_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-15 17:26:27.000000 nacl_middleware-0.0.8/nacl_middleware.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-15 17:26:27.000000 nacl_middleware-0.0.8/nacl_middleware.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-15 17:26:12.000000 nacl_middleware-0.0.8/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-15 17:26:27.904315 nacl_middleware-0.0.8/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 17:26:27.904315 nacl_middleware-0.0.8/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.8/tests/test_server.py
```

### Comparing `nacl_middleware-0.0.7/PKG-INFO` & `nacl_middleware-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.7
+Version: 0.0.8
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -61,105 +61,99 @@
 
 
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
-    from aiohttp.web import Application, json_response, run_app
-    from nacl.public import PrivateKey
-
+    from aiohttp.web import Application, Response, run_app
     from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
-    public_key_hex = pynacl.decodedPublicKey()
+    pynacl = Nacl()
+    public_key_hex = pynacl.decoded_public_key()
     print(public_key_hex)
 
     app = Application(middlewares=[
-        nacl_middleware(private_key)
+        nacl_middleware(pynacl.private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
         mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
-            return json_response(mail_box.box('You are welcome!'))
-        return json_response(mail_box.box("Pardon me?"))
+            text = 'You are welcome!'
+        text = "Pardon me?"
+        return Response(text = mail_box.box(text))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
 
 
 Example Client Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
-    from nacl.public import PrivateKey
     from nacl_middleware import MailBox, Nacl
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
+    pynacl = Nacl()
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
-        mail_box = MailBox(private_key, server_hex_public_key)
+        mail_box = MailBox(pynacl.private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": pynacl.decodedPublicKey(),
+                "publicKey": pynacl.decoded_public_key(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
-                encryted_reply = await response.json()
+                encryted_reply = await response.text()
                 reply = mail_box.unbox(encryted_reply)
                 print("Reply:", reply)
 
     run(main())
 
 .. warning::
 
     Make sure the server's public key in this client code example is correctly set to the public key print by the server's example code in the console.
 
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
-        from aiohttp.web import Application, json_response, run_app
-        from nacl.public import PrivateKey
-
+        from aiohttp.web import Application, Response, run_app
         from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-        private_key = PrivateKey.generate()
-        pynacl = Nacl(private_key)
-        public_key_hex = pynacl.decodedPublicKey()
+        pynacl = Nacl()
+        public_key_hex = pynacl.decoded_public_key()
         print(public_key_hex)
 
         app = Application(middlewares=[
-            nacl_middleware(private_key, exclude_routes=['/get_public_key'])
+            nacl_middleware(pynacl.private_key)
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
-                return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Pardon me?"))
+                text = 'You are welcome!'
+            text = "Pardon me?"
+            return Response(text = mail_box.box(text))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            return json_response(public_key_hex)
+            return Response(text = public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.7/README.rst` & `nacl_middleware-0.0.8/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -20,105 +20,99 @@
 
 
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
-    from aiohttp.web import Application, json_response, run_app
-    from nacl.public import PrivateKey
-
+    from aiohttp.web import Application, Response, run_app
     from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
-    public_key_hex = pynacl.decodedPublicKey()
+    pynacl = Nacl()
+    public_key_hex = pynacl.decoded_public_key()
     print(public_key_hex)
 
     app = Application(middlewares=[
-        nacl_middleware(private_key)
+        nacl_middleware(pynacl.private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
         mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
-            return json_response(mail_box.box('You are welcome!'))
-        return json_response(mail_box.box("Pardon me?"))
+            text = 'You are welcome!'
+        text = "Pardon me?"
+        return Response(text = mail_box.box(text))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
 
 
 Example Client Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
-    from nacl.public import PrivateKey
     from nacl_middleware import MailBox, Nacl
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
+    pynacl = Nacl()
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
-        mail_box = MailBox(private_key, server_hex_public_key)
+        mail_box = MailBox(pynacl.private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": pynacl.decodedPublicKey(),
+                "publicKey": pynacl.decoded_public_key(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
-                encryted_reply = await response.json()
+                encryted_reply = await response.text()
                 reply = mail_box.unbox(encryted_reply)
                 print("Reply:", reply)
 
     run(main())
 
 .. warning::
 
     Make sure the server's public key in this client code example is correctly set to the public key print by the server's example code in the console.
 
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
-        from aiohttp.web import Application, json_response, run_app
-        from nacl.public import PrivateKey
-
+        from aiohttp.web import Application, Response, run_app
         from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-        private_key = PrivateKey.generate()
-        pynacl = Nacl(private_key)
-        public_key_hex = pynacl.decodedPublicKey()
+        pynacl = Nacl()
+        public_key_hex = pynacl.decoded_public_key()
         print(public_key_hex)
 
         app = Application(middlewares=[
-            nacl_middleware(private_key, exclude_routes=['/get_public_key'])
+            nacl_middleware(pynacl.private_key)
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
-                return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Pardon me?"))
+                text = 'You are welcome!'
+            text = "Pardon me?"
+            return Response(text = mail_box.box(text))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            return json_response(public_key_hex)
+            return Response(text = public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.7/nacl_middleware/nacl_middleware.py` & `nacl_middleware-0.0.8/nacl_middleware/nacl_middleware.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.7/nacl_middleware/nacl_utils.py` & `nacl_middleware-0.0.8/nacl_middleware/nacl_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 class Nacl:
     """
     A class that provides utility functions for encoding and decoding Nacl keys.
     """
 
     private_key: PrivateKey
 
-    def __init__(self, private_key: PrivateKey, encoder=HexEncoder) -> None:
+    def __init__(
+        self, private_key: PrivateKey = PrivateKey.generate(), encoder=HexEncoder
+    ) -> None:
         self.private_key = private_key
         self.encoder = encoder
 
     def _decode(self, parameter: Union[PrivateKey, PublicKey]) -> str:
         """
         Decode the given Nacl key parameter using the specified encoder.
 
@@ -24,24 +26,24 @@
             parameter (Union[PrivateKey, PublicKey]): The Nacl key parameter to decode.
 
         Returns:
             str: The decoded Nacl key as a string.
         """
         return parameter.encode(encoder=self.encoder).decode()
 
-    def decodedPrivateKey(self) -> str:
+    def decoded_private_key(self) -> str:
         """
         Decode the private key using the specified encoder.
 
         Returns:
             str: The decoded private key as a string.
         """
         return self._decode(self.private_key)
 
-    def decodedPublicKey(self) -> str:
+    def decoded_public_key(self) -> str:
         """
         Decode the public key of the private key using the specified encoder.
 
         Returns:
             str: The decoded public key as a string.
         """
         return self._decode(self.private_key.public_key)
```

### Comparing `nacl_middleware-0.0.7/nacl_middleware/utils.py` & `nacl_middleware-0.0.8/nacl_middleware/utils.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.7/nacl_middleware.egg-info/PKG-INFO` & `nacl_middleware-0.0.8/nacl_middleware.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.7
+Version: 0.0.8
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -61,105 +61,99 @@
 
 
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
-    from aiohttp.web import Application, json_response, run_app
-    from nacl.public import PrivateKey
-
+    from aiohttp.web import Application, Response, run_app
     from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
-    public_key_hex = pynacl.decodedPublicKey()
+    pynacl = Nacl()
+    public_key_hex = pynacl.decoded_public_key()
     print(public_key_hex)
 
     app = Application(middlewares=[
-        nacl_middleware(private_key)
+        nacl_middleware(pynacl.private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
         mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
-            return json_response(mail_box.box('You are welcome!'))
-        return json_response(mail_box.box("Pardon me?"))
+            text = 'You are welcome!'
+        text = "Pardon me?"
+        return Response(text = mail_box.box(text))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
 
 
 Example Client Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
-    from nacl.public import PrivateKey
     from nacl_middleware import MailBox, Nacl
 
-    private_key = PrivateKey.generate()
-    pynacl = Nacl(private_key)
+    pynacl = Nacl()
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
-        mail_box = MailBox(private_key, server_hex_public_key)
+        mail_box = MailBox(pynacl.private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": pynacl.decodedPublicKey(),
+                "publicKey": pynacl.decoded_public_key(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
-                encryted_reply = await response.json()
+                encryted_reply = await response.text()
                 reply = mail_box.unbox(encryted_reply)
                 print("Reply:", reply)
 
     run(main())
 
 .. warning::
 
     Make sure the server's public key in this client code example is correctly set to the public key print by the server's example code in the console.
 
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
-        from aiohttp.web import Application, json_response, run_app
-        from nacl.public import PrivateKey
-
+        from aiohttp.web import Application, Response, run_app
         from nacl_middleware import nacl_middleware, Nacl, MailBox
 
-        private_key = PrivateKey.generate()
-        pynacl = Nacl(private_key)
-        public_key_hex = pynacl.decodedPublicKey()
+        pynacl = Nacl()
+        public_key_hex = pynacl.decoded_public_key()
         print(public_key_hex)
 
         app = Application(middlewares=[
-            nacl_middleware(private_key, exclude_routes=['/get_public_key'])
+            nacl_middleware(pynacl.private_key)
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
-                return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Pardon me?"))
+                text = 'You are welcome!'
+            text = "Pardon me?"
+            return Response(text = mail_box.box(text))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            return json_response(public_key_hex)
+            return Response(text = public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.7/pyproject.toml` & `nacl_middleware-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Declare the build backend (required)
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "nacl_middleware"
-version = "0.0.7"
+version = "0.0.8"
 description = "aiohttp compatible pynacl middleware"
 license = { text = "GNU General Public License v3 or later (GPLv3+)" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `nacl_middleware-0.0.7/tests/test_server.py` & `nacl_middleware-0.0.8/tests/test_server.py`

 * *Files identical despite different names*

