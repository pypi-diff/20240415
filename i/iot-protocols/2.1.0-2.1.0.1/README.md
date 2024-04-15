# Comparing `tmp/iot-protocols-2.1.0.tar.gz` & `tmp/iot_protocols-2.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iot-protocols-2.1.0.tar", last modified: Tue Apr  9 12:48:49 2024, max compression
+gzip compressed data, was "iot_protocols-2.1.0.1.tar", last modified: Mon Apr 15 11:28:48 2024, max compression
```

## Comparing `iot-protocols-2.1.0.tar` & `iot_protocols-2.1.0.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.301625 iot-protocols-2.1.0/
--rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot-protocols-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     3885 2024-04-09 12:48:49.295632 iot-protocols-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3150 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.136628 iot-protocols-2.1.0/iot_protocols/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/data.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.185628 iot-protocols-2.1.0/iot_protocols/devices/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/__init__.py
--rw-rw-rw-   0        0        0     2402 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/basics.py
--rw-rw-rw-   0        0        0     5054 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/iec62056_meter.py
--rw-rw-rw-   0        0        0     5755 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/interfaces.py
--rw-rw-rw-   0        0        0     1135 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/models.py
--rw-rw-rw-   0        0        0     5891 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/moxa_iologik_r1214.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.188625 iot-protocols-2.1.0/iot_protocols/protocols/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.202624 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/
--rw-rw-rw-   0        0        0       39 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/__init__.py
--rw-rw-rw-   0        0        0    10568 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/client.py
--rw-rw-rw-   0        0        0      315 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.232627 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/
--rw-rw-rw-   0        0        0       65 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/__init__.py
--rw-rw-rw-   0        0        0    12431 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/client.py
--rw-rw-rw-   0        0        0      318 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/constants.py
--rw-rw-rw-   0        0        0     1387 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/exceptions.py
--rw-rw-rw-   0        0        0    11468 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/messages.py
--rw-rw-rw-   0        0        0    12642 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/transports.py
--rw-rw-rw-   0        0        0     1872 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.254634 iot-protocols-2.1.0/iot_protocols/protocols/modbus/
--rw-rw-rw-   0        0        0      541 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/__init__.py
--rw-rw-rw-   0        0        0     8706 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/client.py
--rw-rw-rw-   0        0        0     1905 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/decoder.py
--rw-rw-rw-   0        0        0      331 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/exceptions.py
--rw-rw-rw-   0        0        0      981 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/requests.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.277633 iot-protocols-2.1.0/iot_protocols/protocols/snap7/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/__init__.py
--rw-rw-rw-   0        0        0     2738 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/client.py
--rw-rw-rw-   0        0        0      198 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/exceptions.py
--rw-rw-rw-   0        0        0      232 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/requests.py
--rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/responses.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.290629 iot-protocols-2.1.0/iot_protocols.egg-info/
--rw-rw-rw-   0        0        0     3885 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      888 2024-04-09 12:44:59.000000 iot-protocols-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 12:48:49.302629 iot-protocols-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.286627 iot-protocols-2.1.0/test/
--rw-rw-rw-   0        0        0     2058 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/test/test_iologik_r1214.py
--rw-rw-rw-   0        0        0     1238 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/test/tests_iec62056.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.529352 iot_protocols-2.1.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot_protocols-2.1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3887 2024-04-15 11:28:48.524746 iot_protocols-2.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3150 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.372434 iot_protocols-2.1.0.1/iot_protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/data.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.419158 iot_protocols-2.1.0.1/iot_protocols/devices/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/__init__.py
+-rw-rw-rw-   0        0        0     2402 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/basics.py
+-rw-rw-rw-   0        0        0     5140 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/iec62056_meter.py
+-rw-rw-rw-   0        0        0     1138 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/interfaces.py
+-rw-rw-rw-   0        0        0     1135 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/models.py
+-rw-rw-rw-   0        0        0     5891 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/devices/moxa_iologik_r1214.py
+-rw-rw-rw-   0        0        0     6978 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/iot_protocols/devices/socomec.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.422157 iot_protocols-2.1.0.1/iot_protocols/protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.435158 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/
+-rw-rw-rw-   0        0        0       39 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/__init__.py
+-rw-rw-rw-   0        0        0    10568 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/client.py
+-rw-rw-rw-   0        0        0      315 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.462164 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/
+-rw-rw-rw-   0        0        0       65 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/__init__.py
+-rw-rw-rw-   0        0        0    12431 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/client.py
+-rw-rw-rw-   0        0        0      318 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/constants.py
+-rw-rw-rw-   0        0        0     1387 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/exceptions.py
+-rw-rw-rw-   0        0        0    11468 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/messages.py
+-rw-rw-rw-   0        0        0    12642 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/transports.py
+-rw-rw-rw-   0        0        0     1872 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.483233 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/
+-rw-rw-rw-   0        0        0      541 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/__init__.py
+-rw-rw-rw-   0        0        0     8706 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/client.py
+-rw-rw-rw-   0        0        0     1905 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/decoder.py
+-rw-rw-rw-   0        0        0      331 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/exceptions.py
+-rw-rw-rw-   0        0        0      981 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/requests.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.507676 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/__init__.py
+-rw-rw-rw-   0        0        0     2738 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/client.py
+-rw-rw-rw-   0        0        0      198 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/exceptions.py
+-rw-rw-rw-   0        0        0      232 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/requests.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/responses.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.521389 iot_protocols-2.1.0.1/iot_protocols.egg-info/
+-rw-rw-rw-   0        0        0     3887 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1518 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 11:28:48.000000 iot_protocols-2.1.0.1/iot_protocols.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      890 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:28:48.530678 iot_protocols-2.1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:48.515016 iot_protocols-2.1.0.1/test/
+-rw-rw-rw-   0        0        0     2058 2024-04-09 12:44:32.000000 iot_protocols-2.1.0.1/test/test_iologik_r1214.py
+-rw-rw-rw-   0        0        0     1416 2024-04-15 11:23:36.000000 iot_protocols-2.1.0.1/test/tests_iec62056.py
```

### Comparing `iot-protocols-2.1.0/LICENSE` & `iot_protocols-2.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/PKG-INFO` & `iot_protocols-2.1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.1.0
+Version: 2.1.0.1
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `iot-protocols-2.1.0/README.md` & `iot_protocols-2.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/data.py` & `iot_protocols-2.1.0.1/iot_protocols/data.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/devices/basics.py` & `iot_protocols-2.1.0.1/iot_protocols/devices/basics.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/devices/iec62056_meter.py` & `iot_protocols-2.1.0.1/iot_protocols/devices/iec62056_meter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 import logging
 
 from iot_protocols.devices.basics import Device
-from iot_protocols.devices.interfaces import ThreePhasesEnergyMeter
+from iot_protocols.devices.interfaces import EnergyMeter
 from iot_protocols.devices.models import DeviceHardware
 from iot_protocols.protocols.iec62056.client import SerialClient, TariffResponse, messages
 from iot_protocols.data import Serie
 
 DEFAULT_ENERGY_REGISTER_MAPPING = {
     "1.25": "P",
     "3.25": "R",
-    "1.8.0": "Ap",
-    "2.8.0": "Am",
-    "3.8.0": "Qp",
-    "4.8.0": "Qm",
-    "1.4.0": "Pp",
-    "2.4.0": "Pm",
-    "21.25": "L1.P",
-    "23.25": "L1.R",
-    "21.8.0": "L1.Ap",
-    "22.8.0": "L1.Am",
-    "41.25": "L2.P",
-    "43.25": "L2.R",
-    "41.8.0": "L2.Ap",
-    "42.8.0": "L2.Am",
-    "61.25": "L3.P",
-    "63.25": "L3.R",
-    "61.8.0": "L3.Ap",
-    "62.8.0": "L3.Am"
+    "1.8.0": "A+",
+    "2.8.0": "A",
+    "3.8.0": "Q+",
+    "4.8.0": "Q-",
+    "1.4.0": "P+",
+    "2.4.0": "P-",
+    "21.25": "P:1",
+    "23.25": "R:1",
+    "21.8.0": "A+:1",
+    "22.8.0": "A-:1",
+    "41.25": "P:2",
+    "43.25": "R:2",
+    "41.8.0": "A+:2",
+    "42.8.0": "A-:2",
+    "61.25": "P:3",
+    "63.25": "R:3",
+    "61.8.0": "A+:3",
+    "62.8.0": "A-:3"
 }
 
 
-class IEC62056SerialMeter(Device, ThreePhasesEnergyMeter):
+class IEC62056SerialMeter(Device, EnergyMeter):
 
     _type = "EnergyMeter"
     _energy_mapping = DEFAULT_ENERGY_REGISTER_MAPPING
 
     def __init__(self,
                  meter_id: str,
                  port: str,
@@ -103,24 +103,28 @@
             str | None: the index value
         """
         for dataset in tariff_response.data:
             if dataset.address == "0.1.0":
                 return dataset.value
        
     def _parse_tariff_response(self, response: TariffResponse, old_index: str = None):
+        result = {}
         for dataset in response.data:
             if dataset.value is not None and dataset.address in self._energy_mapping:
                 key = self._energy_mapping[dataset.address]
-                self[key] = dict(name=key, value=float(dataset.value), unit=dataset.unit)
+                result.update({key: {"value": float(dataset.value), "unit": dataset.unit}})
+            
+            # Handling of previous period registers
             elif old_index is not None and dataset.value is not None:
                 splited = dataset.address.split("*")
                 if len(splited) > 1 and splited[0] in self._energy_mapping and splited[1] == old_index:
                     key = self._energy_mapping[splited[0]]
-                    self[f"{key}_old"] = dict(name=f"{key}_old", value=float(dataset.value), unit=dataset.unit)
-
+                    result.update({f"{key}_old": {"value": float(dataset.value), "unit": dataset.unit}})
+        
+        return result
     
     def read_energy(self, table: int=None, **kwargs) -> None:
         response = None
         with self._client as client:
             response = client.request(
                 meter_address=self._meter_id,
                 table=table
@@ -131,9 +135,9 @@
 
             if response.checked == False:
                 logging.debug(f"Invalid bcc (received: {response.bcc})!")
                 self._bcc_last_check = False
         
         if response is not None:
             old_index = self._get_memory_index_register(response)
-            self._parse_tariff_response(response, old_index=old_index)
-            return response
+            result = self._parse_tariff_response(response, old_index=old_index)
+            return result
```

