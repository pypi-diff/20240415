# Comparing `tmp/ta-cmi-3.2.0.tar.gz` & `tmp/ta-cmi-3.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-3.2.0.tar", last modified: Mon Jan 15 17:55:26 2024, max compression
+gzip compressed data, was "ta-cmi-3.2.1.dev0.tar", last modified: Mon Apr 15 18:16:34 2024, max compression
```

## Comparing `ta-cmi-3.2.0.tar` & `ta-cmi-3.2.1.dev0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.981505 ta-cmi-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8133 2024-01-15 17:55:26.980505 ta-cmi-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6562 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 17:55:26.981505 ta-cmi-3.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.979505 ta-cmi-3.2.0/ta_cmi/
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/channel.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi_api.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe_api.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3567 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/const.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.980505 ta-cmi-3.2.0/ta_cmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8133 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-15 18:16:33.997783 ta-cmi-3.2.1.dev0/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1067 2023-04-18 18:49:16.000000 ta-cmi-3.2.1.dev0/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     8198 2024-04-15 18:16:33.992282 ta-cmi-3.2.1.dev0/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     6681 2024-01-15 17:46:52.000000 ta-cmi-3.2.1.dev0/README.md
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2024-04-15 18:16:33.998782 ta-cmi-3.2.1.dev0/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      656 2024-04-15 18:16:28.000000 ta-cmi-3.2.1.dev0/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-15 18:16:33.833781 ta-cmi-3.2.1.dev0/ta_cmi/
+-rwxrwxrwx   0 user      (1000) user      (1000)      423 2024-01-15 17:51:33.000000 ta-cmi-3.2.1.dev0/ta_cmi/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2918 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/ta_cmi/api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1228 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/ta_cmi/channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      638 2023-04-18 18:49:16.000000 ta-cmi-3.2.1.dev0/ta_cmi/cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2700 2023-07-28 19:34:46.000000 ta-cmi-3.2.1.dev0/ta_cmi/cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      543 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/ta_cmi/cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3559 2023-12-02 09:25:43.000000 ta-cmi-3.2.1.dev0/ta_cmi/coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4557 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/ta_cmi/coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      403 2023-04-21 23:42:39.000000 ta-cmi-3.2.1.dev0/ta_cmi/coe_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3806 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/ta_cmi/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4003 2024-04-14 18:36:50.000000 ta-cmi-3.2.1.dev0/ta_cmi/device.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-15 18:16:33.986282 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     8198 2024-04-15 18:16:33.000000 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      512 2024-04-15 18:16:33.000000 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-04-15 18:16:33.000000 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       31 2024-04-15 18:16:33.000000 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2024-04-15 18:16:33.000000 ta-cmi-3.2.1.dev0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-15 18:16:33.971781 ta-cmi-3.2.1.dev0/tests/
+-rwxrwxrwx   0 user      (1000) user      (1000)     3792 2023-07-28 19:34:46.000000 ta-cmi-3.2.1.dev0/tests/test_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      624 2023-04-18 18:49:17.000000 ta-cmi-3.2.1.dev0/tests/test_cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     5148 2023-07-28 19:34:46.000000 ta-cmi-3.2.1.dev0/tests/test_cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      967 2023-04-18 18:49:17.000000 ta-cmi-3.2.1.dev0/tests/test_cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     6522 2023-12-02 09:24:54.000000 ta-cmi-3.2.1.dev0/tests/test_coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4427 2024-03-28 14:09:07.000000 ta-cmi-3.2.1.dev0/tests/test_coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    10811 2024-04-14 18:36:50.000000 ta-cmi-3.2.1.dev0/tests/test_device.py
```

### Comparing `ta-cmi-3.2.0/LICENSE` & `ta-cmi-3.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ta-cmi-3.2.0/PKG-INFO` & `ta-cmi-3.2.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 3.2.0
-Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+Version: 3.2.1.dev0
+Summary: A Python wrapper to read out sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
         
@@ -24,14 +24,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.9.3
+Requires-Dist: packaging>=24.0
 
 # TA-CMI
 A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 
 ## How to use package
 
 ### Json API
