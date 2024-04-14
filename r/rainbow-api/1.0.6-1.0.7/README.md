# Comparing `tmp/rainbow-api-1.0.6.tar.gz` & `tmp/rainbow_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow-api-1.0.6.tar", last modified: Tue Feb  6 19:57:20 2024, max compression
+gzip compressed data, was "rainbow_api-1.0.7.tar", last modified: Sun Apr 14 23:04:34 2024, max compression
```

## Comparing `rainbow-api-1.0.6.tar` & `rainbow_api-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.888227 rainbow-api-1.0.6/
--rw-r--r--   0 marvinj    (502) staff       (20)    35148 2023-12-22 00:47:12.000000 rainbow-api-1.0.6/COPYING
--rw-r--r--   0 marvinj    (502) staff       (20)     2979 2024-02-06 19:57:20.887217 rainbow-api-1.0.6/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)     2446 2023-12-22 00:47:12.000000 rainbow-api-1.0.6/README.md
--rw-r--r--   0 marvinj    (502) staff       (20)      634 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/pyproject.toml
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.800910 rainbow-api-1.0.6/rainbow/
--rw-r--r--   0 marvinj    (502) staff       (20)     2524 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/rainbow/__init__.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.825037 rainbow-api-1.0.6/rainbow/agilent/
--rw-r--r--   0 marvinj    (502) staff       (20)     1709 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/rainbow/agilent/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    26774 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/rainbow/agilent/chemstation.py
--rw-r--r--   0 marvinj    (502) staff       (20)     9030 2023-12-22 00:47:12.000000 rainbow-api-1.0.6/rainbow/agilent/masshunter.py
--rw-r--r--   0 marvinj    (502) staff       (20)     4994 2023-12-22 00:47:12.000000 rainbow-api-1.0.6/rainbow/datadirectory.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5281 2023-12-22 00:47:12.000000 rainbow-api-1.0.6/rainbow/datafile.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.844392 rainbow-api-1.0.6/rainbow/waters/
--rw-r--r--   0 marvinj    (502) staff       (20)     1574 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/rainbow/waters/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    22696 2024-02-06 19:56:19.000000 rainbow-api-1.0.6/rainbow/waters/masslynx.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.886295 rainbow-api-1.0.6/rainbow_api.egg-info/
--rw-r--r--   0 marvinj    (502) staff       (20)     2979 2024-02-06 19:57:20.000000 rainbow-api-1.0.6/rainbow_api.egg-info/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)      508 2024-02-06 19:57:20.000000 rainbow-api-1.0.6/rainbow_api.egg-info/SOURCES.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-02-06 19:57:20.000000 rainbow-api-1.0.6/rainbow_api.egg-info/dependency_links.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       22 2024-02-06 19:57:20.000000 rainbow-api-1.0.6/rainbow_api.egg-info/requires.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-02-06 19:57:20.000000 rainbow-api-1.0.6/rainbow_api.egg-info/top_level.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-02-06 19:57:20.888373 rainbow-api-1.0.6/setup.cfg
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-02-06 19:57:20.885119 rainbow-api-1.0.6/tests/
--rw-r--r--   0 marvinj    (502) staff       (20)     1607 2023-12-22 00:47:14.000000 rainbow-api-1.0.6/tests/test_agilent.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3414 2023-12-22 00:47:14.000000 rainbow-api-1.0.6/tests/test_datadirectory.py
--rw-r--r--   0 marvinj    (502) staff       (20)     4460 2023-12-22 00:47:14.000000 rainbow-api-1.0.6/tests/test_datafile.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1191 2023-12-22 00:47:14.000000 rainbow-api-1.0.6/tests/test_waters.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.804229 rainbow_api-1.0.7/
+-rw-r--r--   0 marvinj    (502) staff       (20)    35148 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/COPYING
+-rw-r--r--   0 marvinj    (502) staff       (20)     2979 2024-04-14 23:04:34.802628 rainbow_api-1.0.7/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)     2446 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/README.md
+-rw-r--r--   0 marvinj    (502) staff       (20)      634 2024-04-14 05:00:45.000000 rainbow_api-1.0.7/pyproject.toml
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.705649 rainbow_api-1.0.7/rainbow/
+-rw-r--r--   0 marvinj    (502) staff       (20)     2524 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/rainbow/__init__.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.731632 rainbow_api-1.0.7/rainbow/agilent/
+-rw-r--r--   0 marvinj    (502) staff       (20)     1709 2024-04-14 06:22:37.000000 rainbow_api-1.0.7/rainbow/agilent/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    28270 2024-04-14 06:39:02.000000 rainbow_api-1.0.7/rainbow/agilent/chemstation.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     9030 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/rainbow/agilent/masshunter.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     4994 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/rainbow/datadirectory.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5281 2024-04-14 06:19:19.000000 rainbow_api-1.0.7/rainbow/datafile.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.755496 rainbow_api-1.0.7/rainbow/waters/
+-rw-r--r--   0 marvinj    (502) staff       (20)     1574 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/rainbow/waters/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    22696 2024-04-14 05:00:12.000000 rainbow_api-1.0.7/rainbow/waters/masslynx.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.801013 rainbow_api-1.0.7/rainbow_api.egg-info/
+-rw-r--r--   0 marvinj    (502) staff       (20)     2979 2024-04-14 23:04:34.000000 rainbow_api-1.0.7/rainbow_api.egg-info/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)      508 2024-04-14 23:04:34.000000 rainbow_api-1.0.7/rainbow_api.egg-info/SOURCES.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-04-14 23:04:34.000000 rainbow_api-1.0.7/rainbow_api.egg-info/dependency_links.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       22 2024-04-14 23:04:34.000000 rainbow_api-1.0.7/rainbow_api.egg-info/requires.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-04-14 23:04:34.000000 rainbow_api-1.0.7/rainbow_api.egg-info/top_level.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-04-14 23:04:34.804447 rainbow_api-1.0.7/setup.cfg
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-14 23:04:34.799414 rainbow_api-1.0.7/tests/
+-rw-r--r--   0 marvinj    (502) staff       (20)     1607 2024-04-14 05:00:14.000000 rainbow_api-1.0.7/tests/test_agilent.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3414 2024-04-14 05:00:14.000000 rainbow_api-1.0.7/tests/test_datadirectory.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     4460 2024-04-14 05:00:14.000000 rainbow_api-1.0.7/tests/test_datafile.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1191 2024-04-14 05:00:14.000000 rainbow_api-1.0.7/tests/test_waters.py
```

### Comparing `rainbow-api-1.0.6/COPYING` & `rainbow_api-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/PKG-INFO` & `rainbow_api-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Read chromatography and mass spectrometry binary files
 Author: Evan Shi and Eugene Kwan
 Author-email: evanyshi@cmu.edu
 License: COPYING
 Project-URL: Repository, https://github.com/evanyeyeye/rainbow
 Project-URL: Documentation, https://rainbow-api.readthedocs.io
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rainbow-api-1.0.6/README.md` & `rainbow_api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/pyproject.toml` & `rainbow_api-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rainbow-api"
-version = "1.0.6"
+version = "1.0.7"
 description = "Read chromatography and mass spectrometry binary files"
 readme = "README.md"
 license = {text = "COPYING"}
 authors = [
     {name = "Evan Shi and Eugene Kwan"},
     {email = "evanyshi@cmu.edu"}
 ]
