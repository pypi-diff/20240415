# Comparing `tmp/touch_sdk-0.6.7.tar.gz` & `tmp/touch_sdk-0.7.0.tar.gz`

## Comparing `touch_sdk-0.6.7.tar` & `touch_sdk-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.gitlab-ci.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.pylintrc
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/version.sh
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/basic.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/basic_threaded.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/custom_data.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/magnetometer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/osc.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/plotter.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/pressure.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/raycasting.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/sensors.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/basic.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/pressure.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/gatt_scanner.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/uuids.py
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/watch.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/watch_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/vec_pb2.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_input_pb2.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_output_pb2.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.gitignore
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/LICENSE
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/.pylintrc
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/basic.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/basic_threaded.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/custom_data.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/magnetometer.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/mouse.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/osc.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/osc_client_server.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/pinch_probability.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/plotter.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/pressure.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/raycasting.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/examples/sensors.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/gatt_scanner.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/stream_watch.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/uuids.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/watch.py
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/watch_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/protobuf/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/protobuf/common_pb2.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/protobuf/watch_input_pb2.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/src/touch_sdk/protobuf/watch_output_pb2.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/.gitignore
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 touch_sdk-0.7.0/PKG-INFO
```

### Comparing `touch_sdk-0.6.7/examples/basic.py` & `touch_sdk-0.7.0/examples/basic_threaded.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from threading import Thread
 from touch_sdk import Watch
+import logging
+# Get helpful log info
+logging.basicConfig(level=logging.INFO)
 
 class MyWatch(Watch):
 
     # def on_sensors(self, sensors):
     #     print(sensors)
 
     def on_tap(self):
@@ -24,10 +27,10 @@
     def on_back_button(self):
         self.trigger_haptics(1.0, 20)
         print('back button')
 
 watch = MyWatch()
 thread = Thread(target=watch.start)
 thread.start()
-input("Press enter to exit")
+input("Press enter to exit\n")
 watch.stop()
-thread.join()
+thread.join()
```

### Comparing `touch_sdk-0.6.7/examples/basic_threaded.py` & `touch_sdk-0.7.0/examples/basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from threading import Thread
 from touch_sdk import Watch
+import logging
+# Get helpful log info
+logging.basicConfig(level=logging.INFO)
 
 class MyWatch(Watch):
 
     # def on_sensors(self, sensors):
     #     print(sensors)
 
     def on_tap(self):
@@ -22,12 +24,8 @@
         print('rotary', direction)
 
     def on_back_button(self):
         self.trigger_haptics(1.0, 20)
         print('back button')
 
 watch = MyWatch()
-thread = Thread(target=watch.start)
-thread.start()
-input("Press enter to exit\n")
-watch.stop()
-thread.join()
+watch.start()
```

### Comparing `touch_sdk-0.6.7/examples/magnetometer.py` & `touch_sdk-0.7.0/examples/magnetometer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from touch_sdk import Watch
+import logging
+# Get helpful log info
+logging.basicConfig(level=logging.INFO)
 
 class MyWatch(Watch):
 
     def on_sensors(self, sensors):
         print(sensors.magnetic_field, sensors.magnetic_field_calibration)
 
     def on_tap(self):
```

### Comparing `touch_sdk-0.6.7/examples/plotter.py` & `touch_sdk-0.7.0/examples/plotter.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 import numpy as np
 
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 
 from touch_sdk import Watch
+import logging
+# Get helpful log info
+logging.basicConfig(level=logging.INFO)
 
 
 class MyWatch(Watch):
     def __init__(self, name=""):
         super().__init__(name)
         self.sensor_queue = Queue()
