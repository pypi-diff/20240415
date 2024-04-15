# Comparing `tmp/pcffont-0.0.2.tar.gz` & `tmp/pcffont-0.0.3.tar.gz`

## Comparing `pcffont-0.0.2.tar` & `pcffont-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.2/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/artwiz/anorexia.pcf
--rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/artwiz/kates.pcf
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/dweep/dweep.pcf
--rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/profont-x11/ProFont_r400-29.pcf
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/raize/raize-normal-19.pcf
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/sgi/rock36.pcf
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/trisk/trisk.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.2/examples/__init__.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pcffont-0.0.2/examples/demo.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/error.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/font.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/header.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/metric.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/table.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/xlfd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/util.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_dump.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_load_save.py
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.2/LICENSE
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pcffont-0.0.2/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 pcffont-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/artwiz/anorexia.pcf
+-rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/artwiz/kates.pcf
+-rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/dweep/dweep.pcf
+-rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/profont-x11/ProFont_r400-29.pcf
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/raize/raize-normal-19.pcf
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/sgi/rock36.pcf
+-rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/trisk/trisk.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/__init__.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/create.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/load.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/error.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/font.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/format.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/header.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/metric.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/util.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_dump.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_example.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_load_save.py
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_reload.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 pcffont-0.0.3/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pcffont-0.0.3/PKG-INFO
```

### Comparing `pcffont-0.0.2/.github/workflows/publish.yml` & `pcffont-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/.github/workflows/test.yml` & `pcffont-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/artwiz/anorexia.pcf` & `pcffont-0.0.3/assets/artwiz/anorexia.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/artwiz/kates.pcf` & `pcffont-0.0.3/assets/artwiz/kates.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/dweep/dweep.pcf` & `pcffont-0.0.3/assets/dweep/dweep.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/profont-x11/ProFont_r400-29.pcf` & `pcffont-0.0.3/assets/profont-x11/ProFont_r400-29.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/raize/raize-normal-19.pcf` & `pcffont-0.0.3/assets/raize/raize-normal-19.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/sgi/rock36.pcf` & `pcffont-0.0.3/assets/sgi/rock36.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/trisk/trisk.pcf` & `pcffont-0.0.3/assets/trisk/trisk.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/unifont/OFL.txt` & `pcffont-0.0.3/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.3/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/examples/demo.py` & `pcffont-0.0.3/examples/load.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 
 from examples import assets_dir, build_dir
 from pcffont import PcfFont
 
 
 def main():
-    outputs_dir = os.path.join(build_dir, 'demo')
+    outputs_dir = os.path.join(build_dir, 'load')
     if os.path.exists(outputs_dir):
         shutil.rmtree(outputs_dir)
     os.makedirs(outputs_dir)
 
     font = PcfFont.load(os.path.join(assets_dir, 'unifont', 'unifont-15.1.05.pcf'))
     print(f'name: {font.properties.font}')
     print(f'size: {font.properties.pixel_size}')
@@ -20,16 +20,17 @@
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
         glyph_name = font.glyph_names[glyph_index]
         metric = font.metrics[glyph_index]
         bitmap = font.bitmaps[glyph_index]
         print(f'char: {chr(code_point)} ({code_point:04X})')
         print(f'glyph_name: {glyph_name}')
         print(f'advance_width: {metric.character_width}')
-        print(f'offset: ({-metric.left_sided_bearing}, {-metric.character_descent})')
+        print(f'offset: ({-metric.left_side_bearing}, {-metric.descent})')
         for bitmap_row in bitmap:
