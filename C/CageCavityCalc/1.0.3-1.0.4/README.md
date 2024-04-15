# Comparing `tmp/CageCavityCalc-1.0.3.tar.gz` & `tmp/CageCavityCalc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CageCavityCalc-1.0.3.tar", last modified: Wed Sep  6 18:50:16 2023, max compression
+gzip compressed data, was "CageCavityCalc-1.0.4.tar", last modified: Mon Apr 15 18:26:50 2024, max compression
```

## Comparing `CageCavityCalc-1.0.3.tar` & `CageCavityCalc-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,220 @@
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.885021 CageCavityCalc-1.0.3/
--rw-r--r--   0 chem1540 (20152) fd        (6900)        7 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/.gitignore
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.878021 CageCavityCalc-1.0.3/.idea/
--rw-r--r--   0 chem1540 (20152) fd        (6900)       39 2022-09-12 17:18:36.000000 CageCavityCalc-1.0.3/.idea/.gitignore
--rw-r--r--   0 chem1540 (20152) fd        (6900)      552 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.3/.idea/CageCavityCalc.iml
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.878021 CageCavityCalc-1.0.3/.idea/inspectionProfiles/
--rw-r--r--   0 chem1540 (20152) fd        (6900)      174 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      194 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.3/.idea/misc.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      280 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.3/.idea/modules.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      180 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.3/.idea/vcs.xml
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.882021 CageCavityCalc-1.0.3/CageCavityCalc/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    28820 2023-09-06 18:31:13.000000 CageCavityCalc-1.0.3/CageCavityCalc/CageCavityCalc.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)       90 2023-09-06 16:21:44.000000 CageCavityCalc-1.0.3/CageCavityCalc/__init__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     4443 2023-09-06 13:18:08.000000 CageCavityCalc-1.0.3/CageCavityCalc/__main__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1862 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.3/CageCavityCalc/calculations.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18977 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/data.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     2902 2023-09-06 16:22:06.000000 CageCavityCalc-1.0.3/CageCavityCalc/electrostatics.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     3843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/grid_classes.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     2773 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.3/CageCavityCalc/hydrophobicity.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    10095 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.3/CageCavityCalc/input_output.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)      843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/log.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.884021 CageCavityCalc-1.0.3/CageCavityCalc/old/
--rw-r--r--   0 chem1540 (20152) fd        (6900)        0 2023-09-06 12:53:06.000000 CageCavityCalc-1.0.3/CageCavityCalc/old/__init__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    19237 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/old/cavity_calculator_v08.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    44930 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/old/main_06-09-21_vicente.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    46895 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/old/main_06-09-21_vicente_tomasz.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    27884 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/CageCavityCalc/old/main_21-5-20_tomasz.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.885021 CageCavityCalc-1.0.3/CageCavityCalc/pymol_plugin/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    10170 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.3/CageCavityCalc/pymol_plugin/__init__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1065 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.3/CageCavityCalc/pymol_plugin/simple.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     3962 2023-09-06 13:17:45.000000 CageCavityCalc-1.0.3/CageCavityCalc/window_size.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2023-09-06 18:50:16.883021 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/
--rw-r--r--   0 chem1540 (20152) fd        (6900)       80 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/PKG-INFO
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1048 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/SOURCES.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)        1 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/dependency_links.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       64 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/entry_points.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       31 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/requires.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       15 2023-09-06 18:50:16.000000 CageCavityCalc-1.0.3/CageCavityCalc.egg-info/top_level.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/LICENSE
--rw-r--r--   0 chem1540 (20152) fd        (6900)       80 2023-09-06 18:50:16.885021 CageCavityCalc-1.0.3/PKG-INFO
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1692 2023-09-06 13:48:36.000000 CageCavityCalc-1.0.3/README.md
--rw-r--r--   0 chem1540 (20152) fd        (6900)      296 2023-09-06 18:50:09.000000 CageCavityCalc-1.0.3/pyproject.toml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      261 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.3/readme_testing.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       38 2023-09-06 18:50:16.885021 CageCavityCalc-1.0.3/setup.cfg
--rw-r--r--   0 chem1540 (20152) fd        (6900)      359 2023-09-06 18:50:04.000000 CageCavityCalc-1.0.3/setup.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.539184 CageCavityCalc-1.0.4/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        7 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/.gitignore
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.507183 CageCavityCalc-1.0.4/.idea/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       39 2022-09-12 17:18:36.000000 CageCavityCalc-1.0.4/.idea/.gitignore
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      552 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/CageCavityCalc.iml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.508183 CageCavityCalc-1.0.4/.idea/inspectionProfiles/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      174 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      194 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/misc.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      280 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/modules.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      180 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/vcs.xml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.509183 CageCavityCalc-1.0.4/CageCavityCalc/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    29950 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/CageCavityCalc.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       90 2023-09-06 16:21:44.000000 CageCavityCalc-1.0.4/CageCavityCalc/__init__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     4446 2024-04-12 14:48:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/__main__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1862 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/calculations.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18977 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/data.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3248 2024-04-12 14:52:13.000000 CageCavityCalc-1.0.4/CageCavityCalc/electrostatics.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.506183 CageCavityCalc-1.0.4/CageCavityCalc/examples/
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.510183 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   190548 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      245 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/example_10.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.510183 CageCavityCalc-1.0.4/CageCavityCalc/examples/11_errors/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      332 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/11_errors/example_11.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.513183 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   342847 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_1.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    80747 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_2.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    81842 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_3.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   118370 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_4.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    93217 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_5.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    87207 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_6.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11688 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     8219 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    73728 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.spartan
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   188164 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_box_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30968 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      250 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   626971 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      137 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   255592 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_extra_data.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      973 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_hydrophobicity_cavity_dummy_atoms.txt
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11744 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    85162 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       97 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    20960 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    28203 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    25196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49454 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   100017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   178145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   162704 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   340174 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17348 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    24016 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    21656 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40369 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    26387 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    45188 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    22922 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40290 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     7146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_ACIE_2016-CCDC_1492902.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10812 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    53167 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      143 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    33191 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    50718 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      129 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    39579 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      134 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    78911 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30924 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    48269 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      142 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    15997 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_24_OrgLett_2010_12_1740_cage_ol.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    13100 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18012 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    58196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   138645 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    29116 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49770 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      121 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18844 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    25991 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      117 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57771 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   144017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    35519 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    22910 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      141 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57359 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30189 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    88796 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     6662 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      128 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     8078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   110284 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   140936 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   141884 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    64640 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    87532 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      264 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      400 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/example_14.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     9129 2022-12-08 14:47:43.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/ncage.xyz
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/15_from_table/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40230 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/15_from_table/example_15.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.525184 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   342187 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       92 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      246 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/example_1.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   151889 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    83899 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.xyz
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18404 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   210710 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63831 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   106484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_box_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   118804 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   524484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      186 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/example_2.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   231083 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/file.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/test/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/test/cage_ACIE_2006_45_901.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      300 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/example_3.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/file.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.529184 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      243 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/example_4.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.529184 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    25859 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30224 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage_cavity.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      152 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/example_5.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.530184 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1068 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/.short.xtc_offsets.npz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      265 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/example_6.py
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    21919 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.gro
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    11948 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.xtc
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.530184 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57903 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   496989 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       62 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/run.sh
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.532184 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16384 2023-07-25 17:12:29.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/.cage_cavity_hydrophobicity.pdb.swp
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_1_JACS_2006_128_14120.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_aromatic_contact.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:22.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_esp.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      263 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_solvent_accessibility.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      472 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/example_8.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.533184 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   157210 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/cage.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      519 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/example_9.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.534184 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    34049 2022-09-14 14:09:50.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_replace_spaces_before_after_Pd.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    28352 2022-09-14 15:28:29.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-14 15:29:14.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    37525 2022-09-14 15:30:50.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity_cluster.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   161261 2022-09-12 17:13:04.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   201845 2022-09-12 17:22:41.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/grid_classes.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     2773 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/hydrophobicity.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10095 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/input_output.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/log.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.537184 CageCavityCalc-1.0.4/CageCavityCalc/pic/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   453532 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/cage.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   425171 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/cavity.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   531480 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/hydrophobicity.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   619706 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle
+-rw-r--r--   0 chem1540 (20152) fd        (6900)  1051047 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   619827 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.svg
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.538184 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10170 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/__init__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    12998 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/cavecav_widget.ui
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1065 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/simple.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3962 2023-09-06 13:17:45.000000 CageCavityCalc-1.0.4/CageCavityCalc/window_size.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.509183 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/PKG-INFO
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11321 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        1 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       64 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/entry_points.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       31 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/requires.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       15 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/top_level.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/LICENSE
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-04-15 18:26:50.538184 CageCavityCalc-1.0.4/PKG-INFO
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1697 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/README.md
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      296 2024-04-15 18:26:23.000000 CageCavityCalc-1.0.4/pyproject.toml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      261 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/readme_testing.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        0 2023-09-06 12:38:38.000000 CageCavityCalc-1.0.4/requirements.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       38 2024-04-15 18:26:50.539184 CageCavityCalc-1.0.4/setup.cfg
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      359 2023-09-06 18:50:04.000000 CageCavityCalc-1.0.4/setup.py
```

### Comparing `CageCavityCalc-1.0.3/.idea/CageCavityCalc.iml` & `CageCavityCalc-1.0.4/.idea/CageCavityCalc.iml`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/CageCavityCalc.py` & `CageCavityCalc-1.0.4/CageCavityCalc/CageCavityCalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,15 +141,19 @@
     def calculate_center_and_radius(self):
         #Calculate the center of mass of the cage using RDKit
         pore_center_of_mass = np.array(sum(self.atom_masses[i]*self.positions[i] for i in range(self.n_atoms)))/sum(self.atom_masses)
         logger.info(f"center_of_mass= {pore_center_of_mass:}")
 
         #We use the center of mass of the molecule as the pore center of mass
         kdtxyzAtoms = KDTree(self.positions, leafsize = 20) #Calculate the KDTree of the cage atom positions
-        distancesFromCOM = kdtxyzAtoms.query(pore_center_of_mass, k = None, p = 2)
+        distancesFromCOM = kdtxyzAtoms.query(pore_center_of_mass, k = self.n_atoms, p = 2)
+        #print("++++++++++++++++++++++++++++++++++++++++++")
+        #print("distancesFromCOM: ")
+        #print(distancesFromCOM)
+        #print(len(distancesFromCOM))
         maxDistanceFromCOM = (distancesFromCOM[0][-1])
         pore_radius = distancesFromCOM[0][0]*self.distanceFromCOMFactor
         '''
         #Determine the atom types and correct the pore radius  with the atom radius of the cage. We use the max radius of the different cage atom types
         atomTypesInCage = list(dict.fromkeys(self.atom_names))
         print(atomTypesInCage)
         atomTypesInCageRadius=[*map(vdw_radii.get, atomTypesInCage)]
@@ -225,23 +229,37 @@
                     vect1Norm = (np.array(pore_center_of_mass)-np.array(i.pos)) / dist1
             if dist1 < pore_radius:
                     i.inside_cavity = 1
             if i.inside_cavity == 0:
                 summAngles = []
                 distancesAngles = []
                 for atom_type in self.atom_type_list:
-                    xyzAtomsSet2 = self.KDTree_dict[atom_type].query(i.pos, k = None, p = 2,
+                    xyzAtomsSet2 = self.KDTree_dict[atom_type].query(i.pos, k = self.n_atoms, p = 2,
                                                                 distance_upper_bound = self.distance_threshold_for_90_deg_angle)
-                    if xyzAtomsSet2[1]:
+
+
+
+
+                    #print("xyzAtomsSet2[0]:",xyzAtomsSet2[0])
+                    for index_atom_iter in range(0, len(xyzAtomsSet2[0])):
+                        if xyzAtomsSet2[0][index_atom_iter] == math.inf:
+                            index_inf = index_atom_iter
+                            xyzAtomsSet3_dist = xyzAtomsSet2[0][:index_inf]
+                            xyzAtomsSet3_index = xyzAtomsSet2[1][:index_inf]
+                            break
+
+                    #print("xyzAtomsSet3_dist:",xyzAtomsSet3_dist)
+                    if len(xyzAtomsSet3_dist) > 0:
+                        #print("if xyzAtomsSet2[1]:",xyzAtomsSet2[0])
                         vdwR = vdwR_dict[atom_type][0]
                         distThreshold = vdwR + vdwRdummy
-                        if xyzAtomsSet2[0][0] < distThreshold:
+                        if xyzAtomsSet3_dist[0] < distThreshold:
                             i.overlapping_with_cage = 1
 
-                        for atom_pos_index in xyzAtomsSet2[1]:
+                        for atom_pos_index in xyzAtomsSet3_index:
                             atom_pos = coords_dict[atom_type][atom_pos_index]
                             dist2 = np.linalg.norm(np.array(atom_pos)-np.array(i.pos))
                             vect2Norm = (np.array(atom_pos)-np.array(i.pos)) / dist2
                             angle = np.arccos(np.dot(vect1Norm, vect2Norm))
                             summAngles.append(angle)
                             distancesAngles.append(1/(1+dist2))
                 if (summAngles):
@@ -258,16 +276,16 @@
             if i.inside_cavity == 1:
                 calculatedGirdContacts.append(i.pos)
         calculatedGirdContactsKDTree = KDTree(calculatedGirdContacts, leafsize = 20)
 
         # Calculate the number of neighbors for each dummy atom. From 1 to 7 (as 1 contact is always, the atom itself)
         for i, dummy_atom in enumerate(calculatedGird.grid):
             if dummy_atom.inside_cavity == 1:
-                xyzDummySet = calculatedGirdContactsKDTree.query(dummy_atom.pos, k=None, p=2, distance_upper_bound=1.1*self.grid_spacing)
-                dummy_atom.number_of_neighbors = len(xyzDummySet[1])
+                xyzDummySet = calculatedGirdContactsKDTree.query_ball_point(dummy_atom.pos, r=1.1*self.grid_spacing, p=2)
+                dummy_atom.number_of_neighbors = len(xyzDummySet)
         
         if self.clustering_to_remove_cavity_noise != "false":
             cavity_dummy_atoms_positions = []
             cavity_dummy_atoms_index = []
             for i, dummy_atom in enumerate(calculatedGird.grid):
                 if dummy_atom.inside_cavity == 1:
                     cavity_dummy_atoms_positions.append([dummy_atom.x,dummy_atom.y,dummy_atom.z])
@@ -492,44 +510,50 @@
             #if (printLevel == 2): fileExtraData.write("-------------\n")
             dummy_hydrophobicity = []
             dummy_aromatic_contacts = []
             dummy_solvent_accessibility = []
 
             for atom_type in self.atom_type_list:
 
-                dist = self.KDTree_dict[atom_type].query(dummy_atom, k=None, p=2,
+                dist = self.KDTree_dict[atom_type].query(dummy_atom, k=self.n_atoms, p=2,
                                                     distance_upper_bound=self.distThreshold_atom_contacts)
                 '''
                 if (printLevel == 2):
                     fileExtraData.write(str(atom_type) + ": " + str(dist[0]) + "\n")
                     fileExtraData.write(str(atom_type) + " Index: " + str(
                         [x + 1 for x in dist[1]]) + "\n")  # Add 1 to key as atom number starts with 1 and list number with 0
                     fileExtraData.write("Global Index: " + str([atomTypes_HydrophValues_dict[atom_type].get(key + 1) for key in
                                                                 dist[1]]) + "\n")  # Add 1 to key as atom number starts with 1 and list number with 0
                 '''
+                for index_atom_iter in range(0, len(dist[0])):
+                    if dist[0][index_atom_iter] == math.inf:
+                        index_inf = index_atom_iter
+                        dist_dist = dist[0][:index_inf]
+                        dist_index = dist[1][:index_inf]
+                        break
 
-                if dist[0]:
-                    for k in range(0, len(dist[0])):
+                if len(dist_dist) > 0:
+                    for k in range(0, len(dist_dist)):
 
                         # calculate hydrophobicity
-                        Hydroph_Value = atomTypesMeanListHydrophValues[atomTypes_HydrophValues_dict[atom_type][1 + dist[1][
+                        Hydroph_Value = atomTypesMeanListHydrophValues[atomTypes_HydrophValues_dict[atom_type][1 + dist_index[
                             k]] - 1]  # we need to add +1 to the k index as atom numbering is starts at 1 and lists index at 0. After taht, we need to add -1 to the atom index from the dict to obtain the value from the list that starts from 0
 
-                        hydro = calc_single_hydrophobicity(dist[0][k], Hydroph_Value, self.distance_function)
+                        hydro = calc_single_hydrophobicity(dist_dist[k], Hydroph_Value, self.distance_function)
                         dummy_hydrophobicity.append(hydro)
 
                         #calculate aromatic contact
-                        isAromatic = rdkit_cage.GetAtomWithIdx(self.atom_idx_dict[atom_type][dist[1][k]]).GetIsAromatic()
+                        isAromatic = rdkit_cage.GetAtomWithIdx(self.atom_idx_dict[atom_type][dist_index[k]]).GetIsAromatic()
                         if isAromatic == True:
-                            dummy_aromatic_contacts.append(1 / (1 + dist[0][k]))
+                            dummy_aromatic_contacts.append(1 / (1 + dist_dist[k]))
                         else:
                             dummy_aromatic_contacts.append(0)
 
                         #calculate solvent accessibility
-                        dummy_solvent_accessibility.append(1/dist[0][k])
+                        dummy_solvent_accessibility.append(1/dist_dist[k])
 
             self.hydrophobicity.append(np.sum(dummy_hydrophobicity))
             self.aromatic_constacts.append(np.sum(dummy_aromatic_contacts))
             self.solvent_accessibility.append(np.sum(dummy_solvent_accessibility))
 
         '''
         elif compute_aromatic_contacts == True:
@@ -543,15 +567,15 @@
         total_cavity_hydrophobicity = average_cavity_hydrophobicity * self.volume
         logger.info(f"Hydrophobicity method and distance function = {self.hydrophMethod}, {self.distance_function}")
         logger.info(f"Average cavity hydrophobicity = {average_cavity_hydrophobicity:.2f} A^-3")
         logger.info(f"Total cavity hydrophobicity = {total_cavity_hydrophobicity:.2f}")
         return self.hydrophobicity
 
     def calculate_esp(self, metal_name=None, metal_charge=None, method='eem', max_memory=1e9):
-        factor = (8.987551792e10)*(1.602176634e-19)*(1e10) #(Coulomb constant)*(elementary charge)/ Angstrom
+        factor = (8.987551792e9)*(1.602176634e-19)*(1e10) #(Coulomb constant)*(elementary charge)/ Angstrom
 
         partial_charges = calculate_partial_charges(self.positions, self.atom_names, method=method, metal_name=metal_name, metal_charge=metal_charge)
 
         if len(self.dummy_atoms_positions) * len(self.positions) * 8 < max_memory:
             dist_matrix = distance_matrix(self.dummy_atoms_positions, self.positions)
             grid_charges = (factor / dist_matrix).dot(partial_charges)
         else:
@@ -563,7 +587,8 @@
         self.esp_grid = grid_charges
 
     def calculate_window(self):
 
         self.window_radius = get_max_escape_sphere(self.positions, self.atom_names)
         return self.window_radius
 
+
```

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/__main__.py` & `CageCavityCalc-1.0.4/CageCavityCalc/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         cavity_hydrophobicity_values = cav.calculate_hydrophobicity()
         average_cavity_hydrophobicity = np.mean(cavity_hydrophobicity_values)
         print(f"Hydrophobicity method and distance function = {cav.hydrophMethod}, {cav.distance_function}")
         print(f"Average cavity hydrophobicity = {average_cavity_hydrophobicity:.5f} A^-3")
         print(f"Total cavity hydrophobicity = {average_cavity_hydrophobicity * volume:.5f}")
         mlp_pos = [i for i in cavity_hydrophobicity_values if i > 0]
         mlp_neg = [i for i in cavity_hydrophobicity_values if i < 0]