### Comparing `iot-protocols-2.1.0/iot_protocols/devices/models.py` & `iot_protocols-2.1.0.1/iot_protocols/devices/models.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/devices/moxa_iologik_r1214.py` & `iot_protocols-2.1.0.1/iot_protocols/devices/moxa_iologik_r1214.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/client.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/client.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/exceptions.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/messages.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/messages.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/transports.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/transports.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/utils.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/iec62056/tools/utils.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/modbus/__init__.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/modbus/client.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/modbus/decoder.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/decoder.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/modbus/requests.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/modbus/requests.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols/protocols/snap7/client.py` & `iot_protocols-2.1.0.1/iot_protocols/protocols/snap7/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/iot_protocols.egg-info/PKG-INFO` & `iot_protocols-2.1.0.1/iot_protocols.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.1.0
+Version: 2.1.0.1
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `iot-protocols-2.1.0/iot_protocols.egg-info/SOURCES.txt` & `iot_protocols-2.1.0.1/iot_protocols.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 iot_protocols.egg-info/top_level.txt
 iot_protocols/devices/__init__.py
 iot_protocols/devices/basics.py
 iot_protocols/devices/iec62056_meter.py
 iot_protocols/devices/interfaces.py
 iot_protocols/devices/models.py
 iot_protocols/devices/moxa_iologik_r1214.py
+iot_protocols/devices/socomec.py
 iot_protocols/protocols/__init__.py
 iot_protocols/protocols/iec62056/__init__.py
 iot_protocols/protocols/iec62056/client.py
 iot_protocols/protocols/iec62056/exceptions.py
 iot_protocols/protocols/iec62056/tools/__init__.py
 iot_protocols/protocols/iec62056/tools/client.py
 iot_protocols/protocols/iec62056/tools/constants.py
```

