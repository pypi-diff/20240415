# Comparing `tmp/easymcp2221-1.7.1.tar.gz` & `tmp/easymcp2221-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymcp2221-1.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "easymcp2221-1.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easymcp2221-1.7.1.tar` & `easymcp2221-1.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7734 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/Constants.py
--rw-r--r--   0        0        0     6681 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/I2C_Slave.py
--rw-r--r--   0        0        0    74903 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/MCP2221.py
--rw-r--r--   0        0        0     1482 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/__init__.py
--rw-r--r--   0        0        0     1867 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/exceptions.py
--rw-r--r--   0        0        0     9416 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/EasyMCP2221/smbus.py
--rw-r--r--   0        0        0     1036 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/LICENSE
--rw-r--r--   0        0        0     1868 2023-06-16 14:47:10.376538 easymcp2221-1.7.1/README.rst
--rw-r--r--   0        0        0      768 2023-06-16 14:47:10.712562 easymcp2221-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 easymcp2221-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     7734 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/Constants.py
+-rw-r--r--   0        0        0     7566 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/I2C_Slave.py
+-rw-r--r--   0        0        0    76317 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/MCP2221.py
+-rw-r--r--   0        0        0     1482 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/__init__.py
+-rw-r--r--   0        0        0     1867 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/exceptions.py
+-rw-r--r--   0        0        0     9416 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/EasyMCP2221/smbus.py
+-rw-r--r--   0        0        0     1036 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/LICENSE
+-rw-r--r--   0        0        0     1868 2024-04-15 19:51:36.049461 easymcp2221-1.7.2/README.rst
+-rw-r--r--   0        0        0      768 2024-04-15 19:51:36.293462 easymcp2221-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 easymcp2221-1.7.2/PKG-INFO
```

### Comparing `easymcp2221-1.7.1/EasyMCP2221/Constants.py` & `easymcp2221-1.7.2/EasyMCP2221/Constants.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/EasyMCP2221/I2C_Slave.py` & `easymcp2221-1.7.2/EasyMCP2221/I2C_Slave.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,44 +8,48 @@
     Usually you create new instances of this class using :func:`EasyMCP2221.Device.I2C_Slave` function. See *examples* section.
 
     Parameters:
         mcp (EasyMCP2221.Device): MCP2221 connected to this slave
         addr  (int) : Slave's I2C bus address
         force (bool, optional): Create an I2C_Slave even if the target device does not answer. Default: False.
         speed (int, optional): I2C bus speed. Valid values from 50000 to 400000. See :func:`EasyMCP2221.Device.I2C_speed`.
+        reg_bytes     (int, optional): How many bytes is the register, position or command to send (default 1 byte).
+        reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default 'big'.
 
     Raises:
         RuntimeError: If the device didn't acknowledge.
 
     Examples:
         You should create I2C_Slave objects from the inside of an EasyMCP2221.Device:
 
         >>> import EasyMCP2221
         >>> mcp = EasyMCP2221.Device()
-        >>> eeprom = mcp.I2C_Slave(0x50)
+        >>> eeprom = mcp.I2C_Slave(0x50, reg_bytes = 2)
         >>> eeprom
         EasyMCP2221's I2C slave device at bus address 0x50.
 
         Or in a stand-alone way:
 
         >>> import EasyMCP2221
         >>> from EasyMCP2221 import I2C_Slave
         >>> mcp = EasyMCP2221.Device()
