# Comparing `tmp/jms-metabolite-services-0.5.7.tar.gz` & `tmp/jms_metabolite_services-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-3nackh_x/jms-metabolite-services-0.5.7.tar", last modified: Sat May 13 20:48:43 2023, max compression
+gzip compressed data, was "jms_metabolite_services-0.5.8.tar", last modified: Mon Apr 15 19:43:11 2024, max compression
```

## Comparing `jms-metabolite-services-0.5.7.tar` & `jms_metabolite_services-0.5.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/
--rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.7/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.7/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms/
--rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-05-13 20:46:32.000000 jms-metabolite-services-0.5.7/jms/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4443 2023-04-11 00:19:46.000000 jms-metabolite-services-0.5.7/jms/coverage.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms/data/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.7/jms/data/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)   749330 2023-04-11 00:03:32.000000 jms-metabolite-services-0.5.7/jms/data/humangem_pathways.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.7/jms/data/list_formula_mass.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.7/jms/data/masters.py
--rw-r--r--   0 shuzhao    (501) staff       (20) 20170544 2023-04-11 00:13:02.000000 jms-metabolite-services-0.5.7/jms/data/smpdb_pathways.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    38468 2023-05-13 20:47:33.000000 jms-metabolite-services-0.5.7/jms/dbStructures.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4898 2023-04-10 13:43:20.000000 jms-metabolite-services-0.5.7/jms/empiricalCpds.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2229 2023-04-10 18:43:40.000000 jms-metabolite-services-0.5.7/jms/formula.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4788 2023-05-13 20:35:55.000000 jms-metabolite-services-0.5.7/jms/io.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.7/jms/ions.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    14660 2023-04-10 19:30:36.000000 jms-metabolite-services-0.5.7/jms/modelConvert.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.7/jms/model_port.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.7/jms/search.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.7/jms/test.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.7/jms/updates.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms/utils/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.7/jms/utils/Tabular2Json.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.7/jms/utils/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.7/jms/utils/chemebi.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.7/jms/utils/gems.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.7/jms/utils/hmdb.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.7/jms/utils/pubchem.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.7/jms/utils/refmet.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      723 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-05-13 20:48:43.000000 jms-metabolite-services-0.5.7/setup.cfg
--rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.7/setup.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:43:11.976969 jms_metabolite_services-0.5.8/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1073 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/LICENSE
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5622 2024-04-15 19:43:11.976481 jms_metabolite_services-0.5.8/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     4720 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/README.md
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:43:11.929047 jms_metabolite_services-0.5.8/jms/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       22 2024-04-15 19:25:38.000000 jms_metabolite_services-0.5.8/jms/__init__.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    10646 2024-04-11 15:05:31.000000 jms_metabolite_services-0.5.8/jms/coverage.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:43:11.948448 jms_metabolite_services-0.5.8/jms/data/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/jms/data/__init__.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)   749330 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/jms/data/humangem_pathways.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)  3085036 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/jms/data/list_formula_mass.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       84 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/jms/data/masters.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553) 20170544 2024-02-02 16:28:45.000000 jms_metabolite_services-0.5.8/jms/data/smpdb_pathways.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    38592 2024-02-22 02:06:18.000000 jms_metabolite_services-0.5.8/jms/dbStructures.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    10936 2024-04-11 15:01:32.000000 jms_metabolite_services-0.5.8/jms/empiricalCpds.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     2119 2024-02-07 01:31:57.000000 jms_metabolite_services-0.5.8/jms/formula.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     4884 2024-04-15 19:25:38.000000 jms_metabolite_services-0.5.8/jms/io.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1801 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/ions.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    14660 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/modelConvert.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      461 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/model_port.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    11998 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/search.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      649 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/test.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       58 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/updates.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:43:11.972868 jms_metabolite_services-0.5.8/jms/utils/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5832 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/Tabular2Json.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/__init__.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/chemebi.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    10125 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/gems.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    11707 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/hmdb.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/pubchem.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/jms/utils/refmet.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:43:11.976010 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5622 2024-04-15 19:43:11.000000 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      723 2024-04-15 19:43:11.000000 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/SOURCES.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-04-15 19:43:11.000000 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/dependency_links.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       10 2024-04-15 19:43:11.000000 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/requires.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        4 2024-04-15 19:43:11.000000 jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/top_level.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2024-04-15 19:43:11.977012 jms_metabolite_services-0.5.8/setup.cfg
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1300 2024-02-02 16:28:46.000000 jms_metabolite_services-0.5.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jms-metabolite-services-0.5.7/LICENSE` & `jms_metabolite_services-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/PKG-INFO` & `jms_metabolite_services-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.7
+Version: 0.5.8
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mass2chem
 
 Json's Metabolite Services (JMS)
 ================================
 
 A Python library for 
 - mapping identifiers between genome scale metabolic models and metabolite databases
 - reusable data structures for peaks, compounds and indexed data stores
