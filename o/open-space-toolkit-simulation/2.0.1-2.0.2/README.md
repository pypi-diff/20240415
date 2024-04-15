# Comparing `tmp/open_space_toolkit_simulation-2.0.1-py39-none-manylinux2014_x86_64.whl.zip` & `tmp/open_space_toolkit_simulation-2.0.2-py39-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 2935888 bytes, number of entries: 13
--rw-r--r--  2.0 unx       21 b- defN 24-Mar-28 14:54 ostk/__init__.py
--rwxr-xr-x  2.0 unx   385040 b- defN 24-Mar-28 14:54 ostk/simulation/OpenSpaceToolkitSimulationPy.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      100 b- defN 24-Mar-28 14:54 ostk/simulation/__init__.py
--rwxr-xr-x  2.0 unx 10632824 b- defN 24-Mar-28 14:54 ostk/simulation/libopen-space-toolkit-simulation.so.2
--rw-r--r--  2.0 unx       21 b- defN 24-Mar-28 14:54 ostk/simulation/test/__init__.py
--rw-r--r--  2.0 unx      114 b- defN 24-Mar-28 14:54 ostk/simulation/test/test_import.py
--rw-r--r--  2.0 unx     1694 b- defN 24-Mar-28 14:54 ostk/simulation/test/test_satellite.py
--rw-r--r--  2.0 unx     7184 b- defN 24-Mar-28 14:54 ostk/simulation/test/test_simulator.py
--rw-r--r--  2.0 unx     1658 b- defN 24-Mar-28 14:54 open_space_toolkit_simulation-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-28 14:54 open_space_toolkit_simulation-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-28 14:54 open_space_toolkit_simulation-2.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-28 14:54 open_space_toolkit_simulation-2.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1264 b- defN 24-Mar-28 14:54 open_space_toolkit_simulation-2.0.1.dist-info/RECORD
-13 files, 11030036 bytes uncompressed, 2933710 bytes compressed:  73.4%
+Zip file size: 2935918 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-15 16:45 ostk/__init__.py
+-rwxr-xr-x  2.0 unx   385040 b- defN 24-Apr-15 16:45 ostk/simulation/OpenSpaceToolkitSimulationPy.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      100 b- defN 24-Apr-15 16:45 ostk/simulation/__init__.py
+-rwxr-xr-x  2.0 unx 10632824 b- defN 24-Apr-15 16:45 ostk/simulation/libopen-space-toolkit-simulation.so.2
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-15 16:45 ostk/simulation/test/__init__.py
+-rw-r--r--  2.0 unx      114 b- defN 24-Apr-15 16:45 ostk/simulation/test/test_import.py
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-15 16:45 ostk/simulation/test/test_satellite.py
+-rw-r--r--  2.0 unx     7184 b- defN 24-Apr-15 16:45 ostk/simulation/test/test_simulator.py
+-rw-r--r--  2.0 unx     1844 b- defN 24-Apr-15 16:45 open_space_toolkit_simulation-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-15 16:45 open_space_toolkit_simulation-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-15 16:45 open_space_toolkit_simulation-2.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-15 16:45 open_space_toolkit_simulation-2.0.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1264 b- defN 24-Apr-15 16:45 open_space_toolkit_simulation-2.0.2.dist-info/RECORD
+13 files, 11030222 bytes uncompressed, 2933740 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: ostk/simulation/test/test_satellite.py
 Comment: 
 
 Filename: ostk/simulation/test/test_simulator.py
 Comment: 
 
