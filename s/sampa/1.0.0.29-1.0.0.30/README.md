# Comparing `tmp/sampa-1.0.0.29.tar.gz` & `tmp/sampa-1.0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.29.tar", last modified: Sun Apr 14 20:52:09 2024, max compression
+gzip compressed data, was "sampa-1.0.0.30.tar", last modified: Mon Apr 15 01:53:02 2024, max compression
```

## Comparing `sampa-1.0.0.29.tar` & `sampa-1.0.0.30.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.456330 sampa-1.0.0.29/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.29/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2024-04-14 20:52:09.456330 sampa-1.0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.29/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.380536 sampa-1.0.0.29/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.29/sampa/__init__.py
--rw-rw-rw-   0        0        0     8200 2024-04-14 20:51:58.000000 sampa-1.0.0.29/sampa/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.432432 sampa-1.0.0.29/sampa/src/
--rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.29/sampa/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.446299 sampa-1.0.0.29/sampa/src/INPUTS/
--rw-rw-rw-   0        0        0      227 2024-04-11 17:38:09.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      268 2024-04-11 17:38:16.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      222 2024-04-11 17:38:23.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      263 2024-04-11 17:38:30.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      211 2024-04-11 17:38:37.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      252 2024-04-11 17:38:44.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      200 2024-04-11 17:38:57.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      213 2024-04-11 17:39:09.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      254 2024-04-11 17:39:15.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_scf.SO
--rw-rw-rw-   0        0        0      198 2024-04-11 17:39:53.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_xy-scan
--rw-rw-rw-   0        0        0      198 2024-04-11 17:39:53.000000 sampa-1.0.0.29/sampa/src/INPUTS/INCAR_z-scan
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.455337 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.29/sampa/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     2678 2024-04-14 20:41:50.000000 sampa-1.0.0.29/sampa/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.29/sampa/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.29/sampa/src/bader
--rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.29/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.29/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.29/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.29/sampa/src/chgsum.pl
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.29/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0      633 2024-04-14 20:51:39.000000 sampa-1.0.0.29/sampa/src/energy_scan.py
--rw-rw-rw-   0        0        0    12893 2024-04-14 20:11:17.000000 sampa-1.0.0.29/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.29/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    19701 2024-04-14 19:48:31.000000 sampa-1.0.0.29/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     4765 2024-04-14 14:20:19.000000 sampa-1.0.0.29/sampa/src/output.py
--rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.29/sampa/src/potcar.py
--rw-rw-rw-   0        0        0      284 2024-04-13 18:15:55.000000 sampa-1.0.0.29/sampa/src/scan_update.py
--rw-rw-rw-   0        0        0     7559 2024-04-14 20:39:23.000000 sampa-1.0.0.29/sampa/src/xy-scan.py
--rw-rw-rw-   0        0        0     9028 2024-04-14 20:39:11.000000 sampa-1.0.0.29/sampa/src/z-scan.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:52:09.398744 sampa-1.0.0.29/sampa.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1447 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-14 20:52:09.000000 sampa-1.0.0.29/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-14 20:52:09.458586 sampa-1.0.0.29/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-14 20:51:51.000000 sampa-1.0.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.421421 sampa-1.0.0.30/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.30/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2024-04-15 01:53:02.421421 sampa-1.0.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.30/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.296202 sampa-1.0.0.30/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.30/sampa/__init__.py
+-rw-rw-rw-   0        0        0     8200 2024-04-15 01:52:26.000000 sampa-1.0.0.30/sampa/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.384824 sampa-1.0.0.30/sampa/src/
+-rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.30/sampa/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.406742 sampa-1.0.0.30/sampa/src/INPUTS/
+-rw-rw-rw-   0        0        0      227 2024-04-11 17:38:09.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      268 2024-04-11 17:38:16.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      222 2024-04-11 17:38:23.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      263 2024-04-11 17:38:30.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      211 2024-04-11 17:38:37.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      252 2024-04-11 17:38:44.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      200 2024-04-11 17:38:57.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      213 2024-04-11 17:39:09.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      254 2024-04-11 17:39:15.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_scf.SO
+-rw-rw-rw-   0        0        0      198 2024-04-11 17:39:53.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_xy-scan
+-rw-rw-rw-   0        0        0      198 2024-04-11 17:39:53.000000 sampa-1.0.0.30/sampa/src/INPUTS/INCAR_z-scan
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.419156 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.30/sampa/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     2678 2024-04-14 20:41:50.000000 sampa-1.0.0.30/sampa/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.30/sampa/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.30/sampa/src/bader
+-rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.30/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.30/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.30/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.30/sampa/src/chgsum.pl
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.30/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0      595 2024-04-15 00:29:04.000000 sampa-1.0.0.30/sampa/src/energy_scan.py
+-rw-rw-rw-   0        0        0    12898 2024-04-15 01:48:11.000000 sampa-1.0.0.30/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.30/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    19711 2024-04-15 01:47:36.000000 sampa-1.0.0.30/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     4738 2024-04-15 01:46:05.000000 sampa-1.0.0.30/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.30/sampa/src/potcar.py
+-rw-rw-rw-   0        0        0     7559 2024-04-14 20:39:23.000000 sampa-1.0.0.30/sampa/src/xy-scan.py
+-rw-rw-rw-   0        0        0     3176 2024-04-15 01:52:04.000000 sampa-1.0.0.30/sampa/src/xy-scan_update.py
+-rw-rw-rw-   0        0        0     9028 2024-04-14 20:39:11.000000 sampa-1.0.0.30/sampa/src/z-scan.py
+-rw-rw-rw-   0        0        0     1420 2024-04-15 01:43:57.000000 sampa-1.0.0.30/sampa/src/z-scan_update.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:53:02.344829 sampa-1.0.0.30/sampa.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1477 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 01:53:02.000000 sampa-1.0.0.30/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-15 01:53:02.424422 sampa-1.0.0.30/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-15 01:52:18.000000 sampa-1.0.0.30/setup.py
```

### Comparing `sampa-1.0.0.29/sampa/__main__.py` & `sampa-1.0.0.30/sampa/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pyfiglet
 import shutil
 import time
 import sys
 import os
 
 
