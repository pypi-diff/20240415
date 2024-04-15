# Comparing `tmp/esp-coredump-1.8.0.tar.gz` & `tmp/esp-coredump-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-coredump-1.8.0.tar", last modified: Fri Nov 24 10:56:23 2023, max compression
+gzip compressed data, was "dist/esp-coredump-1.9.0.tar", last modified: Thu Dec  7 14:10:40 2023, max compression
```

## Comparing `esp-coredump-1.8.0.tar` & `esp-coredump-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump/
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/cli_ext.py
--rwxrwxrwx   0 root         (0) root         (0)    24681 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/coredump.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/_parse_soc_header.py
--rw-rw-rw-   0 root         (0) root         (0)    12112 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     5875 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)    28562 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/riscv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32c2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32c3.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32c6.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32h2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32s2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/soc_headers/esp32s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11177 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/corefile/xtensa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/scripts/espcoredump.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/scripts/run_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/esp_coredump/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1088 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/esp_coredump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 10:56:23.000000 esp-coredump-1.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 10:56:03.000000 esp-coredump-1.8.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4334 2023-11-24 10:55:23.000000 esp-coredump-1.8.0/tests/test_espcoredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/cli_ext.py
+-rwxrwxrwx   0 root         (0) root         (0)    24800 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/coredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump/corefile/
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/_parse_soc_header.py
+-rw-rw-rw-   0 root         (0) root         (0)    12112 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5875 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)    29941 2023-12-07 13:40:43.000000 esp-coredump-1.9.0/esp_coredump/corefile/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/riscv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/soc_headers/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/corefile/xtensa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/scripts/espcoredump.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/scripts/run_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/esp_coredump/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/esp_coredump.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 14:10:40.000000 esp-coredump-1.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-07 14:10:30.000000 esp-coredump-1.9.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2023-12-07 12:46:02.000000 esp-coredump-1.9.0/tests/test_espcoredump.py
```

### Comparing `esp-coredump-1.8.0/LICENSE` & `esp-coredump-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/PKG-INFO` & `esp-coredump-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.8.0
+Version: 1.9.0
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.8.0/README.md` & `esp-coredump-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/__init__.py` & `esp-coredump-1.9.0/esp_coredump/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 from .coredump import CoreDump
 
 __all__ = [
     'CoreDump',
 ]
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
```

### Comparing `esp-coredump-1.8.0/esp_coredump/cli_ext.py` & `esp-coredump-1.9.0/esp_coredump/cli_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
                          help='Log level (0..3)')
 common_args.add_argument('--gdb', '-g',
                          help='Path to gdb')
 common_args.add_argument('--extra-gdbinit-file', '-ex',
                          help='Path to additional gdbinit file')
 common_args.add_argument('--core', '-c',
                          help='Path to core dump file (if skipped core dump will be read from flash)')
-common_args.add_argument('--core-format', '-t', choices=['b64', 'elf', 'raw'], default='elf',
-                         help='File specified with "-c" is an ELF ("elf"), '
-                              'raw (raw) or base64-encoded (b64) binary')
+common_args.add_argument('--core-format', '-t', choices=['auto', 'b64', 'elf', 'raw'], default='auto',
+                         help='File specified with "-c" is an ELF (elf), raw (raw) or base64-encoded (b64) binary. '
+                         'For autodetection based on file header use "auto".')
 common_args.add_argument('--off', '-o', type=int,
                          help='Offset of coredump partition in flash (type "make partition_table" to see).')
 common_args.add_argument('--save-core', '-s',
                          help='Save core to file. Otherwise temporary core file will be deleted. '
                               'Does not work with "-c"', )
 common_args.add_argument('--rom-elf', '-r',
                          help='Path to ROM ELF file. Will use "<target>_rom.elf" if not specified')
