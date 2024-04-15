# Comparing `tmp/dm-aiomodbus-0.1.5.tar.gz` & `tmp/dm_aiomodbus-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-aiomodbus-0.1.5.tar", last modified: Sun Mar 31 07:01:57 2024, max compression
+gzip compressed data, was "dm_aiomodbus-0.1.6.tar", last modified: Mon Apr 15 07:48:33 2024, max compression
```

## Comparing `dm-aiomodbus-0.1.5.tar` & `dm_aiomodbus-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:01:57.556810 dm-aiomodbus-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-31 07:01:57.556810 dm-aiomodbus-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:01:57.556810 dm-aiomodbus-0.1.5/dm_aiomodbus/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/dm_aiomodbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_simulator_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-31 07:01:45.000000 dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_temp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:01:57.556810 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 07:01:57.556810 dm-aiomodbus-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-31 07:01:57.000000 dm-aiomodbus-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:48:33.026452 dm_aiomodbus-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-15 07:48:33.026452 dm_aiomodbus-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:48:33.022452 dm_aiomodbus-0.1.6/dm_aiomodbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/dm_aiomodbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_simulator_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-15 07:48:22.000000 dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_temp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:48:33.026452 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:48:33.026452 dm_aiomodbus-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-15 07:48:32.000000 dm_aiomodbus-0.1.6/setup.py
```

### Comparing `dm-aiomodbus-0.1.5/PKG-INFO` & `dm_aiomodbus-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomodbus
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is my custom aiomodbus client
 Home-page: https://pypi.org/project/dm-aiomodbus
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomodbus
 Keywords: dm aiomodbus
 Classifier: Programming Language :: Python :: 3.8
@@ -19,26 +19,14 @@
 # DM-aiomodbus
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomodbus)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomodbus)
 
-### Run in Windows
-
-_If you run async code in **Windows**, set correct selector_
-
-```python
-import asyncio
-import sys
-
-if sys.platform == "win32":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-```
-
 ## Usage
 
 ### Connection
 
 * Serial
    ```python
    from dm_aiomodbus import DMAioModbusSerialClient
@@ -69,29 +57,29 @@
 from dm_aiomodbus import DMAioModbusTcpClient, DMAioModbusTempClientInterface
 import asyncio
 
 
 async def main():
     # create client
     modbus_client = DMAioModbusTcpClient(
-       host="192.168.0.0",
-       port=501,
-       name_tag="my_tcp_plc"
+        host="192.168.0.0",
+        port=501,
+        name_tag="my_tcp_plc"
     )
 
     # create read callback
     async def read_callback(client: DMAioModbusTempClientInterface):
-        reg_258_259 = await client.read_holding_registers(258, count=2)
-        reg_256 = await client.read_holding_registers(256)
-        reg_260_2 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
+        reg_258_259, err1 = await client.read_holding_registers(258, count=2)  # get values and error if any
+        reg_256, err2 = await client.read_holding_registers(256)
+        reg_260_2, err3 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
         print(reg_258_259, reg_256, reg_260_2)
 
     # create read callback
     async def write_callback(client: DMAioModbusTempClientInterface):
-        await client.write_register(256, 1)
+        status, err = await client.write_register(256, 1)  # get write status and error if any
         await client.write_register(260, value=0, slave=2)  # write second slave-device
 
     # request to plc
     modbus_client.execute(read_callback)  # execute without waiting result
     # or
     await modbus_client.execute_and_return(write_callback, timeout=3)  # execute and wait result with timeout 3s (default 5)
 
@@ -129,7 +117,19 @@
     def error(self, message):
         print(message)
 
 
 # set up custom logger for all clients
 DMAioModbusTcpClient.set_logger(MyLogger())
 ```
+
+### Run in Windows
+
+_If you run async code in **Windows**, set correct selector_
+
+```python
+import asyncio
+import sys
+
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+```
```

### Comparing `dm-aiomodbus-0.1.5/README.md` & `dm_aiomodbus-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 # DM-aiomodbus
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomodbus)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomodbus)
 