-Filename: open_space_toolkit_simulation-2.0.1.dist-info/METADATA
+Filename: open_space_toolkit_simulation-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: open_space_toolkit_simulation-2.0.1.dist-info/WHEEL
+Filename: open_space_toolkit_simulation-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: open_space_toolkit_simulation-2.0.1.dist-info/top_level.txt
+Filename: open_space_toolkit_simulation-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: open_space_toolkit_simulation-2.0.1.dist-info/zip-safe
+Filename: open_space_toolkit_simulation-2.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: open_space_toolkit_simulation-2.0.1.dist-info/RECORD
+Filename: open_space_toolkit_simulation-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `open_space_toolkit_simulation-2.0.1.dist-info/METADATA` & `open_space_toolkit_simulation-2.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: open-space-toolkit-simulation
-Version: 2.0.1
+Version: 2.0.2
 Summary: Spacecraft simulation.
 Author: Open Space Collective
 Author-email: contact@open-space-collective.org
 License: Apache License 2.0
 Keywords: open-space-collective,open-space-toolkit simulation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-Requires-Dist: open-space-toolkit-astrodynamics ~=9.0.3
+Requires-Dist: open-space-toolkit-core ~=3.0
+Requires-Dist: open-space-toolkit-io ~=3.0
+Requires-Dist: open-space-toolkit-mathematics ~=3.0
+Requires-Dist: open-space-toolkit-physics ~=6.0
+Requires-Dist: open-space-toolkit-astrodynamics ~=9.1
 
 # Open Space Toolkit ▸ Simulation
 
 Spacecraft simulation.
 
 [![Build and Test](https://github.com/open-space-collective/open-space-toolkit-simulation/actions/workflows/build-test.yml/badge.svg?branch=main)](https://github.com/open-space-collective/open-space-toolkit-simulation/actions/workflows/build-test.yml)
 [![Code Coverage](https://codecov.io/gh/open-space-collective/open-space-toolkit-simulation/branch/main/graph/badge.svg)](https://codecov.io/gh/open-space-collective/open-space-toolkit-simulation)
```

## Comparing `open_space_toolkit_simulation-2.0.1.dist-info/RECORD` & `open_space_toolkit_simulation-2.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 ostk/simulation/OpenSpaceToolkitSimulationPy.cpython-39-x86_64-linux-gnu.so,sha256=Yckdb3EhKvPAqUxrnHeaEJZzsilinvUfNZuJGzBLYWw,385040
 ostk/simulation/__init__.py,sha256=ci3ecZ6SPuphlo5g00jFyegN3Z5HHbEY1_5JqvgTba4,100
 ostk/simulation/libopen-space-toolkit-simulation.so.2,sha256=j-BjSCNXIV9jRmtjw0oEg4LbrpYsqzW26aVfR1jafB0,10632824
 ostk/simulation/test/__init__.py,sha256=epnVn2PwdQkUDZ1msqBRO5nEZIOUBIq-IfK3IlNPijE,21
 ostk/simulation/test/test_import.py,sha256=Ujgsz4EfK0amh_z00H9CuxB9OmzXDCT7wimy40I-m-k,114
 ostk/simulation/test/test_satellite.py,sha256=JhqPtLDwgPeVeRly3m8QzfAwXJSeajfs2XCyeXoiQsM,1694
 ostk/simulation/test/test_simulator.py,sha256=PSxGoWSOVWQUHRDQhpYF4VX56h9MFkf0EzuNSORgzgU,7184
-open_space_toolkit_simulation-2.0.1.dist-info/METADATA,sha256=2CUqH8PkswuxnOS2tQi_N9lvXLuATUoutQ8duhTIWTg,1658
-open_space_toolkit_simulation-2.0.1.dist-info/WHEEL,sha256=C8VPa8ubJV_FsX03Y77FSLYpZ55_QAdcCwG5DPGyjjM,110
-open_space_toolkit_simulation-2.0.1.dist-info/top_level.txt,sha256=zOR18699uDYnafgarhL8WU_LmTZY_5NVqutv-flp_x4,5
-open_space_toolkit_simulation-2.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-open_space_toolkit_simulation-2.0.1.dist-info/RECORD,,
+open_space_toolkit_simulation-2.0.2.dist-info/METADATA,sha256=DHC9QH6VEdVYiDmfps4NnzsXYuAqBQArX7J3XcqOl8k,1844
+open_space_toolkit_simulation-2.0.2.dist-info/WHEEL,sha256=C8VPa8ubJV_FsX03Y77FSLYpZ55_QAdcCwG5DPGyjjM,110
+open_space_toolkit_simulation-2.0.2.dist-info/top_level.txt,sha256=zOR18699uDYnafgarhL8WU_LmTZY_5NVqutv-flp_x4,5
+open_space_toolkit_simulation-2.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+open_space_toolkit_simulation-2.0.2.dist-info/RECORD,,
```