```

### Comparing `ta-cmi-3.2.0/README.md` & `ta-cmi-3.2.1.dev0/ta_cmi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: ta-cmi
+Version: 3.2.1.dev0
+Summary: A Python wrapper to read out sensors from Technische Alternative using the C.M.I.
+Home-page: https://gitlab.com/DeerMaximum/ta-cmi
+Author: DeerMaximum
+Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
+License: MIT License
+        
+        Copyright (c) 2021 DeerMaximum
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.9.3
+Requires-Dist: packaging>=24.0
+
 # TA-CMI
 A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 
 ## How to use package
 
 ### Json API
 
@@ -113,8 +146,8 @@
     except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
         print(f"Error: {error}")
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 loop.close()
-```
+```
```

### Comparing `ta-cmi-3.2.0/ta_cmi/cmi.py` & `ta-cmi-3.2.1.dev0/ta_cmi/cmi.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-3.2.0/ta_cmi/coe.py` & `ta-cmi-3.2.1.dev0/ta_cmi/coe.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-3.2.0/ta_cmi/coe_api.py` & `ta-cmi-3.2.1.dev0/ta_cmi/coe_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from typing import Any, Dict
-
-from aiohttp import ClientSession
-
-from .api import API
-from .coe_channel import CoEChannel
-from .const import _LOGGER, ChannelMode
-
-
-class CoEAPI(API):
-    """Class to perform API requests to the CoE Addon."""
-
-    COE_VERSION = "/version"
-    COE_DATA = "/receive/{id}"
-    COE_SEND_ANALOG = "/send/analog"
-    COE_SEND_DIGITAL = "/send/digital"
-
-    DIGITAL_VALUES_PER_PAGE = 16
-    ANALOG_VALUES_PER_PAGE = 4
-
-    def __init__(self, host: str, session: ClientSession = None) -> None:
-        """Initialize."""
-        super().__init__(session)
-
-        self.host = host
-
-    async def get_coe_data(self, can_id: int) -> Dict[str, Any] | None:
-        """Get the CoE data."""
-        url = f"{self.host}{self.COE_DATA.replace('{id}', str(can_id))}"
-
-        _LOGGER.debug("Receive data from CoE server: %s", url)
-
-        data = await self._make_request_get(url)
-
-        _LOGGER.debug("Received data from CoE server: %s", data)
-
-        if len(data) == 0:
-            return None
-
-        return data
-
-    async def get_coe_version(self) -> str | None:
-        """Get the version of the CoE server."""
-        url = f"{self.host}{self.COE_VERSION}"
-
-        _LOGGER.debug("Receive current version from CoE server: %s", url)
-
-        data = await self._make_request_get(url)
-
-        _LOGGER.debug("Received version from CoE server: %s", data)
-
-        if len(data) == 0:
-            return None
-
-        return data.get("version", None)
-
-    @staticmethod
-    def _check_channel_type(
-        target_mode: ChannelMode, channel_to_check: list[CoEChannel]
-    ) -> bool:
-        """Check if the channel type equals the target."""
-        for channel in channel_to_check:
-            if channel.type != target_mode:
-                _LOGGER.warning(
-                    f"Channel has wrong type. Expected type: {target_mode}, actual type: {channel.type}"
-                )
-                return False
-
-        return True
-
-    @staticmethod
-    def _check_array_length(array: list, target_size: int) -> bool:
-        """Check if a list has the required length."""
-        if len(array) != target_size:
-            _LOGGER.warning(
-                f"List has wrong length. Expected length: {target_size}, actual length: {len(array)}"
-            )
-            return False
-
-        return True
-
-    @staticmethod
-    def _check_analog_page_size(provided: int) -> bool:
-        """Check if the page is in the right number range."""
-        if not (0 < provided < 9):
-            _LOGGER.warning(
-                f"Page is not in the expected range. Expected range: 0 < page < 9, actual value: {provided}"
-            )
-            return False
-
-        return True
-
-    @staticmethod
-    def _convert_analog_channel_to_dict(channel: CoEChannel) -> dict[str, Any]:
-        """Convert a analog coe channel to a dict."""
-        return {"value": channel.value, "unit": int(channel.unit)}
-
-    async def send_analog_values(self, channels: list[CoEChannel], page: int):
-        """Send analog values to the CoE server."""
-        _LOGGER.debug("Send analog values to CoE server")
-
-        if (
-            not self._check_channel_type(ChannelMode.ANALOG, channels)
-            or not self._check_array_length(channels, self.ANALOG_VALUES_PER_PAGE)
-            or not self._check_analog_page_size(page)
-        ):
-            _LOGGER.error("Could not send analog values. Please see logs for details.")
-            return
-
-        data = {
-            "values": [
-                self._convert_analog_channel_to_dict(channel) for channel in channels
-            ],
-            "page": page,
-        }
-
-        url = f"{self.host}{self.COE_SEND_ANALOG}"
-
-        await self._make_request_post(url, data)
-
-    async def send_digital_values(
-        self, channels: list[CoEChannel], second_page: bool = False
-    ) -> None:
-        """Send digital values to the CoE server."""
-        _LOGGER.debug("Send digital values to CoE server")
-
-        if not self._check_channel_type(
-            ChannelMode.DIGITAL, channels
-        ) or not self._check_array_length(channels, self.DIGITAL_VALUES_PER_PAGE):
-            _LOGGER.error("Could not send digital values. Please see logs for details.")
-            return
-
-        data = {"values": [bool(x.value) for x in channels], "page": int(second_page)}
-
-        url = f"{self.host}{self.COE_SEND_DIGITAL}"
-        await self._make_request_post(url, data)
+from typing import Any, Dict
+
+from aiohttp import ClientSession
+
+from .api import API
+from .coe_channel import CoEChannel
+from .const import _LOGGER, ChannelMode
+
+
+class CoEAPI(API):
+    """Class to perform API requests to the CoE Addon."""
+
+    COE_VERSION = "/version"
+    COE_DATA = "/receive/{id}"
+    COE_SEND_ANALOG = "/send/analog"
+    COE_SEND_DIGITAL = "/send/digital"
+
+    DIGITAL_VALUES_PER_PAGE = 16
+    ANALOG_VALUES_PER_PAGE = 4
+
+    def __init__(self, host: str, session: ClientSession = None) -> None:
+        """Initialize."""
+        super().__init__(session)
+
+        self.host = host
+
+    async def get_coe_data(self, can_id: int) -> Dict[str, Any] | None:
+        """Get the CoE data."""
+        url = f"{self.host}{self.COE_DATA.replace('{id}', str(can_id))}"
+
+        _LOGGER.debug("Receive data from CoE server: %s", url)
+
+        data = await self._make_request_get(url)
+
+        _LOGGER.debug("Received data from CoE server: %s", data)
+
+        if len(data) == 0:
+            return None
+
+        return data
+
+    async def get_coe_version(self) -> str | None:
+        """Get the version of the CoE server."""
+        url = f"{self.host}{self.COE_VERSION}"
+
+        _LOGGER.debug("Receive current version from CoE server: %s", url)
+
+        data = await self._make_request_get(url)
+
+        _LOGGER.debug("Received version from CoE server: %s", data)
+
+        if len(data) == 0:
+            return None
+
+        return data.get("version", None)
+
+    @staticmethod
+    def _check_channel_mode(
+        target_mode: ChannelMode, channel_to_check: list[CoEChannel]
+    ) -> bool:
+        """Check if the channel type equals the target."""
+        for channel in channel_to_check:
+            if channel.mode != target_mode:
+                _LOGGER.warning(
+                    f"Channel has wrong mode. Expected mode: {target_mode}, actual mode: {channel.mode}"
+                )
+                return False
+
+        return True
+
+    @staticmethod
+    def _check_array_length(array: list, target_size: int) -> bool:
+        """Check if a list has the required length."""
+        if len(array) != target_size:
+            _LOGGER.warning(
+                f"List has wrong length. Expected length: {target_size}, actual length: {len(array)}"
+            )
+            return False
+
+        return True
+
+    @staticmethod
+    def _check_analog_page_size(provided: int) -> bool:
+        """Check if the page is in the right number range."""
+        if not (0 < provided < 9):
+            _LOGGER.warning(
+                f"Page is not in the expected range. Expected range: 0 < page < 9, actual value: {provided}"
+            )
+            return False
+
+        return True
+
+    @staticmethod
+    def _convert_analog_channel_to_dict(channel: CoEChannel) -> dict[str, Any]:
+        """Convert a analog coe channel to a dict."""
+        return {"value": channel.value, "unit": int(channel.unit)}
+
+    async def send_analog_values(self, channels: list[CoEChannel], page: int):
+        """Send analog values to the CoE server."""
+        _LOGGER.debug("Send analog values to CoE server")
+
+        if (
+            not self._check_channel_mode(ChannelMode.ANALOG, channels)
+            or not self._check_array_length(channels, self.ANALOG_VALUES_PER_PAGE)
+            or not self._check_analog_page_size(page)
+        ):
+            _LOGGER.error("Could not send analog values. Please see logs for details.")
+            return
+
+        data = {
+            "values": [
+                self._convert_analog_channel_to_dict(channel) for channel in channels
+            ],
+            "page": page,
+        }
+
+        url = f"{self.host}{self.COE_SEND_ANALOG}"
+
+        await self._make_request_post(url, data)
+
+    async def send_digital_values(
+        self, channels: list[CoEChannel], second_page: bool = False
+    ) -> None:
+        """Send digital values to the CoE server."""
+        _LOGGER.debug("Send digital values to CoE server")
+
+        if not self._check_channel_mode(
+            ChannelMode.DIGITAL, channels
+        ) or not self._check_array_length(channels, self.DIGITAL_VALUES_PER_PAGE):
+            _LOGGER.error("Could not send digital values. Please see logs for details.")
+            return
+
+        data = {"values": [bool(x.value) for x in channels], "page": int(second_page)}
+
+        url = f"{self.host}{self.COE_SEND_DIGITAL}"
+        await self._make_request_post(url, data)
```

### Comparing `ta-cmi-3.2.0/ta_cmi/const.py` & `ta-cmi-3.2.1.dev0/ta_cmi/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,199 @@
-import enum
-from logging import Logger, NullHandler, getLogger
-from typing import Dict
-
-HTTP_OK: int = 200
-HTTP_UNAUTHORIZED: int = 401
-
-_LOGGER: Logger = getLogger(__package__)
-_LOGGER.addHandler(NullHandler())
-
-
-class ChannelType(enum.Enum):
-    INPUT = "Inputs"
-    OUTPUT = "Outputs"
-    DL_BUS = "DL-Bus"
-    SYSTEM_VALUES_GENERAL = "General"
-    SYSTEM_VALUES_DATE = "Date"
-    SYSTEM_VALUES_TIME = "Time"
-    SYSTEM_VALUES_SUN = "Sun"
-    SYSTEM_VALUES_E_POWER = "Electrical power"
-    NETWORK_ANALOG = "Network Analog"
-    NETWORK_DIGITAL = "Network Digital"
-    MBUS = "MBus"
-    MODBUS = "Modbus"
-    KNX = "KNX"
-    ANALOG_LOGGING = "Logging Analog"
-    DIGITAL_LOGGING = "Logging Digital"
-
-
-class ChannelMode(enum.Enum):
-    ANALOG = "A"
-    DIGITAL = "D"
-
-
-class ReadOnlyClass(type):
-    def __setattr__(self, name, value):
-        raise ValueError(name)
-
-
-class Languages(enum.Enum):
-    DE = 0
-    EN = 1
-
-
-DEVICES: Dict[str, str] = {
-    "22": "DUMMY-NO-IO",
-    "80": "UVR1611",
-    "87": "UVR16x2",
-    "88": "RSM610",
-    "89": "CAN-I/O45",
-    "8B": "CAN-EZ2",
-    "8C": "CAN-MTx2",
-    "8D": "CAN-BC2",
-    "8E": "UVR65",
-    "8F": "CAN-EZ3",
-    "91": "UVR610",
-    "92": "UVR67",
-}
-
-SUPPORTED_PARAMS_FOR_DEVICE: Dict[str, str] = {
-    "22": "AM",
-    "80": "I,O,Na,Nd",
-    "87": "I,O,D,Sg,Sd,St,Ss,La,Ld",
-    "88": "I,O,D,M",
-    "89": "I,O,D",
-    "8B": "I,O,Sp",
-    "8D": "M,AM,Ak",
-    "8F": "D,Sg,Sd,St,Ss,Sp,AM,La,Ld",
-    "91": "I,O,D,M,La,Ld",
-}
-
-UNITS_EN: Dict[str, str] = {
-    "1": "°C",
-    "2": "W/m²",
-    "3": "l/h",
-    "4": "sec",
-    "5": "min",
-    "6": "l/Imp",
-    "7": "K",
-    "8": "%",
-    "10": "kW",
-    "11": "kWh",
-    "12": "MWh",
-    "13": "V",
-    "14": "mA",
-    "15": "hr",
-    "16": "Days",
-    "17": "Imp",
-    "18": "kΩ",
-    "19": "l",
-    "20": "km/h",
-    "21": "Hz",
-    "22": "l/min",
-    "23": "bar",
-    "24": "",
-    "25": "km",
-    "26": "m",
-    "27": "mm",
-    "28": "m³",
-    "35": "l/d",
-    "36": "m/s",
-    "37": "m³/min",
-    "38": "m³/h",
-    "39": "m³/d",
-    "40": "mm/min",
-    "41": "mm/h",
-    "42": "mm/d",
-    "43": "On/Off",
-    "44": "No/Yes",
-    "46": "°C",
-    "50": "€",
-    "51": "$",
-    "52": "g/m³",
-    "54": "°",
-    "56": "°",
-    "57": "sec",
-    "59": "%",
-    "60": "h",
-    "63": "A",
-    "65": "mbar",
-    "66": "Pa",
-    "67": "ppm",
-    "69": "W",
-    "70": "t",
-    "71": "kg",
-    "72": "g",
-    "73": "cm",
-    "74": "K",
-    "75": "lx",
-}
-
-UNITS_DE: Dict[str, str] = {
-    "1": "°C",
-    "2": "W/m²",
-    "3": "l/h",
-    "4": "Sek",
-    "5": "Min",
-    "6": "l/Imp",
-    "7": "K",
-    "8": "%",
-    "10": "kW",
-    "11": "kWh",
-    "12": "MWh",
-    "13": "V",
-    "14": "mA",
-    "15": "Std",
-    "16": "Tage",
-    "17": "Imp",
-    "18": "kΩ",
-    "19": "l",
-    "20": "km/h",
-    "21": "Hz",
-    "22": "l/min",
-    "23": "bar",
-    "24": "",
-    "25": "km",
-    "26": "m",
-    "27": "mm",
-    "28": "m³",
-    "35": "l/d",
-    "36": "m/s",
-    "37": "m³/min",
-    "38": "m³/h",
-    "39": "m³/d",
-    "40": "mm/min",
-    "41": "mm/h",
-    "42": "mm/d",
-    "43": "Aus/Ein",
-    "44": "Nein/Ja",
-    "46": "°C",
-    "50": "€",
-    "51": "$",
-    "52": "g/m³",
-    "54": "°",
-    "56": "°",
-    "57": "Sek",
-    "59": "%",
-    "60": "Uhr",
-    "63": "A",
-    "65": "mbar",
-    "66": "Pa",
-    "67": "ppm",
-    "69": "W",
-    "70": "t",
-    "71": "kg",
-    "72": "g",
-    "73": "cm",
-    "74": "K",
-    "75": "lx",
-}
-
-RAS_STATE: Dict[int, str] = {
-    0: "Time/auto",
-    1: "Standard",
-    2: "Setback",
-    3: "Standby/frost pr",
-}
+import enum
+from logging import Logger, NullHandler, getLogger
+from typing import Dict
+
+HTTP_OK: int = 200
+HTTP_UNAUTHORIZED: int = 401
+
+_LOGGER: Logger = getLogger(__package__)
+_LOGGER.addHandler(NullHandler())
+
+
+class ChannelType(enum.Enum):
+    INPUT = "Inputs"
+    OUTPUT = "Outputs"
+    DL_BUS = "DL-Bus"
+    SYSTEM_VALUES_GENERAL = "General"
+    SYSTEM_VALUES_DATE = "Date"
+    SYSTEM_VALUES_TIME = "Time"
+    SYSTEM_VALUES_SUN = "Sun"
+    SYSTEM_VALUES_E_POWER = "Electrical power"
+    NETWORK_ANALOG = "Network Analog"
+    NETWORK_DIGITAL = "Network Digital"
+    MBUS = "MBus"
+    MODBUS = "Modbus"
+    KNX = "KNX"
+    ANALOG_LOGGING = "Logging Analog"
+    DIGITAL_LOGGING = "Logging Digital"
+
+
+class ChannelMode(enum.Enum):
+    ANALOG = "A"
+    DIGITAL = "D"
+
+
+class ReadOnlyClass(type):
+    def __setattr__(self, name, value):
+        raise ValueError(name)
+
+
+class Languages(enum.Enum):
+    DE = 0
+    EN = 1
+
+
+DEVICES: Dict[str, str] = {
+    "22": "DUMMY-NO-IO",
+    "80": "UVR1611",
+    "87": "UVR16x2",
+    "88": "RSM610",
+    "89": "CAN-I/O45",
+    "8B": "CAN-EZ2",
+    "8C": "CAN-MTx2",
+    "8D": "CAN-BC2",
+    "8E": "UVR65",
+    "8F": "CAN-EZ3",
+    "91": "UVR610",
+    "92": "UVR67",
+}
+
+SUPPORTED_PARAMS_FOR_DEVICE: Dict[str, str] = {
+    "22": "AM",
+    "80": "I,O,Na,Nd",
+    "87": "I,O,D,Sg,Sd,St,Ss,La,Ld",
+    "88": "I,O,D,M",
+    "89": "I,O,D",
+    "8B": "I,O,Sp",
+    "8D": "M,AM,Ak",
+    "8F": "D,Sg,Sd,St,Ss,Sp,AM,La,Ld",
+    "91": "I,O,D,M,La,Ld",
+}
+
+UNITS_EN: Dict[str, str] = {
+    "1": "°C",
+    "2": "W/m²",
+    "3": "l/h",
+    "4": "sec",
+    "5": "min",
+    "6": "l/Imp",
+    "7": "K",
+    "8": "%",
+    "10": "kW",
+    "11": "kWh",
+    "12": "MWh",
+    "13": "V",
+    "14": "mA",
+    "15": "hr",
+    "16": "Days",
+    "17": "Imp",
+    "18": "kΩ",
+    "19": "l",
+    "20": "km/h",
+    "21": "Hz",
+    "22": "l/min",
+    "23": "bar",
+    "24": "",
+    "25": "km",
+    "26": "m",
+    "27": "mm",
+    "28": "m³",
+    "35": "l/d",
+    "36": "m/s",
+    "37": "m³/min",
+    "38": "m³/h",
+    "39": "m³/d",
+    "40": "mm/min",
+    "41": "mm/h",
+    "42": "mm/d",
+    "43": "On/Off",
+    "44": "No/Yes",
+    "46": "°C",
+    "50": "€",
+    "51": "$",
+    "52": "g/m³",
+    "54": "°",
+    "56": "°",
+    "57": "sec",
+    "59": "%",
+    "60": "h",
+    "63": "A",
+    "65": "mbar",
+    "66": "Pa",
+    "67": "ppm",
+    "69": "W",
+    "70": "t",
+    "71": "kg",
+    "72": "g",
+    "73": "cm",
+    "74": "K",
+    "75": "lx",
+    "76": "Bg/m³",
+}
+
+UNITS_DE: Dict[str, str] = {
+    "1": "°C",
+    "2": "W/m²",
+    "3": "l/h",
+    "4": "Sek",
+    "5": "Min",
+    "6": "l/Imp",
+    "7": "K",
+    "8": "%",
+    "10": "kW",
+    "11": "kWh",
+    "12": "MWh",
+    "13": "V",
+    "14": "mA",
+    "15": "Std",
+    "16": "Tage",
+    "17": "Imp",
+    "18": "kΩ",
+    "19": "l",
+    "20": "km/h",
+    "21": "Hz",
+    "22": "l/min",
+    "23": "bar",
+    "24": "",
+    "25": "km",
+    "26": "m",
+    "27": "mm",
+    "28": "m³",
+    "35": "l/d",
+    "36": "m/s",
+    "37": "m³/min",
+    "38": "m³/h",
+    "39": "m³/d",
+    "40": "mm/min",
+    "41": "mm/h",
+    "42": "mm/d",
+    "43": "Aus/Ein",
+    "44": "Nein/Ja",
+    "46": "°C",
+    "50": "€",
+    "51": "$",
+    "52": "g/m³",
+    "54": "°",
+    "56": "°",
+    "57": "Sek",
+    "59": "%",
+    "60": "Uhr",
+    "63": "A",
+    "65": "mbar",
+    "66": "Pa",
+    "67": "ppm",
+    "69": "W",
+    "70": "t",
+    "71": "kg",
+    "72": "g",
+    "73": "cm",
+    "74": "K",
+    "75": "lx",
+    "76": "Bg/m³",
+}
+
+RAS_STATE: Dict[int, str] = {
+    0: "Time/auto",
+    1: "Standard",
+    2: "Setback",
+    3: "Standby/frost pr",
+}
```