-version = '1.0.0.29'
+version = '1.0.0.30'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
```

### Comparing `sampa-1.0.0.29/sampa/src/HeteroStructure_Generator.py` & `sampa-1.0.0.30/sampa/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `sampa-1.0.0.30/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/SAMBA_HeteroStructure.input` & `sampa-1.0.0.30/sampa/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/SAMBA_WorkFlow.input` & `sampa-1.0.0.30/sampa/src/SAMBA_WorkFlow.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/_info_pseudo.py` & `sampa-1.0.0.30/sampa/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/bader` & `sampa-1.0.0.30/sampa/src/bader`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/bader_poscar.py` & `sampa-1.0.0.30/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/bader_update.py` & `sampa-1.0.0.30/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/charge_transfer.py` & `sampa-1.0.0.30/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/chgsum.pl` & `sampa-1.0.0.30/sampa/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/energy_scan.py` & `sampa-1.0.0.30/sampa/src/energy_scan.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,12 +12,11 @@
 else:  energy = open('../energy_scan.txt', "w")
 
 with open('OSZICAR') as file:
     lines = file.readlines()
 VTemp = lines[-1].strip()
 
 energia = VTemp.replace('=',' ').split()
-name_dir = name_dir.replace('_',' ')
 
 energy.write(f'{name_dir} {energia[4]} \n')
 
 energy.close()
```

### Comparing `sampa-1.0.0.29/sampa/src/job.py` & `sampa-1.0.0.30/sampa/src/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 job.write(f'               $vasp_std \n')
 job.write(f'               rm -r CHG CHGCAR DOSCAR PROCAR WAVECAR EIGENVAL IBZKPT vasprun.xml \n')
 job.write(f'               bzip2 OUTCAR \n')
 job.write(f'               python3 energy_scan.py \n')
 job.write(f'           done \n')
 job.write(f'           #------------- \n')
 job.write(f'           cd $dir0/$i/$j \n')
-job.write(f'           python3 scan_update.py \n')
+job.write(f'           python3 z-scan_update.py \n')
 job.write(f'           for k in "{tasks}"; do \n')
 job.write(f'               if [ "$k" != "z-scan" ]; then \n')
 job.write(f'                  cp  $dir0/$i/$j/POSCAR  $dir0/$i/$k/POSCAR \n')
 job.write(f'               fi \n')
 job.write(f'           done \n')
 job.write(f'        #---------------------------------------------------------------------------- \n')
 job.write(f'        elif [ "$j" == "xy-scan" ]; then \n')
@@ -99,15 +99,15 @@
 job.write(f'               $vasp_std \n')
 job.write(f'               rm -r CHG CHGCAR DOSCAR PROCAR WAVECAR EIGENVAL IBZKPT vasprun.xml \n')
 job.write(f'               bzip2 OUTCAR \n')
 job.write(f'               python3 energy_scan.py \n')
 job.write(f'           done \n')
 job.write(f'           #------------- \n')
 job.write(f'           cd $dir0/$i/$j \n')
-job.write(f'           python3 scan_update.py \n')
+job.write(f'           python3 xy-scan_update.py \n')
 job.write(f'           for k in "{tasks}"; do \n')
 job.write(f'               if [[ "$k" != "z-scan" && "$k" != "xy-scan" ]]; then \n')
 job.write(f'                  cp  $dir0/$i/$j/POSCAR  $dir0/$i/$k/POSCAR \n')
 job.write(f'               fi \n')
 job.write(f'           done \n')
 job.write(f'        #---------------------------------------------------------------------------- \n')
 job.write(f'        elif [ "$j" == "relax" ]; then \n')