-### Run in Windows
-
-_If you run async code in **Windows**, set correct selector_
-
-```python
-import asyncio
-import sys
-
-if sys.platform == "win32":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-```
-
 ## Usage
 
 ### Connection
 
 * Serial
    ```python
    from dm_aiomodbus import DMAioModbusSerialClient
@@ -51,29 +39,29 @@
 from dm_aiomodbus import DMAioModbusTcpClient, DMAioModbusTempClientInterface
 import asyncio
 
 
 async def main():
     # create client
     modbus_client = DMAioModbusTcpClient(
-       host="192.168.0.0",
-       port=501,
-       name_tag="my_tcp_plc"
+        host="192.168.0.0",
+        port=501,
+        name_tag="my_tcp_plc"
     )
 
     # create read callback
     async def read_callback(client: DMAioModbusTempClientInterface):
-        reg_258_259 = await client.read_holding_registers(258, count=2)
-        reg_256 = await client.read_holding_registers(256)
-        reg_260_2 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
+        reg_258_259, err1 = await client.read_holding_registers(258, count=2)  # get values and error if any
+        reg_256, err2 = await client.read_holding_registers(256)
+        reg_260_2, err3 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
         print(reg_258_259, reg_256, reg_260_2)
 
     # create read callback
     async def write_callback(client: DMAioModbusTempClientInterface):
-        await client.write_register(256, 1)
+        status, err = await client.write_register(256, 1)  # get write status and error if any
         await client.write_register(260, value=0, slave=2)  # write second slave-device
 
     # request to plc
     modbus_client.execute(read_callback)  # execute without waiting result
     # or
     await modbus_client.execute_and_return(write_callback, timeout=3)  # execute and wait result with timeout 3s (default 5)
 
@@ -111,7 +99,19 @@
     def error(self, message):
         print(message)
 
 
 # set up custom logger for all clients
 DMAioModbusTcpClient.set_logger(MyLogger())
 ```
+
+### Run in Windows
+
+_If you run async code in **Windows**, set correct selector_
+
+```python
+import asyncio
+import sys
+
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+```
```

### Comparing `dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_base_client.py` & `dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from typing import Callable, Coroutine, Type
 from dm_logger import DMLogger
 from pymodbus.client import AsyncModbusSerialClient, AsyncModbusTcpClient
 from pymodbus import ModbusException, ExceptionResponse
+from pymodbus.pdu import ModbusExceptions
 import asyncio
 from .aiomodbus_temp_client import DMAioModbusTempClientInterface
 
 __all__ = ['DMAioModbusBaseClient']
 
 
 class DMAioModbusBaseClient:
@@ -100,98 +101,101 @@
     def _is_connected(self) -> bool:
         return self.__client.connected
 
     async def _connect(self) -> None:
         try:
             if not await self.__client.connect():
                 raise ConnectionError("No connection established")
-            self._logger.info("Connected!")
         except Exception as e:
             self._logger.error(f"Connection error: {e}")
 
     def _disconnect(self) -> None:
         self.__client.close()
-        self._logger.info("Disconnected!")
 
     async def __wait_on_disconnect(self) -> None:
         await asyncio.sleep(self.__disconnect_time_s)
 
         if self._is_connected:
             self._disconnect()
 
-    async def __error_handler(self, method: Callable, kwargs: dict) -> None:
+    async def __error_handler(self, method: Callable, kwargs: dict) -> (any, str):
+        result = None
+        error = ""
         try:
             result = await method(**kwargs)
             await asyncio.sleep(self.__after_execute_timeout_ms)
             if result.isError() or isinstance(result, ExceptionResponse):
+                error = f"{result.exception_code}_{ModbusExceptions.decode(result.exception_code)}"
                 raise ModbusException(result)
-            return result
         except Exception as e:
             self._logger.error(f"Error: {e}", method=method.__name__, params=kwargs)
+            if not error:
+                error = str(e)
             if not self._is_connected:
                 await self._connect()
+        return (result, error)
 
