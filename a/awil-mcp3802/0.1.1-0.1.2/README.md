# Comparing `tmp/awil_mcp3802-0.1.1.tar.gz` & `tmp/awil_mcp3802-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awil_mcp3802-0.1.1.tar", last modified: Wed Apr 10 09:32:54 2024, max compression
+gzip compressed data, was "awil_mcp3802-0.1.2.tar", last modified: Mon Apr 15 04:46:30 2024, max compression
```

## Comparing `awil_mcp3802-0.1.1.tar` & `awil_mcp3802-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:32:54.104290 awil_mcp3802-0.1.1/
--rw-rw-rw-   0        0        0     1084 2024-04-08 06:37:53.000000 awil_mcp3802-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      556 2024-04-10 09:32:54.103291 awil_mcp3802-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-10 09:13:15.000000 awil_mcp3802-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 09:32:54.095289 awil_mcp3802-0.1.1/awil_mcp3802/
--rw-rw-rw-   0        0        0       27 2024-04-08 06:43:12.000000 awil_mcp3802-0.1.1/awil_mcp3802/__init__.py
--rw-rw-rw-   0        0        0     1933 2024-04-10 09:28:53.000000 awil_mcp3802-0.1.1/awil_mcp3802/awil_mcp3802.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:32:54.103291 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/
--rw-rw-rw-   0        0        0      556 2024-04-10 09:32:54.000000 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-04-10 09:32:54.000000 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:32:54.000000 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 09:32:54.000000 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 09:32:54.000000 awil_mcp3802-0.1.1/awil_mcp3802.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:32:54.104290 awil_mcp3802-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-04-10 09:32:22.000000 awil_mcp3802-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:46:30.877990 awil_mcp3802-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2024-04-08 06:37:53.000000 awil_mcp3802-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      556 2024-04-15 04:46:30.877990 awil_mcp3802-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-10 09:13:15.000000 awil_mcp3802-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 04:46:30.872990 awil_mcp3802-0.1.2/awil_mcp3802/
+-rw-rw-rw-   0        0        0       27 2024-04-08 06:43:12.000000 awil_mcp3802-0.1.2/awil_mcp3802/__init__.py
+-rw-rw-rw-   0        0        0     1902 2024-04-15 04:44:03.000000 awil_mcp3802-0.1.2/awil_mcp3802/awil_mcp3802.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:46:30.876990 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/
+-rw-rw-rw-   0        0        0      556 2024-04-15 04:46:30.000000 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-15 04:46:30.000000 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 04:46:30.000000 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 04:46:30.000000 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 04:46:30.000000 awil_mcp3802-0.1.2/awil_mcp3802.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 04:46:30.877990 awil_mcp3802-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-04-15 04:44:10.000000 awil_mcp3802-0.1.2/setup.py
```

### Comparing `awil_mcp3802-0.1.1/LICENSE` & `awil_mcp3802-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awil_mcp3802-0.1.1/PKG-INFO` & `awil_mcp3802-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_mcp3802
-Version: 0.1.1
+Version: 0.1.2
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: awil_ft232h
```

### Comparing `awil_mcp3802-0.1.1/awil_mcp3802/awil_mcp3802.py` & `awil_mcp3802-0.1.2/awil_mcp3802/awil_mcp3802.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         self._awil_ft232h = awil_ft232h
 
         self._supply_voltage = supply_voltage
         self._spi_channel = spi_channel
         self._spi_frequency = spi_requency
 
     def read_voltage(self, channel: Channel) -> float:
-        transmitted_data = [
+        send_data = [
             ControlBit.START |  # Start bit
             ControlBit.SINGLE_ENDED |  # Single/Diff
             channel >> 2,  # Channel (MSB)
             (channel << 6 & 0b11000000),  # Channel (LSB)
             0b00000000
         ]
-        received_data = self._awil_ft232h.exchange(transmitted_data, cs=self._spi_channel, freq=self._spi_frequency, mode=self._SPI_MODE)
+        received_data = self._awil_ft232h.exchange(send_data, self._spi_channel, self._spi_frequency, self._SPI_MODE)
         voltage = self._received_data_to_voltage(received_data)
         return voltage
-    
+
     def read_all_voltages(self) -> List[float]:
         voltages = []
         for channel in range(self.AMOUNT_OF_CHANNELS):
             voltage = self.read_voltage(channel)
             voltages.append(voltage)
         return voltages
```

### Comparing `awil_mcp3802-0.1.1/awil_mcp3802.egg-info/PKG-INFO` & `awil_mcp3802-0.1.2/awil_mcp3802.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_mcp3802
-Version: 0.1.1
+Version: 0.1.2
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: awil_ft232h
```