```

### Comparing `esp-coredump-1.8.0/esp_coredump/coredump.py` & `esp-coredump-1.9.0/esp_coredump/coredump.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 from construct import Container, GreedyRange, Int32ul, ListContainer, Struct
 
 from .corefile import RISCV_TARGETS, SUPPORTED_TARGETS, XTENSA_TARGETS, xtensa
 from .corefile.elf import (TASK_STATUS_CORRECT, ElfFile, ElfSegment,
                            ESPCoreDumpElfFile, EspTaskStatus)
 from .corefile.gdb import DEFAULT_GDB_TIMEOUT_SEC, EspGDB
 from .corefile.loader import (ESPCoreDumpFileLoader, ESPCoreDumpFlashLoader,
-                              ESPCoreDumpLoaderError, EspCoreDumpVersion)
+                              ESPCoreDumpLoaderError, EspCoreDumpVersion,
+                              get_core_file_format)
 
 IDF_PATH = os.getenv('IDF_PATH', '')
 ESP_ROM_ELF_DIR = os.getenv('ESP_ROM_ELF_DIR')
 ROMS_JSON = os.path.join(IDF_PATH, 'tools', 'idf_py_actions', 'roms.json')  # type: ignore
 
 MORE_INFO_MSG = 'Read more: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html'
 GDB_NOT_FOUND_ERROR = (
@@ -59,15 +60,15 @@
     CLOSE_FDS = True
 
 
 class CoreDump:
     def __init__(self,
                  baud: Optional[int] = int(os.environ.get('ESPTOOL_BAUD', ESPLoader.ESP_ROM_BAUD)),
                  chip: str = os.environ.get('ESPTOOL_CHIP', 'auto'),
-                 core_format: str = 'elf',
+                 core_format: str = 'auto',
                  port: str = os.environ.get('ESPTOOL_PORT', ESPLoader.DEFAULT_PORT),
                  gdb_timeout_sec: int = DEFAULT_GDB_TIMEOUT_SEC,
                  core: Optional[str] = None,
                  chip_rev: Optional[int] = None,
                  gdb: Optional[str] = None,
                  extra_gdbinit_file: Optional[str] = None,
                  off: Optional[int] = None,
@@ -80,15 +81,15 @@
         if prog is None:
             raise ValueError("Path to program\'s ELF binary is not provided")
 
         self.baud = baud
         self.chip = chip
         self.core = core
         self.chip_rev = chip_rev
-        self.core_format = core_format
+        self.core_format = get_core_file_format(core) if core and core_format == 'auto' else core_format
         self.gdb = gdb
         self.gdb_timeout_sec = gdb_timeout_sec
         self.extra_gdbinit_file = extra_gdbinit_file
         self.coredump_off = off
         self.parttable_off = parttable_off
         self.prog = prog
         self.port = port
```

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/__init__.py` & `esp-coredump-1.9.0/esp_coredump/corefile/__init__.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/_parse_soc_header.py` & `esp-coredump-1.9.0/esp_coredump/corefile/_parse_soc_header.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/elf.py` & `esp-coredump-1.9.0/esp_coredump/corefile/elf.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/gdb.py` & `esp-coredump-1.9.0/esp_coredump/corefile/gdb.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/loader.py` & `esp-coredump-1.9.0/esp_coredump/corefile/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import binascii
 import hashlib
 import logging
 import os
 import subprocess
 import sys
 import tempfile
+from base64 import b64decode
 from typing import Optional, Tuple
 
 from construct import (AlignedStruct, Bytes, GreedyRange, Int32ul, Padding,
                        Struct, abs_, this)
 
 from . import ESPCoreDumpLoaderError
 from .elf import (TASK_STATUS_CORRECT, TASK_STATUS_TCB_CORRUPTED, ElfFile,
@@ -66,14 +67,43 @@
 MemSegmentHeader = Struct(
     'mem_start' / Int32ul,
     'mem_sz' / Int32ul,
     'data' / Bytes(this.mem_sz),
 )
 
 
+def get_core_file_format(core_file: str) -> str:
+    """Get format of core_file based on the header"""
+    with open(core_file, 'rb') as f:
+        coredump_bytes = f.read(16)
+
+        # Check if this is an ELF file without the core dump header (core_dump_header_t)
+        if coredump_bytes.startswith(b'\x7fELF'):
+            return 'elf'
+
+        # Check if this is a core dump with a core_dump_header_t header
+        core_version = EspCoreDumpVersion(int.from_bytes(coredump_bytes[4:7], 'little'))
+        if core_version.dump_ver in EspCoreDumpLoader.CORE_VERSIONS:
+            return 'raw'
+
+    # Neither of theses headers matched, so this might be a base64 encoded core dump;
+    # however in case it's just some unknown binary, ignore decoding errors.
+    with open(core_file, 'r', encoding='utf-8', errors='ignore') as c:
+        coredump_str = c.read()
+        try:
+            b64decode(coredump_str)
+        except Exception:
+            raise SystemExit(
+                'The format of the provided core-file is not recognized. '
+                'Please ensure that the core-format matches one of the following: ELF (“elf”), '
+                'raw (raw) or base64-encoded (b64) binary'
+            )
+        return 'b64'
+
+
 class EspCoreDumpVersion(object):
     """Core dump version class, it contains all version-dependent params
     """
     # Chip IDs should be in sync with components/esp_hw_support/include/esp_chip_info.h
     ESP32 = 0
     ESP32S2 = 2
     ESP32S3 = 9
@@ -125,14 +155,15 @@
     BIN_V1 = EspCoreDumpVersion.make_dump_ver(0, 1)
     BIN_V2 = EspCoreDumpVersion.make_dump_ver(0, 2)
     BIN_V2_1 = EspCoreDumpVersion.make_dump_ver(0, 3)
     ELF_CRC32_V2 = EspCoreDumpVersion.make_dump_ver(1, 0)
     ELF_CRC32_V2_1 = EspCoreDumpVersion.make_dump_ver(1, 2)
     ELF_SHA256_V2 = EspCoreDumpVersion.make_dump_ver(1, 1)
     ELF_SHA256_V2_1 = EspCoreDumpVersion.make_dump_ver(1, 3)
+    CORE_VERSIONS = [BIN_V1, BIN_V2, BIN_V2_1, ELF_CRC32_V2, ELF_CRC32_V2_1, ELF_SHA256_V2, ELF_SHA256_V2_1]
 
     def __init__(self):  # type: () -> None
         super(EspCoreDumpLoader, self).__init__()
         self.core_src_file = None  # type: Optional[str]
         self.core_src_struct = None
         self.core_src = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/riscv.py` & `esp-coredump-1.9.0/esp_coredump/corefile/riscv.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/corefile/xtensa.py` & `esp-coredump-1.9.0/esp_coredump/corefile/xtensa.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/scripts/espcoredump.py` & `esp-coredump-1.9.0/esp_coredump/scripts/espcoredump.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump/scripts/run_tests.py` & `esp-coredump-1.9.0/esp_coredump/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/esp_coredump.egg-info/PKG-INFO` & `esp-coredump-1.9.0/esp_coredump.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.8.0
+Version: 1.9.0
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.8.0/esp_coredump.egg-info/SOURCES.txt` & `esp-coredump-1.9.0/esp_coredump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/setup.py` & `esp-coredump-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.8.0/tests/test_espcoredump.py` & `esp-coredump-1.9.0/tests/test_espcoredump.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 SUPPORTED_TARGET = ['esp32', 'esp32c3']
 COREDUMP_FILE_NAME = 'coredump'
 
 TEST_DIR_ABS_PATH = os.path.dirname(__file__)
 ESP_PROG_DIR = os.path.join(TEST_DIR_ABS_PATH, 'test_apps', 'built_apps')
 
 
-def get_coredump_kwargs(core_ext: str, target: str, save_core=False):
-    core_format = 'raw' if core_ext == 'bin' else core_ext
+def get_coredump_kwargs(core_ext: str, target: str, save_core: bool = False, auto_format: bool = False):
+    core_format = 'auto' if auto_format else 'raw' if core_ext == 'bin' else core_ext
     kwargs = {
         'gdb_timeout_sec': 5,
         'chip': target,
         'print_mem': True,
         'core_format': core_format,
         'core': os.path.join(TEST_DIR_ABS_PATH, target, f'{COREDUMP_FILE_NAME}.{core_ext}'),
         'save_core': os.path.join(TEST_DIR_ABS_PATH, target, f'{COREDUMP_FILE_NAME}.elf') if save_core else None,
@@ -39,16 +39,16 @@
 def get_expected_output(target: str):
     expected_output_file = os.path.join(TEST_DIR_ABS_PATH, target, 'expected_output')
     with open(expected_output_file) as file:
         output = file.read()
     return output
 
 
-def get_output(core_ext: str, target: str, save_core=False):
-    kwargs = get_coredump_kwargs(core_ext=core_ext, save_core=save_core, target=target)
+def get_output(core_ext: str, target: str, save_core: bool = False, auto_format: bool = False):
+    kwargs = get_coredump_kwargs(core_ext=core_ext, save_core=save_core, target=target, auto_format=auto_format)
     coredump = CoreDump(**kwargs)
     output_file = os.path.join(TEST_DIR_ABS_PATH, target, f'output_from_{core_ext}')
     with io.StringIO() as buffer, contextlib.redirect_stdout(buffer):
         coredump.info_corefile()
         output = buffer.getvalue()
 
     with open(output_file, 'w') as f:
@@ -81,14 +81,26 @@
     def test_coredump_decode_from_bin(self):
         for target in SUPPORTED_TARGET:
             decode_from_b64_to_bin(target)
             output = get_output(core_ext='bin', target=target)
             expected_output = get_expected_output(target)
             self.assertEqual(expected_output, output)
 
+    def test_coredump_decode_auto_format(self):
+        # make sure that .elf and .bin inputs are created
+        for target in SUPPORTED_TARGET:
+            get_output(core_ext='b64', save_core=True, target=target)
+            decode_from_b64_to_bin(target)
+        for format in ['bin', 'elf', 'b64']:
+            with self.subTest(format=format):
+                for target in SUPPORTED_TARGET:
+                    output = get_output(core_ext=format, target=target, auto_format=True)
+                    expected_output = get_expected_output(target)
+                    self.assertEqual(expected_output, output)
+
 
 class TestESPCoreDumpElfFile(unittest.TestCase):
     def test_read_elf(self):
         for target in SUPPORTED_TARGET:
             elf = ESPCoreDumpElfFile(os.path.join(TEST_DIR_ABS_PATH, target, f'{COREDUMP_FILE_NAME}.elf'))
             self.assertIsNotNone(elf.load_segments)
             self.assertIsNotNone(elf.note_segments)
```