```

### Comparing `touch_sdk-0.6.7/examples/sensors.py` & `touch_sdk-0.7.0/examples/sensors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from touch_sdk import Watch
+import logging
+# Get helpful log info
+logging.basicConfig(level=logging.INFO)
 
 class MyWatch(Watch):
     def on_sensors(self, sensors):
         def format_tuple(data):
             return ' '.join(format(field, '.3f') for field in data)
 
         print(format_tuple(sensors.acceleration), end='\t')
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/gatt_scanner.py` & `touch_sdk-0.7.0/src/touch_sdk/gatt_scanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from bleak import BleakScanner
+import logging
+logger = logging.getLogger(__file__)
 
 __doc__ = """Scans for Bluetooth devices with a given GATT service UUID."""
 
 class GattScanner:
     """Scans for Bluetooth devices with service_uuid.
 
     on_scan_result gets called every time the scanner finds a new device.
@@ -36,15 +38,15 @@
 
     async def start_scanning(self):
         """Start scanning. This function should not be called before GattScanner.run
         has been called."""
         if not self._scanning:
             self._addresses.clear()  # Reset found addresses list
         self._scanning = True
-        print("Scanning...")
+        logger.info("Scanning...")
 
     def forget_address(self, address):
         """Forget address, i.e., act as if the device with that address had
         never been discovered."""
         self._addresses.discard(address)
 
     async def _detection_callback(self, device, advertisement_data):
@@ -63,9 +65,9 @@
         )
 
         if self.service_uuid in advertisement_data.service_uuids:
             if self.name_filter is not None:
                 if self.name_filter.lower() not in name.lower():
                     return
 
-            print(f"Found {name}")
+            logger.info(f"Found {name}")
             await self.on_scan_result(device, name)
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/utils.py` & `touch_sdk-0.7.0/src/touch_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.7/src/touch_sdk/watch.py` & `touch_sdk-0.7.0/src/touch_sdk/watch.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import asyncio_atexit
 
 from touch_sdk.uuids import PROTOBUF_OUTPUT, PROTOBUF_INPUT
 from touch_sdk.utils import unpack_chained
 from touch_sdk.watch_connector import WatchConnector
 
 # pylint: disable=no-name-in-module
+from touch_sdk.protobuf.common_pb2 import GestureType
 from touch_sdk.protobuf.watch_output_pb2 import Update, Gesture, TouchEvent
 from touch_sdk.protobuf.watch_input_pb2 import InputUpdate, HapticEvent
 
 
 __doc__ = """Discovering Touch SDK compatible BLE devices and interfacing with them."""
 
 
@@ -70,15 +71,71 @@
 
         self._event_loop = None
 
         self.custom_data = None
         if hasattr(self.__class__, "custom_data"):
             self.custom_data = self.__class__.custom_data
 
-        self.hand = Hand.NONE
+        self._hand = Hand.NONE
+        self._battery_percentage = -1
+
+        self._screen_resolution = None
+        self._haptics_available = False
+
+        self._app_version = ""
+        self._app_id = ""
+        self._device_name = ""
+        self._manufacturer = ""
+        self._model_info = ""
+
+    @property
+    def hand(self) -> Hand:
+        """Which hand the device is worn on."""
+        return self._hand
+
+    @property
+    def battery_percentage(self) -> int:
+        """Last known battery percentage of the device."""
+        return self._battery_percentage
+
+    @property
+    def touch_screen_resolution(self) -> Optional[Tuple[int, int]]:
+        """Resolution of the touch screen (width, height) in pixels.
+        None if not fetched, or no touch screen is available."""
+        return self._screen_resolution
+
+    @property
+    def haptics_available(self) -> bool:
+        """Whether the device supports haptic feedback."""
+        return self._haptics_available
+
+    @property
+    def app_version(self) -> str:
+        """Version of the software running on the device."""
+        return self._app_version
+
+    @property
+    def app_id(self) -> str:
+        """Identifier of the software running on the device."""
+        return self._app_id
+
+    @property
+    def device_name(self) -> str:
+        """Type name of the device."""
+        return self._device_name
+
+    @property
+    def manufacturer(self) -> str:
+        """Manufacturer of the device."""
+        return self._manufacturer
+
+    @property
+    def model_info(self) -> str:
+        """Miscellaneous info about the gesture detection model."""
+        return self._model_info
 
     def start(self):
         """Blocking event loop that starts the Bluetooth scanner
 
         More handy than Watch.run when only this event loop is needed."""
         try:
             asyncio.run(self.run())
@@ -110,15 +167,15 @@
         await self._subscribe_to_custom_characteristics(client)
 
     async def _fetch_info(self, client):
         data = await client.read_gatt_char(PROTOBUF_OUTPUT)
         update = Update()
         update.ParseFromString(bytes(data))
         if update.HasField("info"):
-            self.hand = Hand(update.info.hand)
+            self._proto_on_info(update.info)
 
     # Custom characteristics
 
     async def _subscribe_to_custom_characteristics(self, client):
         if self.custom_data is None:
             return
 
@@ -139,14 +196,21 @@
 
     def on_custom_data(self, uuid: str, content: Tuple):
         """Receive data from custom characteristics"""
 
     # Main protobuf characteristic
 
     async def _on_protobuf(self, message):
+
+        for entry in message.probabilities:
+            if entry.label == GestureType.PINCH_HOLD or entry.label == GestureType.PINCH_TAP:
+                self.on_gesture_probability(entry.probability)
+            elif entry.label == GestureType.NONE:
+                self.on_gesture_probability(1 - entry.probability)
+
         self._proto_on_sensors(message.sensorFrames, message.unixTime)
         self._proto_on_gestures(message.gestures)
         self._proto_on_touch_events(message.touchEvents)
         self._proto_on_button_events(message.buttonEvents)
         self._proto_on_rotary_events(message.rotaryEvents)
 
         if message.HasField("info"):
@@ -188,15 +252,15 @@
             return [x / length for x in vector]
 
         grav = normalize(sensor_frame.gravity)
 
         av_x = -sensor_frame.angular_velocity[2]  # right = +
         av_y = -sensor_frame.angular_velocity[1]  # down = +
 
-        handedness_scale = -1 if self.hand == Hand.LEFT else 1
+        handedness_scale = -1 if self._hand == Hand.LEFT else 1
 
         delta_x = av_x * grav[2] + av_y * grav[1]
         delta_y = handedness_scale * (av_y * grav[2] - av_x * grav[1])
 
         self.on_arm_direction_change(delta_x, delta_y)
 
     def on_arm_direction_change(self, delta_x: float, delta_y: float):
@@ -204,19 +268,22 @@
 
     def on_pressure(self, pressure: float):
         """Called when new pressure value (in hectopascals) is received."""
 
     # Gestures
 
     def _proto_on_gestures(self, gestures):
-        if any(g.type == Gesture.GestureType.TAP for g in gestures):
+        if any(g.type == GestureType.PINCH_TAP for g in gestures):
             self.on_tap()
 
+    def on_gesture_probability(self, prob: float):
+        """Called when gesture probability is received."""
+
     def on_tap(self):
-        """Called when the tap gesture happens."""
+        """Called when a pinch tap gesture happens."""
 
     # Touch screen
 
     def _proto_on_touch_events(self, touch_events):
         for touch in touch_events:
             coords = _protovec2_to_tuple(touch.coords[0])
             if touch.eventType == TouchEvent.TouchEventType.BEGIN:
@@ -261,15 +328,36 @@
         """Rotary dial around the watch screen is turned.
 
         direction: +1 for clockwise, -1 for counterclockwise."""
 
     # Info
 
     def _proto_on_info(self, info):
-        self.hand = Hand(info.hand)
+        self._hand = Hand(info.hand)
+
+        if battery_percentage := info.batteryPercentage:
+            self._battery_percentage = battery_percentage
+
+        if (screen_resolution := info.touchScreenResolution) is not None:
+            self._screen_resolution = (screen_resolution.x, screen_resolution.y)
+
+        if haptics_available := info.hapticsAvailable:
+            self._haptics_available = haptics_available
+
+        if app_version := info.appVersion:
+            self._app_version = app_version
+
+        if app_id := info.appId:
+            self._app_id = app_id
+
+        if device_name := info.deviceName:
+            self._device_name = device_name
+
+        if manufacturer := info.manufacturer:
+            self._manufacturer = manufacturer
 
     # Haptics
 
     def trigger_haptics(self, intensity: float, duration_ms: int):
         """Trigger vibration haptics on the watch.
 
         intensity: between 0 and 1
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/watch_connector.py` & `touch_sdk-0.7.0/src/touch_sdk/watch_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import asyncio
 import sys
 import platform
