# Comparing `tmp/bluetti_mqtt_asyncio-0.16.1.tar.gz` & `tmp/bluetti_mqtt_asyncio-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetti_mqtt_asyncio-0.16.1.tar", last modified: Mon Apr 15 16:18:00 2024, max compression
+gzip compressed data, was "bluetti_mqtt_asyncio-0.16.2.tar", last modified: Mon Apr 15 16:50:28 2024, max compression
```

## Comparing `bluetti_mqtt_asyncio-0.16.1.tar` & `bluetti_mqtt_asyncio-0.16.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.431787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.431787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac180.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac200m.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac300.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac500.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac60.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/bluetti_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/eb3a.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500p.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep600.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/device_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/discovery_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/logger_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24223 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/server_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.231513 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.231513 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac180.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac200m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac500.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac60.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/bluetti_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/eb3a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep500.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep500p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep600.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/discovery_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/logger_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24223 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/server_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 16:50:28.000000 bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 16:50:28.235514 bluetti_mqtt_asyncio-0.16.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 16:50:16.000000 bluetti_mqtt_asyncio-0.16.2/setup.py
```

### Comparing `bluetti_mqtt_asyncio-0.16.1/LICENSE` & `bluetti_mqtt_asyncio-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/PKG-INFO` & `bluetti_mqtt_asyncio-0.16.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti_mqtt_asyncio
-Version: 0.16.1
+Version: 0.16.2
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/DmytroPotapov/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt_asyncio-0.16.1/README.rst` & `bluetti_mqtt_asyncio-0.16.2/README.rst`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/__init__.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/client.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/client.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/manager.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bluetooth/manager.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bus.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/bus.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/commands.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/commands.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac180.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep600.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 from typing import List
 from ..commands import ReadHoldingRegisters
 from .bluetti_device import BluettiDevice
 from .struct import DeviceStruct
 
 
-class AC180(BluettiDevice):
+class EP600(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
-        # Core
-        # self.struct.add_swap_string_field('device_type', 110, 6)
-        # self.struct.add_sn_field('serial_number', 116)
-        self.struct.add_swap_string_field("device_type", 1101, 6)
-        self.struct.add_sn_field("serial_number", 1107)
-
-        # Battery Data
-        self.struct.add_swap_string_field("battery_type", 6101, 6)
-        self.struct.add_sn_field("battery_serial_number", 6107)
-        self.struct.add_version_field("bcu_version", 6175)
-        self.struct.add_uint_field("total_battery_percent", 102)
-
-        # Power IO
-        self.struct.add_uint_field(
-            "output_mode", 123
-        )  # 32 when both loads off, 40 when AC is on, 48 when DC is on, 56 when both on
-        self.struct.add_uint_field("dc_output_power", 140)
-        self.struct.add_uint_field("ac_output_power", 142)
-        self.struct.add_uint_field("dc_input_power", 144)
-        self.struct.add_uint_field(
-            "ac_input_power", 146
-        )  # this is a guess because I didn't have a PV module handy to test
-
-        # History
-        # self.struct.add_decimal_field('power_generation', 154, 1)  # Total power generated since last reset (kwh)
-        self.struct.add_decimal_field(
-            "power_generation", 1202, 1
-        )  # Total power generated since last reset (kwh)
-
-        # this is usefule for investigating the available data
-        # registers = {0:21,100:67,700:6,720:49,1100:51,1200:90,1300:31,1400:48,1
-        # 500:30,2000:67,2200:29,3000:27,6000:31,6100:100,6300:52,7000:5}
-        # for k in registers:
-        #     for v in range(registers[k]):
-        #         self.struct.add_uint_field('testI' + str(v+k), v+k)
-        # Controls
-        self.struct.add_bool_field('ac_output_on', 3007)
-        self.struct.add_bool_field('dc_output_on', 3008)
-        self.struct.add_bool_field('power_off', 3060)
-        self.struct.add_bool_field('eco_on', 3063)
-        super().__init__(address, "AC180P", sn)
+        self.struct.add_uint_field('total_battery_percent', 102)
+        self.struct.add_swap_string_field('device_type', 110, 6)
+        self.struct.add_sn_field('serial_number', 116)
+        self.struct.add_decimal_field('power_generation', 154, 1)  # Total power generated since last reset (kwh)
+        self.struct.add_swap_string_field('device_type', 1101, 6)
+        self.struct.add_sn_field('serial_number', 1107)
+        self.struct.add_decimal_field('power_generation', 1202, 1)  # Total power generated since last reset (kwh)
+        # 2001-2003 is the current device time & date without a timezone
+        self.struct.add_uint_field('battery_range_start', 2022)
+        self.struct.add_uint_field('battery_range_end', 2023)
+        self.struct.add_uint_field('max_ac_input_power', 2213)
+        self.struct.add_uint_field('max_ac_input_current', 2214)
+        self.struct.add_uint_field('max_ac_output_power', 2215)
+        self.struct.add_uint_field('max_ac_output_current', 2216)
+        self.struct.add_swap_string_field('battery_type', 6101, 6)
+        self.struct.add_sn_field('battery_serial_number', 6107)
+        self.struct.add_version_field('bcu_version', 6175)
+        self.struct.add_version_field('bmu_version', 6178)
+        self.struct.add_version_field('safety_module_version', 6181)
+        self.struct.add_version_field('high_voltage_module_version', 6184)
+
+        super().__init__(address, 'EP600', sn)
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(100, 62),
+            ReadHoldingRegisters(2022, 2),
         ]
 
     @property
     def logging_commands(self) -> List[ReadHoldingRegisters]:
         return [
-            ReadHoldingRegisters(0, 21),
-            ReadHoldingRegisters(100, 67),
-            ReadHoldingRegisters(700, 6),
-            ReadHoldingRegisters(720, 49),
+            ReadHoldingRegisters(100, 62),
             ReadHoldingRegisters(1100, 51),
             ReadHoldingRegisters(1200, 90),
             ReadHoldingRegisters(1300, 31),
             ReadHoldingRegisters(1400, 48),
             ReadHoldingRegisters(1500, 30),
-            ReadHoldingRegisters(2000, 67),
-            ReadHoldingRegisters(2200, 29),
-            ReadHoldingRegisters(3000, 27),
-            ReadHoldingRegisters(6000, 31),
+            ReadHoldingRegisters(2000, 89),
+            ReadHoldingRegisters(2200, 41),
+            ReadHoldingRegisters(2300, 36),
+            ReadHoldingRegisters(6000, 32),
             ReadHoldingRegisters(6100, 100),
-            ReadHoldingRegisters(6300, 52),
-            ReadHoldingRegisters(7000, 5),
+            ReadHoldingRegisters(6300, 100),
         ]
```

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac200m.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac200m.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac300.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac300.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac500.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac500.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac60.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac60.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/bluetti_device.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/bluetti_device.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/eb3a.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/eb3a.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep500.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500p.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ep500p.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep600.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/ac180.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,96 @@
+from enum import Enum, unique
 from typing import List
 from ..commands import ReadHoldingRegisters
 from .bluetti_device import BluettiDevice
 from .struct import DeviceStruct
 
 
