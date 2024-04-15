# Comparing `tmp/trinnov_altitude-1.2.2.tar.gz` & `tmp/trinnov_altitude-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov_altitude-1.2.2.tar", last modified: Sat Apr 13 19:30:42 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.2.3.tar", last modified: Sun Apr 14 17:40:34 2024, max compression
```

## Comparing `trinnov_altitude-1.2.2.tar` & `trinnov_altitude-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26189 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:40:34.463965 trinnov_altitude-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-14 17:40:34.463965 trinnov_altitude-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-14 17:40:34.463965 trinnov_altitude-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:40:34.459965 trinnov_altitude-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:40:34.459965 trinnov_altitude-1.2.3/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-14 17:40:30.000000 trinnov_altitude-1.2.3/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:40:34.463965 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-14 17:40:34.000000 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-14 17:40:34.000000 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:40:34.000000 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 17:40:34.000000 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 17:40:34.000000 trinnov_altitude-1.2.3/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov_altitude-1.2.2/LICENSE` & `trinnov_altitude-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/PKG-INFO` & `trinnov_altitude-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.2
+Version: 1.2.3
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,16 +13,15 @@
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wakeonlan>=3.1
 
 # Trinnov Altitude Python Library
 
-A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the
-[TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude.
+A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the [TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude. Initially built for the [Trinnov Altitude Home Assistant integration] (https://github.com/binarylogic/trinnov-altitude-homeassistant)
 
 ## Overview
 
 The Trinnov Altitude processor is an audio/video processor that exposes an
 automation protocol over TCP/IP for remote control.
 
 The interface is a two-way communication protocol. At any time the processor
```

### Comparing `trinnov_altitude-1.2.2/README.md` & `trinnov_altitude-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Trinnov Altitude Python Library
 
-A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the
-[TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude.
+A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the [TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude. Initially built for the [Trinnov Altitude Home Assistant integration] (https://github.com/binarylogic/trinnov-altitude-homeassistant)
 
 ## Overview
 
 The Trinnov Altitude processor is an audio/video processor that exposes an
 automation protocol over TCP/IP for remote control.
 
 The interface is a two-way communication protocol. At any time the processor
```

### Comparing `trinnov_altitude-1.2.2/setup.cfg` & `trinnov_altitude-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/tests/test_trinnov_altitude.py` & `trinnov_altitude-1.2.3/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude/const.py` & `trinnov_altitude-1.2.3/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude/exceptions.py` & `trinnov_altitude-1.2.3/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude/messages.py` & `trinnov_altitude-1.2.3/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude/mocks.py` & `trinnov_altitude-1.2.3/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude/trinnov_altitude.py` & `trinnov_altitude-1.2.3/trinnov_altitude/trinnov_altitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,22 @@
     def power_on(self):
         """Power on."""
         if self.mac is None:
             raise exceptions.NoMacAddressError()
 
         send_magic_packet(self.mac)
 
+    def power_on_available(self) -> bool:
+        """
+        Can the device be powered on.
+
+        A mac address is required to do so.
+        """
+        return self.mac is not None
+
     async def preset_get(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Requests the current present.
         """
         await self._write("get_current_preset", timeout)
 
     async def preset_set(
@@ -634,47 +642,54 @@
         Raise the volume by 0.5 dB
         """
         await self.volume_adjust(0.5, timeout)
 
     # --------------------------
     # Utility
     # --------------------------
-    async def _listen(self, reconnect: bool, backoff: float):
+    async def _listen(
+        self,
+        read_timeout: float = 30.0,
+        read_backoff: float = 1.0,
+        reconnect: bool = True,
+        reconnect_timeout: float = 2.0,
+        reconnect_backoff: float = 2.0,
+    ):
         """
         Listen for messages and sync internal state
 
         This method will automatically reconnect when necessary if `reconnect`
         is set to `True`.
         """
         try:
             while True:
                 try:
-                    await self._read(backoff)
+                    await self._read(read_timeout)
                 except asyncio.TimeoutError:
                     self.logger.debug(
-                        f"Read operation timed out, trying again in {backoff} seconds"
+                        f"Read operation timed out, trying again in {read_backoff} seconds"
                     )
-                    await asyncio.sleep(backoff)
+                    await asyncio.sleep(read_backoff)
                 except (exceptions.NotConnectedError, EOFError, OSError) as e:
                     if reconnect:
                         self.logger.debug(
                             f"Unable to read message from Trinnov Altitude, reconnecting...: {e}",
                         )
 
                         try:
-                            await self.reconnect(timeout=backoff)
+                            await self.reconnect(timeout=reconnect_timeout)
                         except (
                             asyncio.TimeoutError,
                             exceptions.ConnectionTimeoutError,
                             exceptions.ConnectionFailedError,
                         ) as e:
                             self.logger.debug(
-                                f"Trinnov Altitude reconnect failed, trying again in {backoff} seconds...: {e}"
+                                f"Trinnov Altitude reconnect failed, trying again in {reconnect_backoff} seconds...: {e}"
                             )
-                            await asyncio.sleep(backoff)
+                            await asyncio.sleep(reconnect_backoff)
                     else:
                         raise e
         except asyncio.CancelledError:
             self.logger.debug(
                 "Trinnov Altitude listen task received cancel, shutting down..."
             )
```

### Comparing `trinnov_altitude-1.2.2/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1.2.3/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.2
+Version: 1.2.3
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,16 +13,15 @@
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wakeonlan>=3.1
 
 # Trinnov Altitude Python Library
 
-A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the
-[TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude.
+A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the [TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude. Initially built for the [Trinnov Altitude Home Assistant integration] (https://github.com/binarylogic/trinnov-altitude-homeassistant)
 
 ## Overview
 
 The Trinnov Altitude processor is an audio/video processor that exposes an
 automation protocol over TCP/IP for remote control.
 
 The interface is a two-way communication protocol. At any time the processor
```

