# Comparing `tmp/nacl_middleware-0.0.6.tar.gz` & `tmp/nacl_middleware-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacl_middleware-0.0.6.tar", last modified: Sun Apr 14 02:45:04 2024, max compression
+gzip compressed data, was "nacl_middleware-0.0.7.tar", last modified: Mon Apr 15 15:19:52 2024, max compression
```

## Comparing `nacl_middleware-0.0.6.tar` & `nacl_middleware-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8629 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7012 2024-04-14 02:43:39.000000 nacl_middleware-0.0.6/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/nacl_middleware/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.6/nacl_middleware/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.6/nacl_middleware/nacl_middleware.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2999 2024-04-14 00:46:30.000000 nacl_middleware-0.0.6/nacl_middleware/nacl_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.6/nacl_middleware/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/nacl_middleware.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8629 2024-04-14 02:45:04.000000 nacl_middleware-0.0.6/nacl_middleware.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-14 02:45:04.000000 nacl_middleware-0.0.6/nacl_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-14 02:45:04.000000 nacl_middleware-0.0.6/nacl_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-14 02:45:04.000000 nacl_middleware-0.0.6/nacl_middleware.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-14 02:45:04.000000 nacl_middleware-0.0.6/nacl_middleware.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-14 02:44:38.000000 nacl_middleware-0.0.6/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:45:04.555916 nacl_middleware-0.0.6/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.6/tests/test_server.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8442 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6825 2024-04-15 15:18:08.000000 nacl_middleware-0.0.7/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.339354 nacl_middleware-0.0.7/nacl_middleware/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.7/nacl_middleware/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/nacl_middleware/nacl_middleware.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3086 2024-04-15 10:14:26.000000 nacl_middleware-0.0.7/nacl_middleware/nacl_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/nacl_middleware/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/nacl_middleware.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8442 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-15 15:19:52.000000 nacl_middleware-0.0.7/nacl_middleware.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-15 15:19:40.000000 nacl_middleware-0.0.7/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:19:52.349354 nacl_middleware-0.0.7/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.7/tests/test_server.py
```

### Comparing `nacl_middleware-0.0.6/PKG-INFO` & `nacl_middleware-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.6
+Version: 0.0.7
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -63,29 +63,29 @@
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp.web import Application, json_response, run_app
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
 
-    from nacl_middleware import nacl_middleware
+    from nacl_middleware import nacl_middleware, Nacl, MailBox
 
     private_key = PrivateKey.generate()