-        >>> eeprom = I2C_Slave.I2C_Slave(mcp, 0x50)
+        >>> eeprom = I2C_Slave.I2C_Slave(mcp, 0x50, reg_bytes = 2)
 
     Note:
         MCP2221 firmware exposes a subset of predefined I2C operations, but does not allow I2C primitives (i.e. start, stop, read + ack, read + nak, clock bus, etc.).
     """
 
     mcp = None
     addr = None
 
-    def __init__(self, mcp, addr, force = False, speed = 100000):
+    def __init__(self, mcp, addr, force = False, speed = 100000, reg_bytes = 1, reg_byteorder = 'big'):
         self.mcp = mcp
         self.addr = addr
+        self.reg_bytes = reg_bytes
+        self.reg_byteorder = reg_byteorder
 
         mcp.I2C_speed(speed)
 
         if not force and not self.is_present():
             raise RuntimeError("No device found at address 0x%02X." % (addr))
 
 
@@ -67,15 +71,15 @@
         except NotAckError:
             return False
 
 
     #######################################################################
     # Read
     #######################################################################
-    def read_register(self, register, length = 1, reg_bytes = 1, reg_byteorder = 'big'):
+    def read_register(self, register, length = 1, reg_bytes = None, reg_byteorder = None):
         """ Read from a specific register, position or command.
 
         Sequence:
 
         - Start
         - Send device I2C address + R/W bit 0
         - Send register byte, memory position or command
@@ -85,31 +89,38 @@
         - Stop
 
         See :func:`EasyMCP2221.Device.I2C_read` for more information.
 
         Parameters:
             register      (int): Register to read, memory position or command.
             length        (int, optional): How many bytes is the answer to read (default read 1 byte).
-            reg_bytes     (int, optional): How many bytes is the register, position or command to send (default 1 byte).
-            reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default 'big'.
+            reg_bytes     (int, optional): How many bytes is the register, position or command to send (default is defined in the class constructor).
+            reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default is defined in the class constructor.
 
         Return:
             bytes string
 
         Examples:
             Read from a regular i2c device, register 0x0D:
 
             >>> bme.read_register(0x0D)
             >>> b'\xff'
 
             Read 10 bytes from I2C EEPROM (2 bytes memory position):
 
-            >>> eeprom.read_register(2000, 25, reg_bytes=2)
+            >>> eeprom = mcp.I2C_Slave(0x50, reg_bytes = 2)
+            >>> eeprom.read_register(2000, 25)
             >>> b'en muchas partes hallaba '
         """
+        if reg_bytes is None:
+            reg_bytes = self.reg_bytes
+
+        if reg_byteorder is None:
+            reg_byteorder = self.reg_byteorder
+
         self.mcp.I2C_write(
             self.addr,
             register.to_bytes(reg_bytes, byteorder = reg_byteorder),
             kind = 'nonstop')
 
         data = self.mcp.I2C_read(
             self.addr,
@@ -136,15 +147,15 @@
         return self.mcp.I2C_read(self.addr, length)
 
 
 
     #######################################################################
     # Write
     #######################################################################
-    def write_register(self, register, data, reg_bytes = 1, reg_byteorder = 'big'):
+    def write_register(self, register, data,  reg_bytes = None, reg_byteorder = None):
         """ Write to a specific register, position or command.
 
         Sequence:
 
         - Start
         - Send device I2C address + R/W bit 0
         - Send register byte, memory position or command
@@ -154,28 +165,35 @@
         - Stop
 
         See :func:`EasyMCP2221.Device.I2C_write` for more information.
 
         Parameters:
             register      (int): Register to read, memory position or command.
             data        (bytes): Data to write. Bytes, int from 0 to 255, or list of ints from 0 to 255.
-            reg_bytes     (int, optional): How many bytes is the register, position or command to send (default 1 byte).
-            reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default 'big'.
+            reg_bytes     (int, optional): How many bytes is the register, position or command to send (default is defined in the class constructor.).
+            reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default is defined in the class constructor.
 
         Examples:
             Set PCF8591's DAC output to 255. Command 0bx1xxxxxx.
 
             >>> pcf.write_register(0b01000000, 255)
 
             Write a stream of bytes to an EEPROM at position 0x1A00 (2 bytes memory position):
 