-    async def _read(self, method, kwargs: dict) -> list | None:
-        result = await self.__error_handler(method, kwargs)
-        return result.registers if hasattr(result, "registers") else []
-
-    async def _write(self, method, kwargs: dict) -> bool:
-        result = await self.__error_handler(method, kwargs)
-        return bool(result)
+    async def _read(self, method, kwargs: dict) -> (list, str):
+        result, error = await self.__error_handler(method, kwargs)
+        return (result.registers, error) if hasattr(result, "registers") else ([], error)
 
-    async def __read_coils(self, address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def _write(self, method, kwargs: dict) -> (bool, str):
+        result, error = await self.__error_handler(method, kwargs)
+        return (bool(result), error)
+
+    async def __read_coils(self, address: int, count: int = 1, slave: int = 1) -> (list, str):
         return await self._read(self.__client.read_coils, {
             "address": address,
             "count": count,
             "slave": slave
         })
 
-    async def __read_discrete_inputs(self, address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def __read_discrete_inputs(self, address: int, count: int = 1, slave: int = 1) -> (list, str):
         return await self._read(self.__client.read_discrete_inputs, {
             "address": address,
             "count": count,
             "slave": slave
         })
 
-    async def __read_holding_registers(self, address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def __read_holding_registers(self, address: int, count: int = 1, slave: int = 1) -> (list, str):
         return await self._read(self.__client.read_holding_registers, {
             "address": address,
             "count": count,
             "slave": slave
         })
 
-    async def __read_input_registers(self, address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def __read_input_registers(self, address: int, count: int = 1, slave: int = 1) -> (list, str):
         return await self._read(self.__client.read_input_registers, {
             "address": address,
             "count": count,
             "slave": slave
         })
 
-    async def __write_coil(self, address: int, value: int, slave: int = 1) -> bool:
+    async def __write_coil(self, address: int, value: int, slave: int = 1) -> (bool, str):
         return await self._write(self.__client.write_coil, {
             "address": address,
             "value": value,
             "slave": slave
         })
 
-    async def __write_register(self, address: int, value: int, slave: int = 1) -> bool:
+    async def __write_register(self, address: int, value: int, slave: int = 1) -> (bool, str):
         return await self._write(self.__client.write_register, {
             "address": address,
             "value": value,
             "slave": slave
         })
 
-    async def __write_coils(self, address: int, values: list[int] | int, slave: int = 1) -> bool:
+    async def __write_coils(self, address: int, values: list[int] | int, slave: int = 1) -> (bool, str):
         return await self._write(self.__client.write_coils, {
             "address": address,
             "values": values,
             "slave": slave
         })
 
-    async def __write_registers(self, address: int, values: list[int] | int, slave: int = 1) -> bool:
+    async def __write_registers(self, address: int, values: list[int] | int, slave: int = 1) -> (bool, str):
         return await self._write(self.__client.write_registers, {
             "address": address,
             "values": values,
             "slave": slave
         })
 
     def __create_temp_client(self) -> DMAioModbusTempClientInterface:
```

### Comparing `dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_clients.py` & `dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_clients.py`

 * *Files identical despite different names*

### Comparing `dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_simulator_client.py` & `dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_simulator_client.py`

 * *Files identical despite different names*

### Comparing `dm-aiomodbus-0.1.5/dm_aiomodbus/aiomodbus_temp_client.py` & `dm_aiomodbus-0.1.6/dm_aiomodbus/aiomodbus_temp_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
 
 class DMAioModbusTempClientInterface:
     @staticmethod
-    async def read_coils(address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def read_coils(address: int, count: int = 1, slave: int = 1) -> (list, str):
         raise NotImplementedError
 
     @staticmethod
-    async def read_discrete_inputs(address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def read_discrete_inputs(address: int, count: int = 1, slave: int = 1) -> (list, str):
         raise NotImplementedError
 
     @staticmethod
-    async def read_holding_registers(address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def read_holding_registers(address: int, count: int = 1, slave: int = 1) -> (list, str):
         raise NotImplementedError
 
     @staticmethod
-    async def read_input_registers(address: int, count: int = 1, slave: int = 1) -> list | None:
+    async def read_input_registers(address: int, count: int = 1, slave: int = 1) -> (list, str):
         raise NotImplementedError
 
     @staticmethod
-    async def write_coil(address: int, value: int, slave: int = 1) -> bool:
+    async def write_coil(address: int, value: int, slave: int = 1) -> (bool, str):
         raise NotImplementedError
 
     @staticmethod
-    async def write_register(address: int, value: int, slave: int = 1) -> bool:
+    async def write_register(address: int, value: int, slave: int = 1) -> (bool, str):
         raise NotImplementedError
 
     @staticmethod
-    async def write_coils(address: int, values: list[int] | int, slave: int = 1) -> bool:
+    async def write_coils(address: int, values: list[int] | int, slave: int = 1) -> (bool, str):
         raise NotImplementedError
 
     @staticmethod
-    async def write_registers(address: int, values: list[int] | int, slave: int = 1) -> bool:
+    async def write_registers(address: int, values: list[int] | int, slave: int = 1) -> (bool, str):
         raise NotImplementedError
```

### Comparing `dm-aiomodbus-0.1.5/dm_aiomodbus.egg-info/PKG-INFO` & `dm_aiomodbus-0.1.6/dm_aiomodbus.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomodbus
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is my custom aiomodbus client
 Home-page: https://pypi.org/project/dm-aiomodbus
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomodbus
 Keywords: dm aiomodbus
 Classifier: Programming Language :: Python :: 3.8
@@ -19,26 +19,14 @@
 # DM-aiomodbus
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomodbus)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomodbus)
 
-### Run in Windows
-
-_If you run async code in **Windows**, set correct selector_
-
-```python
-import asyncio
-import sys
-
-if sys.platform == "win32":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-```
-
 ## Usage
 
 ### Connection
 
 * Serial
    ```python
    from dm_aiomodbus import DMAioModbusSerialClient
@@ -69,29 +57,29 @@
 from dm_aiomodbus import DMAioModbusTcpClient, DMAioModbusTempClientInterface
 import asyncio
 
 
 async def main():
     # create client
     modbus_client = DMAioModbusTcpClient(
-       host="192.168.0.0",
-       port=501,
-       name_tag="my_tcp_plc"
+        host="192.168.0.0",
+        port=501,
+        name_tag="my_tcp_plc"
     )
 
     # create read callback
     async def read_callback(client: DMAioModbusTempClientInterface):
-        reg_258_259 = await client.read_holding_registers(258, count=2)
-        reg_256 = await client.read_holding_registers(256)
-        reg_260_2 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
+        reg_258_259, err1 = await client.read_holding_registers(258, count=2)  # get values and error if any
+        reg_256, err2 = await client.read_holding_registers(256)
+        reg_260_2, err3 = await client.read_holding_registers(address=260, slave=2)  # read second slave-device
         print(reg_258_259, reg_256, reg_260_2)
 
     # create read callback
     async def write_callback(client: DMAioModbusTempClientInterface):
-        await client.write_register(256, 1)
+        status, err = await client.write_register(256, 1)  # get write status and error if any
         await client.write_register(260, value=0, slave=2)  # write second slave-device
 
     # request to plc
     modbus_client.execute(read_callback)  # execute without waiting result
     # or
     await modbus_client.execute_and_return(write_callback, timeout=3)  # execute and wait result with timeout 3s (default 5)
 
@@ -129,7 +117,19 @@
     def error(self, message):
         print(message)
 
 
 # set up custom logger for all clients
 DMAioModbusTcpClient.set_logger(MyLogger())
 ```
+
+### Run in Windows
+
+_If you run async code in **Windows**, set correct selector_
+
+```python
+import asyncio
+import sys
+
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+```
```

### Comparing `dm-aiomodbus-0.1.5/setup.py` & `dm_aiomodbus-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomodbus',
-    version='v0.1.5',
+    version='v0.1.6',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomodbus client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomodbus',
     packages=find_packages(),
```