-    public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+    pynacl = Nacl(private_key)
+    public_key_hex = pynacl.decodedPublicKey()
     print(public_key_hex)
 
     app = Application(middlewares=[
         nacl_middleware(private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
-        mail_box = request['mail_box']
+        mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
             return json_response(mail_box.box('You are welcome!'))
         return json_response(mail_box.box("Pardon me?"))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
@@ -95,28 +95,26 @@
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
-    from nacl_middleware import MailBox
+    from nacl_middleware import MailBox, Nacl
 
     private_key = PrivateKey.generate()
+    pynacl = Nacl(private_key)
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
         mail_box = MailBox(private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": private_key.public_key.encode(
-                    encoder=HexEncoder
-                ).decode(),
+                "publicKey": pynacl.decodedPublicKey(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
                 encryted_reply = await response.json()
                 reply = mail_box.unbox(encryted_reply)
@@ -131,38 +129,37 @@
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
         from aiohttp.web import Application, json_response, run_app
         from nacl.public import PrivateKey
-        from nacl.encoding import HexEncoder
 
-        from nacl_middleware import nacl_middleware
+        from nacl_middleware import nacl_middleware, Nacl, MailBox
 
         private_key = PrivateKey.generate()
-        public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+        pynacl = Nacl(private_key)
+        public_key_hex = pynacl.decodedPublicKey()
         print(public_key_hex)
 
         app = Application(middlewares=[
             nacl_middleware(private_key, exclude_routes=['/get_public_key'])
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
-            mail_box = request['mail_box']
+            mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
             return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            decoded_public_key = Nacl(private_key).decodedPublicKey()
-            return json_response(decoded_public_key)
+            return json_response(public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.6/README.rst` & `nacl_middleware-0.0.7/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp.web import Application, json_response, run_app
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
 
-    from nacl_middleware import nacl_middleware
+    from nacl_middleware import nacl_middleware, Nacl, MailBox
 
     private_key = PrivateKey.generate()
-    public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+    pynacl = Nacl(private_key)
+    public_key_hex = pynacl.decodedPublicKey()
     print(public_key_hex)
 
     app = Application(middlewares=[
         nacl_middleware(private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
-        mail_box = request['mail_box']
+        mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
             return json_response(mail_box.box('You are welcome!'))
         return json_response(mail_box.box("Pardon me?"))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
@@ -54,28 +54,26 @@
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
-    from nacl_middleware import MailBox
+    from nacl_middleware import MailBox, Nacl
 
     private_key = PrivateKey.generate()
+    pynacl = Nacl(private_key)
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
         mail_box = MailBox(private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": private_key.public_key.encode(
-                    encoder=HexEncoder
-                ).decode(),
+                "publicKey": pynacl.decodedPublicKey(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
                 encryted_reply = await response.json()
                 reply = mail_box.unbox(encryted_reply)
@@ -90,38 +88,37 @@
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
         from aiohttp.web import Application, json_response, run_app
         from nacl.public import PrivateKey
-        from nacl.encoding import HexEncoder
 
-        from nacl_middleware import nacl_middleware
+        from nacl_middleware import nacl_middleware, Nacl, MailBox
 
         private_key = PrivateKey.generate()
-        public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+        pynacl = Nacl(private_key)
+        public_key_hex = pynacl.decodedPublicKey()
         print(public_key_hex)
 
         app = Application(middlewares=[
             nacl_middleware(private_key, exclude_routes=['/get_public_key'])
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
-            mail_box = request['mail_box']
+            mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
             return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            decoded_public_key = Nacl(private_key).decodedPublicKey()
-            return json_response(decoded_public_key)
+            return json_response(public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.6/nacl_middleware/nacl_middleware.py` & `nacl_middleware-0.0.7/nacl_middleware/nacl_middleware.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.6/nacl_middleware/nacl_utils.py` & `nacl_middleware-0.0.7/nacl_middleware/nacl_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,38 +60,48 @@
     """
     if isinstance(obj, str):
         obj = f'"{obj}"'
     return loads(obj)
 
 
 class MailBox:
-    """
-    A class representing a mailbox for encryption and decryption of messages.
-
-    Attributes:
-        _private_key (PrivateKey): The private key used for encryption and decryption.
-        _box (Box): The encryption and decryption box.
-
-    Methods:
-        __init__(self, private_key: PrivateKey, hex_public_key: str) -> None:
-            Initializes the MailBox with the provided private key and hex-encoded public key.
-
-        unbox(self, encrypted_message) -> any:
-            Decrypts the encrypted message using the private key and returns the decrypted message.
-
-        box(self, message: any) -> str:
-            Encrypts the message using the public key and returns the encrypted message as a string.
-    """
-
     _private_key: PrivateKey
     _box: Box
 
     def __init__(self, private_key: PrivateKey, hex_public_key: str) -> None:
+        """
+        Initializes the MailBox with the provided private key and hex-encoded public key.
+
+        Parameters:
+        private_key (PrivateKey): The private key used for encryption and decryption.
+        hex_public_key (str): The hex-encoded public key.
+
+        Returns:
+        None
+        """
         self._private_key = private_key
         self._box = Box(self._private_key, PublicKey(hex_public_key, HexEncoder))
 
-    def unbox(self, encrypted_message) -> any:
+    def unbox(self, encrypted_message: str) -> any:
+        """
+        Decrypts the encrypted message using the private key and returns the decrypted message.
+
+        Parameters:
+        encrypted_message (str): The encrypted message to be decrypted.
+
+        Returns:
+        any: The decrypted message.
+        """
         decrypted_message = self._box.decrypt(encrypted_message, encoder=Base64Encoder)
         return custom_loads(decrypted_message)
 
     def box(self, message: any) -> str:
+        """
+        Encrypts the given message using the NaCl encryption algorithm.
+
+        Parameters:
+        message (any): The message to be encrypted.
+
+        Returns:
+        str: The encrypted message as a string.
+        """
         return self._box.encrypt(dumps(message).encode(), encoder=Base64Encoder).decode()
```

### Comparing `nacl_middleware-0.0.6/nacl_middleware/utils.py` & `nacl_middleware-0.0.7/nacl_middleware/utils.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.6/nacl_middleware.egg-info/PKG-INFO` & `nacl_middleware-0.0.7/nacl_middleware.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.6
+Version: 0.0.7
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -63,29 +63,29 @@
 Example Server Code
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp.web import Application, json_response, run_app
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
 
-    from nacl_middleware import nacl_middleware
+    from nacl_middleware import nacl_middleware, Nacl, MailBox
 
     private_key = PrivateKey.generate()
-    public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+    pynacl = Nacl(private_key)
+    public_key_hex = pynacl.decodedPublicKey()
     print(public_key_hex)
 
     app = Application(middlewares=[
         nacl_middleware(private_key)
     ])
 
     async def thanks_handler(request):
         decrypted_message = request['decrypted_message']
-        mail_box = request['mail_box']
+        mail_box: MailBox = request['mail_box']
         if decrypted_message == 'Thank you!':
             return json_response(mail_box.box('You are welcome!'))
         return json_response(mail_box.box("Pardon me?"))
 
     app.router.add_get('/handle_thanks', thanks_handler)
 
     run_app(app)
@@ -95,28 +95,26 @@
 ^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     from aiohttp import ClientSession
     from asyncio import run
     from nacl.public import PrivateKey
-    from nacl.encoding import HexEncoder
-    from nacl_middleware import MailBox
+    from nacl_middleware import MailBox, Nacl
 
     private_key = PrivateKey.generate()
+    pynacl = Nacl(private_key)
     server_hex_public_key = "cbe3b3cf345b24bd050db13bb5f1165f47f36f7151bbba9b27bdef0922674f4d"
 
     async def main():
         mail_box = MailBox(private_key, server_hex_public_key)
 
         def get_params(message):
             return {
-                "publicKey": private_key.public_key.encode(
-                    encoder=HexEncoder
-                ).decode(),
+                "publicKey": pynacl.decodedPublicKey(),
                 "encryptedMessage": mail_box.box(message)
             }
 
         async with ClientSession() as session:
             async with session.get('http://localhost:8080/handle_thanks', params=get_params('Thank you!')) as response:
                 encryted_reply = await response.json()
                 reply = mail_box.unbox(encryted_reply)
@@ -131,38 +129,37 @@
 .. tip::
    Add a path to get the server's public key to the middleware's route exclusion to allow the server's public key to be obtained by sending a GET request to the server's public key endpoint with, for example:
 
     .. code-block:: python
 
         from aiohttp.web import Application, json_response, run_app
         from nacl.public import PrivateKey
-        from nacl.encoding import HexEncoder
 
-        from nacl_middleware import nacl_middleware
+        from nacl_middleware import nacl_middleware, Nacl, MailBox
 
         private_key = PrivateKey.generate()
-        public_key_hex = private_key.public_key.encode(encoder=HexEncoder).decode()
+        pynacl = Nacl(private_key)
+        public_key_hex = pynacl.decodedPublicKey()
         print(public_key_hex)
 
         app = Application(middlewares=[
             nacl_middleware(private_key, exclude_routes=['/get_public_key'])
         ])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
-            mail_box = request['mail_box']
+            mail_box: MailBox = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
             return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
-            decoded_public_key = Nacl(private_key).decodedPublicKey()
-            return json_response(decoded_public_key)
+            return json_response(public_key_hex)
 
         app.router.add_get("/get_public_key", get_public_key)
 
         run_app(app)
 
 
 Development
```

### Comparing `nacl_middleware-0.0.6/pyproject.toml` & `nacl_middleware-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Declare the build backend (required)
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "nacl_middleware"
-version = "0.0.6"
+version = "0.0.7"
 description = "aiohttp compatible pynacl middleware"
 license = { text = "GNU General Public License v3 or later (GPLv3+)" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `nacl_middleware-0.0.6/tests/test_server.py` & `nacl_middleware-0.0.7/tests/test_server.py`

 * *Files identical despite different names*