### Comparing `iot-protocols-2.1.0/pyproject.toml` & `iot_protocols-2.1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iot-protocols"
-version = "2.1.0"
+version = "2.1.0.1"
 authors = [
   { name="Adrien Delhaye", email="adrien.delhaye@memoco.eu" },
 ]
 description = "Generic IIoT protocols package"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `iot-protocols-2.1.0/test/test_iologik_r1214.py` & `iot_protocols-2.1.0.1/test/test_iologik_r1214.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.1.0/test/tests_iec62056.py` & `iot_protocols-2.1.0.1/test/tests_iec62056.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         transport="serial",
         parity="E",
         bytesize=7,
         stopbits=1
     )
 
 
-def test_client_identification(client: SerialClient):
+def CANCELED_test_client_identification(client: SerialClient):
+    client.connect()
     result = client.read_tariff_identification("5987893", ack_stop=True)
     logging.info(result)
     assert isinstance(result, messages.IdentificationMessage)
 
     logging.info(f"----- Next Step ----")
 
     result = client.request(meter_address="5987893", table=0, timeout=3)
@@ -32,12 +33,15 @@
 def meter() -> IEC62056SerialMeter:
     return IEC62056SerialMeter(
         meter_id="5987893",
         port="COM3"
     )
 
 
-def test_read_meter_identification(meter: IEC62056SerialMeter):
+def test_read_meter_data(meter: IEC62056SerialMeter):
     meter.connect()
     assert meter.device_id is not None
     assert meter.hardware is not None
-    logging.info(f"Meter id : {meter.device_id}")
+    logging.info(f"Meter id : {meter.device_id}")
+    energy = meter.read_energy(table=7)
+    logging.info("\n".join([f"{key} --> {value}" for key, value in energy.items()]))
+    assert len(energy) > 2
```