```

### Comparing `sampa-1.0.0.29/sampa/src/kpoints.py` & `sampa-1.0.0.30/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/make_files.py` & `sampa-1.0.0.30/sampa/src/make_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         #==================================================
         dir_task = dir_out + '/' + files[i] + '/' + task[j]
         #==================================================
         os.mkdir(dir_task)
         shutil.copyfile(dir_files + '/Structures' + '/' + files[i], dir_task + '/POSCAR')
         #================================================================================
         if (task[j] == 'z-scan'):
-           shutil.copyfile(dir_codes + '/scan_update.py', dir_task + '/scan_update.py')
+           shutil.copyfile(dir_codes + '/z-scan_update.py', dir_task + '/z-scan_update.py')
            shutil.copyfile(dir_codes + '/energy_scan.py', dir_task + '/energy_scan.py')
            shutil.copyfile(dir_codes + '/z-scan.py', dir_task + '/z-scan.py')
            #---------------------------------------------------------------------------
-           # Atualizando o arquivo xy-scan.py -----------------------------------------
+           # Atualizando o arquivo z-scan.py ------------------------------------------
            #---------------------------------------------------------------------------
            with open(dir_task + '/z-scan.py', "r") as file:  content = file.read()
            content = content.replace('replace_deltaZ_i', str(deltaZ_i))
            content = content.replace('replace_deltaZ_f', str(deltaZ_f))
            content = content.replace('replace_passo_z', str(passo_z))
            content = content.replace('replace_vacuo', str(vacuo))
            with open(dir_task + '/z-scan.py', "w") as file: file.write(content)
         #=============================================
         if (task[j] == 'xy-scan'):
-           shutil.copyfile(dir_codes + '/scan_update.py', dir_task + '/scan_update.py')
+           shutil.copyfile(dir_codes + '/xy-scan_update.py', dir_task + '/xy-scan_update.py')
            shutil.copyfile(dir_codes + '/energy_scan.py', dir_task + '/energy_scan.py')
            shutil.copyfile(dir_codes + '/xy-scan.py', dir_task + '/xy-scan.py')
            #---------------------------------------------------------------------------
            # Atualizando o arquivo xy-scan.py -----------------------------------------
            #---------------------------------------------------------------------------
            with open(dir_task + '/xy-scan.py', "r") as file:  content = file.read()
            content = content.replace('replace_displacement_A1', str(displacement_A1))
```

### Comparing `sampa-1.0.0.29/sampa/src/output.py` & `sampa-1.0.0.30/sampa/src/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 for i in range(len(folders)):
     #-----------------------------------
     dir_folders = folders[i] + '/output'
     #-----------------------------------
     if (folders[i] == 'z-scan'):
        os.mkdir('output/z-scan') 
-       if os.path.isfile(folders[i] + '/energy_scan.txt'):  shutil.copy(folders[i] + '/energy_scan.txt',  'output/z-scan/energy_scan.txt')
+       if os.path.isfile(folders[i] + '/z-scan.dat'):  shutil.copy(folders[i] + '/z-scan.dat',  'output/z-scan/z-scan.dat')
        if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/z-scan/POSCAR_z-scan')
     #--------------------------------
     if (folders[i] == 'xy-scan'):
        os.mkdir('output/xy-scan') 
-       if os.path.isfile(folders[i] + '/energy_scan.txt'):  shutil.copy(folders[i] + '/energy_scan.txt',  'output/xy-scan/energy_scan.txt')
+       if os.path.isfile(folders[i] + '/xy-scan.dat'):  shutil.copy(folders[i] + '/xy-scan.dat',  'output/xy-scan/xy-scan.dat')
        if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/xy-scan/POSCAR_xy-scan')
     #--------------------------------
     if (folders[i] == 'scf'):
        if os.path.isdir(dir_folders + '/Potencial'):  shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_scf')
        if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'scf.SO'):
```

### Comparing `sampa-1.0.0.29/sampa/src/potcar.py` & `sampa-1.0.0.30/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/xy-scan.py` & `sampa-1.0.0.30/sampa/src/xy-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa/src/z-scan.py` & `sampa-1.0.0.30/sampa/src/z-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.29/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.30/sampa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 sampa/src/contcar_update.py
 sampa/src/energy_scan.py
 sampa/src/job.py
 sampa/src/kpoints.py
 sampa/src/make_files.py
 sampa/src/output.py
 sampa/src/potcar.py
-sampa/src/scan_update.py
 sampa/src/xy-scan.py
+sampa/src/xy-scan_update.py
 sampa/src/z-scan.py
+sampa/src/z-scan_update.py
 sampa/src/INPUTS/INCAR_bader
 sampa/src/INPUTS/INCAR_bader.SO
 sampa/src/INPUTS/INCAR_bands
 sampa/src/INPUTS/INCAR_bands.SO
 sampa/src/INPUTS/INCAR_dos
 sampa/src/INPUTS/INCAR_dos.SO
 sampa/src/INPUTS/INCAR_relax
```

### Comparing `sampa-1.0.0.29/setup.py` & `sampa-1.0.0.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.29",
+    version = "1.0.0.30",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