```

### Comparing `rainbow-api-1.0.6/rainbow/__init__.py` & `rainbow_api-1.0.7/rainbow/__init__.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/agilent/__init__.py` & `rainbow_api-1.0.7/rainbow/agilent/__init__.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/agilent/chemstation.py` & `rainbow_api-1.0.7/rainbow/agilent/chemstation.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,82 +84,98 @@
     Returns:
         DataFile with data from a channel, if the file can be parsed. \
             Otherwise, None.
 
     """
     with open(path, 'rb') as f:
         head = read_string(f, offset=0, gap=1)
-        if head == '179':
-            return parse_ch_fid(path)
-        elif head == '130' or head == '30':
+        if head in ['179', '181']:
+            return parse_ch_fid(path, head)
+        elif head in ['130', '30']:
             return parse_ch_other(path, head)
         return None
 
 
-def parse_ch_fid(path):
+def parse_ch_fid(path, head):
     """
     Parses an Agilent .ch file with FID channel data. 
     
     This method should not be called directly. Use :obj:`parse_ch` instead. 
 
     Learn more about this file format :ref:`here <ch_fid>`.
 
     Args:
         path (str): Path to the .ch file with FID data. 
 
     Returns:
         DataFile with FID data, if the file can be parsed. Otherwise, None.
 
     """
-    data_offsets = {
-        'num_times': 0x116,
-        'scaling_factor': 0x127C,
-        'data_start': 0x1800
-    }
+    if head == '181':
+        data_offsets = {
+            'num_times': 0x116,
+            'scaling_factor': 0x127C,
+            'data_start': 0x1800
+        }
+        metadata_offsets = {
+            'notebook': 0x35A,
+            'date': 0x957,
+            'method': 0xA0E,
+            'instrument': 0xC11,
+            'unit': 0x104C,
+        }
+        gap = 2
+    elif head == '179':
+        data_offsets = {
+            'num_times': 0x116,
+            'scaling_factor': 0x127C,
+            'data_start': 0x1800
+        }
+        metadata_offsets = {
+            'notebook': 0x35A,
+            'date': 0x957,
+            'method': 0xA0E,
+            'instrument': 0xC11,
+            'unit': 0x104C,
+            'signal': 0x1075
+        }
 
     f = open(path, 'rb')
     raw_bytes = f.read()
+    file_size = f.tell()
 
     # Extract the number of retention times.
-    f.seek(data_offsets['num_times'])
-    num_times = struct.unpack(">I", f.read(4))[0]
-    if num_times == 0:
-        return None
+    num_times = (file_size - data_offsets['data_start']) // 8
 
+    f.seek(data_offsets['num_times'] + 4)
     # Compute retention times using the first and last times. 
     start_time = struct.unpack(">f", f.read(4))[0]
     end_time = struct.unpack(">f", f.read(4))[0]
     delta_time = (end_time - start_time) / (num_times - 1)
     times = np.arange(start_time, end_time + 1e-3, delta_time)
 
     # Extract the raw data values.
-    data = np.ndarray(
-        num_times, '<d', raw_bytes, data_offsets['data_start'], 8)
+    if head == '181':
+        data = np.array(decode_double_delta(f, data_offsets['data_start']), dtype=np.float64)
+    else:
+        data = np.ndarray(num_times, '<d', raw_bytes, data_offsets['data_start'], 8)
     data = data.copy().reshape(-1, 1)
 
     # Convert times into minutes.
     times /= 60000
 
     # Scale the absorbances.
     f.seek(data_offsets['scaling_factor'])
     scaling_factor = struct.unpack('>d', f.read(8))[0]
     data *= scaling_factor
 
     # No ylabel for FID data. 
     ylabels = np.array([''])
 
     # Extract metadata from file header.
-    metadata_offsets = {
-        'notebook': 0x35A,
-        'date': 0x957,
-        'method': 0xA0E,
-        'instrument': 0xC11,
-        'unit': 0x104C,
-        'signal': 0x1075
-    }
     metadata = read_header(f, metadata_offsets)
     f.close()
 
     return DataFile(path, 'FID', times, ylabels, data, metadata)
 
 
 def parse_ch_other(path, head):
@@ -214,39 +230,18 @@
 
     f = open(path, 'rb')
     byte_unpack = struct.Struct('>B').unpack
     short_unpack = struct.Struct('>h').unpack
     int_unpack = struct.Struct('>i').unpack
 
     # Extract the raw data values.
-    # Count the total number of retention times. 
-    f.seek(data_offsets['data_start'])
-    absorbances = []
-    absorb_accum = 0
-    while True:
-        # If the segment header is invalid, stop reading.  
-        head = byte_unpack(f.read(1))[0]
-        if head != 0x10:
-            break
-        num_times_seg = byte_unpack(f.read(1))[0]
-
-        # If the next short is equal to -0x8000
-        #     then the next absorbance value is the next integer. 
-        # Otherwise, the short is a delta from the last absorbance value.
-        for _ in range(num_times_seg):
-            check_int = short_unpack(f.read(2))[0]
-            if check_int == -0x8000:
-                absorb_accum = int_unpack(f.read(4))[0]
-            else:
-                absorb_accum += check_int
-            absorbances.append(absorb_accum)
-
+    # Count the total number of retention times.
     # Process the extracted values.
-    # If no values are extracted, this file is invalid. 
-    data = np.array(absorbances)
+    # If no values are extracted, this file is invalid.
+    data = np.array(decode_delta(f, data_offsets['data_start']))
     num_times = data.size
     if num_times == 0:
         return None
 
     # Calculate retention times using the first and last times.
     f.seek(data_offsets['time_range'])
     start_time, end_time = struct.unpack('>ii', f.read(8))
@@ -275,14 +270,65 @@
         detector = 'UV'
     elif 'ADC' in signal:
         detector = 'ELSD' if 'CHANNEL' in signal else 'CAD'
     ylabels = np.array([ylabel])
 
     return DataFile(path, detector, times, ylabels, data, metadata)
 
+def decode_delta(f, offset):
+    byte_unpack = struct.Struct('>B').unpack
+    short_unpack = struct.Struct('>h').unpack
+    int_unpack = struct.Struct('>i').unpack
+    # Extract the raw data values.
+    # Count the total number of retention times.
+    f.seek(offset)
+    absorbances = []
+    absorb_accum = 0
+    while True:
+        # If the segment header is invalid, stop reading.
+        head = byte_unpack(f.read(1))[0]
+        if head != 0x10:
+            break
+        num_times_seg = byte_unpack(f.read(1))[0]
+
+        # If the next short is equal to -0x8000
+        #     then the next absorbance value is the next integer.
+        # Otherwise, the short is a delta from the last absorbance value.
+        for _ in range(num_times_seg):
+            check_int = short_unpack(f.read(2))[0]
+            if check_int == -0x8000:
+                absorb_accum = int_unpack(f.read(4))[0]
+            else:
+                absorb_accum += check_int
+            absorbances.append(absorb_accum)
+
+    return absorbances
+
+def decode_double_delta(f, offset):
+    byte_unpack = struct.Struct('>B').unpack
+    short_unpack = struct.Struct('>h').unpack
+    int_unpack = struct.Struct('>i').unpack
+    f.seek(0, 2)
+    file_size = f.tell()
+    f.seek(offset)
+    signals = []
+    count = 1
+    buffer = [0, 0, 0]
+
+    while f.tell() < file_size:
+        buffer[2] = short_unpack(f.read(2))[0]
+        if buffer[2] == 0x7fff:
+            buffer[0] = short_unpack(f.read(2))[0] << 32 | int_unpack(f.read(4))[0]
+            buffer[1] = 0
+        else:
+            buffer[1] += buffer[2]
+            buffer[0] += buffer[1]
+        signals.append(buffer[0])
+
+    return signals
 
 """
 .uv PARSING METHODS
 
 """
```

### Comparing `rainbow-api-1.0.6/rainbow/agilent/masshunter.py` & `rainbow_api-1.0.7/rainbow/agilent/masshunter.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/datadirectory.py` & `rainbow_api-1.0.7/rainbow/datadirectory.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/datafile.py` & `rainbow_api-1.0.7/rainbow/datafile.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/waters/__init__.py` & `rainbow_api-1.0.7/rainbow/waters/__init__.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow/waters/masslynx.py` & `rainbow_api-1.0.7/rainbow/waters/masslynx.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/rainbow_api.egg-info/PKG-INFO` & `rainbow_api-1.0.7/rainbow_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Read chromatography and mass spectrometry binary files
 Author: Evan Shi and Eugene Kwan
 Author-email: evanyshi@cmu.edu
 License: COPYING
 Project-URL: Repository, https://github.com/evanyeyeye/rainbow
 Project-URL: Documentation, https://rainbow-api.readthedocs.io
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rainbow-api-1.0.6/tests/test_agilent.py` & `rainbow_api-1.0.7/tests/test_agilent.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/tests/test_datadirectory.py` & `rainbow_api-1.0.7/tests/test_datadirectory.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/tests/test_datafile.py` & `rainbow_api-1.0.7/tests/test_datafile.py`

 * *Files identical despite different names*

### Comparing `rainbow-api-1.0.6/tests/test_waters.py` & `rainbow_api-1.0.7/tests/test_waters.py`

 * *Files identical despite different names*