-            >>> eeprom.write_register(0x1A00, b'Testing 123...', reg_bytes=2)
-            >>> eeprom.read_register(0x1A00, 14, reg_bytes=2)
+            >>> eeprom = mcp.I2C_Slave(0x50, reg_bytes = 2)
+            >>> eeprom.write_register(0x1A00, b'Testing 123...')
+            >>> eeprom.read_register(0x1A00, 14)
             b'Testing 123...'
         """
+        if reg_bytes is None:
+            reg_bytes = self.reg_bytes
+
+        if reg_byteorder is None:
+            reg_byteorder = self.reg_byteorder
+
         if type(data) == int:
             data = bytes([data])
         elif type(data) == list:
             data = bytes(data)
 
         self.mcp.I2C_write(
             self.addr,
```

### Comparing `easymcp2221-1.7.1/EasyMCP2221/MCP2221.py` & `easymcp2221-1.7.2/EasyMCP2221/MCP2221.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,17 @@
 
             # This command does not return anything
             if buf[0] == CMD_RESET_CHIP:
                 return None
 
             # Read response
             try:
-                r = self.hidhandler.read(PACKET_SIZE, 50)
+                # timeout 50 removed due to Issue
+                # https://github.com/electronicayciencia/EasyMCP2221/issues/7
+                r = self.hidhandler.read(PACKET_SIZE)
             except OSError:
                 if retry < self.cmd_retries:
                     continue
                 else:
                     raise
 
             if self.trace_packets:
@@ -1147,24 +1149,27 @@
 
         self.SRAM_config(adc_ref = ref | vrm)
 
         # When GP1, 2 and 3 are ADC and ADC_REF is Vdd. If Vrm ref is selected, ADC stop working.
         self._reinforce_SRAM()
 
 
-    def ADC_read(self):
+    def ADC_read(self, norm=False):
         """ Read all Analog to Digital Converter (ADC) channels.
 
         Analog value is always available regardless of pin function (see :func:`set_pin_function`).
         If pin is configured as output (GPIO_OUT or LED_I2C), the read value is always the output state.
 
         ADC is 10 bits, so the minimum value is 0 and the maximum value is 1023.
 
+        Parameters:
+            norm (bool, optional): Divide output values by 1024 and return output between 0 and 1. Default  is ``False``.
+
         Return:
