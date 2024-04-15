# Comparing `tmp/archerdfu_bmp-1.0.2.tar.gz` & `tmp/archerdfu_bmp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archerdfu_bmp-1.0.2.tar", last modified: Sun Apr 14 18:50:50 2024, max compression
+gzip compressed data, was "archerdfu_bmp-1.0.3.tar", last modified: Mon Apr 15 18:44:03 2024, max compression
```

## Comparing `archerdfu_bmp-1.0.2.tar` & `archerdfu_bmp-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.931304 archerdfu_bmp-1.0.2/archerdfu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/archerdfu/bmp/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/archerdfu/bmp/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/__pyinstaller/hook-archerdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/caliber_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/archerdfu/bmp/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/fonts/default.flf
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/fonts/pixel.flf
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/archerdfu/bmp/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 18:50:50.000000 archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:50:50.935304 archerdfu_bmp-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-14 18:50:45.000000 archerdfu_bmp-1.0.2/tests/test_caliber_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.714989 archerdfu_bmp-1.0.3/archerdfu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/archerdfu/bmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/archerdfu/bmp/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/__pyinstaller/hook-archerdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/caliber_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/archerdfu/bmp/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/fonts/default.flf
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/fonts/pixel.flf
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/gui_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/archerdfu/bmp/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 18:44:03.000000 archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:03.718989 archerdfu_bmp-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/tests/test_caliber_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 18:43:57.000000 archerdfu_bmp-1.0.3/tests/test_gui_fonts.py
```

### Comparing `archerdfu_bmp-1.0.2/LICENSE` & `archerdfu_bmp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.2/PKG-INFO` & `archerdfu_bmp-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.bmp
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `archerdfu_bmp-1.0.2/archerdfu/bmp/__main__.py` & `archerdfu_bmp-1.0.3/archerdfu/bmp/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import argparse
 from pathlib import Path
 from importlib import metadata
 
 from archerdfu.bmp import CaliberIcon, matrix_to_bmp
 
-__version__ = metadata.version("archerdfu.bmp")
+try:
+    __version__ = metadata.version("archerdfu.bmp")
+except metadata.PackageNotFoundError:
+    __version__ = 'Unknown'
 
 
 def get_argparser():
     parser = argparse.ArgumentParser(
         prog='archerdfu bmp processor',
         epilog='Text at the bottom of help',
         conflict_handler='resolve',
@@ -64,10 +67,10 @@
 
 
 if __name__ == "__main__":
     COMMANDLINE_PARSER = get_argparser()
 
     try:
         COMMANDLINE_ARGS, UNKNOWN = COMMANDLINE_PARSER.parse_known_args()
+        main(COMMANDLINE_ARGS)
     except Exception as exc:
         COMMANDLINE_PARSER.parse_known_args(('-h',))
-    main(COMMANDLINE_ARGS)
```

### Comparing `archerdfu_bmp-1.0.2/archerdfu/bmp/caliber_icons.py` & `archerdfu_bmp-1.0.3/archerdfu/bmp/caliber_icons.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,21 +74,24 @@
         w_pad_pxl = [cls.WHITE_ROW] * w_height_pad
 
         caliber_pxl = cal_pad_pxl + cls.make_line(caliber_txt) + cal_pad_pxl
 
         weight_pxl = w_pad_pxl + cls.make_line(weight_txt) + w_pad_pxl
         delimiter_pxl = [cls.BLACK_ROW] * 2
 
-        pixels = caliber_pxl + delimiter_pxl + weight_pxl
-        return pixels
+        matrix = caliber_pxl + delimiter_pxl + weight_pxl
+        matrix.reverse()
+        return matrix
 
     @classmethod
     def matrix_to_icon(cls, matrix: list):
+        _matrix = matrix.copy()
+        _matrix.reverse()
         output = b''
-        for row in matrix:
+        for row in _matrix:
             line = b''.join([b'\x00' if p == cls.WHITE else b'\xC0' for p in row])
             output += line * 2
         return output
 
     @staticmethod
     def concat_icons(icons: [bytes, bytearray]):
         return b''.join(icons)
```

### Comparing `archerdfu_bmp-1.0.2/archerdfu/bmp/fonts/default.flf` & `archerdfu_bmp-1.0.3/archerdfu/bmp/fonts/default.flf`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.2/archerdfu/bmp/fonts/pixel.flf` & `archerdfu_bmp-1.0.3/archerdfu/bmp/fonts/pixel.flf`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.2/archerdfu.bmp.egg-info/PKG-INFO` & `archerdfu_bmp-1.0.3/archerdfu.bmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.bmp
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `archerdfu_bmp-1.0.2/pyproject.toml` & `archerdfu_bmp-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "archerdfu.bmp"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name="o-murphy" },
 ]
 
 description = "PyDfuUtil binds for archerdfu library"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `archerdfu_bmp-1.0.2/tests/test_caliber_icons.py` & `archerdfu_bmp-1.0.3/tests/test_caliber_icons.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,40 @@
         matrix = bmp_to_matrix("../assets/icon.bmp")
         binicon = c.matrix_to_icon(matrix)
         with open("../assets/icon.bin", 'wb') as fp:
             fp.write(binicon)
 
         self.assertEqual(len(binicon), 2048)
 
+        with open('../assets/icon.bin', 'rb') as fp0:
+            with open('../assets/icon1.bin', 'rb') as fp1:
+                self.assertEqual(fp0.read(), fp1.read())
+
     def test_concat_icons(self):
         c = CaliberIcon()
         icons = (
             c.create_icon("308WIN", 175),
             c.create_icon("338LM", 300),
         )
         binicons = c.concat_icons(icons)
         with open("../assets/icons.bin", 'wb') as fp:
             fp.write(binicons)
 
         self.assertEqual(len(binicons), 4096)
 
+    def test_create_icon(self):
+        matrix = CaliberIcon.create_icon_matrix('338LM', 300)
+        matrix_to_bmp(matrix, "../assets/338LM-300gr.bmp")
+
     def test_other_size_conversion(self):
         matrix = bmp_to_matrix("../assets/640x480.bmp")
         self.assertEqual(len(matrix[0]), 640)
         self.assertEqual(len(matrix), 480)
 
         matrix_to_bmp(matrix, "../assets/640x480_24.bmp", 24)
         matrix_to_bmp(matrix, "../assets/640x480_32.bmp", 32)
 
     def test_icon_load(self):
-        matrix = bmp_to_matrix("../assets/16x16.bmp")
+        matrix = bmp_to_matrix("../assets/16.bmp")
         matrix_to_bmp(matrix, "../assets/icons.bmp", 24)
         self.assertEqual(len(matrix[0]), 16)
         self.assertEqual(len(matrix) % 16, 0)
```