```

### Comparing `jms-metabolite-services-0.5.7/README.md` & `jms_metabolite_services-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/data/humangem_pathways.py` & `jms_metabolite_services-0.5.8/jms/data/humangem_pathways.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/data/list_formula_mass.py` & `jms_metabolite_services-0.5.8/jms/data/list_formula_mass.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/data/smpdb_pathways.py` & `jms_metabolite_services-0.5.8/jms/data/smpdb_pathways.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/dbStructures.py` & `jms_metabolite_services-0.5.8/jms/dbStructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,16 @@
                             self.peak_to_empCpd_ion_relation[peak['id_number']] = peak['ion_relation']
                             self.peak_to_empCpd[peak['id_number']] = E['interim_id']
                             # this may overwrite 1:N relationships
 
     def singleton_formula_search(self, KCD):
         '''
         Search singletons for formulae first by KCD search then .data.formula_tree.
+        Allowing flexible M0 adducts provided in KCD.
+        
         KCD: knownCompoundDatabase instance.
 
         Returns
         -------
         List of first matched KCD compound for each singleton in self.dict_peaks, e.g.
         [('F17904', {'interim_id': 15321, 'neutral_formula_mass': 916.606449, 'neutral_formula': 'C56H84O10',...}), ...]
         '''
@@ -568,15 +570,15 @@
         for p in singletons:
             _mz = self.dict_peaks[p]['mz']
             list_matches = KCD.search_mz_single(_mz, self.mode, self.mz_tolerance_ppm)
             # [{'mz': 130.017306555, 'parent_epd_id': 'C4H3FN2O2_130.017856', 'ion_relation': 'M[1+]'}]
             if list_matches:
                 # take 1st match only here; will model better in future
                 _epd = KCD.mass_indexed_compounds[list_matches[0]['parent_epd_id']]
-                _epd['isotope'] = '13C/12C'
+                _epd['isotope'] = 'M0'
                 _epd['ion_relation'] = _epd['modification'] = list_matches[0]['ion_relation']
                 found.append((p, _epd))
             else:
                 # formula search
                 F = self.search_mz_for_formula(_mz, self.mz_tolerance_ppm)
                 if F:
                     found.append((p, F))            # p is id_number
@@ -627,35 +629,36 @@
                 formula_to_peaks[k] = [(p, F)]
 
         found_peaks = set([x[0] for x in found])
         peakList = [P for P in self.list_peaks if P['id_number'] not in self.peak_to_empCpd and
                                                   P['id_number'] not in found_peaks]
         peakTree = build_centurion_tree(peakList)
 
-        new_id_start = len(self.dict_empCpds) + 10000
+        new_id_start = len(self.dict_empCpds)
         for formula, PP in formula_to_peaks.items():
             neutral_formula_mass = PP[0][1]['neutral_formula_mass']
             P1 = self.dict_peaks[PP[0][0]]
             tmp = [P1, ]
             for jj in range(1, len(PP)):
                 _P = self.dict_peaks[PP[jj][0]]
                 if is_coeluted(tmp[-1], _P, rt_tolerance=self.rt_tolerance):
                     tmp.append(_P)
                 else:
                     # not coeluted, new empCpd
                     new_id_start += 1