+import logging
 
 import bleak
 from bleak import BleakClient
 
 from touch_sdk.utils import partial_async
 from touch_sdk.uuids import PROTOBUF_OUTPUT, PROTOBUF_INPUT, INTERACTION_SERVICE
 from touch_sdk.gatt_scanner import GattScanner
 
 # pylint: disable=no-name-in-module
 from touch_sdk.protobuf.watch_output_pb2 import Update
 from touch_sdk.protobuf.watch_input_pb2 import InputUpdate, ClientInfo
 
+logger = logging.getLogger(__file__)
+
 
 __doc__ = """Discovering Touch SDK compatible BLE devices and interfacing with them."""
 
 
 class WatchConnector:
     """Manages connections to watches.
 
@@ -32,15 +35,16 @@
     Discovering the Bluetooth devices is delegated to a GattScanner instance.
     """
 
     def __init__(self, on_approved_connection, on_message, name_filter=None):
         """Creates a new instance of WatchConnector. Does not start scanning for Bluetooth
         devices. Use WatchConnector.run to enter the scanning and connection event loop.
 
-        Optional name_filter connects only to watches with that name (case insensitive)"""
+        Optional name_filter connects only to watches with that name (case insensitive)
+        """
         self._scanner = GattScanner(
             self._on_scan_result, INTERACTION_SERVICE, name_filter
         )
         self._approved_addresses = set()
         self._informed_addresses = (
             set()
         )  # Bluetooth addresses to which client info has successfully been sent
@@ -106,15 +110,15 @@
             # [org.bluez.Error.NotConnected] Not Connected
             #
             # Sometimes (~50%) Bleak thinks the client is connected even though
             # BlueZ thinks it's not. We could try to reconnect, but that messes
             # up with _monitor_connections. Easier to just give up and try again
             # through the scanner, even though it adds a delay and a bit of
             # noise to the console.
-            print("Connecting failed, trying again")
+            logger.info("Connecting failed, trying again")
             await self._disconnect(address)
 
     async def _disconnect(self, address, resume=True):
         if (client := self._clients.pop(address, None)) is not None:
             await client.disconnect()
 
         self._approved_addresses.discard(address)
@@ -141,15 +145,15 @@
 
     async def _handle_approved_connection(self, device, name):
         if device.address in self._approved_addresses:
             return
         self._approved_addresses.add(device.address)
 
         if (client := self._clients.get(device.address)) is not None:
-            print(f"Connection approved by {name}")
+            logger.info(f"Connection approved by {name}")
             await self._scanner.stop_scanning()
 
             disconnect_tasks = [
                 self._disconnect(address)
                 for address in self._clients
                 if address != device.address
             ]
@@ -159,30 +163,32 @@
             try:
                 await self._on_approved_connection(client)
             except bleak.exc.BleakDBusError as _:
                 # Catches "Unlikely GATT error"
                 await self._disconnect(device.address)
 
     async def _handle_disconnect_signal(self, device, name):
-        print(f"Connection declined from {name}")
+        logger.warning(f"Connection declined from {name}")
         await self._disconnect(device.address)
 
     async def _send_client_info(self, client):
         if client.address in self._informed_addresses:
             return
 
         client_info = ClientInfo()
         client_info.appName = sys.argv[0]
         client_info.deviceName = platform.node()
         client_info.os = platform.system()
         input_update = InputUpdate()
         input_update.clientInfo.CopyFrom(client_info)
 
         try:
-            await client.write_gatt_char(PROTOBUF_INPUT, input_update.SerializeToString(), True)
+            await client.write_gatt_char(
+                PROTOBUF_INPUT, input_update.SerializeToString(), True
+            )
         except bleak.exc.BleakDBusError:
             # [org.bluez.Error.Failed] Operation failed with ATT error:
             # 0x01 (Invalid Handle)
             #
             # This happens if the client is not already approved by the
             # watch before this connection (= connection dialog shows up).
             # However, the client info seems to still end up to the watch,
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/protobuf/vec_pb2.py` & `touch_sdk-0.7.0/src/touch_sdk/protobuf/common_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: vec.proto
+# source: common.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tvec.proto\"\x1c\n\x04Vec2\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"\'\n\x04Vec3\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"2\n\x04Quat\x12\t\n\x01w\x18\x01 \x01(\x02\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\x12\t\n\x01z\x18\x04 \x01(\x02\x42\r\xaa\x02\nPsix.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\"\x1c\n\x04Vec2\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"\'\n\x04Vec3\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"2\n\x04Quat\x12\t\n\x01w\x18\x01 \x01(\x02\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\x12\t\n\x01z\x18\x04 \x01(\x02\"\'\n\x05Model\x12\x1e\n\x08gestures\x18\x01 \x03(\x0e\x32\x0c.GestureType*S\n\x0bGestureType\x12\x08\n\x04NONE\x10\x00\x12\r\n\tPINCH_TAP\x10\x01\x12\n\n\x06\x43LENCH\x10\x02\x12\x0f\n\x0bSURFACE_TAP\x10\x03\x12\x0e\n\nPINCH_HOLD\x10\x04\x42\r\xaa\x02\nPsix.Protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vec_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\nPsix.Proto'
-  _VEC2._serialized_start=13
-  _VEC2._serialized_end=41
-  _VEC3._serialized_start=43
-  _VEC3._serialized_end=82
-  _QUAT._serialized_start=84
-  _QUAT._serialized_end=134
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\252\002\nPsix.Proto'
+  _globals['_GESTURETYPE']._serialized_start=180
+  _globals['_GESTURETYPE']._serialized_end=263
+  _globals['_VEC2']._serialized_start=16
+  _globals['_VEC2']._serialized_end=44
+  _globals['_VEC3']._serialized_start=46
+  _globals['_VEC3']._serialized_end=85
+  _globals['_QUAT']._serialized_start=87
+  _globals['_QUAT']._serialized_end=137
+  _globals['_MODEL']._serialized_start=139
+  _globals['_MODEL']._serialized_end=178
 # @@protoc_insertion_point(module_scope)
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_input_pb2.py` & `touch_sdk-0.7.0/src/touch_sdk/protobuf/watch_input_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: watch_input.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import touch_sdk.protobuf.common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11watch_input.proto\"~\n\x0bHapticEvent\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.HapticEvent.HapticType\x12\x11\n\tintensity\x18\x02 \x01(\x02\x12\x0e\n\x06length\x18\x03 \x01(\x05\"%\n\nHapticType\x12\n\n\x06\x43\x41NCEL\x10\x00\x12\x0b\n\x07ONESHOT\x10\x01\"L\n\nClientInfo\x12\x0f\n\x07\x61ppName\x18\x01 \x01(\t\x12\x12\n\ndeviceName\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\n\n\x02os\x18\x04 \x01(\t\"Q\n\x0bInputUpdate\x12!\n\x0bhapticEvent\x18\x01 \x01(\x0b\x32\x0c.HapticEvent\x12\x1f\n\nclientInfo\x18\x02 \x01(\x0b\x32\x0b.ClientInfoB\r\xaa\x02\nPsix.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11watch_input.proto\x1a\x0c\x63ommon.proto\"~\n\x0bHapticEvent\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.HapticEvent.HapticType\x12\x11\n\tintensity\x18\x02 \x01(\x02\x12\x0e\n\x06length\x18\x03 \x01(\x05\"%\n\nHapticType\x12\n\n\x06\x43\x41NCEL\x10\x00\x12\x0b\n\x07ONESHOT\x10\x01\"L\n\nClientInfo\x12\x0f\n\x07\x61ppName\x18\x01 \x01(\t\x12\x12\n\ndeviceName\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\n\n\x02os\x18\x04 \x01(\t\"o\n\x0bInputUpdate\x12!\n\x0bhapticEvent\x18\x01 \x01(\x0b\x32\x0c.HapticEvent\x12\x1f\n\nclientInfo\x18\x02 \x01(\x0b\x32\x0b.ClientInfo\x12\x1c\n\x0cmodelRequest\x18\x03 \x01(\x0b\x32\x06.ModelB\r\xaa\x02\nPsix.Protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'watch_input_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'watch_input_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\nPsix.Proto'
-  _HAPTICEVENT._serialized_start=21
-  _HAPTICEVENT._serialized_end=147
-  _HAPTICEVENT_HAPTICTYPE._serialized_start=110
-  _HAPTICEVENT_HAPTICTYPE._serialized_end=147
-  _CLIENTINFO._serialized_start=149
-  _CLIENTINFO._serialized_end=225
-  _INPUTUPDATE._serialized_start=227
-  _INPUTUPDATE._serialized_end=308
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\252\002\nPsix.Proto'
+  _globals['_HAPTICEVENT']._serialized_start=35
+  _globals['_HAPTICEVENT']._serialized_end=161
+  _globals['_HAPTICEVENT_HAPTICTYPE']._serialized_start=124
+  _globals['_HAPTICEVENT_HAPTICTYPE']._serialized_end=161
+  _globals['_CLIENTINFO']._serialized_start=163
+  _globals['_CLIENTINFO']._serialized_end=239
+  _globals['_INPUTUPDATE']._serialized_start=241
+  _globals['_INPUTUPDATE']._serialized_end=352
 # @@protoc_insertion_point(module_scope)
```

### Comparing `touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_output_pb2.py` & `touch_sdk-0.7.0/src/touch_sdk/protobuf/watch_output_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: watch_output.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import touch_sdk.protobuf.vec_pb2 as vec__pb2
+import touch_sdk.protobuf.common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12watch_output.proto\x1a\tvec.proto\"j\n\x04Info\x12\x18\n\x04hand\x18\x01 \x01(\x0e\x32\n.Info.Hand\x12\r\n\x05\x61ppId\x18\x02 \x01(\t\x12\x12\n\nappVersion\x18\x03 \x01(\t\"%\n\x04Hand\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05RIGHT\x10\x01\x12\x08\n\x04LEFT\x10\x02\"\x9e\x01\n\x0bSensorFrame\x12\x13\n\x04gyro\x18\x01 \x01(\x0b\x32\x05.Vec3\x12\x12\n\x03\x61\x63\x63\x18\x02 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04grav\x18\x03 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04quat\x18\x04 \x01(\x0b\x32\x05.Quat\x12\x12\n\x03mag\x18\x06 \x01(\x0b\x32\x05.Vec3\x12\x15\n\x06magCal\x18\x07 \x01(\x0b\x32\x05.Vec3\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"n\n\x07Gesture\x12\"\n\x04type\x18\x01 \x01(\x0e\x32\x14.Gesture.GestureType\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0bGestureType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03TAP\x10\x01\x12\n\n\x06\x43LENCH\x10\x02\"\xd4\x01\n\nTouchEvent\x12-\n\teventType\x18\x01 \x01(\x0e\x32\x1a.TouchEvent.TouchEventType\x12\x13\n\x0b\x61\x63tionIndex\x18\x02 \x01(\x05\x12\x12\n\npointerIds\x18\x03 \x03(\x05\x12\x15\n\x06\x63oords\x18\x04 \x03(\x0b\x32\x05.Vec2\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"D\n\x0eTouchEventType\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x42\x45GIN\x10\x01\x12\x07\n\x03\x45ND\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04\".\n\x0bRotaryEvent\x12\x0c\n\x04step\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0b\x42uttonEvent\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\"\xf1\x02\n\x06Update\x12\"\n\x0csensorFrames\x18\x01 \x03(\x0b\x32\x0c.SensorFrame\x12\x1a\n\x08gestures\x18\x02 \x03(\x0b\x32\x08.Gesture\x12 \n\x0btouchEvents\x18\x03 \x03(\x0b\x32\x0b.TouchEvent\x12\"\n\x0c\x62uttonEvents\x18\x04 \x03(\x0b\x32\x0c.ButtonEvent\x12\"\n\x0crotaryEvents\x18\x05 \x03(\x0b\x32\x0c.RotaryEvent\x12\x1f\n\x07signals\x18\x06 \x03(\x0e\x32\x0e.Update.Signal\x12\x11\n\tdeltaTime\x18\x07 \x01(\x05\x12\x10\n\x08unixTime\x18\x08 \x01(\x03\x12\x13\n\x04info\x18\t \x01(\x0b\x32\x05.Info\x12\x10\n\x08pressure\x18\x10 \x01(\x02\"P\n\x06Signal\x12\x08\n\x04NONE\x10\x00\x12\x0e\n\nDISCONNECT\x10\x01\x12\x14\n\x10\x43ONNECT_APPROVED\x10\x02\x12\x16\n\x12\x44\x45SCRIPTION_UPDATE\x10\x03\x42\r\xaa\x02\nPsix.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12watch_output.proto\x1a\x0c\x63ommon.proto\"\xc0\x02\n\x04Info\x12\x18\n\x04hand\x18\x01 \x01(\x0e\x32\n.Info.Hand\x12\r\n\x05\x61ppId\x18\x02 \x01(\t\x12\x12\n\nappVersion\x18\x03 \x01(\t\x12\x1f\n\x0f\x61vailableModels\x18\x04 \x03(\x0b\x32\x06.Model\x12\x1b\n\x0b\x61\x63tiveModel\x18\x05 \x01(\x0b\x32\x06.Model\x12\x11\n\tmodelInfo\x18\x06 \x01(\t\x12\x14\n\x0cmanufacturer\x18\x07 \x01(\t\x12\x12\n\ndeviceName\x18\x08 \x01(\t\x12\x19\n\x11\x62\x61tteryPercentage\x18\t \x01(\x05\x12\x18\n\x10hapticsAvailable\x18\n \x01(\x08\x12$\n\x15touchScreenResolution\x18\x0b \x01(\x0b\x32\x05.Vec2\"%\n\x04Hand\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05RIGHT\x10\x01\x12\x08\n\x04LEFT\x10\x02\"\x9e\x01\n\x0bSensorFrame\x12\x13\n\x04gyro\x18\x01 \x01(\x0b\x32\x05.Vec3\x12\x12\n\x03\x61\x63\x63\x18\x02 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04grav\x18\x03 \x01(\x0b\x32\x05.Vec3\x12\x13\n\x04quat\x18\x04 \x01(\x0b\x32\x05.Quat\x12\x12\n\x03mag\x18\x06 \x01(\x0b\x32\x05.Vec3\x12\x15\n\x06magCal\x18\x07 \x01(\x0b\x32\x05.Vec3\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"8\n\x07Gesture\x12\x1a\n\x04type\x18\x01 \x01(\x0e\x32\x0c.GestureType\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\"\xd4\x01\n\nTouchEvent\x12-\n\teventType\x18\x01 \x01(\x0e\x32\x1a.TouchEvent.TouchEventType\x12\x13\n\x0b\x61\x63tionIndex\x18\x02 \x01(\x05\x12\x12\n\npointerIds\x18\x03 \x03(\x05\x12\x15\n\x06\x63oords\x18\x04 \x03(\x0b\x32\x05.Vec2\x12\x11\n\tdeltaTime\x18\x05 \x01(\x05\"D\n\x0eTouchEventType\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x42\x45GIN\x10\x01\x12\x07\n\x03\x45ND\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04\".\n\x0bRotaryEvent\x12\x0c\n\x04step\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\",\n\x0b\x42uttonEvent\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tdeltaTime\x18\x02 \x01(\x05\"D\n\x10ProbabilityEntry\x12\x1b\n\x05label\x18\x01 \x01(\x0e\x32\x0c.GestureType\x12\x13\n\x0bprobability\x18\x02 \x01(\x02\"\x9b\x03\n\x06Update\x12\"\n\x0csensorFrames\x18\x01 \x03(\x0b\x32\x0c.SensorFrame\x12\x1a\n\x08gestures\x18\x02 \x03(\x0b\x32\x08.Gesture\x12 \n\x0btouchEvents\x18\x03 \x03(\x0b\x32\x0b.TouchEvent\x12\"\n\x0c\x62uttonEvents\x18\x04 \x03(\x0b\x32\x0c.ButtonEvent\x12\"\n\x0crotaryEvents\x18\x05 \x03(\x0b\x32\x0c.RotaryEvent\x12\x1f\n\x07signals\x18\x06 \x03(\x0e\x32\x0e.Update.Signal\x12\x11\n\tdeltaTime\x18\x07 \x01(\x05\x12\x10\n\x08unixTime\x18\x08 \x01(\x03\x12\x13\n\x04info\x18\t \x01(\x0b\x32\x05.Info\x12(\n\rprobabilities\x18\n \x03(\x0b\x32\x11.ProbabilityEntry\x12\x10\n\x08pressure\x18\x10 \x01(\x02\"P\n\x06Signal\x12\x08\n\x04NONE\x10\x00\x12\x0e\n\nDISCONNECT\x10\x01\x12\x14\n\x10\x43ONNECT_APPROVED\x10\x02\x12\x16\n\x12\x44\x45SCRIPTION_UPDATE\x10\x03\x42\r\xaa\x02\nPsix.Protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'watch_output_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'watch_output_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\nPsix.Proto'
-  _INFO._serialized_start=33
-  _INFO._serialized_end=139
-  _INFO_HAND._serialized_start=102
-  _INFO_HAND._serialized_end=139
-  _SENSORFRAME._serialized_start=142
-  _SENSORFRAME._serialized_end=300
-  _GESTURE._serialized_start=302
-  _GESTURE._serialized_end=412
-  _GESTURE_GESTURETYPE._serialized_start=368
-  _GESTURE_GESTURETYPE._serialized_end=412
-  _TOUCHEVENT._serialized_start=415
-  _TOUCHEVENT._serialized_end=627
-  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_start=559
-  _TOUCHEVENT_TOUCHEVENTTYPE._serialized_end=627
-  _ROTARYEVENT._serialized_start=629
-  _ROTARYEVENT._serialized_end=675
-  _BUTTONEVENT._serialized_start=677
-  _BUTTONEVENT._serialized_end=721
-  _UPDATE._serialized_start=724
-  _UPDATE._serialized_end=1093
-  _UPDATE_SIGNAL._serialized_start=1013
-  _UPDATE_SIGNAL._serialized_end=1093
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\252\002\nPsix.Proto'
+  _globals['_INFO']._serialized_start=37
+  _globals['_INFO']._serialized_end=357
+  _globals['_INFO_HAND']._serialized_start=320
+  _globals['_INFO_HAND']._serialized_end=357
+  _globals['_SENSORFRAME']._serialized_start=360
+  _globals['_SENSORFRAME']._serialized_end=518
+  _globals['_GESTURE']._serialized_start=520
+  _globals['_GESTURE']._serialized_end=576
+  _globals['_TOUCHEVENT']._serialized_start=579
+  _globals['_TOUCHEVENT']._serialized_end=791
+  _globals['_TOUCHEVENT_TOUCHEVENTTYPE']._serialized_start=723
+  _globals['_TOUCHEVENT_TOUCHEVENTTYPE']._serialized_end=791
+  _globals['_ROTARYEVENT']._serialized_start=793
+  _globals['_ROTARYEVENT']._serialized_end=839
+  _globals['_BUTTONEVENT']._serialized_start=841
+  _globals['_BUTTONEVENT']._serialized_end=885
+  _globals['_PROBABILITYENTRY']._serialized_start=887
+  _globals['_PROBABILITYENTRY']._serialized_end=955
+  _globals['_UPDATE']._serialized_start=958
+  _globals['_UPDATE']._serialized_end=1369
+  _globals['_UPDATE_SIGNAL']._serialized_start=1289
+  _globals['_UPDATE_SIGNAL']._serialized_end=1369
 # @@protoc_insertion_point(module_scope)
```

### Comparing `touch_sdk-0.6.7/LICENSE` & `touch_sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.7/README.md` & `touch_sdk-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -79,19 +79,39 @@
 Outputs +1 for clockwise and -1 for counter-clockwise.
 
 ### Back button
 ```python
 def on_back_button(self):
     print('back button')
 ```
+
 Called when the back button is pressed and released. Wear OS does not support separate button down and button up events for the back button.
 
+### Probability output
+```python
+def on_gesture_probability(self, prob):
+    print(f'probability: {prob}')
+```
+Triggered when a gesture detection model produces an output. See `examples/pinch_probability.py` for a complete example.
+
 ### Haptics
 The `trigger_haptics(intensity, length)` method can be used to initiate one-shot haptic effects on the watch. For example, to drive the haptics motor for 300 ms at 100% intensity on `watch`, call `watch.trigger_haptics(1.0, 300)`.
 
+### Miscellaneous
+```python
+watch.hand # Hand.NONE, Hand.LEFT or Hand.RIGHT
+watch.battery_percentage # 0-100
+watch.touch_screen_resolution # (width, height) or None
+watch.haptics_available # True if device supports haptic feedback
+```
+
+## Acting as backend for Unity Play Mode
+
+This package provides the `stream_watch` module, which makes it possible to use touch-sdk-py as the backend for touch-sdk-unity (>=0.12.0) applications in Play Mode. To use this feature, create a virtual environment in which touch-sdk-py is installed, and then set the python path of the `BluetoothWatchProvider` script in your Unity project to the virtual environment's python executable.
+
 ## Unexplainable bugs
 Sometimes turning your device's Bluetooth off and on again fixes problems – this has been observed on Linux, Mac and Windows. This is unideal, but those error states are hard to reproduce and thus hard to fix.
 
 ## Pylint
 ```sh
 python3 -m pylint src --rcfile=.pylintrc
 ```
```

### Comparing `touch_sdk-0.6.7/pyproject.toml` & `touch_sdk-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "touch-sdk"
-version = "0.6.7"
+version = "0.7.0"
 description = "Doublepoint Touch SDK"
 license = "ISC"
 authors = [
     { name="Doublepoint", email="developer@doublepoint.com" },
 ]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["bluetooth"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: ISC License (ISCL)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `touch_sdk-0.6.7/PKG-INFO` & `touch_sdk-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: touch-sdk
-Version: 0.6.7
+Version: 0.7.0
 Summary: Doublepoint Touch SDK
 Project-URL: Homepage, https://github.com/doublepointlab/touch-sdk-py#readme
 Project-URL: Bug Tracker, https://github.com/doublepointlab/touch-sdk-py/issues
 Author-email: Doublepoint <developer@doublepoint.com>
 License-Expression: ISC
 License-File: LICENSE
 Keywords: bluetooth
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: Android
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: asyncio-atexit~=1.0.1
 Requires-Dist: bleak~=0.20.1
 Requires-Dist: protobuf~=3.20.0
 Description-Content-Type: text/markdown
 
 # Touch SDK py
 
@@ -104,19 +104,39 @@
 Outputs +1 for clockwise and -1 for counter-clockwise.
 
 ### Back button
 ```python
 def on_back_button(self):
     print('back button')
 ```
+
 Called when the back button is pressed and released. Wear OS does not support separate button down and button up events for the back button.
 
+### Probability output
+```python
+def on_gesture_probability(self, prob):
+    print(f'probability: {prob}')
+```
+Triggered when a gesture detection model produces an output. See `examples/pinch_probability.py` for a complete example.
+
 ### Haptics
 The `trigger_haptics(intensity, length)` method can be used to initiate one-shot haptic effects on the watch. For example, to drive the haptics motor for 300 ms at 100% intensity on `watch`, call `watch.trigger_haptics(1.0, 300)`.
 
+### Miscellaneous
+```python
+watch.hand # Hand.NONE, Hand.LEFT or Hand.RIGHT
+watch.battery_percentage # 0-100
+watch.touch_screen_resolution # (width, height) or None
+watch.haptics_available # True if device supports haptic feedback
+```
+
+## Acting as backend for Unity Play Mode
+
+This package provides the `stream_watch` module, which makes it possible to use touch-sdk-py as the backend for touch-sdk-unity (>=0.12.0) applications in Play Mode. To use this feature, create a virtual environment in which touch-sdk-py is installed, and then set the python path of the `BluetoothWatchProvider` script in your Unity project to the virtual environment's python executable.
+
 ## Unexplainable bugs
 Sometimes turning your device's Bluetooth off and on again fixes problems – this has been observed on Linux, Mac and Windows. This is unideal, but those error states are hard to reproduce and thus hard to fix.
 
 ## Pylint
 ```sh
 python3 -m pylint src --rcfile=.pylintrc
 ```
```

