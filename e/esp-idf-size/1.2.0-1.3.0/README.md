# Comparing `tmp/esp-idf-size-1.2.0.tar.gz` & `tmp/esp-idf-size-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-3fkxkkr5/esp-idf-size-1.2.0.tar", last modified: Mon Mar 18 12:36:42 2024, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-_1j2ui7g/esp-idf-size-1.3.0.tar", last modified: Mon Apr 15 11:27:38 2024, max compression
```

## Comparing `esp-idf-size-1.2.0.tar` & `esp-idf-size-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32c5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32p4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    57268 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size/ng/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/format_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/format_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/format_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/format_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/format_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/mapfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    49691 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/esp_idf_size/ng/memorymap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/esp_idf_size.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:36:42.000000 esp-idf-size-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-18 12:36:30.000000 esp-idf-size-1.2.0/test/test_idf_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c61.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32p4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57441 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/ng/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16584 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/mapfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51323 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/memorymap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/test/test_idf_size.py
```

### Comparing `esp-idf-size-1.2.0/LICENSE` & `esp-idf-size-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/PKG-INFO` & `esp-idf-size-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 1.2.0
+Version: 1.3.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32.yaml` & `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   length: value or equation
 #   secondary_address: value if exist
 DRAM:
   primary_address: 0x3FFAE000
   length: 17 * 0x2000 + 4 * 0x8000 + 4 * 0x4000
 IRAM:
   primary_address: 0x40070000
-  length: 2 * 0x8000 + 16 * 0x2000
+  length: 0x50000
 CACHE_I:
   primary_address: 0x400C2000
   length: 0xB3E000
   name: Flash Code
 CACHE_D_1:
   primary_address: 0x3F400000
   length: 0x400000
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32p4.yaml` & `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32p4.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32s2.yaml` & `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/esp_idf_size/chip_info/esp32s3.yaml` & `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/esp_idf_size/core.py` & `esp-idf-size-1.3.0/esp_idf_size/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         'text': r'.*\.text',
         'data': r'.*\.data',
         'bss': r'.*\.bss',
         'rodata': r'.*\.rodata',
         'rodata_noload': r'.*\.rodata_noload',
         'noinit': r'.*noinit',
         'vectors': r'.*\.vectors',
-        'flash': r'.*(flash|eh_frame).*',
+        'flash': r'.*\.(flash|eh_frame).*',
     }.items()}
 
     @staticmethod
     def in_section(section: str, section_name_or_list: Union[str, Iterable]) -> bool:
         """
         Check if section in section_name_or_list
         """
@@ -680,16 +680,18 @@
 
         r.flash_code = get_size(flash_text_list)
         r.flash_rodata = get_size(flash_rodata_list)
 
         r.flash_other = get_size(flash_other_list)
         r.used_flash_non_ram = r.flash_code + r.flash_rodata + r.flash_other
 