-            tuple of int: Value of 3 channels (gp1, gp2, gp3).
+            tuple: Value of 3 channels (gp1, gp2, gp3).
 
         Examples:
             All three pins configured as ADC inputs.
 
             >>> mcp.ADC_config(ref = "VDD")
             >>> mcp.set_pin_function(
             ...    gp1 = "ADC",
@@ -1182,14 +1187,20 @@
             >>> mcp.ADC_read()
             (1023, 0, 198)
         """
         buf = self.send_cmd([CMD_POLL_STATUS_SET_PARAMETERS])
         adc1 = buf[I2C_POLL_RESP_ADC_CH0_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH0_MSB]
         adc2 = buf[I2C_POLL_RESP_ADC_CH1_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH1_MSB]
         adc3 = buf[I2C_POLL_RESP_ADC_CH2_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH2_MSB]
+
+        if norm:
+            adc1 = adc1 / 1024
+            adc2 = adc2 / 1024
+            adc3 = adc3 / 1024
+
         return (adc1, adc2, adc3)
 
 
     #######################################################################
     # DAC
     #######################################################################
     def DAC_config(self, ref = "VDD", out = None):
@@ -1250,39 +1261,48 @@
             raise ValueError("Accepted values for out are from 0 to 31.")
 
         self.SRAM_config(
             dac_ref = ref | vrm,
             dac_value = out)
 
 
-    def DAC_write(self, out):
+    def DAC_write(self, out, norm=False):
         """ Set the DAC output value.
 
         Valid ``out`` values are 0 to 31.
 
         To use a GP pin as DAC, you must assign the function "DAC" (see :func:`set_pin_function`).
         MCP2221 only have 1 DAC. So if you assign to "DAC" GP2 and GP3 you will
         see the same output value in both.
 
         Parameters:
             out (int): Value to output (max. 32) referenced to DAC ref voltage.
+            norm (bool, optional): Accept input values as floats between 0 and 1. Default  is ``False``.
 
         Examples:
             >>> mcp.set_pin_function(gp2 = "DAC")
             >>> mcp.DAC_config(ref = "VDD")
             >>> mcp.DAC_write(31)
             >>>
 
             >>> mcp.DAC_write(32)
             Traceback (most recent call last):
             ...
             ValueError: Accepted values for out are from 0 to 31.
         """
-        if out not in range(0, 32):
-            raise ValueError("Accepted values for out are from 0 to 31.")
+        if norm:
+            if not 0 <= out <= 1:
+                raise ValueError("Accepted values for out when norm=True are from 0 to 1.")
+
+            out = out * 32
+            if out > 31: out = 31
+
+        else:
+            if out not in range(0, 32):
+                raise ValueError("Accepted values for out are from 0 to 31.")
 
         self.SRAM_config(dac_value = out)
 
 
     #######################################################################
     # Interrupt On Change
     #######################################################################
@@ -1743,33 +1763,43 @@
 
             else:
                 self._i2c_release()
                 raise RuntimeError("I2C read error. Internal status %02x." % (rbuf[I2C_INTERNAL_STATUS_BYTE]))
 
 
 
-    def I2C_Slave(self, addr, force = False, speed = 100000):
+    def I2C_Slave(self, addr, force = False, speed = 100000, reg_bytes = 1, reg_byteorder = 'big'):
         """ Create a new I2C_Slave object.
 
         See :class:`EasyMCP2221.I2C_Slave.I2C_Slave` for detailed information.
 
         Parameters:
-            addr (int): Slave's I2C bus address
+            addr  (int) : Slave's I2C bus address
+            force (bool, optional): Create an I2C_Slave even if the target device does not answer. Default: False.
+            speed (int, optional): I2C bus speed. Valid values from 50000 to 400000. See :func:`EasyMCP2221.Device.I2C_speed`.
+            reg_bytes     (int, optional): How many bytes is the register, position or command to send (default 1 byte).
+            reg_byteorder (str, optional): Byte order of the register address. *'little'* or *'big'*. Default 'big'.
 
         Return:
             I2C_Slave object.
 
         Example:
             >>> pcf    = mcp.I2C_Slave(0x48)
-            >>> eeprom = mcp.I2C_Slave(0x50)
+            >>> eeprom = mcp.I2C_Slave(0x50, reg_bytes = 2)
             >>> eeprom
             EasyMCP2221's I2C slave device at bus address 0x50.
 
         """
-        return I2C_Slave.I2C_Slave(self, addr, force, speed)
+        return I2C_Slave.I2C_Slave(
+            self,
+            addr = addr,
+            force = force,
+            speed = speed,
+            reg_bytes = reg_bytes,
+            reg_byteorder = reg_byteorder)
 
 
 
     def _i2c_release(self):
         """ Try to make the I2C bus ready for the next operation.
 
         This is a private method, the **API can change** without previous notice.
```

### Comparing `easymcp2221-1.7.1/EasyMCP2221/__init__.py` & `easymcp2221-1.7.2/EasyMCP2221/__init__.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/EasyMCP2221/exceptions.py` & `easymcp2221-1.7.2/EasyMCP2221/exceptions.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/EasyMCP2221/smbus.py` & `easymcp2221-1.7.2/EasyMCP2221/smbus.py`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/LICENSE` & `easymcp2221-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/README.rst` & `easymcp2221-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `easymcp2221-1.7.1/pyproject.toml` & `easymcp2221-1.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "EasyMCP2221"
-version = "1.7.1"
+version = "1.7.2"
 authors = [
   { name="Reinoso Guzman", email="electronicayciencia@gmail.com" },
 ]
 description = "Python module to interface with MCP2221 focused on ease of use."
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `easymcp2221-1.7.1/PKG-INFO` & `easymcp2221-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyMCP2221
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python module to interface with MCP2221 focused on ease of use.
 Author-email: Reinoso Guzman <electronicayciencia@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

