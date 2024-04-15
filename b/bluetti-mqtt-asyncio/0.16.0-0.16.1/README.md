# Comparing `tmp/bluetti_mqtt_asyncio-0.16.0.tar.gz` & `tmp/bluetti_mqtt_asyncio-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetti_mqtt_asyncio-0.16.0.tar", last modified: Mon Apr 15 13:07:03 2024, max compression
+gzip compressed data, was "bluetti_mqtt_asyncio-0.16.1.tar", last modified: Mon Apr 15 16:18:00 2024, max compression
```

## Comparing `bluetti_mqtt_asyncio-0.16.0.tar` & `bluetti_mqtt_asyncio-0.16.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.466207 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.466207 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac180.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac200m.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac300.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac500.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac60.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/bluetti_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/eb3a.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep500.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep500p.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep600.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/device_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/discovery_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/logger_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24223 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/server_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 13:07:03.000000 bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 13:07:03.470207 bluetti_mqtt_asyncio-0.16.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 13:06:54.000000 bluetti_mqtt_asyncio-0.16.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.431787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.431787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac180.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac200m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac500.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac60.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/bluetti_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/eb3a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep600.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/discovery_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/logger_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24223 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/server_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 16:18:00.000000 bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 16:18:00.435787 bluetti_mqtt_asyncio-0.16.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 16:17:55.000000 bluetti_mqtt_asyncio-0.16.1/setup.py
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/LICENSE` & `bluetti_mqtt_asyncio-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/PKG-INFO` & `bluetti_mqtt_asyncio-0.16.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti_mqtt_asyncio
-Version: 0.16.0
+Version: 0.16.1
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/DmytroPotapov/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/README.rst` & `bluetti_mqtt_asyncio-0.16.1/README.rst`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/__init__.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/client.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/client.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bluetooth/manager.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bluetooth/manager.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/bus.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/bus.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/commands.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/commands.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac180.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac180.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,19 @@
 
         # this is usefule for investigating the available data
         # registers = {0:21,100:67,700:6,720:49,1100:51,1200:90,1300:31,1400:48,1
         # 500:30,2000:67,2200:29,3000:27,6000:31,6100:100,6300:52,7000:5}
         # for k in registers:
         #     for v in range(registers[k]):
         #         self.struct.add_uint_field('testI' + str(v+k), v+k)
-
+        # Controls
+        self.struct.add_bool_field('ac_output_on', 3007)
+        self.struct.add_bool_field('dc_output_on', 3008)
+        self.struct.add_bool_field('power_off', 3060)
+        self.struct.add_bool_field('eco_on', 3063)
         super().__init__(address, "AC180P", sn)
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(100, 62),
         ]
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac200m.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac200m.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac300.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac300.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac500.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class AutoSleepMode(Enum):
     THIRTY_SECONDS = 2
     ONE_MINUTE = 3
     FIVE_MINUTES = 4
     NEVER = 5
 
 
-class AC500(BluettiDevice):
+class EP500(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
         # Core
         self.struct.add_string_field('device_type', 10, 6)
         self.struct.add_sn_field('serial_number', 17)
         self.struct.add_version_field('arm_version', 23)
@@ -64,22 +64,22 @@
         self.struct.add_uint_field('internal_power_two', 76)
         self.struct.add_decimal_field('ac_input_voltage', 77, 1)
         self.struct.add_decimal_field('internal_current_three', 78, 1)
         self.struct.add_uint_field('internal_power_three', 79)
         self.struct.add_decimal_field('ac_input_frequency', 80, 2)
         self.struct.add_decimal_field('internal_dc_input_voltage', 86, 1)
         self.struct.add_uint_field('internal_dc_input_power', 87)
-        self.struct.add_decimal_field('internal_dc_input_current', 88, 1)
+        self.struct.add_decimal_field('internal_dc_input_current', 88, 1, (0, 15))
 
         # Battery Data
         self.struct.add_uint_field('pack_num_max', 91)
         self.struct.add_decimal_field('total_battery_voltage', 92, 1)
+        self.struct.add_decimal_field('pack_voltage', 92, 1)  # Full pack voltage
+        self.struct.add_uint_field('pack_battery_percent', 94)
         self.struct.add_uint_field('pack_num', 96)
-        self.struct.add_decimal_field('pack_voltage', 98, 2)  # Full pack voltage
-        self.struct.add_uint_field('pack_battery_percent', 99)
         self.struct.add_decimal_array_field('cell_voltages', 105, 16, 2)
 
         # Controls
         self.struct.add_enum_field('ups_mode', 3001, UpsMode)
         self.struct.add_bool_field('split_phase_on', 3004)
         self.struct.add_enum_field('split_phase_machine_mode', 3005, MachineAddress)
         self.struct.add_uint_field('pack_num', 3006)
@@ -90,19 +90,15 @@
         self.struct.add_uint_field('battery_range_start', 3015)
         self.struct.add_uint_field('battery_range_end', 3016)
         # 3031-3033 is the current device time & date without a timezone
         self.struct.add_bool_field('bluetooth_connected', 3036)
         # 3039-3056 is the time control programming
         self.struct.add_enum_field('auto_sleep_mode', 3061, AutoSleepMode)
 
-        super().__init__(address, 'AC500', sn)
-
-    @property
-    def pack_num_max(self):
-        return 6
+        super().__init__(address, 'EP500', sn)
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(10, 40),
             ReadHoldingRegisters(70, 21),
             ReadHoldingRegisters(3001, 61),
@@ -113,15 +109,15 @@
         return [ReadHoldingRegisters(91, 37)]
 
     @property
     def logging_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(0, 70),
             ReadHoldingRegisters(70, 21),
-            ReadHoldingRegisters(3000, 62),
+            ReadHoldingRegisters(3001, 61),
         ]
 
     @property
     def pack_logging_commands(self) -> List[ReadHoldingRegisters]:
         return [ReadHoldingRegisters(91, 119)]
 
     @property
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ac60.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac60.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/bluetti_device.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/bluetti_device.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/eb3a.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/eb3a.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep500.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep500p.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class AutoSleepMode(Enum):
     THIRTY_SECONDS = 2
     ONE_MINUTE = 3
     FIVE_MINUTES = 4
     NEVER = 5
 
 
-class EP500(BluettiDevice):
+class EP500P(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
         # Core
         self.struct.add_string_field('device_type', 10, 6)
         self.struct.add_sn_field('serial_number', 17)
         self.struct.add_version_field('arm_version', 23)
@@ -90,15 +90,15 @@
         self.struct.add_uint_field('battery_range_start', 3015)
         self.struct.add_uint_field('battery_range_end', 3016)
         # 3031-3033 is the current device time & date without a timezone
         self.struct.add_bool_field('bluetooth_connected', 3036)
         # 3039-3056 is the time control programming
         self.struct.add_enum_field('auto_sleep_mode', 3061, AutoSleepMode)
 
-        super().__init__(address, 'EP500', sn)
+        super().__init__(address, 'EP500P', sn)
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(10, 40),
             ReadHoldingRegisters(70, 21),
             ReadHoldingRegisters(3001, 61),
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep500p.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ac500.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,73 +32,79 @@
 class AutoSleepMode(Enum):
     THIRTY_SECONDS = 2
     ONE_MINUTE = 3
     FIVE_MINUTES = 4
     NEVER = 5
 
 
-class EP500P(BluettiDevice):
+class AC500(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
         # Core
-        self.struct.add_string_field('device_type', 10, 6)
-        self.struct.add_sn_field('serial_number', 17)
-        self.struct.add_version_field('arm_version', 23)
-        self.struct.add_version_field('dsp_version', 25)
-        self.struct.add_uint_field('dc_input_power', 36)
-        self.struct.add_uint_field('ac_input_power', 37)
-        self.struct.add_uint_field('ac_output_power', 38)
-        self.struct.add_uint_field('dc_output_power', 39)
-        self.struct.add_decimal_field('power_generation', 41, 1)  # Total power generated since last reset (kwh)
-        self.struct.add_uint_field('total_battery_percent', 43)
-        self.struct.add_bool_field('ac_output_on', 48)
-        self.struct.add_bool_field('dc_output_on', 49)
+        self.struct.add_string_field("device_type", 10, 6)
+        self.struct.add_sn_field("serial_number", 17)
+        self.struct.add_version_field("arm_version", 23)
+        self.struct.add_version_field("dsp_version", 25)
+        self.struct.add_uint_field("dc_input_power", 36)
+        self.struct.add_uint_field("ac_input_power", 37)
+        self.struct.add_uint_field("ac_output_power", 38)
+        self.struct.add_uint_field("dc_output_power", 39)
+        self.struct.add_decimal_field(
+            "power_generation", 41, 1
+        )  # Total power generated since last reset (kwh)
+        self.struct.add_uint_field("total_battery_percent", 43)
+        self.struct.add_bool_field("ac_output_on", 48)
+        self.struct.add_bool_field("dc_output_on", 49)
 
         # Details
-        self.struct.add_enum_field('ac_output_mode', 70, OutputMode)
-        self.struct.add_decimal_field('internal_ac_voltage', 71, 1)
-        self.struct.add_decimal_field('internal_current_one', 72, 1)
-        self.struct.add_uint_field('internal_power_one', 73)
-        self.struct.add_decimal_field('internal_ac_frequency', 74, 2)
-        self.struct.add_decimal_field('internal_current_two', 75, 1)
-        self.struct.add_uint_field('internal_power_two', 76)
-        self.struct.add_decimal_field('ac_input_voltage', 77, 1)
-        self.struct.add_decimal_field('internal_current_three', 78, 1)
-        self.struct.add_uint_field('internal_power_three', 79)
-        self.struct.add_decimal_field('ac_input_frequency', 80, 2)
-        self.struct.add_decimal_field('internal_dc_input_voltage', 86, 1)
-        self.struct.add_uint_field('internal_dc_input_power', 87)
-        self.struct.add_decimal_field('internal_dc_input_current', 88, 1, (0, 15))
+        self.struct.add_enum_field("ac_output_mode", 70, OutputMode)
+        self.struct.add_decimal_field("internal_ac_voltage", 71, 1)
+        self.struct.add_decimal_field("internal_current_one", 72, 1)
+        self.struct.add_uint_field("internal_power_one", 73)
+        self.struct.add_decimal_field("internal_ac_frequency", 74, 2)
+        self.struct.add_decimal_field("internal_current_two", 75, 1)
+        self.struct.add_uint_field("internal_power_two", 76)
+        self.struct.add_decimal_field("ac_input_voltage", 77, 1)
+        self.struct.add_decimal_field("internal_current_three", 78, 1)
+        self.struct.add_uint_field("internal_power_three", 79)
+        self.struct.add_decimal_field("ac_input_frequency", 80, 2)
+        self.struct.add_decimal_field("internal_dc_input_voltage", 86, 1)
+        self.struct.add_uint_field("internal_dc_input_power", 87)
+        self.struct.add_decimal_field("internal_dc_input_current", 88, 1)
 
         # Battery Data
-        self.struct.add_uint_field('pack_num_max', 91)
-        self.struct.add_decimal_field('total_battery_voltage', 92, 1)
-        self.struct.add_decimal_field('pack_voltage', 92, 1)  # Full pack voltage
-        self.struct.add_uint_field('pack_battery_percent', 94)
-        self.struct.add_uint_field('pack_num', 96)
-        self.struct.add_decimal_array_field('cell_voltages', 105, 16, 2)
+        self.struct.add_uint_field("pack_num_max", 91)
+        self.struct.add_decimal_field("total_battery_voltage", 92, 1)
+        self.struct.add_uint_field("pack_num", 96)
+        self.struct.add_decimal_field("pack_voltage", 98, 2)  # Full pack voltage
+        self.struct.add_uint_field("pack_battery_percent", 99)
+        self.struct.add_decimal_array_field("cell_voltages", 105, 16, 2)
 
         # Controls
-        self.struct.add_enum_field('ups_mode', 3001, UpsMode)
-        self.struct.add_bool_field('split_phase_on', 3004)
-        self.struct.add_enum_field('split_phase_machine_mode', 3005, MachineAddress)
-        self.struct.add_uint_field('pack_num', 3006)
-        self.struct.add_bool_field('ac_output_on', 3007)
-        self.struct.add_bool_field('dc_output_on', 3008)
-        self.struct.add_bool_field('grid_charge_on', 3011)
-        self.struct.add_bool_field('time_control_on', 3013)
-        self.struct.add_uint_field('battery_range_start', 3015)
-        self.struct.add_uint_field('battery_range_end', 3016)
+        self.struct.add_enum_field("ups_mode", 3001, UpsMode)
+        self.struct.add_bool_field("split_phase_on", 3004)
+        self.struct.add_enum_field("split_phase_machine_mode", 3005, MachineAddress)
+        self.struct.add_uint_field("pack_num", 3006)
+        self.struct.add_bool_field("ac_output_on", 3007)
+        self.struct.add_bool_field("dc_output_on", 3008)
+        self.struct.add_bool_field("grid_charge_on", 3011)
+        self.struct.add_bool_field("time_control_on", 3013)
+        self.struct.add_uint_field("battery_range_start", 3015)
+        self.struct.add_uint_field("battery_range_end", 3016)
         # 3031-3033 is the current device time & date without a timezone
-        self.struct.add_bool_field('bluetooth_connected', 3036)
+        self.struct.add_bool_field("bluetooth_connected", 3036)
         # 3039-3056 is the time control programming
-        self.struct.add_enum_field('auto_sleep_mode', 3061, AutoSleepMode)
+        self.struct.add_enum_field("auto_sleep_mode", 3061, AutoSleepMode)
 
-        super().__init__(address, 'EP500P', sn)
+        super().__init__(address, "AC500", sn)
+
+    @property
+    def pack_num_max(self):
+        return 6
 
     @property
     def polling_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(10, 40),
             ReadHoldingRegisters(70, 21),
             ReadHoldingRegisters(3001, 61),
@@ -109,15 +115,15 @@
         return [ReadHoldingRegisters(91, 37)]
 
     @property
     def logging_commands(self) -> List[ReadHoldingRegisters]:
         return [
             ReadHoldingRegisters(0, 70),
             ReadHoldingRegisters(70, 21),
-            ReadHoldingRegisters(3001, 61),
+            ReadHoldingRegisters(3000, 62),
         ]
 
     @property
     def pack_logging_commands(self) -> List[ReadHoldingRegisters]:
         return [ReadHoldingRegisters(91, 119)]
 
     @property
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/ep600.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/ep600.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/core/devices/struct.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/core/devices/struct.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/device_handler.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/device_handler.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/discovery_cli.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/discovery_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/logger_cli.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/logger_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/mqtt_client.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt/server_cli.py` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt/server_cli.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/PKG-INFO` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti_mqtt_asyncio
-Version: 0.16.0
+Version: 0.16.1
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/DmytroPotapov/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt_asyncio-0.16.0/bluetti_mqtt_asyncio.egg-info/SOURCES.txt` & `bluetti_mqtt_asyncio-0.16.1/bluetti_mqtt_asyncio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt_asyncio-0.16.0/setup.cfg` & `bluetti_mqtt_asyncio-0.16.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bluetti_mqtt_asyncio
-version = 0.16.0
+version = 0.16.1
 url = http://github.com/DmytroPotapov/bluetti_mqtt
 author = Stephen Augenstein
 author_email = perl.programmer@gmail.com
 description = MQTT interface to Bluetti power stations
 long_description = file: README.rst
 license = MIT
 classifiers =
```