-                    self.dict_empCpds[new_id_start] = {'interim_id': str(new_id_start),
+                    interim_id = '_singleton_' + str(new_id_start)
+                    self.dict_empCpds[interim_id] = {'interim_id': interim_id,
                             'neutral_formula_mass': neutral_formula_mass, 'neutral_formula': formula,
                             'MS1_pseudo_Spectra': self.__extend_peakList__(
                                 formula, neutral_formula_mass, tmp, peakTree, self.mz_tolerance_ppm),
                     }
                     tmp = [_P, ]
 
             new_id_start += 1
-            self.dict_empCpds[new_id_start] = {'interim_id': str(new_id_start),
+            self.dict_empCpds[new_id_start] = {'interim_id': '_singleton_' + str(new_id_start),
                     'neutral_formula_mass': neutral_formula_mass, 'neutral_formula': formula,
                     'MS1_pseudo_Spectra': self.__extend_peakList__(
                                 formula, neutral_formula_mass, tmp, peakTree, self.mz_tolerance_ppm),
             }
 
 
     def __extend_peakList__(self, neutral_formula, neutral_formula_mass, epd_peaks, peakTree,
```

### Comparing `jms-metabolite-services-0.5.7/jms/formula.py` & `jms_metabolite_services-0.5.8/jms/formula.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-'''
-Based on mass2chem.formula 
-
-1. to find formula for anchor ions
-2. to search for any formula (to-do)
-'''
-
 from mass2chem.formula import compute_adducts_formulae, \
                                     parse_chemformula_dict, \
                                         add_formula_dict, \
                                             dict_to_hill_formula
 
 from .search import build_centurion_tree, find_best_match_centurion_indexed_list
```

### Comparing `jms-metabolite-services-0.5.7/jms/io.py` & `jms_metabolite_services-0.5.8/jms/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     'm/z': 'mz',
     'mz': 'mz',
     'apex': 'rtime',
     # ...,
 }
 
 def read_table_to_peaks(infile, 
-                        has_header=True, mz_col=1, rtime_col=2, intensity=(11,21), feature_id=None,
-                        full_extract=True, max_col=21,
+                        has_header=True, mz_col=1, rtime_col=2, intensity=None, feature_id=None,
+                        full_extract=True, max_col=None,
                         delimiter='\t'):
     '''
     Read a text feature table, and 
     return list of peaks, e.g. [ {
         'id_number': 555,
         'mz': 133.0970, 
         'apex': 654, 
@@ -47,41 +47,39 @@
     
     full_extract: to keep all fields in output as strings, only if has_header.
     feature_id: if None, create id for each peak/feature.
     '''
     def _make_id(ii, mz, rt):
         return 'F' + str(ii) + '_' + str(round(mz, 6)) + '@' + str(round(rt, 2))
 
-    list_peaks = []
-    w = open(infile).readlines()
+    with open(infile) as ft_fh:
+        ft = ft_fh.readlines()
     if has_header:
-        header = w[0].rstrip().split(delimiter)[:max_col]
-        w = w[1:]
-    ii = 0
-    for line in w:
-        a = line.split(delimiter)[:max_col]   # not rstrip, so trailing EOL will be carried forward
-        mz, rt = float(a[mz_col]), float(a[rtime_col])
-        intensities = [float(x) for x in a[intensity[0]: intensity[1]]]
-        if feature_id != None:
-            fid = a[feature_id].strip()
-        else:
-            ii += 1
-            fid = _make_id(ii, mz, rt)
-        peak = {'id_number': fid, 'mz': mz, 'rtime': rt, 'apex': rt, 'representative_intensity': sum(intensities) / len(intensities)}
+        header = ft[0].rstrip().split(delimiter)
+        if max_col and not full_extract:
+            header = header[:max_col]
+        ft = ft[1:]
+    list_peaks = []
+    for ii, entry in enumerate(ft):
+        values = entry.split(delimiter)
+        if max_col and not full_extract:
+            values = line[:max_col]
+        mz, rt = float(values[mz_col]), float(values[rtime_col])
+        fid = values[feature_id].strip() if feature_id is not None else _make_id(ii, mz, rt)
+        representative_intensity = [float(x) for x in values[intensity[0]: intensity[1]]] if intensity else 0
+        peak = {'id_number': fid, 'id': fid, 'mz': mz, 'rtime': rt, 'apex': rt, 'representative_intensity': representative_intensity}
         if has_header and full_extract:
-            # will remove redundant fields
-            peak2 = dict(zip(header, a))
-            peak2.update(peak)
-            peak = peak2
-
-        list_peaks.append( peak )
-
+            for k, v in zip(header, values):
+                if k not in peak:
+                    peak[k] = float(v)
+        list_peaks.append(peak)
     return list_peaks
 
 
+
 def read_tsv_hmdb_to_empCpds(infile, delimiter='\t'):
     '''
     Previously parsed HMDB4 in short tsv format.
     Ref:
     https://github.com/shuzhao-li/JMS/wiki/Scripting-to-create-a-dictionary-from-HMDB-data
     https://github.com/shuzhao-li/JMS/blob/main/jms/utils/hmdb.py
     A copy of HMDB4_compounds.tsv is under
```

### Comparing `jms-metabolite-services-0.5.7/jms/ions.py` & `jms_metabolite_services-0.5.8/jms/ions.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/modelConvert.py` & `jms_metabolite_services-0.5.8/jms/modelConvert.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/search.py` & `jms_metabolite_services-0.5.8/jms/search.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/test.py` & `jms_metabolite_services-0.5.8/jms/test.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/utils/Tabular2Json.py` & `jms_metabolite_services-0.5.8/jms/utils/Tabular2Json.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/utils/gems.py` & `jms_metabolite_services-0.5.8/jms/utils/gems.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms/utils/hmdb.py` & `jms_metabolite_services-0.5.8/jms/utils/hmdb.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/PKG-INFO` & `jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.7
+Version: 0.5.8
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mass2chem
 
 Json's Metabolite Services (JMS)
 ================================
 
 A Python library for 
 - mapping identifiers between genome scale metabolic models and metabolite databases
 - reusable data structures for peaks, compounds and indexed data stores
```

### Comparing `jms-metabolite-services-0.5.7/jms_metabolite_services.egg-info/SOURCES.txt` & `jms_metabolite_services-0.5.8/jms_metabolite_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.7/setup.py` & `jms_metabolite_services-0.5.8/setup.py`

 * *Files identical despite different names*

