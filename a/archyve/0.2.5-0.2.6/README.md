# Comparing `tmp/archyve-0.2.5.tar.gz` & `tmp/archyve-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archyve-0.2.5.tar", max compression
+gzip compressed data, was "archyve-0.2.6.tar", max compression
```

## Comparing `archyve-0.2.5.tar` & `archyve-0.2.6.tar`

### file list

```diff
@@ -1,4 +1,64 @@
--rw-r--r--   0        0        0     9665 2024-04-14 22:44:03.801273 archyve-0.2.5/archyve.py
--rw-r--r--   0        0        0      369 2024-04-14 23:07:22.402536 archyve-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2331 2024-04-14 22:57:12.016031 archyve-0.2.5/README.md
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 archyve-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-14 23:08:50.878429 archyve-0.2.6/archyve/__init__.py
+-rw-r--r--   0        0        0     9665 2024-04-14 22:44:03.801273 archyve-0.2.6/archyve/archyve.py
+-rw-r--r--   0        0        0     7666 2024-04-14 22:50:21.605913 archyve-0.2.6/archyve/entry.py
+-rw-r--r--   0        0        0     2392 2024-04-14 22:50:21.617433 archyve-0.2.6/archyve/examples.py
+-rw-r--r--   0        0        0     3687 2024-04-14 14:29:28.121250 archyve-0.2.6/archyve/file_structure_functions.py
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.121250 archyve-0.2.6/archyve/scripts/__init__.py
+-rw-r--r--   0        0        0     1050 2024-04-14 23:09:24.900836 archyve-0.2.6/archyve/scripts/clean_image_lib.py
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.122250 archyve-0.2.6/archyve/tests/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-14 14:29:28.123250 archyve-0.2.6/archyve/tests/run_unit_tests.py
+-rw-r--r--   0        0        0     3376 2024-04-14 23:09:24.910843 archyve-0.2.6/archyve/tests/test_entry.py
+-rw-r--r--   0        0        0     1253 2024-04-14 23:09:24.905845 archyve-0.2.6/archyve/tests/test_file_structure_functions.py
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.125250 archyve-0.2.6/archyve/tests/test_materials/entry/audio.mp3
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.125250 archyve-0.2.6/archyve/tests/test_materials/entry/audio.wav
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.126251 archyve-0.2.6/archyve/tests/test_materials/entry/black_square.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.127250 archyve-0.2.6/archyve/tests/test_materials/entry/black_square1.jpg
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.127250 archyve-0.2.6/archyve/tests/test_materials/entry/image.jpg
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.127250 archyve-0.2.6/archyve/tests/test_materials/entry/image.png
+-rw-r--r--   0        0        0  2500480 2024-04-14 14:29:28.137251 archyve-0.2.6/archyve/tests/test_materials/entry/image_with_exif.jpg
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.137251 archyve-0.2.6/archyve/tests/test_materials/entry/unknown
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.138250 archyve-0.2.6/archyve/tests/test_materials/entry/unknown.1234
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.138250 archyve-0.2.6/archyve/tests/test_materials/entry/video.mp4
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.138250 archyve-0.2.6/archyve/tests/test_materials/entry/video.mpeg
+-rw-r--r--   0        0        0        7 2024-04-14 14:36:42.427501 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_dirs/dir1/placeholder.txt
+-rw-r--r--   0        0        0        7 2024-04-14 14:36:42.427501 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_dirs/dir2/placeholder.txt
+-rw-r--r--   0        0        0        7 2024-04-14 14:36:42.427501 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_dirs/dir3/placeholder.txt
+-rw-r--r--   0        0        0        7 2024-04-14 14:36:42.427501 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_dirs/dir4/placeholder.txt
+-rw-r--r--   0        0        0       50 2024-04-14 14:29:28.140251 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_files/file1.txt
+-rw-r--r--   0        0        0       50 2024-04-14 14:29:28.140251 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_files/file2.txt
+-rw-r--r--   0        0        0       50 2024-04-14 14:29:28.141250 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_files/file3.txt
+-rw-r--r--   0        0        0       50 2024-04-14 14:29:28.141250 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_files/file4.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.142609 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir1/file1.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.142609 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir1/file2.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.143618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir1/file3.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.143618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir1/file4.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.144617 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir2/file5.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.144617 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir2/file6.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.145618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir2/file7.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.145618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir2/file8.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.146618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir3/file10.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.146618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir3/file11.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.147618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir3/file12.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.147618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir3/file9.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.148618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/file13.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.149618 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/file14.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.150095 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/subdir/file15.txt
+-rw-r--r--   0        0        0        2 2024-04-14 14:29:28.150095 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/subdir/file16.txt
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.151104 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/subdir/subsubdir/file17.txt
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.151104 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/subdir/subsubdir/file18.txt
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.152104 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/dir4/subdir/subsubdir/subsubsubdir/file19.txt
+-rw-r--r--   0        0        0        0 2024-04-14 14:29:28.152104 archyve-0.2.6/archyve/tests/test_materials/file_structure_functions/sub_paths/file20.txt
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.153104 archyve-0.2.6/archyve/tests/test_materials/images/black_square.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.153104 archyve-0.2.6/archyve/tests/test_materials/images/black_square1.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.154106 archyve-0.2.6/archyve/tests/test_materials/images/black_square2.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.154106 archyve-0.2.6/archyve/tests/test_materials/images/black_square3.jpg
+-rw-r--r--   0        0        0     4008 2024-04-14 14:29:28.155104 archyve-0.2.6/archyve/tests/test_materials/images/black_square_with_one_line.jpg
+-rw-r--r--   0        0        0     4008 2024-04-14 14:29:28.155104 archyve-0.2.6/archyve/tests/test_materials/images/black_square_with_one_line1.jpg
+-rw-r--r--   0        0        0     4008 2024-04-14 14:29:28.156103 archyve-0.2.6/archyve/tests/test_materials/images/black_square_with_one_line2.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.156103 archyve-0.2.6/archyve/tests/test_materials/images/images_sub_dir/black_square2.jpg
+-rw-r--r--   0        0        0     3990 2024-04-14 14:29:28.157104 archyve-0.2.6/archyve/tests/test_materials/images/images_sub_dir/black_square3.jpg
+-rw-r--r--   0        0        0     4029 2024-04-14 14:29:28.158103 archyve-0.2.6/archyve/tests/test_materials/images/images_sub_dir/black_square_with_cross.jpg
+-rw-r--r--   0        0        0     4008 2024-04-14 14:29:28.158103 archyve-0.2.6/archyve/tests/test_materials/images/images_sub_dir/black_square_with_one_line1.jpg
+-rw-r--r--   0        0        0      369 2024-04-14 23:09:55.862447 archyve-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2331 2024-04-14 22:57:12.016031 archyve-0.2.6/README.md
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 archyve-0.2.6/PKG-INFO
```

### Comparing `archyve-0.2.5/archyve.py` & `archyve-0.2.6/archyve/archyve.py`

 * *Files identical despite different names*

### Comparing `archyve-0.2.5/README.md` & `archyve-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `archyve-0.2.5/PKG-INFO` & `archyve-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archyve
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python toolkit for the mass management and analysis of files.
 Author: Alistair Kellaway
 Author-email: ali.kellaway139@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
```