-class EP600(BluettiDevice):
+@unique
+class OutputMode(Enum):
+    STOP = 0
+    INVERTER_OUTPUT = 1
+    BYPASS_OUTPUT_C = 2
+    BYPASS_OUTPUT_D = 3
+    LOAD_MATCHING = 4
+
+
+class AC180(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
-        self.struct.add_uint_field('total_battery_percent', 102)
-        self.struct.add_swap_string_field('device_type', 110, 6)
-        self.struct.add_sn_field('serial_number', 116)
-        self.struct.add_decimal_field('power_generation', 154, 1)  # Total power generated since last reset (kwh)
-        self.struct.add_swap_string_field('device_type', 1101, 6)
-        self.struct.add_sn_field('serial_number', 1107)
-        self.struct.add_decimal_field('power_generation', 1202, 1)  # Total power generated since last reset (kwh)
-        # 2001-2003 is the current device time & date without a timezone
-        self.struct.add_uint_field('battery_range_start', 2022)
-        self.struct.add_uint_field('battery_range_end', 2023)
-        self.struct.add_uint_field('max_ac_input_power', 2213)
-        self.struct.add_uint_field('max_ac_input_current', 2214)
-        self.struct.add_uint_field('max_ac_output_power', 2215)
-        self.struct.add_uint_field('max_ac_output_current', 2216)
-        self.struct.add_swap_string_field('battery_type', 6101, 6)
-        self.struct.add_sn_field('battery_serial_number', 6107)
-        self.struct.add_version_field('bcu_version', 6175)
-        self.struct.add_version_field('bmu_version', 6178)
-        self.struct.add_version_field('safety_module_version', 6181)
-        self.struct.add_version_field('high_voltage_module_version', 6184)
+        # Core
+        # self.struct.add_swap_string_field('device_type', 110, 6)
+        # self.struct.add_sn_field('serial_number', 116)
+        self.struct.add_swap_string_field("device_type", 1101, 6)
+        self.struct.add_sn_field("serial_number", 1107)
+
+        # Battery Data
+        self.struct.add_swap_string_field("battery_type", 6101, 6)
+        self.struct.add_sn_field("battery_serial_number", 6107)
+        self.struct.add_version_field("bcu_version", 6175)
+        self.struct.add_uint_field("total_battery_percent", 102)
+
+        # Power IO
+        self.struct.add_uint_field(
+            "output_mode", 123
+        )  # 32 when both loads off, 40 when AC is on, 48 when DC is on, 56 when both on
+        self.struct.add_uint_field("dc_output_power", 140)
+        self.struct.add_uint_field("ac_output_power", 142)
+        self.struct.add_uint_field("dc_input_power", 144)
+        self.struct.add_uint_field("ac_input_power", 146)
+        # History
+        # self.struct.add_decimal_field('power_generation', 154, 1)  # Total power generated since last reset (kwh)
+        self.struct.add_decimal_field(
+            "power_generation", 1202, 1
+        )  # Total power generated since last reset (kwh)
+
+        # this is usefule for investigating the available data
+        # registers = {0:21,100:67,700:6,720:49,1100:51,1200:90,1300:31,1400:48,1
+        # 500:30,2000:67,2200:29,3000:27,6000:31,6100:100,6300:52,7000:5}
+        # for k in registers:
+        #     for v in range(registers[k]):
+        #         self.struct.add_uint_field('testI' + str(v+k), v+k)
+        # Controls TEST
+        self.struct.add_bool_field("ac_output_on", 3007)
+        self.struct.add_bool_field("dc_output_on", 3008)
+        self.struct.add_bool_field("power_off", 3060)
+        self.struct.add_bool_field("eco_on", 3063)
+        self.struct.add_enum_field("ac_output_mode", 70, OutputMode)
+        self.struct.add_uint_field("internal_ac_voltage", 71)
+        self.struct.add_decimal_field("internal_current_one", 72, 1)
+        self.struct.add_uint_field("internal_power_one", 73)
+        self.struct.add_decimal_field("internal_ac_frequency", 74, 1)
+        self.struct.add_uint_field("internal_dc_input_voltage", 86)
+        self.struct.add_decimal_field("internal_dc_input_power", 87, 1)
+        self.struct.add_decimal_field("internal_dc_input_current", 88, 2)
+        self.struct.add_bool_field("ac_output_on", 48)
+        self.struct.add_bool_field("dc_output_on", 49)
 
-        super().__init__(address, 'EP600', sn)
+        super().__init__(address, "AC180P", sn)
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(100, 62),
-            ReadHoldingRegisters(2022, 2),
         ]
 
     @property
     def logging_commands(self) -> List[ReadHoldingRegisters]:
         return [
-            ReadHoldingRegisters(100, 62),
+            ReadHoldingRegisters(0, 21),
+            ReadHoldingRegisters(100, 67),
+            ReadHoldingRegisters(700, 6),
+            ReadHoldingRegisters(720, 49),
             ReadHoldingRegisters(1100, 51),
             ReadHoldingRegisters(1200, 90),
             ReadHoldingRegisters(1300, 31),
             ReadHoldingRegisters(1400, 48),
             ReadHoldingRegisters(1500, 30),
-            ReadHoldingRegisters(2000, 89),
-            ReadHoldingRegisters(2200, 41),
-            ReadHoldingRegisters(2300, 36),
-            ReadHoldingRegisters(6000, 32),
+            ReadHoldingRegisters(2000, 67),
+            ReadHoldingRegisters(2200, 29),
+            ReadHoldingRegisters(3000, 27),
+            ReadHoldingRegisters(6000, 31),
             ReadHoldingRegisters(6100, 100),
-            ReadHoldingRegisters(6300, 100),
+            ReadHoldingRegisters(6300, 52),
+            ReadHoldingRegisters(7000, 5),
         ]
```

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/struct.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/core/devices/struct.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/device_handler.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/device_handler.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/discovery_cli.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/discovery_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/logger_cli.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/logger_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/mqtt_client.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/server_cli.py` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt/server_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/PKG-INFO` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti_mqtt_asyncio
-Version: 0.16.1
+Version: 0.16.2
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/DmytroPotapov/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/SOURCES.txt` & `bluetti_mqtt_asyncio-0.16.2/bluetti_mqtt_asyncio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.1/setup.cfg` & `bluetti_mqtt_asyncio-0.16.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bluetti_mqtt_asyncio
-version = 0.16.1
+version = 0.16.2
 url = http://github.com/DmytroPotapov/bluetti_mqtt
 author = Stephen Augenstein
 author_email = perl.programmer@gmail.com
 description = MQTT interface to Bluetti power stations
 long_description = file: README.rst
 license = MIT
 classifiers =
```