-        lipophilic_index = sum(mlp_pos) / (sum(mlp_pos) - sum(mlp_neg))
-        print(f"Lipophilic_index (LI) = {lipophilic_index:.3f}")
+        hydrophobic_index = sum(mlp_pos) / (sum(mlp_pos) - sum(mlp_neg))
+        print(f"Hydrophobic_index (HI) = {hydrophobic_index:.3f}")
 
         cav.print_to_file(args.o, 'h')
         if args.pymol == True:
             pymol_filename = args.o[:args.o.find('.')] + ".pml"
             cav.print_to_pymol(pymol_filename, 'h')
     else:
         cav.print_to_file(args.o)
```

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/calculations.py` & `CageCavityCalc-1.0.4/CageCavityCalc/calculations.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/data.py` & `CageCavityCalc-1.0.4/CageCavityCalc/data.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/electrostatics.py` & `CageCavityCalc-1.0.4/CageCavityCalc/electrostatics.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,16 +31,23 @@
 
     tmpdir_path = mkdtemp()
     print_to_pdb_file(tmpdir_path + "/temp.pdb", positions, atom_names)
 
     ob_conversion = openbabel.OBConversion()
     ob_conversion.SetInAndOutFormats("pdb", "mol2")
 
+    # We firstly change pdb -> mol2, because charges are not assigned correctly when used with pdb
     mol = openbabel.OBMol()
     ob_conversion.ReadFile(mol, tmpdir_path + "/temp.pdb")
+    ob_conversion.WriteFile(mol, tmpdir_path + "/temp.mol2")
+    ob_conversion.SetInAndOutFormats("mol2", "mol2")
+
+    mol = openbabel.OBMol()
+    ob_conversion.ReadFile(mol, tmpdir_path + "/temp.mol2")
+
 
     ob_charge_model = openbabel.OBChargeModel.FindType(method)
 
     is_calculated = ob_charge_model.ComputeCharges(mol)
 
     if is_calculated:
         return ob_charge_model.GetPartialCharges()
@@ -54,9 +61,10 @@
         positions = np.delete(positions, list_of_metals, axis=0)
         atom_names = np.delete(atom_names, list_of_metals)
         partial_charges = list(calculate_partial_charges_using_ob(positions, atom_names, method))
         for index in list_of_metals:
             partial_charges.insert(index, metal_charge)
     else:
         partial_charges = list(calculate_partial_charges_using_ob(positions, atom_names, method))
+    #print("Sum", np.sum(partial_charges))
     return partial_charges
```

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/grid_classes.py` & `CageCavityCalc-1.0.4/CageCavityCalc/grid_classes.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/hydrophobicity.py` & `CageCavityCalc-1.0.4/CageCavityCalc/hydrophobicity.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/input_output.py` & `CageCavityCalc-1.0.4/CageCavityCalc/input_output.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/log.py` & `CageCavityCalc-1.0.4/CageCavityCalc/log.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/pymol_plugin/__init__.py` & `CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/pymol_plugin/simple.py` & `CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/simple.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/CageCavityCalc/window_size.py` & `CageCavityCalc-1.0.4/CageCavityCalc/window_size.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/LICENSE` & `CageCavityCalc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.3/README.md` & `CageCavityCalc-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 cavity_calc.print_to_pymol("cage_cavity_hydrophobicity.pml")
 ```
 ![Alt text](CageCavityCalc/pic/hydrophobicity.png "Principle")
 
 
 From bash:
 ```
-python ../../main.py -f cage.pdb -o cage_cavity.pdb
+python -m CageCavityCalc -f cage.pdb -o cage_cavity.pdb
 ```
 
 ### Additional support
 
 Reading cage class from cgbind:
 ```
 from cgbind import Linker, Cage
@@ -72,8 +72,8 @@
 ```
 
 ### Other
 To make the calculation loud use CAV_LOG_LEVEL environmental variable
 
 ```commandline
 export CAV_LOG_LEVEL=INFO
-```
+```
```