-        # The used DRAM BSS is counted into the "Used static DRAM" but not into the "Total image size"
-        r.total_size = r.used_dram - r.dram_bss + r.used_iram + r.used_diram - r.diram_bss + r.used_flash_non_ram
+        # The used DRAM BSS and .noinit section are counted into the "Used static DRAM" but not into the "Total image size"
+        noinit_sections = filter_in_section(dram_sections + diram_sections, 'noinit')
+        noinit_total = get_size(noinit_sections)
+        r.total_size = r.used_dram - r.dram_bss + r.used_iram + r.used_diram - r.diram_bss + r.used_flash_non_ram - noinit_total
         return r
 
     def get_dict(self) -> collections.OrderedDict:
         ret = collections.OrderedDict([
             ('dram_data', self.dram_data),
             ('dram_bss', self.dram_bss),
             ('dram_rodata', self.dram_rodata),
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/format_csv.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/format_csv.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/format_json.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/format_json.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 def show_summary(memmap: Dict[str, Any], args: Namespace) -> None:
     summary: Dict[str, Any] = {
         'version': '1.0',
         'layout': [],
     }
 
+    memorymap.sort(memmap, args)
+
     for mem_type_name, mem_type_info in memmap['memory_types'].items():
         mem_type = {
             'name': mem_type_name,
             'total': mem_type_info['size'],
             'used': mem_type_info['used'],
             'free': mem_type_info['size'] - mem_type_info['used'],
             'parts': {},
@@ -30,24 +32,27 @@
             }
 
     log.print(json.dumps(summary, indent=4))
 
 
 def show_object_files(memmap: Dict[str, Any], args: Namespace) -> None:
     summary = memorymap.get_object_files_summary(memmap, args)
+    summary = memorymap.get_summary_sorted(summary, args)
     log.print(json.dumps(summary, indent=4))
 
 
 def show_archives(memmap: Dict[str, Any], args: Namespace) -> None:
     summary = memorymap.get_archives_summary(memmap, args)
+    summary = memorymap.get_summary_sorted(summary, args)
     log.print(json.dumps(summary, indent=4))
 
 
 def show_symbols(memmap: Dict[str, Any], args: Namespace) -> None:
     summary = memorymap.get_symbols_summary(memmap, args)
+    summary = memorymap.get_summary_sorted(summary, args)
     log.print(json.dumps(summary, indent=4))
 
 
 def show(memmap: Dict[str, Any], args: Namespace) -> None:
     if args.archives:
         show_archives(memmap, args)
     elif args.archive_details:
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/format_table.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/format_table.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 from argparse import Namespace
+from collections import namedtuple
 from typing import Any, Dict, List, Union
 
+from rich.markup import escape
 from rich.table import Table
+from rich.text import Text
 
 from . import log, memorymap
 
 
 def show_diff_info(memmap: Dict[str, Any], args: Namespace) -> None:
     if not args.diff:
         return
@@ -52,60 +55,178 @@
     table = Table(title='Memory Type Usage Summary')
     table.add_column('Memory Type/Section', overflow='fold')
     table.add_column(r'Used \[bytes]', overflow='fold', justify='right')
     table.add_column(r'Used \[%]', overflow='fold', justify='right')
     table.add_column(r'Remain \[bytes]', overflow='fold', justify='right')
     table.add_column(r'Total \[bytes]', overflow='fold', justify='right')
 
-    mem_type_sorted = {k: v for k, v in sorted(memmap['memory_types'].items(),
-                                               key=lambda item: int(item[1]['used']),
-                                               reverse=True)}
-
-    for name, info in mem_type_sorted.items():
-        if info['size']:
-            pct = info['used'] / info['size'] * 100
+    # Extend memory types and sections for percentage and remain info
+    for mem_type_name, mem_type_info in memmap['memory_types'].items():
+        if mem_type_info['size']:
+            mem_type_info['pct'] = mem_type_info['used'] / mem_type_info['size'] * 100
         else:
-            pct = 0
-        if info['size'] - info['size_diff']:
-            pct_diff = pct - ((info['used'] - info['used_diff']) / (info['size'] - info['size_diff']) * 100)
+            mem_type_info['pct'] = 0
+
+        if mem_type_info['size'] - mem_type_info['size_diff']:
+            mem_type_info['pct_diff'] = (mem_type_info['pct'] -
+                                         ((mem_type_info['used'] - mem_type_info['used_diff']) /
+                                          (mem_type_info['size'] - mem_type_info['size_diff']) * 100))
+        else:
+            mem_type_info['pct_diff'] = mem_type_info['pct'] - 0
+
+        mem_type_info['remain'] = mem_type_info['size'] - mem_type_info['used']
+        mem_type_info['remain_diff'] = mem_type_info['size_diff'] - mem_type_info['used_diff']
+        mem_type_info['total'] = mem_type_info['size']
+        mem_type_info['total_diff'] = mem_type_info['size_diff']
+
+        for section_name, section_info in mem_type_info['sections'].items():
+            if mem_type_info['size']:
+                section_info['pct'] = section_info['size'] / mem_type_info['size'] * 100
+            else:
+                section_info['pct'] = 0
+
+            if mem_type_info['size'] - mem_type_info['size_diff']:
+                section_info['pct_diff'] = (section_info['pct'] -
+                                            ((section_info['size'] - section_info['size_diff']) /
+                                             (mem_type_info['size'] - mem_type_info['size_diff']) * 100))
+            else:
+                section_info['pct_diff'] = section_info['pct'] - 0
+
+            # Add used/remain into section, so we can use the same sorting keys as for memory types.
+            section_info['used'] = section_info['size']
+            section_info['used_diff'] = section_info['size_diff']
+            section_info['remain'] = 0
+            section_info['remain_diff'] = 0
+            section_info['total'] = 0
+            section_info['total_diff'] = 0
+
+    try:
+        args.sort = int(args.sort)
+    except ValueError:
+        for idx, column in enumerate(table.columns):
+            # We are using rich markup, which uses square brackets, in column header names, so
+            # we need to covert them before comparison.
+            if str(Text.from_markup(column.header)) == args.sort:
+                args.sort = idx
+                break
         else:
-            pct_diff = pct - 0
+            log.die(f'Column "{escape(args.sort)}" not found')
+
+    if args.sort == 0:
+        log.die('Sorting based on column 0, which contains row description, is not supported.')
 
-        table.add_row(name,
-                      color_diff(info['used'], info['used_diff'], args.diff),
-                      color_diff(round(pct, 2), round(pct_diff, 2), args.diff),
-                      color_size(info['size'] - info['used'], info['size_diff'] - info['used_diff'], args.diff),
-                      color_size(info['size'], info['size_diff'], args.diff),
+    try:
+        sort_keys = ['used', 'pct', 'remain', 'total']
+        sort_key = sort_keys[args.sort - 1 if args.sort > 0 else args.sort]
+    except IndexError:
+        log.die((f'Column index {args.sort} is out of range. '
+                 f'Please use 1..{len(sort_keys)} or {-len(sort_keys)}..-1 range.'))
+
+    if args.sort_diff:
+        sort_key += '_diff'
+
+    # Sort memory types first and later sections within them.
+    mem_types_sorted = memorymap.sort_dict_by_key(memmap['memory_types'], sort_key, args.sort_reverse)
+
+    for mem_type_name, mem_type_info in mem_types_sorted.items():
+        table.add_row(mem_type_name,
+                      color_diff(mem_type_info['used'], mem_type_info['used_diff'], args.diff),
+                      color_diff(round(mem_type_info['pct'], 2), round(mem_type_info['pct_diff'], 2), args.diff),
+                      color_size(mem_type_info['remain'], mem_type_info['remain_diff'], args.diff),
+                      color_size(mem_type_info['total'], mem_type_info['total_diff'], args.diff),
                       style='dark_orange')
 
-        sections_sorted = {k: v for k, v in sorted(info['sections'].items(),
-                                                   key=lambda item: int(item[1]['size']),
-                                                   reverse=True)}
+        sections_sorted = memorymap.sort_dict_by_key(mem_type_info['sections'], sort_key, args.sort_reverse)
 
         for section_name, section_info in sections_sorted.items():
             name = section_info['abbrev_name'] if args.abbrev else section_name
 
-            if info['size']:
-                pct = section_info['size'] / info['size'] * 100
-            else:
-                pct = 0
-            if info['size'] - info['size_diff']:
-                pct_diff = pct - ((section_info['size'] - section_info['size_diff']) /
-                                  (info['size'] - info['size_diff']) * 100)
-
             table.add_row(f'   {name}',
-                          color_diff(section_info['size'], section_info['size_diff'], args.diff),
-                          color_diff(round(pct, 2), round(pct_diff, 2), args.diff),
+                          color_diff(section_info['used'], section_info['used_diff'], args.diff),
+                          color_diff(round(section_info['pct'], 2), round(section_info['pct_diff'], 2), args.diff),
                           '',
                           '',
                           style='bright_blue')
 
     return table
 
 
+def _get_table_sorted(summary: Dict[str, Any], table: Table, args: Namespace) -> List[List[str]]:
+    # Helper for get_*_table functions. It converts json summary into
+    # table and sorts it.
+
+    # Each column has three items:
+    #   info - text representing the size, which is printed in the table
+    #   size - used only for sorting purposes
+    #   size_diff - used only for sorting purposes
+    Column = namedtuple('Column', ['info', 'size', 'size_diff'])
+    # Raw has name and list of Columns
+    Row = namedtuple('Row', ['name', 'columns'])
+    columns: List[Column] = []
+    rows: List[Row] = []
+    rows_final: List[List[str]] = []
+
+    for entry_name, entry_info in summary.items():
+        columns = []
+        size = entry_info['size']
+        diff = entry_info['size_diff']
+        info = color_diff(size, diff, args.diff)
+        columns.append(Column(info, size, diff))
+
+        for mem_type_name, mem_type_info in entry_info['memory_types'].items():
+            size = mem_type_info['size']
+            diff = mem_type_info['size_diff']
+            info = color_diff(size, diff, args.diff)
+            columns.append(Column(info, size, diff))
+
+            for section_name, section_info in mem_type_info['sections'].items():
+                size = section_info['size']
+                diff = section_info['size_diff']
+                info = color_diff(size, diff, args.diff)
+                columns.append(Column(info, size, diff))
+
+        name = entry_info['abbrev_name'] if args.abbrev else entry_name
+        rows.append(Row(name, columns))
+
+    try:
+        args.sort = int(args.sort)
+    except ValueError:
+        for idx, column in enumerate(table.columns):
+            if column.header == args.sort:
+                args.sort = idx
+                break
+        else:
+            log.die(f'Column "{args.sort}" not found')
+
+    if args.sort == 0:
+        log.die('Sorting based on column 0, which contains row description, is not supported.')
+
+    def sort_key(row: Row) -> int:
+        sort_key_idx = args.sort - 1 if args.sort > 0 else args.sort
+
+        if args.sort_diff:
+            return int(row.columns[sort_key_idx].size_diff)
+        else:
+            return int(row.columns[sort_key_idx].size)
+
+    try:
+        rows = [row for row in sorted(rows, key=sort_key, reverse=args.sort_reverse)]
+    except IndexError:
+        log.die((f'Column index {args.sort} is out of range. '
+                 f'Please use 1..{len(columns) - 1} or {-len(columns)}..-1 range.'))
+
+    # Return only simple list of rows, where each row is a list
+    # of columns to be printed in table.
+    for row in rows:
+        cols = [row.name] + [col.info for col in row.columns]
+        rows_final.append(cols)
+
+    return rows_final
+
+
 def get_object_files_table(memmap: Dict[str, Any], args: Namespace) -> Table:
     object_files_summary = memorymap.get_object_files_summary(memmap, args)
 
     table = Table(title='Per-file contributions to ELF file')
     table.add_column('Object File', overflow='fold')
     table.add_column('Total Size', overflow='fold', justify='right')
 
@@ -113,23 +234,17 @@
         for mem_type_name, mem_type_info in object_file_info['memory_types'].items():
             table.add_column(mem_type_name, overflow='fold', justify='right', style='dark_orange')
             for section_name, section_info in mem_type_info['sections'].items():
                 name = section_info['abbrev_name'] if args.abbrev else section_name
                 table.add_column(name, overflow='fold', justify='right', style='bright_blue')
         break
 
-    for object_file_name, object_file_info in object_files_summary.items():
-        sizes: List[str] = []
-        sizes.append(color_diff(object_file_info['size'], object_file_info['size_diff'], args.diff))
-        for mem_type_name, mem_type_info in object_file_info['memory_types'].items():
-            sizes.append(color_diff(mem_type_info['size'], mem_type_info['size_diff'], args.diff))
-            for section_name, section_info in mem_type_info['sections'].items():
-                sizes.append(color_diff(section_info['size'], section_info['size_diff'], args.diff))
-        name = object_file_info['abbrev_name'] if args.abbrev else object_file_name
-        table.add_row(name, *sizes)
+    sizes_sorted = _get_table_sorted(object_files_summary, table, args)
+    for sizes in sizes_sorted:
+        table.add_row(*sizes)
 
     return table
 
 
 def get_archives_table(memmap: Dict[str, Any], args: Namespace) -> Table:
     archives_summary = memorymap.get_archives_summary(memmap, args)
 
@@ -141,23 +256,17 @@
         for mem_type_name, mem_type_info in archive_info['memory_types'].items():
             table.add_column(mem_type_name, overflow='fold', justify='right', style='dark_orange')
             for section_name, section_info in mem_type_info['sections'].items():
                 name = section_info['abbrev_name'] if args.abbrev else section_name
                 table.add_column(name, overflow='fold', justify='right', style='bright_blue')
         break
 
-    for archive_name, archive_info in archives_summary.items():
-        sizes: List[str] = []
-        sizes.append(color_diff(archive_info['size'], archive_info['size_diff'], args.diff))
-        for mem_type_name, mem_type_info in archive_info['memory_types'].items():
-            sizes.append(color_diff(mem_type_info['size'], mem_type_info['size_diff'], args.diff))
-            for section_name, section_info in mem_type_info['sections'].items():
-                sizes.append(color_diff(section_info['size'], section_info['size_diff'], args.diff))
-        name = archive_info['abbrev_name'] if args.abbrev else archive_name
-        table.add_row(name, *sizes)
+    sizes_sorted = _get_table_sorted(archives_summary, table, args)
+    for sizes in sizes_sorted:
+        table.add_row(*sizes)
 
     return table
 
 
 def get_symbols_table(memmap: Dict[str, Any], args: Namespace) -> Table:
     symbols_summary = memorymap.get_symbols_summary(memmap, args)
 
@@ -169,23 +278,17 @@
         for mem_type_name, mem_type_info in symbol_info['memory_types'].items():
             table.add_column(mem_type_name, overflow='fold', justify='right', style='dark_orange')
             for section_name, section_info in mem_type_info['sections'].items():
                 name = section_info['abbrev_name'] if args.abbrev else section_name
                 table.add_column(name, overflow='fold', justify='right', style='bright_blue')
         break
 
-    for symbol_name, symbol_info in symbols_summary.items():
-        sizes: List[str] = []
-        sizes.append(color_diff(symbol_info['size'], symbol_info['size_diff'], args.diff))
-        for mem_type_name, mem_type_info in symbol_info['memory_types'].items():
-            sizes.append(color_diff(mem_type_info['size'], mem_type_info['size_diff'], args.diff))
-            for section_name, section_info in mem_type_info['sections'].items():
-                sizes.append(color_diff(section_info['size'], section_info['size_diff'], args.diff))
-        name = symbol_info['abbrev_name'] if args.abbrev else symbol_name
-        table.add_row(name, *sizes)
+    sizes_sorted = _get_table_sorted(symbols_summary, table, args)
+    for sizes in sizes_sorted:
+        table.add_row(*sizes)
 
     return table
 
 
 def show_summary(memmap: Dict[str, Any], args: Namespace) -> None:
     show_diff_info(memmap, args)
     table = get_summary_table(memmap, args)
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/format_tree.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/format_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from argparse import Namespace
 from typing import Any, Dict
 
 from rich.tree import Tree
 
-from . import log
+from . import log, memorymap
 from .format_table import color_diff, color_size
 
 
 def show(memmap: Dict[str, Any], args: Namespace) -> None:
 
+    memorymap.sort(memmap, args)
     tree = Tree('Memory Types')
     for mem_type_name, mem_type_info in memmap['memory_types'].items():
         size = color_size(mem_type_info['size'], mem_type_info['size_diff'], args.diff)
         used = color_diff(mem_type_info['used'], mem_type_info['used_diff'], args.diff)
         mem_type_tree = tree.add(f'{mem_type_name} {used} / {size}',
                                  style='dark_orange', guide_style='dark_orange')
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/log.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/log.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/main.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,14 +57,31 @@
                         action='store_true',
                         help=('Print debug information. Messages are printed to stderr.'))
 
     parser.add_argument('-o', '--output-file',
                         metavar='OUTPUT_FILE',
                         help=('Print output to the specified file instead of stdout.'))
 
+    parser.add_argument('-s', '--sort',
+                        metavar='COLUMN',
+                        default=1,
+                        help=('Sort table rows based on specified column number, starting from 0. '
+                              'Column can be specified also as negative number, where -1 means last column. '
+                              'Default is 1 and column 0, containing row description, cannot be used. '
+                              'The name of the column can be utilized in place of its numerical identifier. '
+                              'Applies only to table and csv formats, otherwise ignored.'))
+
+    parser.add_argument('--sort-diff',
+                        action='store_true',
+                        help=('Sort entries based on diff value instead of size.'))
+
+    parser.add_argument('--sort-reverse',
+                        action='store_false',
+                        help=('Sort entries in reversed order. By default descending order is used.'))
+
     parser.add_argument('-q', '--quiet',
                         action='store_true',
                         help=('Suppress all output.'))
 
     parser.add_argument('--no-color',
                         action='store_true',
                         help=('Disable ANSI color escape sequences.'))
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/mapfile.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/mapfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,14 +179,22 @@
                                                       0xc (size before relaxing)
              .rodata.str1.1
                             0x0000000000402013       0x12 test2.o
             '''
             if not output_section['input_sections']:
                 output_section['input_sections'].append(input_section)
                 return
+
+            if (input_section['address'] < output_section['address'] or
+                    input_section['address'] >= output_section['address'] + output_section['size']):
+                # The linker map might include an output section featuring an input section with an address
+                # beyond the range of the output section. Disregard such sections by setting their size to
+                # zero. Note that padding is still considered in the calculation.
+                input_section['size'] = 0
+
             last_input_section = output_section['input_sections'][-1]
             if last_input_section['address'] == input_section['address']:
                 # The current input section is at the same address as the previous one,
                 # so set the previous input section size to 0, because it's not part
                 # of the final image.
                 last_input_section['size'] = 0
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size/ng/memorymap.py` & `esp-idf-size-1.3.0/esp_idf_size/ng/memorymap.py`

 * *Files 8% similar despite different names*

```diff
@@ -382,14 +382,34 @@
                     if depth == OBJECTS:
                         object_info['symbols'] = {}
                         continue
                     object_info['symbols'] = {k: v for k, v in object_info['symbols'].items()
                                               if changed(v['size_diff'])}
 
 
+def sort(memory_map: Dict[str, Any], args: Namespace) -> None:
+    # For memory types diff, sort based on used key, not size key.
+    sort_key_type = 'used_diff' if args.sort_diff else 'used'
+    sort_key = 'size_diff' if args.sort_diff else 'size'
+    reverse = args.sort_reverse
+
+    memory_map['memory_types'] = sort_dict_by_key(memory_map['memory_types'], sort_key_type, reverse)
+    for mem_type_name, mem_type_info in memory_map['memory_types'].items():
+        mem_type_info['sections'] = sort_dict_by_key(mem_type_info['sections'], sort_key, reverse)
+
+        for section_name, section_info in mem_type_info['sections'].items():
+            section_info['archives'] = sort_dict_by_key(section_info['archives'], sort_key, reverse)
+
+            for archive_name, archive_info in section_info['archives'].items():
+                archive_info['object_files'] = sort_dict_by_key(archive_info['object_files'], sort_key, reverse)
+
+                for object_name, object_info in archive_info['object_files'].items():
+                    object_info['symbols'] = sort_dict_by_key(object_info['symbols'], sort_key, reverse)
+
+
 def _get_summary_memory_types(memory_map: Dict[str, Any]) -> Dict[str, Any]:
     # Helper creating memory type/section dictionary for get_*_summary functions.
     mem_types: Dict[str, Any] = {}
 
     for mem_type_name, mem_type_info in memory_map['memory_types'].items():
         mem_types[mem_type_name] = {
             'size': 0,
@@ -402,14 +422,37 @@
                 'size_diff': 0,
                 'abbrev_name': section_info['abbrev_name'],
             }
 
     return mem_types
 
 
+def sort_dict_by_key(dictionary: Dict[str, Any], key: str, reverse: bool) -> Dict[str, Any]:
+        return {k: v for k, v in sorted(dictionary.items(),
+                                        key=lambda item: int(item[1][key]),
+                                        reverse=reverse)}
+
+
+def get_summary_sorted(entries: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
+    sort_key = 'size_diff' if args.sort_diff else 'size'
+    reverse = args.sort_reverse
+
+    entries = {k: v for k, v in sorted(entries.items(),
+                                       key=lambda item: int(item[1][sort_key]),
+                                       reverse=reverse)}
+
+    for entry_name, entry_info in entries.items():
+        entry_info['memory_types'] = sort_dict_by_key(entry_info['memory_types'], sort_key, reverse)
+
+        for mem_type_name, mem_type_info in entry_info['memory_types'].items():
+            mem_type_info['sections'] = sort_dict_by_key(mem_type_info['sections'], sort_key, reverse)
+
+    return entries
+
+
 def get_symbols_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     symbols: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
     found = False
 
     for (mem_type_name, mem_type_info,
@@ -445,18 +488,14 @@
         symbol_mem_type['sections'][section_name]['size_diff'] = size
         symbol_mem_type['size_diff'] += size
         symbol['size_diff'] += size
 
     if not found:
         log.die(f'Archive "{args.archive_details}" not found.')
 
-    symbols = {k: v for k, v in sorted(symbols.items(),
-                                       key=lambda item: int(item[1]['size']),
-                                       reverse=True)}
-
     return symbols
 
 
 def get_object_files_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     object_files: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
@@ -486,18 +525,14 @@
         object_file['size'] += size
 
         size = object_file_info['size_diff']
         object_file_mem_type['sections'][section_name]['size_diff'] = size
         object_file_mem_type['size_diff'] += size
         object_file['size_diff'] += size
 
-    object_files = {k: v for k, v in sorted(object_files.items(),
-                                            key=lambda item: int(item[1]['size']),
-                                            reverse=True)}
-
     return object_files
 
 
 def get_archives_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     archives: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
@@ -526,18 +561,14 @@
         archive['size'] += size
 
         size = archive_info['size_diff']
         archive_mem_type['sections'][section_name]['size_diff'] = size
         archive_mem_type['size_diff'] += size
         archive['size_diff'] += size
 
-    archives = {k: v for k, v in sorted(archives.items(),
-                                        key=lambda item: int(item[1]['size']),
-                                        reverse=True)}
-
     return archives
 
 
 def _filter_memory_regions(memory_regions: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     memory_regions_filtered: List[Dict[str, Any]] = []
 
     for mem_reg in memory_regions:
@@ -640,16 +671,16 @@
         if elf_sections:
             if section['name'] not in elf_sections:
                 # Section does not occupy memory during process execution, no SHF_ALLOC flag.
                 continue
         else:
             # ELF sections are not available. Filter based on output section names.
             if (not section['name'].endswith(('.text', '.data', '.bss', '.rodata', 'noinit', '.vectors')) and
-                    'flash' not in section['name'] and
-                    'eh_frame' not in section['name']):
+                    '.flash' not in section['name'] and
+                    '.eh_frame' not in section['name']):
                 continue
 
         # Remove input sections, which have zero size
         section['input_sections'] = [s for s in section['input_sections'] if s['size']]
         sections_filtered.append(section)
 
     log.debug(f'linker map output sections filtered', sections_filtered)
@@ -896,15 +927,16 @@
 
 
 def _get_image_size(elf_sections: Optional[Dict[str, Any]], sections: List[Dict[str, Any]]) -> int:
     size = 0
     if not elf_sections:
         # ELF information not available
         for sec in sections:
-            if sec['name'].endswith('.bss'):
+            # NOLOAD(SHT_NOBITS) sections are not part of the image
+            if sec['name'].endswith(('.bss', 'noinit')):
                 continue
             size += sec['size']
         return size
 
     for name, info in elf_sections.items():
         if info['sh_type'] != 'SHT_PROGBITS':
             continue
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size.egg-info/PKG-INFO` & `esp-idf-size-1.3.0/esp_idf_size.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 1.2.0
+Version: 1.3.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-1.2.0/esp_idf_size.egg-info/SOURCES.txt` & `esp-idf-size-1.3.0/esp_idf_size.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 esp_idf_size.egg-info/requires.txt
 esp_idf_size.egg-info/top_level.txt
 esp_idf_size/chip_info/esp32.yaml
 esp_idf_size/chip_info/esp32c2.yaml
 esp_idf_size/chip_info/esp32c3.yaml
 esp_idf_size/chip_info/esp32c5.yaml
 esp_idf_size/chip_info/esp32c6.yaml
+esp_idf_size/chip_info/esp32c61.yaml
 esp_idf_size/chip_info/esp32h2.yaml
 esp_idf_size/chip_info/esp32h4.yaml
 esp_idf_size/chip_info/esp32p4.yaml
 esp_idf_size/chip_info/esp32s2.yaml
 esp_idf_size/chip_info/esp32s3.yaml
 esp_idf_size/ng/__init__.py
 esp_idf_size/ng/__main__.py
```

### Comparing `esp-idf-size-1.2.0/setup.py` & `esp-idf-size-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.2.0/test/test_idf_size.py` & `esp-idf-size-1.3.0/test/test_idf_size.py`

 * *Files identical despite different names*