-            print(f'{''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')}*')
+            text = ''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')
+            print(f'{text}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pcffont-0.0.2/src/pcffont/error.py` & `pcffont-0.0.3/src/pcffont/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 
 class PcfError(Exception):
     pass
 
 
+class PcfParseError(PcfError):
+    pass
+
+
+class PcfTableTypeError(PcfError):
+    pass
+
+
 class PcfPropKeyError(PcfError):
     def __init__(self, key: str, reason: str):
         self.key = key
         self.reason = reason
         super().__init__(f"'{key}': {reason}")
 
 
@@ -19,7 +27,11 @@
 
 
 class PcfXlfdError(PcfError):
     def __init__(self, font_name: str, reason: str):
         self.font_name = font_name
         self.reason = reason
         super().__init__(f"'{font_name}': {reason}")
+
+
+class PcfOutOfRangeError(PcfError):
+    pass
```

### Comparing `pcffont-0.0.2/src/pcffont/font.py` & `pcffont-0.0.3/src/pcffont/font.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from collections import UserDict
 from typing import BinaryIO
 
-from pcffont.error import PcfError
+from pcffont.error import PcfParseError, PcfTableTypeError
 from pcffont.header import PcfTableType, PcfHeader
 from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.t_accelerators import PcfAccelerators
 from pcffont.t_bitmaps import PcfBitmaps
 from pcffont.t_encodings import PcfBdfEncodings
 from pcffont.t_glyph_names import PcfGlyphNames
@@ -22,15 +22,15 @@
         buffer = Buffer(stream)
 
         headers = PcfHeader.parse(buffer)
 
         tables = {}
         for header in headers:
             if header.table_type in tables and strict_level >= 1:
-                raise PcfError(f"Duplicate table '{header.table_type.name}'")
+                raise PcfParseError(f"Duplicate table '{header.table_type.name}'")
             table = util.parse_table(buffer, header, strict_level)
             tables[header.table_type] = table
 
         return PcfFont(tables)
 
     @staticmethod
     def load(
@@ -44,15 +44,15 @@
         super().__init__(tables)
 
     def __setitem__(self, table_type: PcfTableType, table: PcfTable | None):
         if table is None:
             self.pop(table_type, None)
         else:
             if not isinstance(table, util.TABLE_TYPE_REGISTRY[table_type]):
-                raise PcfError(f"Mismatched table type: '{table_type.name}' -> '{type(table)}'")
+                raise PcfTableTypeError(f"Mismatched table type: '{table_type.name}' -> '{type(table)}'")
             super().__setitem__(table_type, table)
 
     def __repr__(self) -> str:
         return object.__repr__(self)
 
     @property
     def properties(self) -> PcfProperties | None:
@@ -122,26 +122,22 @@
     def bdf_accelerators(self) -> PcfAccelerators | None:
         return self.get(PcfTableType.BDF_ACCELERATORS, None)
 
     @bdf_accelerators.setter
     def bdf_accelerators(self, table: PcfAccelerators | None):
         self[PcfTableType.BDF_ACCELERATORS] = table
 
-    def dump(self, stream: BinaryIO, compat_mode: bool = False):
+    def dump(self, stream: BinaryIO):
         buffer = Buffer(stream)
 
         headers = []
         table_offset = 4 + 4 + (4 * 4) * len(self)
         for table_type, table in sorted(self.items()):
-            table_size = table.dump(buffer, table_offset, compat_mode)
+            table_size = table.dump(buffer, table_offset)
             headers.append(PcfHeader(table_type, table.table_format, table_size, table_offset))
             table_offset += table_size
 
         PcfHeader.dump(buffer, headers)
 
-    def save(
-            self,
-            file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
-            compat_mode: bool = False,
-    ):
+    def save(self, file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
         with open(file_path, 'wb') as file:
-            self.dump(file, compat_mode)
+            self.dump(file)
```

### Comparing `pcffont-0.0.2/src/pcffont/header.py` & `pcffont-0.0.3/src/pcffont/header.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-from enum import IntEnum, IntFlag
+from enum import IntEnum
 
-from pcffont.error import PcfError
+from pcffont.error import PcfParseError
 from pcffont.internal.buffer import Buffer
 
-_MAGIC_STRING = b'\x01fcp'
+_FILE_VERSION = b'\x01fcp'
 
 
 class PcfTableType(IntEnum):
     PROPERTIES = 1 << 0
     ACCELERATORS = 1 << 1
     METRICS = 1 << 2
     BITMAPS = 1 << 3
     INK_METRICS = 1 << 4
     BDF_ENCODINGS = 1 << 5
     SWIDTHS = 1 << 6
     GLYPH_NAMES = 1 << 7
     BDF_ACCELERATORS = 1 << 8
 
 
-class PcfTableFormat(IntFlag):
-    DEFAULT_FORMAT = 0b_0000_0000_0000
-    INKBOUNDS = 0b_0010_0000_0000
-    ACCEL_W_INKBOUNDS = 0b_0001_0000_0000
-    COMPRESSED_METRICS = 0b_0001_0000_0000
-
-
-class PcfTableFormatMask(IntFlag):
-    GLYPH_PAD = 0b_0000_0011
-    BYTE = 0b_0000_0100
-    BIT = 0b_0000_1000
-    SCAN_UNIT = 0b_0011_0000
-
-
 class PcfHeader:
     @staticmethod
     def parse(buffer: Buffer) -> list['PcfHeader']:
         buffer.seek(0)
-        if buffer.read(4) != _MAGIC_STRING:
-            raise PcfError('Not PCF format')
+        if buffer.read(4) != _FILE_VERSION:
+            raise PcfParseError('Not PCF format')
 
-        tables_count = buffer.read_int32_le()
+        tables_count = buffer.read_int32()
 
         headers = []
         for _ in range(tables_count):
-            table_type = PcfTableType(buffer.read_int32_le())
-            table_format = buffer.read_int32_le()
-            table_size = buffer.read_int32_le()
-            table_offset = buffer.read_int32_le()
+            table_type = PcfTableType(buffer.read_int32())
+            table_format = buffer.read_int32()
+            table_size = buffer.read_int32()
+            table_offset = buffer.read_int32()
             headers.append(PcfHeader(table_type, table_format, table_size, table_offset))
 
         return headers
 
     @staticmethod
     def dump(buffer: Buffer, headers: list['PcfHeader']):
         buffer.seek(0)
-        buffer.write(_MAGIC_STRING)
+        buffer.write(_FILE_VERSION)
 
-        buffer.write_int32_le(len(headers))
+        buffer.write_int32(len(headers))
         for header in headers:
-            buffer.write_int32_le(header.table_type)
-            buffer.write_int32_le(header.table_format)
-            buffer.write_int32_le(header.table_size)
-            buffer.write_int32_le(header.table_offset)
+            buffer.write_int32(header.table_type)
+            buffer.write_int32(header.table_format)
+            buffer.write_int32(header.table_size)
+            buffer.write_int32(header.table_offset)
 
     def __init__(self, table_type: PcfTableType, table_format: int, table_size: int, table_offset: int):
         self.table_type = table_type
         self.table_format = table_format
         self.table_size = table_size
         self.table_offset = table_offset
```

### Comparing `pcffont-0.0.2/src/pcffont/t_accelerators.py` & `pcffont-0.0.3/src/pcffont/t_accelerators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,140 @@
-from pcffont.header import PcfTableFormat, PcfHeader
-from pcffont.internal import util
+from pcffont.format import PcfTableFormat
+from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
 class PcfAccelerators(PcfTable):
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfAccelerators':
-        table_format = util.read_and_check_table_format(buffer, header)
-        byte_order = util.get_table_byte_order(table_format)
-        is_accel_w_ink_bounds = table_format & PcfTableFormat.ACCEL_W_INKBOUNDS > 0
+        table_format = PcfTableFormat.read_and_check(buffer, header)
+        is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
+        has_ink_bounds = PcfTableFormat.has_ink_bounds(table_format)
 
         no_overlap = buffer.read_bool()
         constant_metrics = buffer.read_bool()
         terminal_font = buffer.read_bool()
         constant_width = buffer.read_bool()
         ink_inside = buffer.read_bool()
         ink_metrics = buffer.read_bool()
-        draw_direction_right_to_left = buffer.read_bool()
+        draw_right_to_left = buffer.read_bool()
         buffer.skip(1)
-        font_ascent = buffer.read_int32(byte_order)
-        font_descent = buffer.read_int32(byte_order)
-        max_overlap = buffer.read_int32(byte_order)
-
-        min_bounds = PcfMetric.parse(buffer, byte_order, False)
-        max_bounds = PcfMetric.parse(buffer, byte_order, False)
-
-        if is_accel_w_ink_bounds:
-            ink_min_bounds = PcfMetric.parse(buffer, byte_order, False)
-            ink_max_bounds = PcfMetric.parse(buffer, byte_order, False)
+        font_ascent = buffer.read_int32(is_ms_byte)
+        font_descent = buffer.read_int32(is_ms_byte)
+        max_overlap = buffer.read_int32(is_ms_byte)
+
+        min_bounds = PcfMetric.parse(buffer, is_ms_byte, False)
+        max_bounds = PcfMetric.parse(buffer, is_ms_byte, False)
+
+        if has_ink_bounds:
+            ink_min_bounds = PcfMetric.parse(buffer, is_ms_byte, False)
+            ink_max_bounds = PcfMetric.parse(buffer, is_ms_byte, False)
         else:
             ink_min_bounds = None
             ink_max_bounds = None
 
         # TODO
         if header.table_size > buffer.tell() - header.table_offset:
             buffer.seek(header.table_offset + 4 + 8 + 4 * 3 + 2 * 6 * 2)
             _compat_chunk_start = buffer.tell() - header.table_offset
             _compat_chunk_size = header.table_size - _compat_chunk_start
             _compat_chunk = buffer.read(_compat_chunk_size)
             _compat_info = _compat_chunk_start, _compat_chunk_size, _compat_chunk
         else:
             _compat_info = None
 
-        return PcfAccelerators(
+        accelerators = PcfAccelerators(
             table_format,
             no_overlap,
             constant_metrics,
             terminal_font,
             constant_width,
             ink_inside,
             ink_metrics,
-            draw_direction_right_to_left,
+            draw_right_to_left,
             font_ascent,
             font_descent,
             max_overlap,
             min_bounds,
             max_bounds,
             ink_min_bounds,
             ink_max_bounds,
-            _compat_info,
         )
 
+        # TODO
+        accelerators._compat_info = _compat_info
+
+        return accelerators
+
     def __init__(
             self,
-            table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
+            table_format: int = PcfTableFormat.build(),
             no_overlap: bool = False,
             constant_metrics: bool = False,
             terminal_font: bool = False,
             constant_width: bool = False,
             ink_inside: bool = False,
             ink_metrics: bool = False,
-            draw_direction_right_to_left: bool = False,
+            draw_right_to_left: bool = False,
             font_ascent: int = 0,
             font_descent: int = 0,
             max_overlap: int = 0,
             min_bounds: PcfMetric = None,
             max_bounds: PcfMetric = None,
             ink_min_bounds: PcfMetric = None,
             ink_max_bounds: PcfMetric = None,
-            _compat_info: tuple[int, int, bytes] = None,
     ):
         super().__init__(table_format)
         self.no_overlap = no_overlap
         self.constant_metrics = constant_metrics
         self.terminal_font = terminal_font
         self.constant_width = constant_width
         self.ink_inside = ink_inside
         self.ink_metrics = ink_metrics
-        self.draw_direction_right_to_left = draw_direction_right_to_left
+        self.draw_right_to_left = draw_right_to_left
         self.font_ascent = font_ascent
         self.font_descent = font_descent
         self.max_overlap = max_overlap
         self.min_bounds = min_bounds
         self.max_bounds = max_bounds
         self.ink_min_bounds = ink_min_bounds
         self.ink_max_bounds = ink_max_bounds
-        self._compat_info = _compat_info
+        self._compat_info: tuple[int, int, bytes] | None = None  # TODO
 
-    def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
-        byte_order = util.get_table_byte_order(self.table_format)
-        is_accel_w_ink_bounds = self.table_format & PcfTableFormat.ACCEL_W_INKBOUNDS > 0
+    def _dump(self, buffer: Buffer, table_offset: int) -> int:
+        is_ms_byte = PcfTableFormat.is_ms_byte(self.table_format)
+        has_ink_bounds = PcfTableFormat.has_ink_bounds(self.table_format)
 
         buffer.seek(table_offset)
-        buffer.write_int32_le(self.table_format)
+        buffer.write_int32(self.table_format)
         buffer.write_bool(self.no_overlap)
         buffer.write_bool(self.constant_metrics)
         buffer.write_bool(self.terminal_font)
         buffer.write_bool(self.constant_width)
         buffer.write_bool(self.ink_inside)
         buffer.write_bool(self.ink_metrics)
-        buffer.write_bool(self.draw_direction_right_to_left)
+        buffer.write_bool(self.draw_right_to_left)
         buffer.write_nulls(1)
-        buffer.write_int32(self.font_ascent, byte_order)
-        buffer.write_int32(self.font_descent, byte_order)
-        buffer.write_int32(self.max_overlap, byte_order)
-
-        self.min_bounds.dump(buffer, byte_order, False)
-        self.max_bounds.dump(buffer, byte_order, False)
-
-        if is_accel_w_ink_bounds:
-            self.ink_min_bounds.dump(buffer, byte_order, False)
-            self.ink_max_bounds.dump(buffer, byte_order, False)
+        buffer.write_int32(self.font_ascent, is_ms_byte)
+        buffer.write_int32(self.font_descent, is_ms_byte)
+        buffer.write_int32(self.max_overlap, is_ms_byte)
+
+        self.min_bounds.dump(buffer, is_ms_byte, False)
+        self.max_bounds.dump(buffer, is_ms_byte, False)
+
+        if has_ink_bounds:
+            self.ink_min_bounds.dump(buffer, is_ms_byte, False)
+            self.ink_max_bounds.dump(buffer, is_ms_byte, False)
 
         table_size = buffer.tell() - table_offset
 
         # TODO
-        if compat_mode and self._compat_info is not None:
+        if self._compat_info is not None:
             _compat_chunk_start, _compat_chunk_size, _compat_chunk = self._compat_info
             _compat_chunk = bytearray(_compat_chunk)
 
             ink_chunk_size = 2 * 6 * 2
             if table_size == _compat_chunk_start + ink_chunk_size:
                 _compat_chunk_start += ink_chunk_size
                 _compat_chunk_size -= ink_chunk_size
```

### Comparing `pcffont-0.0.2/src/pcffont/t_bitmaps.py` & `pcffont-0.0.3/src/pcffont/t_bitmaps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,38 @@
 from collections import UserList
 
 from pcffont.error import PcfError
+from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
-from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 
-def _get_bit_aligned_bitmap(bitmap: list[list[int]], n: int) -> list[list[int]]:
-    new_bitmap = []
-    for bitmap_row in bitmap:
-        new_bitmap_row = []
-        for i in range(n):
-            if i < len(bitmap_row):
-                new_bitmap_row.append(bitmap_row[i])
-            else:
-                new_bitmap_row.append(0)
-        new_bitmap.append(new_bitmap_row)
-    return new_bitmap
-
-
 class PcfBitmaps(PcfTable, UserList[list[list[int]]]):
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBitmaps':
-        table_format = util.read_and_check_table_format(buffer, header)
-        byte_order = util.get_table_byte_order(table_format)
-
-        # How each row in each glyph's bitmap is padded
-        # 0 => byte, 1 => short, 2 => int32, 3 => int64
-        bitmap_padded_mode = table_format & 3
-        bitmap_row_size = [1, 2, 4, 8][bitmap_padded_mode]
-
-        # What the bits are stored
-        # 0 => byte, 1 => short, 2 => int32
-        bits_stored_mode = (table_format >> 4) & 3
-        if bits_stored_mode != 0:
+        table_format = PcfTableFormat.read_and_check(buffer, header)
+        is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
+        is_ms_bit = PcfTableFormat.is_ms_bit(table_format)
+
+        bitmap_pad_mode = PcfTableFormat.bitmap_pad_mode(table_format)
+        bitmap_row_size = [1, 2, 4, 8][bitmap_pad_mode]
+
+        # FIXME
+        bit_scan_mode = PcfTableFormat.bit_scan_mode(table_format)
+        if bit_scan_mode != 0:
             raise PcfError(f'Table format not supported: {table_format:b}')
 
-        glyphs_count = buffer.read_int32(byte_order)
-        bitmap_offsets = [buffer.read_int32(byte_order) for _ in range(glyphs_count)]
-        size_configs = [buffer.read_int32(byte_order) for _ in range(4)]
+        glyphs_count = buffer.read_int32(is_ms_byte)
+        bitmap_offsets = [buffer.read_int32(is_ms_byte) for _ in range(glyphs_count)]
+        size_configs = [buffer.read_int32(is_ms_byte) for _ in range(4)]
         bitmaps_start = buffer.tell()
-        bitmaps_size = size_configs[bitmap_padded_mode]
+        bitmaps_size = size_configs[bitmap_pad_mode]
 
-        bitmaps = []
+        bitmaps = PcfBitmaps(table_format)
         for i in range(glyphs_count):
             bitmap_offset = bitmap_offsets[i]
             if i < glyphs_count - 1:
                 bitmap_offset_next = bitmap_offsets[i + 1]
             else:
                 bitmap_offset_next = bitmaps_size
             bitmap_size = bitmap_offset_next - bitmap_offset
@@ -55,81 +40,82 @@
             bitmap = []
             buffer.seek(bitmaps_start + bitmap_offset)
             for _ in range(bitmap_size // bitmap_row_size):
                 bitmap_row = []
                 for _ in range(bitmap_row_size):
                     data = buffer.read(1)
                     array = [int(c) for c in f'{ord(data):08b}']
-                    if byte_order == 'little':
+                    if not is_ms_bit:
                         array.reverse()
                     bitmap_row.extend(array)
                 bitmap.append(bitmap_row)
             bitmaps.append(bitmap)
 
-        return PcfBitmaps(table_format, bitmaps, size_configs)
+        # TODO
+        bitmaps._compat_size_configs = size_configs
+
+        return bitmaps
 
     def __init__(
             self,
-            table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
+            table_format: int = PcfTableFormat.build(),
             bitmaps: list[list[list[int]]] = None,
-            _compat_size_configs: list[int] = None,
     ):
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, bitmaps)
-        self._compat_size_configs = _compat_size_configs
-
-    def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
-        byte_order = util.get_table_byte_order(self.table_format)
+        self._compat_size_configs: list[int] | None = None  # TODO
 
-        # How each row in each glyph's bitmap is padded
-        # 0 => byte, 1 => short, 2 => int32, 3 => int64
-        bitmap_padded_mode = self.table_format & 3
-        bitmap_row_size = [1, 2, 4, 8][bitmap_padded_mode]
-
-        # What the bits are stored
-        # 0 => byte, 1 => short, 2 => int32
-        bits_stored_mode = (self.table_format >> 4) & 3
-        if bits_stored_mode != 0:
+    def _dump(self, buffer: Buffer, table_offset: int) -> int:
+        is_ms_byte = PcfTableFormat.is_ms_byte(self.table_format)
+        is_ms_bit = PcfTableFormat.is_ms_byte(self.table_format)
+
+        bitmap_pad_mode = PcfTableFormat.bitmap_pad_mode(self.table_format)
+        bitmap_row_size = [1, 2, 4, 8][bitmap_pad_mode]
+
+        # FIXME
+        bit_scan_mode = PcfTableFormat.bit_scan_mode(self.table_format)
+        if bit_scan_mode != 0:
             raise PcfError(f'Table format not supported: {self.table_format:b}')
 
         glyphs_count = len(self)
 
         bitmaps_start = table_offset + 4 + 4 + 4 * glyphs_count + 4 * 4
         bitmaps_size = 0
         bitmap_offsets = []
         buffer.seek(bitmaps_start)
         for bitmap in self:
             bitmap_offsets.append(bitmaps_size)
-            bitmap = _get_bit_aligned_bitmap(bitmap, 8 * bitmap_row_size)
             for bitmap_row in bitmap:
+                if len(bitmap_row) < 8 * bitmap_row_size:
+                    bitmap_row = bitmap_row + [0] * (8 * bitmap_row_size - len(bitmap_row))
                 for i in range(len(bitmap_row) // 8):
                     array = bitmap_row[i * 8:(i + 1) * 8]
-                    if byte_order == 'little':
+                    if not is_ms_bit:
                         array.reverse()
                     bin_string = ''.join(map(str, array))
                     data = int(bin_string, 2).to_bytes(1, 'big')
                     bitmaps_size += buffer.write(data)
 
         # TODO
-        if compat_mode and self._compat_size_configs is not None:
+        if self._compat_size_configs is not None:
             size_configs = list(self._compat_size_configs)
-            size_configs[bitmap_padded_mode] = bitmaps_size
+            size_configs[bitmap_pad_mode] = bitmaps_size
         else:
             unit_size_config = bitmaps_size // bitmap_row_size
             size_configs = [
                 unit_size_config,
                 unit_size_config * 2,
                 unit_size_config * 4,
                 unit_size_config * 8,
             ]
 
         buffer.seek(table_offset)
-        buffer.write_int32_le(self.table_format)
-        buffer.write_int32(glyphs_count, byte_order)
+        buffer.write_int32(self.table_format)
+        buffer.write_int32(glyphs_count, is_ms_byte)
         for offset in bitmap_offsets:
-            buffer.write_int32(offset, byte_order)
+            buffer.write_int32(offset, is_ms_byte)
         for size_config in size_configs:
-            buffer.write_int32(size_config, byte_order)
+            buffer.write_int32(size_config, is_ms_byte)
         buffer.skip(bitmaps_size)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.2/src/pcffont/t_encodings.py` & `pcffont-0.0.3/src/pcffont/t_encodings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,106 @@
 from collections import UserDict
 
-from pcffont.error import PcfError
+from pcffont.error import PcfOutOfRangeError
+from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
-from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
+_MAX_CODE_POINT = 0xFFFF
 _NO_GLYPH_INDEX = 0xFFFF
 
 
 class PcfBdfEncodings(PcfTable, UserDict[int, int]):
     """
     code_point -> glyph_index
     """
 
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBdfEncodings':
-        table_format = util.read_and_check_table_format(buffer, header)
-        byte_order = util.get_table_byte_order(table_format)
+        table_format = PcfTableFormat.read_and_check(buffer, header)
+        is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
 
-        min_char_or_byte2 = buffer.read_int16(byte_order)
-        max_char_or_byte2 = buffer.read_int16(byte_order)
-        min_byte1 = buffer.read_int16(byte_order)
-        max_byte1 = buffer.read_int16(byte_order)
-        default_char = buffer.read_int16(byte_order)
-
-        glyph_indices_count = (max_char_or_byte2 - min_char_or_byte2 + 1) * (max_byte1 - min_byte1 + 1)
-        glyph_indices = [buffer.read_int16(byte_order) for _ in range(glyph_indices_count)]
-
-        mapping = {}
-        if min_byte1 == max_byte1 == 0:
-            for code_point in range(min_char_or_byte2, max_char_or_byte2 + 1):
-                glyph_index = glyph_indices[code_point - min_char_or_byte2]
-                mapping[code_point] = glyph_index
+        min_byte_2 = buffer.read_int16(is_ms_byte)
+        max_byte_2 = buffer.read_int16(is_ms_byte)
+        min_byte_1 = buffer.read_int16(is_ms_byte)
+        max_byte_1 = buffer.read_int16(is_ms_byte)
+        default_char = buffer.read_int16(is_ms_byte)
+
+        glyphs_count = (max_byte_2 - min_byte_2 + 1) * (max_byte_1 - min_byte_1 + 1)
+        glyph_indices = [buffer.read_int16(is_ms_byte) for _ in range(glyphs_count)]
+
+        encodings = PcfBdfEncodings(table_format, default_char)
+        if min_byte_1 == max_byte_1 == 0:
+            for code_point in range(min_byte_2, max_byte_2 + 1):
+                glyph_index = glyph_indices[code_point - min_byte_2]
+                encodings[code_point] = glyph_index
         else:
-            for enc1 in range(min_byte1, max_byte1 + 1):
-                for enc2 in range(min_char_or_byte2, max_char_or_byte2 + 1):
-                    code_point = int.from_bytes(bytes([enc1, enc2]))
-                    glyph_index = glyph_indices[(enc1 - min_byte1) * (max_char_or_byte2 - min_char_or_byte2 + 1) + enc2 - min_char_or_byte2]
-                    mapping[code_point] = glyph_index
-
-        return PcfBdfEncodings(table_format, mapping, default_char)
+            for byte_1 in range(min_byte_1, max_byte_1 + 1):
+                for byte_2 in range(min_byte_2, max_byte_2 + 1):
+                    code_point = int.from_bytes(bytes([byte_1, byte_2]))
+                    glyph_index = glyph_indices[(byte_1 - min_byte_1) * (max_byte_2 - min_byte_2 + 1) + byte_2 - min_byte_2]
+                    encodings[code_point] = glyph_index
+        return encodings
 
     def __init__(
             self,
-            table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
-            mapping: dict[int, int] = None,
+            table_format: int = PcfTableFormat.build(),
             default_char: int = _NO_GLYPH_INDEX,
+            encodings: dict[int, int] = None,
     ):
         PcfTable.__init__(self, table_format)
-        UserDict.__init__(self, mapping)
+        UserDict.__init__(self, encodings)
         self.default_char = default_char
 
     def __setitem__(self, code_point: int, glyph_index: int | None):
-        if code_point < 0 or code_point > 0xFFFF:
-            raise PcfError(f'Code point must between [0, 0xFFFF]')
+        if code_point < 0 or code_point > _MAX_CODE_POINT:
+            raise PcfOutOfRangeError(f'Code point must between [0, {_MAX_CODE_POINT}]')
         if glyph_index < 0 or glyph_index > _NO_GLYPH_INDEX:
-            raise PcfError(f'Glyph index must between [0, 0x{_NO_GLYPH_INDEX:04X}]')
-
-        if glyph_index == _NO_GLYPH_INDEX:
-            glyph_index = None
+            raise PcfOutOfRangeError(f'Glyph index must between [0, {_NO_GLYPH_INDEX}]')
 
-        if glyph_index is None:
+        if glyph_index is None or glyph_index == _NO_GLYPH_INDEX:
             self.pop(code_point, None)
         else:
             super().__setitem__(code_point, glyph_index)
 
-    def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
-        byte_order = util.get_table_byte_order(self.table_format)
+    def _dump(self, buffer: Buffer, table_offset: int) -> int:
+        is_ms_byte = PcfTableFormat.is_ms_byte(self.table_format)
 
-        max_code_point = max(self)
-        if max_code_point <= 0xFF:
-            min_char_or_byte2 = min(self)
-            max_char_or_byte2 = max_code_point
-            min_byte1 = 0
-            max_byte1 = 0
-        else:
-            min_char_or_byte2 = 0
-            max_char_or_byte2 = 0xFF
-            min_byte1 = 0
-            max_byte1 = 0xFF
+        min_byte_2 = 0xFF
+        max_byte_2 = 0
+        min_byte_1 = 0xFF
+        max_byte_1 = 0
+        for code_point in self:
+            bs = code_point.to_bytes(2)
+            byte_1 = bs[0]
+            byte_2 = bs[1]
+            if byte_1 < min_byte_1:
+                min_byte_1 = byte_1
+            if byte_1 > max_byte_1:
+                max_byte_1 = byte_1
+            if byte_2 < min_byte_2:
+                min_byte_2 = byte_2
+            if byte_2 > max_byte_2:
+                max_byte_2 = byte_2
 
         buffer.seek(table_offset)
-        buffer.write_int32_le(self.table_format)
-        buffer.write_int16(min_char_or_byte2, byte_order)
-        buffer.write_int16(max_char_or_byte2, byte_order)
-        buffer.write_int16(min_byte1, byte_order)
-        buffer.write_int16(max_byte1, byte_order)
-        buffer.write_int16(self.default_char, byte_order)
+        buffer.write_int32(self.table_format)
+        buffer.write_int16(min_byte_2, is_ms_byte)
+        buffer.write_int16(max_byte_2, is_ms_byte)
+        buffer.write_int16(min_byte_1, is_ms_byte)
+        buffer.write_int16(max_byte_1, is_ms_byte)
+        buffer.write_int16(self.default_char, is_ms_byte)
 
-        if min_byte1 == max_byte1 == 0:
-            for code_point in range(min_char_or_byte2, max_char_or_byte2 + 1):
+        if min_byte_1 == max_byte_1 == 0:
+            for code_point in range(min_byte_2, max_byte_2 + 1):
                 glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                buffer.write_int16(glyph_index, byte_order)
+                buffer.write_int16(glyph_index, is_ms_byte)
         else:
-            for enc1 in range(min_byte1, max_byte1 + 1):
-                for enc2 in range(min_char_or_byte2, max_char_or_byte2 + 1):
-                    code_point = int.from_bytes(bytes([enc1, enc2]))
+            for byte_1 in range(min_byte_1, max_byte_1 + 1):
+                for byte_2 in range(min_byte_2, max_byte_2 + 1):
+                    code_point = int.from_bytes(bytes([byte_1, byte_2]))
                     glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                    buffer.write_int16(glyph_index, byte_order)
+                    buffer.write_int16(glyph_index, is_ms_byte)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.2/src/pcffont/t_properties.py` & `pcffont-0.0.3/src/pcffont/t_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from collections import UserDict
 
 from pcffont.error import PcfError, PcfPropKeyError, PcfPropValueError, PcfXlfdError
+from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
-from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 _KEY_FOUNDRY = 'FOUNDRY'
 _KEY_FAMILY_NAME = 'FAMILY_NAME'
 _KEY_WEIGHT_NAME = 'WEIGHT_NAME'
 _KEY_SLANT = 'SLANT'
@@ -106,56 +106,52 @@
         if matched is not None:
             raise PcfPropValueError(key, value, f"contains illegal characters '{matched.group()}'")
 
 
 class PcfProperties(PcfTable, UserDict[str, str | int]):
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, strict_level: int) -> 'PcfProperties':
-        table_format = util.read_and_check_table_format(buffer, header)
-        byte_order = util.get_table_byte_order(table_format)
+        table_format = PcfTableFormat.read_and_check(buffer, header)
+        is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
 
-        props_count = buffer.read_int32(byte_order)
+        props_count = buffer.read_int32(is_ms_byte)
 
         prop_infos = []
         for _ in range(props_count):
-            key_offset = buffer.read_int32(byte_order)
+            key_offset = buffer.read_int32(is_ms_byte)
             is_string_prop = buffer.read_bool()
-            value = buffer.read_int32(byte_order)
+            value = buffer.read_int32(is_ms_byte)
             prop_infos.append((key_offset, is_string_prop, value))
 
         # Pad to next int32 boundary
-        padding = 0 if (props_count & 3) == 0 else 4 - (props_count & 3)
+        padding = 3 - (((4 + 1 + 4) * props_count + 3) % 4)
         buffer.skip(padding)
 
         buffer.skip_int()  # strings_size
         strings_start = buffer.tell()
 
-        properties = {}
+        properties = PcfProperties(table_format)
         for key_offset, is_string_prop, value in prop_infos:
             buffer.seek(strings_start + key_offset)
             key = buffer.read_string()
             if is_string_prop:
                 buffer.seek(strings_start + value)
                 value = buffer.read_string()
             else:
                 value = int(value)
-
             try:
-                _check_key(key)
-                _check_value(key, value)
                 properties[key] = value
             except (PcfPropKeyError, PcfPropValueError) as e:
                 if strict_level >= 1:
                     raise e
-
-        return PcfProperties(table_format, properties)
+        return properties
 
     def __init__(
             self,
-            table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
+            table_format: int = PcfTableFormat.build(),
             properties: dict[str, str | int] = None,
     ):
         PcfTable.__init__(self, table_format)
         UserDict.__init__(self, properties)
 
     def __getitem__(self, key: str) -> str | int:
         key = key.upper()
@@ -352,44 +348,44 @@
             else:
                 if key in _XLFD_FONT_NAME_STR_VALUE_KEYS:
                     value = token
                 else:
                     value = int(token)
             self[key] = value
 
-    def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
-        byte_order = util.get_table_byte_order(self.table_format)
+    def _dump(self, buffer: Buffer, table_offset: int) -> int:
+        is_ms_byte = PcfTableFormat.is_ms_byte(self.table_format)
 
         props_count = len(self)
 
         # Pad to next int32 boundary
-        padding = 0 if (props_count & 3) == 0 else 4 - (props_count & 3)
+        padding = 3 - (((4 + 1 + 4) * props_count + 3) % 4)
 
         strings_start = table_offset + 4 + 4 + (4 + 1 + 4) * props_count + padding + 4
         strings_size = 0
         prop_infos = []
         buffer.seek(strings_start)
         for key, value in self.items():
             key_offset = strings_size
             strings_size += buffer.write_string(key)
             value_offset = strings_size
             if isinstance(value, str):
                 strings_size += buffer.write_string(value)
             prop_infos.append((key, key_offset, value, value_offset))
 
         buffer.seek(table_offset)
-        buffer.write_int32_le(self.table_format)
-        buffer.write_int32(props_count, byte_order)
+        buffer.write_int32(self.table_format)
+        buffer.write_int32(props_count, is_ms_byte)
         for key, key_offset, value, value_offset in prop_infos:
-            buffer.write_int32(key_offset, byte_order)
+            buffer.write_int32(key_offset, is_ms_byte)
             if isinstance(value, str):
                 buffer.write_bool(True)
-                buffer.write_int32(value_offset, byte_order)
+                buffer.write_int32(value_offset, is_ms_byte)
             else:
                 buffer.write_bool(False)
-                buffer.write_int32(value, byte_order)
+                buffer.write_int32(value, is_ms_byte)
         buffer.write_nulls(padding)
-        buffer.write_int32(strings_size, byte_order)
+        buffer.write_int32(strings_size, is_ms_byte)
         buffer.skip(strings_size)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.2/src/pcffont/table.py` & `pcffont-0.0.3/src/pcffont/table.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from abc import abstractmethod
 
 from pcffont.internal.buffer import Buffer
 
 
 class PcfTable:
-    DEFAULT_TABLE_FORMAT = 0b_1110
-    DEFAULT_TABLE_FORMAT_2 = 0b_0010
-
     def __init__(self, table_format: int):
         self.table_format = table_format
 
     def __repr__(self) -> str:
         return object.__repr__(self)
 
     @abstractmethod
-    def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
+    def _dump(self, buffer: Buffer, table_offset: int) -> int:
         raise NotImplementedError
 
-    def dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
-        table_size = self._dump(buffer, table_offset, compat_mode)
+    def dump(self, buffer: Buffer, table_offset: int) -> int:
+        table_size = self._dump(buffer, table_offset)
 
         # All tables begin on a 32bit boundary (and will be padded with zeroes).
         padding = 4 - table_size % 4
         if padding != 4:
             buffer.seek(table_offset + table_size)
             table_size += buffer.write_nulls(padding)
```

### Comparing `pcffont-0.0.2/tests/test_dump.py` & `pcffont-0.0.3/tests/test_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,16 @@
         headers_data_size = 4 + 4 + (4 * 4) * len(headers)
         headers_data_in = buffer_in.read(headers_data_size)
         headers_data_out = buffer_out.read(headers_data_size)
         assert _sha256(headers_data_in) == _sha256(headers_data_out)
 
         for header in headers:
             table = util.parse_table(buffer_in, header)
-            if table is None:
-                continue
             table_offset = header.table_offset
-            table_size = table.dump(buffer_out, table_offset, compat_mode=True)
+            table_size = table.dump(buffer_out, table_offset)
             assert table_size == header.table_size
             buffer_in.seek(table_offset)
             buffer_out.seek(table_offset)
             table_data_in = buffer_in.read(table_size)
             table_data_out = buffer_out.read(table_size)
             assert _sha256(table_data_in) == _sha256(table_data_out)
```

### Comparing `pcffont-0.0.2/tests/test_load_save.py` & `pcffont-0.0.3/tests/test_load_save.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,65 +12,65 @@
         return hashlib.sha256(file.read()).hexdigest()
 
 
 def test_unifont(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'unifont', 'unifont-15.1.05.pcf')
     save_file_path = os.path.join(tmp_path, 'unifont-15.1.05.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_dweep(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'dweep', 'dweep.pcf')
     save_file_path = os.path.join(tmp_path, 'dweep.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_rock36(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'sgi', 'rock36.pcf')
     save_file_path = os.path.join(tmp_path, 'rock36.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_raize(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'raize', 'raize-normal-19.pcf')
     save_file_path = os.path.join(tmp_path, 'raize-normal-19.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_anorexia(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'artwiz', 'anorexia.pcf')
     save_file_path = os.path.join(tmp_path, 'anorexia.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_kates(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'artwiz', 'kates.pcf')
     save_file_path = os.path.join(tmp_path, 'kates.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_trisk(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'trisk', 'trisk.pcf')
     save_file_path = os.path.join(tmp_path, 'trisk.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
 
 
 def test_profont(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'profont-x11', 'ProFont_r400-29.pcf')
     save_file_path = os.path.join(tmp_path, 'ProFont_r400-29.pcf')
     font = PcfFont.load(load_file_path)
-    font.save(save_file_path, compat_mode=True)
+    font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
```

### Comparing `pcffont-0.0.2/tests/test_reload.py` & `pcffont-0.0.3/tests/test_reload.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 
 project_root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 
 
 def test_reload(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'unifont', 'unifont-15.1.05.pcf')
     save_file_path = os.path.join(tmp_path, 'unifont-15.1.05.pcf')
+    font = PcfFont.load(load_file_path)
+    font.accelerators._compat_info = None
+    font.bdf_accelerators._compat_info = None
+    font.bitmaps._compat_size_configs = None
+    font.save(save_file_path)
+
     font_1 = PcfFont.load(load_file_path)
-    font_1.save(save_file_path)
     font_2 = PcfFont.load(save_file_path)
 
     assert len(font_1) == len(font_2)
     for table_type, table_1 in font_1.items():
         table_2 = font_2[table_type]
         assert table_1.table_format == table_2.table_format
 
@@ -25,43 +30,43 @@
 
     assert font_1.accelerators.no_overlap == font_2.accelerators.no_overlap
     assert font_1.accelerators.constant_metrics == font_2.accelerators.constant_metrics
     assert font_1.accelerators.terminal_font == font_2.accelerators.terminal_font
     assert font_1.accelerators.constant_width == font_2.accelerators.constant_width
     assert font_1.accelerators.ink_inside == font_2.accelerators.ink_inside
     assert font_1.accelerators.ink_metrics == font_2.accelerators.ink_metrics
-    assert font_1.accelerators.draw_direction_right_to_left == font_2.accelerators.draw_direction_right_to_left
+    assert font_1.accelerators.draw_right_to_left == font_2.accelerators.draw_right_to_left
     assert font_1.accelerators.font_ascent == font_2.accelerators.font_ascent
     assert font_1.accelerators.font_descent == font_2.accelerators.font_descent
     assert font_1.accelerators.max_overlap == font_2.accelerators.max_overlap
 
-    assert font_1.accelerators.min_bounds.left_sided_bearing == font_2.accelerators.min_bounds.left_sided_bearing
+    assert font_1.accelerators.min_bounds.left_side_bearing == font_2.accelerators.min_bounds.left_side_bearing
     assert font_1.accelerators.min_bounds.right_side_bearing == font_2.accelerators.min_bounds.right_side_bearing
     assert font_1.accelerators.min_bounds.character_width == font_2.accelerators.min_bounds.character_width
-    assert font_1.accelerators.min_bounds.character_ascent == font_2.accelerators.min_bounds.character_ascent
-    assert font_1.accelerators.min_bounds.character_descent == font_2.accelerators.min_bounds.character_descent
-    assert font_1.accelerators.min_bounds.character_attributes == font_2.accelerators.min_bounds.character_attributes == 0
+    assert font_1.accelerators.min_bounds.ascent == font_2.accelerators.min_bounds.ascent
+    assert font_1.accelerators.min_bounds.descent == font_2.accelerators.min_bounds.descent
+    assert font_1.accelerators.min_bounds.attributes == font_2.accelerators.min_bounds.attributes == 0
 
     assert font_1.accelerators.ink_min_bounds is None
     assert font_1.accelerators.ink_max_bounds is None
     assert font_2.accelerators.ink_min_bounds is None
     assert font_2.accelerators.ink_max_bounds is None
 
     assert font_1.accelerators._compat_info is not None
     assert font_2.accelerators._compat_info is None
 
     assert len(font_1.metrics) == len(font_2.metrics)
     for glyph_index, metric_1 in enumerate(font_1.metrics):
         metric_2 = font_2.metrics[glyph_index]
-        assert metric_1.left_sided_bearing == metric_2.left_sided_bearing
+        assert metric_1.left_side_bearing == metric_2.left_side_bearing
         assert metric_1.right_side_bearing == metric_2.right_side_bearing
         assert metric_1.character_width == metric_2.character_width
-        assert metric_1.character_ascent == metric_2.character_ascent
-        assert metric_1.character_descent == metric_2.character_descent
-        assert metric_1.character_attributes == metric_2.character_attributes
+        assert metric_1.ascent == metric_2.ascent
+        assert metric_1.descent == metric_2.descent
+        assert metric_1.attributes == metric_2.attributes
 
     assert len(font_1.bitmaps) == len(font_2.bitmaps)
     for glyph_index, bitmap_1 in enumerate(font_1.bitmaps):
         bitmap_2 = font_2.bitmaps[glyph_index]
         assert len(bitmap_1) == len(bitmap_2)
         for i, bitmap_row_1 in enumerate(bitmap_1):
             bitmap_row_2 = bitmap_2[i]
@@ -91,25 +96,25 @@
 
     assert font_1.bdf_accelerators.no_overlap == font_2.bdf_accelerators.no_overlap
     assert font_1.bdf_accelerators.constant_metrics == font_2.bdf_accelerators.constant_metrics
     assert font_1.bdf_accelerators.terminal_font == font_2.bdf_accelerators.terminal_font
     assert font_1.bdf_accelerators.constant_width == font_2.bdf_accelerators.constant_width
     assert font_1.bdf_accelerators.ink_inside == font_2.bdf_accelerators.ink_inside
     assert font_1.bdf_accelerators.ink_metrics == font_2.bdf_accelerators.ink_metrics
-    assert font_1.bdf_accelerators.draw_direction_right_to_left == font_2.bdf_accelerators.draw_direction_right_to_left
+    assert font_1.bdf_accelerators.draw_right_to_left == font_2.bdf_accelerators.draw_right_to_left
     assert font_1.bdf_accelerators.font_ascent == font_2.bdf_accelerators.font_ascent
     assert font_1.bdf_accelerators.font_descent == font_2.bdf_accelerators.font_descent
     assert font_1.bdf_accelerators.max_overlap == font_2.bdf_accelerators.max_overlap
 
-    assert font_1.bdf_accelerators.min_bounds.left_sided_bearing == font_2.bdf_accelerators.min_bounds.left_sided_bearing
+    assert font_1.bdf_accelerators.min_bounds.left_side_bearing == font_2.bdf_accelerators.min_bounds.left_side_bearing
     assert font_1.bdf_accelerators.min_bounds.right_side_bearing == font_2.bdf_accelerators.min_bounds.right_side_bearing
     assert font_1.bdf_accelerators.min_bounds.character_width == font_2.bdf_accelerators.min_bounds.character_width
-    assert font_1.bdf_accelerators.min_bounds.character_ascent == font_2.bdf_accelerators.min_bounds.character_ascent
-    assert font_1.bdf_accelerators.min_bounds.character_descent == font_2.bdf_accelerators.min_bounds.character_descent
-    assert font_1.bdf_accelerators.min_bounds.character_attributes == font_2.bdf_accelerators.min_bounds.character_attributes == 0
+    assert font_1.bdf_accelerators.min_bounds.ascent == font_2.bdf_accelerators.min_bounds.ascent
+    assert font_1.bdf_accelerators.min_bounds.descent == font_2.bdf_accelerators.min_bounds.descent
+    assert font_1.bdf_accelerators.min_bounds.attributes == font_2.bdf_accelerators.min_bounds.attributes == 0
 
     assert font_1.bdf_accelerators.ink_min_bounds is None
     assert font_1.bdf_accelerators.ink_max_bounds is None
     assert font_2.bdf_accelerators.ink_min_bounds is None
     assert font_2.bdf_accelerators.ink_max_bounds is None
 
     assert font_1.bdf_accelerators._compat_info is not None
```

### Comparing `pcffont-0.0.2/.gitignore` & `pcffont-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/LICENSE` & `pcffont-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.2/pyproject.toml` & `pcffont-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

