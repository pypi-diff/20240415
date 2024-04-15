# Comparing `tmp/blue-prints-0.0.4.tar.gz` & `tmp/blue_prints-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue-prints-0.0.4.tar", last modified: Tue Jan  9 12:44:42 2024, max compression
+gzip compressed data, was "blue_prints-0.0.5.tar", last modified: Mon Apr 15 11:21:00 2024, max compression
```

## Comparing `blue-prints-0.0.4.tar` & `blue_prints-0.0.5.tar`

### file list

```diff
@@ -1,176 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.571999 blue-prints-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-01-09 12:44:02.000000 blue-prints-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-01-09 12:44:42.571999 blue-prints-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-09 12:44:02.000000 blue-prints-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blue_prints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-01-09 12:44:42.000000 blue-prints-0.0.4/blue_prints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-01-09 12:44:42.000000 blue-prints-0.0.4/blue_prints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 12:44:42.000000 blue-prints-0.0.4/blue_prints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-09 12:44:42.000000 blue-prints-0.0.4/blue_prints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-09 12:44:42.000000 blue-prints-0.0.4/blue_prints.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/checks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/checks/circular_concrete_section/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/checks/circular_concrete_section/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/checks/circular_hollow_sections/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/checks/circular_hollow_sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/checks/rectangular_concrete_section/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/checks/rectangular_concrete_section/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/checks/steel_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/checks/steel_profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.547999 blue-prints-0.0.4/blueprints/codes/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/cur/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/cur/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/cur/cur_166/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/cur/cur_166/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_10_precast_concrete_elements_and_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_10_precast_concrete_elements_and_structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_11_lightweight_aggregate_concrete_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_11_lightweight_aggregate_concrete_structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.551999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_12_plain_and_lightly_reinforced_concrete_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_12_plain_and_lightly_reinforced_concrete_structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.555999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_14.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_16.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_17.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_18.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_19_20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_21_22.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_23.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_24.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_25.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_26.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_27.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_28.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_29.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_30.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_7.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_9.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/sub_formula_3_28_29_30.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.555999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.559999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.559999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/formula_6_1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.559999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/formula_7_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.559999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_14.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_15.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_17.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_18.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_7.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_8n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_12n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_14.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_16.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_1n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_5n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_6n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_7n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_8n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/formula_2_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/codes/formula.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/external/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/external/cems/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/external/cems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.563999 blue-prints-0.0.4/blueprints/external/scia/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/external/scia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/geometry/line.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/geometry/point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/materials/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/materials/concrete.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/materials/soil.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/materials/steel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/product_data/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/product_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/soil_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/soil_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/soil_profiles/soil_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/soil_profiles/soil_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_elements/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_elements/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/structural_sections/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/structural_sections/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/concrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/concrete/reinforced_concrete_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/concrete/reinforcement_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/concrete/stirrups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/blueprints/structural_sections/sheet_piles/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/sheet_piles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/structural_sections/sheet_piles/sheet_pile_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/type_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-09 12:44:02.000000 blue-prints-0.0.4/blueprints/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-09 12:44:02.000000 blue-prints-0.0.4/docs/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-01-09 12:44:02.000000 blue-prints-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-09 12:44:02.000000 blue-prints-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-09 12:44:02.000000 blue-prints-0.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 12:44:42.571999 blue-prints-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 12:44:42.567999 blue-prints-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-09 12:44:02.000000 blue-prints-0.0.4/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.697695 blue_prints-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-15 11:20:09.000000 blue_prints-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-15 11:21:00.697695 blue_prints-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-15 11:20:09.000000 blue_prints-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blue_prints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-15 11:21:00.000000 blue_prints-0.0.5/blue_prints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-15 11:21:00.000000 blue_prints-0.0.5/blue_prints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:21:00.000000 blue_prints-0.0.5/blue_prints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-15 11:21:00.000000 blue_prints-0.0.5/blue_prints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:21:00.000000 blue_prints-0.0.5/blue_prints.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.669694 blue_prints-0.0.5/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.669694 blue_prints-0.0.5/blueprints/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.669694 blue_prints-0.0.5/blueprints/checks/circular_concrete_section/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/checks/circular_concrete_section/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/checks/circular_hollow_sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/checks/circular_hollow_sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/checks/rectangular_concrete_section/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/checks/rectangular_concrete_section/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/checks/steel_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/checks/steel_profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/cur/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/cur/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/cur/cur_166/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/cur/cur_166/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_1_general_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_1_general_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_1_general_rules/formula_1_0_1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_10_precast_concrete_elements_and_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_10_precast_concrete_elements_and_structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_11_lightweight_aggregate_concrete_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_11_lightweight_aggregate_concrete_structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.673694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_12_plain_and_lightly_reinforced_concrete_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_12_plain_and_lightly_reinforced_concrete_structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.677694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_19_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_21_22.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_23.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_26.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_27.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_28.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_29.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_30.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/sub_formula_3_28_29_30.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.681694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.681694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_8.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.681694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/formula_6_1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.681694 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/formula_7_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.685695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_8n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_12n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_1n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_5n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_6n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_7n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_8n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/formula_2_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_6_ultimate_limit_state/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_6_ultimate_limit_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_6_ultimate_limit_state/formula_6_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/codes/latex_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/external/cems/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/external/cems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.689695 blue_prints-0.0.5/blueprints/external/scia/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/external/scia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/geometry/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/geometry/point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/materials/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/materials/soil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/materials/steel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/product_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/product_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/soil_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/soil_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/soil_profiles/soil_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/soil_profiles/soil_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_elements/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_elements/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/structural_sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/structural_sections/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/concrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/concrete/reinforced_concrete_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/concrete/reinforcement_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/concrete/stirrups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/blueprints/structural_sections/sheet_piles/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/sheet_piles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/structural_sections/sheet_piles/sheet_pile_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/type_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-15 11:20:09.000000 blue_prints-0.0.5/blueprints/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 11:20:09.000000 blue_prints-0.0.5/docs/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-15 11:20:09.000000 blue_prints-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 11:20:09.000000 blue_prints-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 11:20:09.000000 blue_prints-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:21:00.697695 blue_prints-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:21:00.693694 blue_prints-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-15 11:20:09.000000 blue_prints-0.0.5/tests/test_validations.py
```

### Comparing `blue-prints-0.0.4/LICENSE` & `blue_prints-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blue-prints-0.0.4/PKG-INFO` & `blue_prints-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue-prints
-Version: 0.0.4
+Version: 0.0.5
 Summary: Blueprints: Python AEC library.
 Author: Blueprints
 Maintainer: Blueprints Maintainers
 Maintainer-email: Enrique García Méndez <enriquegarcia@live.nl>
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/Blueprints-org/blueprints
 Project-URL: documentation, https://blueprints.readthedocs.io
@@ -26,29 +26,29 @@
 Provides-Extra: minimal-requirements
 Requires-Dist: matplotlib>=3.7.2; extra == "minimal-requirements"
 Requires-Dist: plotly>=5.15.0; extra == "minimal-requirements"
 Requires-Dist: pandas>=2.1.0; extra == "minimal-requirements"
 Requires-Dist: shapely>=2.0.1; extra == "minimal-requirements"
 Requires-Dist: numpy>=1.25.2; extra == "minimal-requirements"
 Provides-Extra: dev
-Requires-Dist: mypy==1.8.0; extra == "dev"
-Requires-Dist: ruff==0.1.11; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: pytest-describe==2.1.0; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: pytest-describe==2.2.0; extra == "dev"
 Requires-Dist: pytest-pspec==0.0.4; extra == "dev"
 Requires-Dist: pytest-raises==0.11; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2023.9.10; extra == "docs"
-Requires-Dist: ipykernel==6.28.0; extra == "docs"
-Requires-Dist: ipython==8.19.0; extra == "docs"
-Requires-Dist: ipywidgets==8.1.1; extra == "docs"
-Requires-Dist: nbconvert==7.14.0; extra == "docs"
+Requires-Dist: furo==2024.1.29; extra == "docs"
+Requires-Dist: ipykernel==6.29.4; extra == "docs"
+Requires-Dist: ipython==8.23.0; extra == "docs"
+Requires-Dist: ipywidgets==8.1.2; extra == "docs"
+Requires-Dist: nbconvert==7.16.3; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-click==5.1.0; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.9.1; extra == "docs"
 Requires-Dist: matplotlib>=3.7.2; extra == "docs"
 
@@ -63,19 +63,23 @@
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/blueprints_banner.png">
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/blueprints_banner.png">
   <img alt="blueprints banner" src="docs/source/_static/blueprints_banner.png">
 </picture>
 
-Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative, open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the workflows within the built environment sector.
+Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative,
+open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the
+workflows within the built environment sector.
 
 ## Vision
 
-Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open source can drive the field of civil engineering to new heights.
+Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily
+challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open
+source can drive the field of civil engineering to new heights.
 
 ## Mission
 
 Our mission is to:
 
 - Foster a community where sharing knowledge and best practices is the norm, not the exception.
 - Provide a solid foundation of code and documentation that adheres to the highest quality standards (100% code coverage).
@@ -90,26 +94,28 @@
 ```
 
 For the actively developed version:
 
 ```shell
 pip install git+https://github.com/Blueprints-org/blueprints.git
 ```
+
 Documentation is available at [blueprints.readthedocs.io](https://blueprints.readthedocs.io/en/latest/).
 
 ## Quick Reference to Blueprint's Objects
 
-This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its equations, tables, and
+This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its formulas, tables, and
 figures for streamlined access and reference.
 
-| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                            |                            Figures                             |
-|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------:|:--------------------------------------------------------------:|
-| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md) | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
-| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md) | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
-| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) |  [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md)  |  [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md)   |
+| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                             |                            Figures                             |
+|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------:|:--------------------------------------------------------------:|
+| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md)  | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
+| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md)  | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
+| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) | [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md) | [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md) |
+| NEN-EN 1993-5:2008         | Eurocode 3: Design of steel structures – Part 5: Piling                                     | [63](docs/source/codes/eurocode/nen_en_1993_5_2008/formulas.md) | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/tables.md)  | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/figures.md)  |
 
 ## Contributing
 
 Contributions are very welcome. To learn more, see the [Contributor Guide](CONTRIBUTING.md).
 
 ## License
```

### Comparing `blue-prints-0.0.4/README.md` & `blue_prints-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/blueprints_banner.png">
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/blueprints_banner.png">
   <img alt="blueprints banner" src="docs/source/_static/blueprints_banner.png">
 </picture>
 
-Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative, open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the workflows within the built environment sector.
+Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative,
+open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the
+workflows within the built environment sector.
 
 ## Vision
 
-Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open source can drive the field of civil engineering to new heights.
+Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily
+challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open
+source can drive the field of civil engineering to new heights.
 
 ## Mission
 
 Our mission is to:
 
 - Foster a community where sharing knowledge and best practices is the norm, not the exception.
 - Provide a solid foundation of code and documentation that adheres to the highest quality standards (100% code coverage).
@@ -36,26 +40,28 @@
 ```
 
 For the actively developed version:
 
 ```shell
 pip install git+https://github.com/Blueprints-org/blueprints.git
 ```
+
 Documentation is available at [blueprints.readthedocs.io](https://blueprints.readthedocs.io/en/latest/).
 
 ## Quick Reference to Blueprint's Objects
 
-This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its equations, tables, and
+This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its formulas, tables, and
 figures for streamlined access and reference.
 
-| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                            |                            Figures                             |
-|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------:|:--------------------------------------------------------------:|
-| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md) | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
-| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md) | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
-| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) |  [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md)  |  [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md)   |
+| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                             |                            Figures                             |
+|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------:|:--------------------------------------------------------------:|
+| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md)  | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
+| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md)  | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
+| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) | [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md) | [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md) |
+| NEN-EN 1993-5:2008         | Eurocode 3: Design of steel structures – Part 5: Piling                                     | [63](docs/source/codes/eurocode/nen_en_1993_5_2008/formulas.md) | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/tables.md)  | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/figures.md)  |
 
 ## Contributing
 
 Contributions are very welcome. To learn more, see the [Contributor Guide](CONTRIBUTING.md).
 
 ## License
```

### Comparing `blue-prints-0.0.4/blue_prints.egg-info/PKG-INFO` & `blue_prints-0.0.5/blue_prints.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue-prints
-Version: 0.0.4
+Version: 0.0.5
 Summary: Blueprints: Python AEC library.
 Author: Blueprints
 Maintainer: Blueprints Maintainers
 Maintainer-email: Enrique García Méndez <enriquegarcia@live.nl>
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/Blueprints-org/blueprints
 Project-URL: documentation, https://blueprints.readthedocs.io
@@ -26,29 +26,29 @@
 Provides-Extra: minimal-requirements
 Requires-Dist: matplotlib>=3.7.2; extra == "minimal-requirements"
 Requires-Dist: plotly>=5.15.0; extra == "minimal-requirements"
 Requires-Dist: pandas>=2.1.0; extra == "minimal-requirements"
 Requires-Dist: shapely>=2.0.1; extra == "minimal-requirements"
 Requires-Dist: numpy>=1.25.2; extra == "minimal-requirements"
 Provides-Extra: dev
-Requires-Dist: mypy==1.8.0; extra == "dev"
-Requires-Dist: ruff==0.1.11; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: pytest-describe==2.1.0; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: pytest-describe==2.2.0; extra == "dev"
 Requires-Dist: pytest-pspec==0.0.4; extra == "dev"
 Requires-Dist: pytest-raises==0.11; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2023.9.10; extra == "docs"
-Requires-Dist: ipykernel==6.28.0; extra == "docs"
-Requires-Dist: ipython==8.19.0; extra == "docs"
-Requires-Dist: ipywidgets==8.1.1; extra == "docs"
-Requires-Dist: nbconvert==7.14.0; extra == "docs"
+Requires-Dist: furo==2024.1.29; extra == "docs"
+Requires-Dist: ipykernel==6.29.4; extra == "docs"
+Requires-Dist: ipython==8.23.0; extra == "docs"
+Requires-Dist: ipywidgets==8.1.2; extra == "docs"
+Requires-Dist: nbconvert==7.16.3; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-click==5.1.0; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.9.1; extra == "docs"
 Requires-Dist: matplotlib>=3.7.2; extra == "docs"
 
@@ -63,19 +63,23 @@
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/blueprints_banner.png">
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/blueprints_banner.png">
   <img alt="blueprints banner" src="docs/source/_static/blueprints_banner.png">
 </picture>
 
-Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative, open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the workflows within the built environment sector.
+Welcome to Blueprints, the cornerstone repository for civil engineering professionals and enthusiasts alike. Blueprints is a collaborative,
+open-source initiative designed to serve as a comprehensive library of code, tools, and best practices, aiming to streamline and innovate the
+workflows within the built environment sector.
 
 ## Vision
 
-Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open source can drive the field of civil engineering to new heights.
+Our vision with Blueprints is to create an accessible, reliable, and community-driven resource that supports engineers, and developers in their daily
+challenges. By harnessing the collective expertise of the industry, Blueprints strives to pave the way for a future where collaboration and open
+source can drive the field of civil engineering to new heights.
 
 ## Mission
 
 Our mission is to:
 
 - Foster a community where sharing knowledge and best practices is the norm, not the exception.
 - Provide a solid foundation of code and documentation that adheres to the highest quality standards (100% code coverage).
@@ -90,26 +94,28 @@
 ```
 
 For the actively developed version:
 
 ```shell
 pip install git+https://github.com/Blueprints-org/blueprints.git
 ```
+
 Documentation is available at [blueprints.readthedocs.io](https://blueprints.readthedocs.io/en/latest/).
 
 ## Quick Reference to Blueprint's Objects
 
-This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its equations, tables, and
+This table serves as a quick navigator to the key elements of the code within Blueprints, offering immediate links to its formulas, tables, and
 figures for streamlined access and reference.
 
-| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                            |                            Figures                             |
-|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------:|:--------------------------------------------------------------:|
-| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md) | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
-| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md) | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
-| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) |  [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md)  |  [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md)   |
+| Document                   | Description                                                                                 |                            Formulas                             |                            Tables                             |                            Figures                             |
+|:---------------------------|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------:|:--------------------------------------------------------------:|
+| NEN-EN 1992-1-1+C2:2011    | Eurocode 2: Design of concrete structures – Part 1-1: General rules and rules for buildings | [304](docs/source/codes/eurocode/ec2_1992_1_1_2011/formulas.md) | [38](docs/source/codes/eurocode/ec2_1992_1_1_2011/tables.md)  | [104](docs/source/codes/eurocode/ec2_1992_1_1_2011/figures.md) |
+| NEN-EN 1993-1-1+C2+A1:2016 | Eurocode 3: Design of steel structures – Part 1-1: General rules and rules for buildings    | [108](docs/source/codes/eurocode/ec3_1993_1_1_2016/formulas.md) | [20](docs/source/codes/eurocode/ec3_1993_1_1_2016/tables.md)  | [28](docs/source/codes/eurocode/ec3_1993_1_1_2016/figures.md)  |
+| NEN 9997-1+C2:2017         | Eurocode 7: Geotechnical design of structures - Part 1: General rules                       | [88](docs/source/codes/eurocode/nen_9997_1_c2_2017/formulas.md) | [11](docs/source/codes/eurocode/nen_9997_1_c2_2017/tables.md) | [25](docs/source/codes/eurocode/nen_9997_1_c2_2017/figures.md) |
+| NEN-EN 1993-5:2008         | Eurocode 3: Design of steel structures – Part 5: Piling                                     | [63](docs/source/codes/eurocode/nen_en_1993_5_2008/formulas.md) | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/tables.md)  | [0](docs/source/codes/eurocode/nen_en_1993_5_2008/figures.md)  |
 
 ## Contributing
 
 Contributions are very welcome. To learn more, see the [Contributor Guide](CONTRIBUTING.md).
 
 ## License
```

### Comparing `blue-prints-0.0.4/blue_prints.egg-info/SOURCES.txt` & `blue_prints-0.0.5/blue_prints.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 blueprints/checks/__init__.py
 blueprints/checks/circular_concrete_section/__init__.py
 blueprints/checks/circular_hollow_sections/__init__.py
 blueprints/checks/rectangular_concrete_section/__init__.py
 blueprints/checks/steel_profiles/__init__.py
 blueprints/codes/__init__.py
 blueprints/codes/formula.py
+blueprints/codes/latex_formula.py
 blueprints/codes/cur/__init__.py
 blueprints/codes/cur/cur_166/__init__.py
 blueprints/codes/eurocode/__init__.py
 blueprints/codes/eurocode/nen_9997_1_c2_2017/__init__.py
+blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_1_general_rules/__init__.py
+blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_1_general_rules/formula_1_0_1.py
 blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/__init__.py
+blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_a.py
 blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_b.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_10_precast_concrete_elements_and_structures/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_11_lightweight_aggregate_concrete_structures/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_12_plain_and_lightly_reinforced_concrete_structures/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_1.py
@@ -62,14 +66,19 @@
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_1.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_2.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_1.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_2.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3a.py
+blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3b.py
+blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_4.py
+blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_5.py
+blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_6.py
+blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_8.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/formula_6_1.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/formula_7_3.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/__init__.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_1.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_10.py
@@ -102,14 +111,26 @@
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_6n.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_7n.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_8n.py
 blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_9.py
 blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/__init__.py
 blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/__init__.py
 blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/formula_2_2.py
+blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_6_ultimate_limit_state/__init__.py
+blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_6_ultimate_limit_state/formula_6_5.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/__init__.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/__init__.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_10.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_2.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_3.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_5.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_6.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_7.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_8.py
+blueprints/codes/eurocode/nen_en_1993_5_2008/chapter_5_ultimate_limit_states/formula_5_9.py
 blueprints/external/__init__.py
 blueprints/external/cems/__init__.py
 blueprints/external/scia/__init__.py
 blueprints/geometry/__init__.py
 blueprints/geometry/line.py
 blueprints/geometry/point.py
 blueprints/materials/__init__.py
```

### Comparing `blue-prints-0.0.4/blue_prints.egg-info/requires.txt` & `blue_prints-0.0.5/blue_prints.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 matplotlib>=3.7.2
 plotly>=5.15.0
 pandas>=2.1.0
 shapely>=2.0.1
 numpy>=1.25.2
 
 [dev]
-mypy==1.8.0
-ruff==0.1.11
+mypy==1.9.0
+ruff==0.3.5
 isort==5.13.2
-pre-commit==3.6.0
-pytest==7.4.4
-pytest-cov==4.1.0
-pytest-describe==2.1.0
+pre-commit==3.7.0
+pytest==8.1.1
+pytest-cov==5.0.0
+pytest-describe==2.2.0
 pytest-pspec==0.0.4
 pytest-raises==0.11
 
 [docs]
-furo==2023.9.10
-ipykernel==6.28.0
-ipython==8.19.0
-ipywidgets==8.1.1
-nbconvert==7.14.0
+furo==2024.1.29
+ipykernel==6.29.4
+ipython==8.23.0
+ipywidgets==8.1.2
+nbconvert==7.16.3
 nbsphinx==0.9.3
 sphinx==7.2.6
 sphinx-click==5.1.0
 sphinx-copybutton==0.5.2
 sphinxext-opengraph==0.9.1
 matplotlib>=3.7.2
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_b.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_9997_1_c2_2017/chapter_2_basic_of_geotechnical_design/formula_2_1_b.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-""""Formula 2.1b from NEN 9997-1+C2:2017: Chapter 2: Basis of geotechnical design."""
+"""Formula 2.1b from NEN 9997-1+C2:2017: Chapter 2: Basis of geotechnical design."""
+
 from blueprints.codes.eurocode.nen_9997_1_c2_2017 import NEN_9997_1_C2_2017
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS
 from blueprints.validations import raise_if_negative
 
 
-class Form2Dot1BRepresentativeValue(Formula):
+class Form2Dot1bRepresentativeValue(Formula):
     """Class representing formula 2.1b for the calculation of the representative value :math:`F_{rep}` of actions."""
 
     label = "2.1b"
     source_document = NEN_9997_1_C2_2017
 
     def __init__(self, psi: DIMENSIONLESS, f_k: float) -> None:
         """[:math:`F_{rep}`] Representative value of actions.
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_1.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.1 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 from blueprints.validations import raise_if_negative
 
 
 class Form3Dot1EstimationConcreteCompressiveStrength(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_10.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_10.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.10 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DAYS, MM, MM2
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_11.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_11.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.11 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 
 
 class Form3Dot11AutogeneShrinkage(Formula):
     """Class representing formula 3.11, which calculates the autogene shrinkage."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_12.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_12.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.12 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot12AutogeneShrinkageInfinity(Formula):
     """Class representing formula 3.12, which calculates the autogene shrinkage at infinity."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_13.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_13.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.13 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DAYS
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_14.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_14.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.14 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot14StressStrainForShortTermLoading(Formula):
     """Class representing formula 3.14, which calculates the compressive stress-strength ratio."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_15.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_15.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.15 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot15DesignValueCompressiveStrength(Formula):
     """Class representing formula 3.15 for the calculation of the concrete compressive strength design value."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_16.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_16.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.16 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot16DesignValueTensileStrength(Formula):
     """Class representing formula 3.16 for the calculation of the concrete tensile strength design value."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_17.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_17.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.17 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot17CompressiveStressConcrete(Formula):
     """Class representing formula 3.17 for the calculation of compressive stress in concrete using stress-strain diagram of figure 3.3."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_18.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_18.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.18 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot18CompressiveStressConcrete(Formula):
     """Class representing formula 3.18 for the calculation of compressive stress in concrete using stress-strain diagram of figure 3.3."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_19_20.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_19_20.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.19 and 3.20 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot19And20EffectivePressureZoneHeight(Formula):
     """Class representing formula 3.19 and 3.20 for the calculation of the λ factor for the effective pressure zone height."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_2.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.2 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DAYS
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_21_22.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_21_22.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.21 and 3.22 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot21And22EffectiveStrength(Formula):
     """Class representing formula 3.21 and 3.22 for the calculation of the η factor for the effective strength."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_23.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_23.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.23 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MM, MPA
 
 
 class Form3Dot23FlexuralTensileStrength(Formula):
     """Class representing formula 3.23 for the calculation of the mean flexural tensile strength of reinforced concrete members."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_24.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_24.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.24 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot24IncreasedCharacteristicCompressiveStrength(Formula):
     """Class representing formula 3.24 for the calculation of the increased characteristic compressive strength due to enclosed concrete."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_25.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_25.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.25 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot25IncreasedCharacteristicCompressiveStrength(Formula):
     """Class representing formula 3.25 for the calculation of the increased characteristic compressive strength due to enclosed concrete."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_26.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_26.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.26 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot26IncreasedStrainAtMaxStrength(Formula):
     """Class representing formula 3.26 for the calculation of the increased strain at the maximum strength due to enclosed concrete."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_27.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_27.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.27 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot27IncreasedStrainLimitValue(Formula):
     """Class representing formula 3.27 for the calculation of the increased strain limit value due to enclosed concrete."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_28.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_28.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.28 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import HOURS, PERCENTAGE
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_29.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_29.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.29 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import HOURS, PERCENTAGE
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_3.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.3 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot3AxialTensileStrengthFromTensileSplittingStrength(Formula):
     """Class representing formula 3.3 for the approximated axial tensile strength, fct, determined by tensile splitting strength."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_30.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_30.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.30 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import HOURS, PERCENTAGE
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_4.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.4 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DAYS, MPA
 
 
 class Form3Dot4DevelopmentTensileStrength(Formula):
     """Class representing formula 3.4 for an initial estimation of the tensile strength, fctm(t), after t days."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_5.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.5 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot5ApproximationVarianceElasticModulusOverTime(Formula):
     """Class representing formula 3.5 for the approximation of the elastic modulus, Ecm(t) at day t."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_6.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.6 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class Form3Dot6CreepDeformationOfConcrete(Formula):
     """Class representing formula 3.6 for the calculation of creep deformation of concrete."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_7.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.7 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 
 
 class Form3Dot7NonLinearCreepCoefficient(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_8.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.8 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 
 
 class Form3Dot8TotalShrinkage(Formula):
     """Class representing formula 3.8 for the calculation of the total shrinkage."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_9.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/formula_3_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 3.9 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 
 
 class Form3Dot9DryingShrinkage(Formula):
     """Class representing formula 3.9 for the calculation of the drying shrinkage."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/sub_formula_3_28_29_30.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_3_materials/sub_formula_3_28_29_30.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sub-formula 3.28, 3.29 and 3.30 from NEN-EN 1992-1-1+C2:2011: Chapter 3 - Materials."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 
 
 class SubForm3Dot282930Mu(Formula):
     """Class representing sub-formula for 3.28, 3.29 and 3.30 for the calculation of μ."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_1.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_4_durability_and_cover/formula_4_1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 """Formula 4.1 from NEN-EN 1992-1-1+C2:2011: Chapter 4 - Durability and cover to reinforcement."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula
 from blueprints.type_alias import MM
+from blueprints.validations import raise_if_negative
 
 
 class Form4Dot1NominalConcreteCover(Formula):
-    """Class representing the formula 4.1 for the calculation of the nominal concrete cover."""
+    """Class representing the formula 4.1 for the calculation of the nominal concrete cover :math:`c_{nom}` [:math:`mm`]."""
 
     label = "4.1"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
         c_min: MM,
         delta_c_dev: MM,
     ) -> None:
-        """[cnom] Calculates the nominal concrete cover [mm].
+        """[:math:`c_{nom}`] Calculates the nominal concrete cover [:math:`mm`].
 
         NEN-EN 1992-1-1+C2:2011 art.4.4.1.1 (2) - Formula (4.1)
 
         Parameters
         ----------
         c_min: MM
-            [cmin] Minimum concrete cover based on art. 4.4.1.2 [mm].
+            [:math:`c_{min}`] Minimum concrete cover based on art. 4.4.1.2 [:math:`mm`].
         delta_c_dev: MM
-            [Δcdev] Construction tolerance based on art. 4.4.1.3 [mm].
+            [:math:`Δc_{dev}`] Construction tolerance based on art. 4.4.1.3 [:math:`mm`].
         """
         super().__init__()
         self.c_min = c_min
         self.delta_c_dev = delta_c_dev
 
     @staticmethod
     def _evaluate(
         c_min: MM,
         delta_c_dev: MM,
     ) -> MM:
         """For more detailed documentation see the class docstring."""
-        if c_min < 0:
-            raise ValueError(f"Negative c_min: {c_min}. c_min cannot be negative")
-        if delta_c_dev < 0:
-            raise ValueError(f"Negative delta_c_dev: {delta_c_dev}. delta_c_dev cannot be negative")
+        raise_if_negative(c_min=c_min, delta_c_dev=delta_c_dev)
         return c_min + delta_c_dev
+
+    def latex(self) -> LatexFormula:
+        """Returns LatexFormula object for formula 4.1."""
+        return LatexFormula(
+            return_symbol=r"c_{nom}",
+            result=str(self),
+            equation=r"c_{min}+\Delta c_{dev}",
+            numeric_equation=f"{self.c_min}+{self.delta_c_dev}",
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_1.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 5.1 from NEN-EN 1992-1-1+C2:2011: Chapter 5 - Structural Analysis."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, M
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_2.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 5.1 from NEN-EN 1992-1-1+C2:2011: Chapter 5 - Structural Analysis."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, M
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
 
 
 class Form5Dot2Eccentricity(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3a.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_3a.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Formula 5.3a from NEN-EN 1992-1-1+C2:2011: Chapter 5 - Structural Analysis."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, KN
 from blueprints.validations import raise_if_negative
 
 
-class Form5Dot3ATransverseForceUnbracedMembers(Formula):
+class Form5Dot3aTransverseForceUnbracedMembers(Formula):
     """Class representing formula 5.3a for the calculation of the transverse force for unbraced members, :math:`H_{i}`.
 
     See Figure 5.1 a1.
     """
 
     label = "5.3a"
     source_document = NEN_EN_1992_1_1_C2_2011
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/formula_6_1.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_6_ultimate_limit_state/formula_6_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 6.1 from NEN-EN 1992-1-1+C2:2011: Chapter 6 - Ultimate limit state."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN
 
 
 class Form6Dot1DesignShearStrength(Formula):
     """Class representing formula 6.1 for the design shear strength, VRd."""
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/formula_7_3.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_7_serviceability_limit_state/formula_7_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 7.3 from NEN-EN 1992-1-1+C2:2011: Chapter 7 - Serviceability limit state (SLS)."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM2, MPA
 from blueprints.unit_conversion import KN_TO_N
 
 
 class Form7Dot3CoefficientKc(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_1.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.1 from NEN-EN 1992-1-1+C2:2011: Chapter 8 Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM, MPA
 from blueprints.unit_conversion import KN_TO_N
 from blueprints.validations import raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_10.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_4.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,152 +1,141 @@
-"""Formula 8.10 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+"""Formula 8.4 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula, latex_max_curly_brackets
 from blueprints.type_alias import DIMENSIONLESS, MM
 from blueprints.validations import raise_if_negative
 
 
-class Form8Dot10DesignLapLength(Formula):
-    """Class representing formula 8.10 for the calculation of the design lap length :math:`l_{0}` [:math:`mm`]."""
+class Form8Dot4DesignAnchorageLength(Formula):
+    """Class representing formula 8.4 for the calculation of the design anchorage length :math:`l_{bd}` [mm]."""
 
-    label = "8.10"
+    label = "8.4"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
         alpha_1: DIMENSIONLESS,
         alpha_2: DIMENSIONLESS,
         alpha_3: DIMENSIONLESS,
+        alpha_4: DIMENSIONLESS,
         alpha_5: DIMENSIONLESS,
-        alpha_6: DIMENSIONLESS,
         l_b_rqd: MM,
-        l_0_min: MM,
+        l_b_min: MM,
     ) -> None:
-        """[:math:`l_{0}`] Design lap length [:math:`mm`].
+        """[:math:`l_{bd}`] Design anchorage length [:math:`mm`].
 
-        NEN-EN 1992-1-1+C2:2011 art.8.7.3(1) - Formula (8.10)
+        NEN-EN 1992-1-1+C2:2011 art.8.4.4(1) - Formula (8.4)
 
         Parameters
         ----------
         alpha_1 : DIMENSIONLESS
             [:math:`α_{1}`] Coefficient for the effect of the form of the bars assuming adequate cover (see figure 8.1) [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1.0` for straight bars in tension.
 
-            :math:`= 1.0` if :math:`c_{d} <= 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
+            :math:`= 1.0 if c_{d} <= 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
 
-            :math:`= 0.7` if :math:`c_{d} > 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
+            :math:`= 0.7 if c_{d} > 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
 
-            Note: see figure 8.3 for values of cd.
+            Note: see figure 8.3 for values of :math:`c_{d}`.
         alpha_2 : DIMENSIONLESS
             [:math:`α_{2}`] Coefficient for the effect of minimum concrete cover (see figure 8.3) [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1 - 0.15 ⋅ (c_{d} - Ø) / Ø <= 1` with a minimum of 0.7 for straight bars in tension.
 
-            :math:`= 1 - 0.15 ⋅ (c_{d} - 3 ⋅ Ø) / Ø <= 1` with a minimum of 0.7 for bars other than straight in tension
-            (see figure 8.1 (b), (c) and (d)).
+            :math:`= 1 - 0.15 ⋅ (c_{d} - 3 ⋅ Ø) / Ø <= 1` with a minimum of 0.7 for bars other than
+            straight in tension (see figure 8.1 (b), (c) and (d)).
 
             Note: see figure 8.3 for values of :math:`c_{d}`.
         alpha_3 : DIMENSIONLESS
             [:math:`α_{3}`] Coefficient for the effect of confinement by transverse reinforcement [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1 - K ⋅ λ <= 1` with a minimum of 0.7 for bars in tension.
 
             Where: :math:`λ = (ΣA_{st} - ΣA_{st,min}) / A_{s}`.
 
-            Where: :math:`ΣA_{st,min} = A_{s} ⋅ (σ_{sd}/f_{yd})`
+            Where: :math:`ΣA_{st,min}` = cross-sectional area of the minimum transverse
+            reinforcement :math:`= 0,25 ⋅ A_{s}` for beams and 0 for slabs.
+
+            Note: see figure 8.4 for values of :math:`K, A_{s} and A_{st}`.
+        alpha_4 : DIMENSIONLESS
+            [:math:`α_{4}`] Coefficient for the influence of one or more welded transverse bars :math:`(Ø_{t} > 0,6 Ø)` along the design anchorage
+            length :math:`l_{bd}` (see 8.6) [-].
 
-            With :math:`A_{s}` = area of one lapped bar [mm²].
+            :math:`= 0.7` for all types, position and size as specified in figure 8.6 (e) in both tension and compression.
 
-            Note: see figure 8.4 for values of :math:`K, A_{s}` and :math:`A_{st}`.
         alpha_5 : DIMENSIONLESS
-            [:math:`α_{5}`] Coefficient for the effect of the pressure transverse to the plane of splitting along the design
-            anchorage length :math:`l_{bd}` (see 8.6) [-].
+            [:math:`α_{5}`] Coefficient for the effect of the pressure transverse to the plane of splitting
+            along the design anchorage length :math:`l_{bd}` (see 8.6) [-].
 
             :math:`= 1 - 0.04 ⋅ p <= 1` with a minimum of 0.7 for all types of anchorage in compression.
 
-            Where: p = transverse pressure at ultimate limit state along :math:`l_{bd}` [:math:`MPa`].
-        alpha_6 : DIMENSIONLESS
-            [:math:`α_{6}`] Coefficient for the effect of reinforcement ratio [-].
-
-            :math:`= (ρ_{1}/25)^{0.5} <= 1.5` with a minimum of 1.0.
-
-            Where: :math:`ρ_{1}` = reinforcement percentage lapped within :math:`0,65 ⋅ l_{0}` from the centre of the lap length
-            considered (see figure 8.8) [-].
-
-            Use your own implementation of this formula or use the :class:`SubForm8Dot10Alpha6` class.
-        l_b_rqd : MM
-            [:math:`l_{b,rqd}`] Basic required anchorage length, for anchoring the force :math:`A_{s} ⋅ σ_{sd}` in a straight bar assuming constant
+            Where: p = transverse pressure at ultimate limit state along :math:`l_{bd}` [MPa].
+        l_b_rqd: MM
+            [:math:`l_{b,rqd}`] Basic required anchorage length, for anchoring the force As⋅σsd in a straight bar assuming constant
             bond stress (formula 8.3) [:math:`mm`].
 
             Use your own implementation for this value or use the :class:`Form8Dot3RequiredAnchorageLength` class.
-        l_0_min : MM
-            [:math:`l_{0,min}`] Minimum design lap length [:math:`mm`].
+        l_b_min : MM
+            [:math:`l_{b,min}`] Minimum anchorage length if no other limitation is applied [:math:`mm`].
 
-            :math:`= max(0.3 ⋅ α_{6} ⋅ l_{b,rqd}, 15 ⋅ Ø, 200)` (formula 8.11).
+            :math:`= max(0.3 ⋅ l_{b,rqd}, 10 ⋅ Ø, 100)` for tension anchorage (formula 8.6).
+            :math:`= max(0.6 ⋅ l_{b,rqd}, 10 ⋅ Ø, 100)` for compression anchorage (formula 8.7).
 
-            Use your own implementation of this formula or use :class:`Form8Dot11MinimumDesignLapLength` class.
+            Use your own implementation of this formula or use the :class:`Form8Dot6MinimumTensionAnchorage` class for tension or
+            :class:`Form8Dot7MinimumCompressionAnchorage` for compression.
+
+        Notes
+        -----
+        NEN-EN 1992-1-1+C2:2011 art.8.4.4(1) - Formula (8.5) prescribes that :math:`(α_{2} ⋅ α_{3} ⋅ α_{5}) >= 0.7`.
         """
         super().__init__()
         self.alpha_1 = alpha_1
         self.alpha_2 = alpha_2
         self.alpha_3 = alpha_3
+        self.alpha_4 = alpha_4
         self.alpha_5 = alpha_5
-        self.alpha_6 = alpha_6
         self.l_b_rqd = l_b_rqd
-        self.l_0_min = l_0_min
+        self.l_b_min = l_b_min
 
     @staticmethod
     def _evaluate(
         alpha_1: DIMENSIONLESS,
         alpha_2: DIMENSIONLESS,
         alpha_3: DIMENSIONLESS,
+        alpha_4: DIMENSIONLESS,
         alpha_5: DIMENSIONLESS,
-        alpha_6: DIMENSIONLESS,
         l_b_rqd: MM,
-        l_0_min: MM,
+        l_b_min: MM,
     ) -> MM:
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(
             alpha_1=alpha_1,
             alpha_2=alpha_2,
             alpha_3=alpha_3,
+            alpha_4=alpha_4,
             alpha_5=alpha_5,
-            alpha_6=alpha_6,
             l_b_rqd=l_b_rqd,
-            l_0_min=l_0_min,
+            l_b_min=l_b_min,
         )
-        return max(alpha_1 * alpha_2 * alpha_3 * alpha_5 * alpha_6 * l_b_rqd, l_0_min)
-
-
-class SubForm8Dot10Alpha6(Formula):
-    """Class representing the formula for the calculation of the coefficient :math:`α_{6}`."""
-
-    label = "8.8"
-    source_document = NEN_EN_1992_1_1_C2_2011
-
-    def __init__(self, rho_1: DIMENSIONLESS) -> None:
-        """[:math:`α_{6}`] Coefficient for the effect of reinforcement ratio [-].
+        return max(alpha_1 * alpha_2 * alpha_3 * alpha_4 * alpha_5 * l_b_rqd, l_b_min)
 
-        NEN-EN 1992-1-1+C2:2011 art.8.7.3(1) - Formula (8.8)
-
-        Parameters
-        ----------
-        rho_1 : DIMENSIONLESS
-            [:math:`ρ_{1}`] Reinforcement percentage lapped within :math:`0,65 ⋅ l_{0}` from the centre of the lap length
-            considered (see figure 8.8) [-].
-        """
-        super().__init__()
-        self.rho_1 = rho_1
-
-    @staticmethod
-    def _evaluate(rho_1: DIMENSIONLESS) -> DIMENSIONLESS:
-        """Evaluates the formula, for more information see the __init__ method."""
-        raise_if_negative(rho_l=rho_1)
-        value_max_1_5 = min((rho_1 / 25) ** 0.5, 1.5)
-        return max(value_max_1_5, 1)
+    def latex(self) -> LatexFormula:
+        """Returns a LatexFormula representation of the formula."""
+        return LatexFormula(
+            return_symbol=r"l_{bd}",
+            result=f"{self:.2f}",
+            equation=latex_max_curly_brackets(r"\alpha_1 \cdot \alpha_2 \cdot \alpha_3 \cdot \alpha_4 \cdot \alpha_5 \cdot l_{b,rqd}", r"l_{b,min}"),
+            numeric_equation=latex_max_curly_brackets(
+                rf"{self.alpha_1} \cdot {self.alpha_2} \cdot {self.alpha_3} \cdot {self.alpha_4} \cdot {self.alpha_5} \cdot {self.l_b_rqd:.2f}",
+                self.l_b_min,
+            ),
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_11.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_11.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Formula 8.11 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula, latex_max_curly_brackets
 from blueprints.type_alias import DIMENSIONLESS, MM
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot11MinimumDesignLapLength(Formula):
     """Class representing formula 8.11 for the calculation of the minimum design lap length :math:`l_{0,min}` [:math:`mm`]."""
 
@@ -54,7 +56,25 @@
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(
             alpha_6=alpha_6,
             l_b_rqd=l_b_rqd,
             diameter=diameter,
         )
         return max(0.3 * alpha_6 * l_b_rqd, 15 * diameter, 200)
+
+    def latex(self) -> LatexFormula:
+        """Returns a representation of the formula in LaTeX format."""
+        arg_1_equation = r"0.3 \cdot \alpha_6 \cdot l_{b,rqd}"
+        arg_2_equation = r"15 \cdot Ø"
+        arg_3_equation = r"200 \ \text{mm}"
+
+        arg_1_numerical_equation = rf"0.3 \cdot {self.alpha_6:.2f} \cdot {self.l_b_rqd:.2f}"
+        arg_2_numerical_equation = rf"15 \cdot {self.diameter}"
+        arg_3_numerical_equation = r"200"
+
+        return LatexFormula(
+            return_symbol=r"l_{0,min}",
+            result=f"{self:.2f}",
+            equation=f"{latex_max_curly_brackets(arg_1_equation, arg_2_equation, arg_3_equation)}",
+            numeric_equation=f"{latex_max_curly_brackets(arg_1_numerical_equation, arg_2_numerical_equation, arg_3_numerical_equation)}",
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_12.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_12.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.12 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, MM2
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot12AdditionalShearReinforcement(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_13.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_13.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.13 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, MM2
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot13AdditionalShearReinforcement(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_14.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_14.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.14 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, MM
 from blueprints.validations import raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_15.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_15.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.15 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, MPA
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
 
 
 class Form8Dot15PrestressTransferStress(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_16.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_16.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.16 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, MM, MPA
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
 
 
 class Form8Dot16BasicTransmissionLength(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_17.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_17.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.17 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MM
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot17DesignValueTransmissionLength1(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_18.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_18.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.18 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MM
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot18DesignValueTransmissionLength2(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_2.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Formula 8.2 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula
 from blueprints.type_alias import DIMENSIONLESS, MM, MPA
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot2UltimateBondStress(Formula):
     """Class representing formula 8.2 for the calculation of the design value of the ultimate bond stress for ribbed bars."""
 
@@ -13,34 +15,35 @@
 
     def __init__(
         self,
         eta_1: DIMENSIONLESS,
         eta_2: DIMENSIONLESS,
         f_ctd: MPA,
     ) -> None:
-        """[fbd] The design value of the ultimate bond stress for ribbed bars [-].
+        r"""[:math:`f_{bd}`] The design value of the ultimate bond stress for ribbed bars [-].
 
         NEN-EN 1992-1-1+C2:2011 art.8.4.2(2) - Formula (8.2)
 
         Parameters
         ----------
         eta_1 : DIMENSIONLESS
-            [η1] coefficient related to the quality of the bond condition and the position of the bar during concreting (see Figure 8.2) [-].
-            = 1 when ‘good’ conditions are obtained;
-            = 0.7 other cases and for bars in structural elements built with slip-forms, unless it can be shown that ‘good’ bond conditions exist;
+            [:math:`η_1`] coefficient related to the quality of the bond condition and the position of the bar during concreting (see Figure 8.2) [-].
+            = :math:`1` when ‘good’ conditions are obtained;
+            = :math:`1` other cases and for bars in structural elements built with slip-forms, unless it can be shown that ‘good’ bond conditions
+            exist;
             Use your own implementation of this formula or use the SubForm8Dot2CoefficientQualityOfBond class.
         eta_2 : DIMENSIONLESS
-            [η2] A factor related to the bar diameter [-].
-            = 1 for bars with a diameter ≤ 32 mm;
-            = (132 - Ø) / 100 for bars with a diameter > 32 mm.
+            [:math:`η_2`] A factor related to the bar diameter [-].
+            = :math:`1` for bars with a diameter ≤ :math:`32 \text{mm}`;
+            = :math:`(132 - Ø) / 100` for bars with a diameter > :math:`32 \text{mm}`.
             Use your own implementation of this value or use the SubForm8Dot2CoefficientBarDiameter class.
         f_ctd : MPA
-            [fctd] Design tensile strength of concrete according to art.3.1.6(2) [MPa].
-            Due to the increasing brittleness of higher strength concrete, fctk,0,05 should be limited here to the value for C60/75, unless it can be
-            verified that the average bond strength increases above this limit.
+            [:math:`f_{ctd}`] Design tensile strength of concrete according to art.3.1.6(2) [MPa].
+            Due to the increasing brittleness of higher strength concrete, :math:`f_{ctk,0,05}` should be limited here to the value for C60/75, unless
+            it can be verified that the average bond strength increases above this limit.
         """
         super().__init__()
         self.eta_1 = eta_1
         self.eta_2 = eta_2
         self.f_ctd = f_ctd
 
     @staticmethod
@@ -49,14 +52,24 @@
         eta_2: DIMENSIONLESS,
         f_ctd: MPA,
     ) -> MPA:
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(eta_1=eta_1, eta_2=eta_2, f_ctd=f_ctd)
         return 2.25 * eta_1 * eta_2 * f_ctd
 
+    def latex(self) -> LatexFormula:
+        """Returns a representation of the formula in LaTeX format."""
+        return LatexFormula(
+            return_symbol=r"f_{bd}",
+            result=f"{self:.2f}",
+            equation=r"2.25 \cdot \eta_1 \cdot \eta_2 \cdot f_{ctd}",
+            numeric_equation=rf"2.25 \cdot {self.eta_1:.2f} \cdot {self.eta_2:.2f} \cdot {self.f_ctd:.2f}",
+            comparison_operator_label="=",
+        )
+
 
 class SubForm8Dot2CoefficientQualityOfBond(Formula):
     """Class representing sub-formula for formula 8.2, which calculates the coefficient 'η1' which is dependent on the quality of the bond."""
 
     source_document = NEN_EN_1992_1_1_C2_2011
     label = "8.2"
 
@@ -91,26 +104,38 @@
 class SubForm8Dot2CoefficientBarDiameter(Formula):
     """Class representing sub-formula for formula 8.2, which calculates the coefficient 'η2' which is dependent on the bar diameter."""
 
     source_document = NEN_EN_1992_1_1_C2_2011
     label = "8.2"
 
     def __init__(self, diameter: MM) -> None:
-        """[η2] Coefficient that depends on the bar diameter [-].
+        """[:math:`η_2`] Coefficient that depends on the bar diameter [-].
 
-        NEN-EN 1992-1-1+C2:2011 art.8.4.2(2) - η2
+        NEN-EN 1992-1-1+C2:2011 art.8.4.2(2) - :math:`η_2`
 
         Parameters
         ----------
         diameter : MM
-            [Ø] Diameter of the bar [mm].
+            [:math:`Ø`] Diameter of the bar [mm].
         """
         super().__init__()
         self.diameter = diameter
 
     @staticmethod
     def _evaluate(diameter: MM) -> DIMENSIONLESS:
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(diameter=diameter)
         if diameter <= 32:
             return 1
         return (132 - diameter) / 100
+
+    def latex(self) -> LatexFormula:
+        """Returns a LatexFormula object for this formula."""
+        numerical_equation = "1.00" if self.diameter <= 32 else f"(132 - {self.diameter}) / 100"
+
+        return LatexFormula(
+            return_symbol=r"\eta_2",
+            result=f"{self:.2f}",
+            equation=r"\begin{matrix} 1.0 & \text{for }Ø ≤ 32 \\ (132 - Ø) / 100 & \text{for }Ø > 32  \end{matrix}",
+            numeric_equation=numerical_equation,
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_3.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1993_1_1_c2_a1_2016/chapter_2_basic_of_design/formula_2_2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,35 @@
-"""Formula 8.3 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
-from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
+"""Formula 2.2 from NEN-EN 1993-1-1+C2+A1:2016: Chapter 2: Basis of design."""
+
+from blueprints.codes.eurocode.nen_en_1993_1_1_c2_a1_2016 import NEN_EN_1993_1_1_C2_A1_2016
 from blueprints.codes.formula import Formula
-from blueprints.type_alias import MM, MPA
-from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
+from blueprints.type_alias import DIMENSIONLESS
+from blueprints.validations import raise_if_negative
 
 
-class Form8Dot3RequiredAnchorageLength(Formula):
-    """Class representing formula 8.3 for the calculation of the basic required anchorage length, assuming constant bond stress fbd."""
+class Form2Dot2CharacteristicValueResistance(Formula):
+    """Class representing formula 2.2 for the calculation of the characteristic value of the resistance :math:`R_k`."""
 
-    label = "8.3"
-    source_document = NEN_EN_1992_1_1_C2_2011
+    label = "2.2"
+    source_document = NEN_EN_1993_1_1_C2_A1_2016
 
-    def __init__(
-        self,
-        diameter: MM,
-        sigma_sd: MPA,
-        f_bd: MPA,
-    ) -> None:
-        """[lb,rqd] Basic required anchorage length, for anchoring the force As*σsd in a straight bar assuming constant bond stress fbd. [mm].
+    def __init__(self, r_d: float, gamma_mi: DIMENSIONLESS) -> None:
+        """[:math:`R_k`] Characteristic value of the resistance [:math:`kN`].
 
-        NEN-EN 1992-1-1+C2:2011 art.8.4.3(2) - Formula (8.3)
+        NEN-EN 1993-1-1+C2+A1:2016 art.2.5(2) - Formula (2.2)
 
         Parameters
         ----------
-        diameter: MM
-            [Ø] Diameter of the bar [mm].
-        sigma_sd: MPA
-            [σsd] design stress of the bar at the position from where the anchorage is measured from [MPa].
-        f_bd: MPA
-            [fbd] Design value ultimate bond stress [MPa].
-            Use your own implementation for this value or use the Form8Dot2UltimateBondStress class.
+        r_d : float
+            [:math:`R_d`] Design value of the resistance according to Annex D of EN 1990.
+        gamma_mi : DIMENSIONLESS
+            [:math:`γ_{Mi}`] Recommended partial factors for the resistance.
         """
         super().__init__()
-        self.diameter = diameter
-        self.sigma_sd = sigma_sd
-        self.f_bd = f_bd
+        self.r_d = r_d
+        self.gamma_mi = gamma_mi
 
     @staticmethod
-    def _evaluate(
-        diameter: MM,
-        sigma_sd: MPA,
-        f_bd: MPA,
-    ) -> MM:
+    def _evaluate(r_d: float, gamma_mi: DIMENSIONLESS) -> float:
         """Evaluates the formula, for more information see the __init__ method."""
-        raise_if_negative(diameter=diameter, sigma_sd=sigma_sd)
-        raise_if_less_or_equal_to_zero(f_bd=f_bd)
-        return (diameter / 4) * (sigma_sd / f_bd)
+        raise_if_negative(r_d=r_d, gamma_mi=gamma_mi)
+        return r_d * gamma_mi
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_4.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_10.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,180 @@
-"""Formula 8.4 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+"""Formula 8.10 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula, latex_max_curly_brackets, latex_min_curly_brackets
 from blueprints.type_alias import DIMENSIONLESS, MM
 from blueprints.validations import raise_if_negative
 
 
-class Form8Dot4DesignAnchorageLength(Formula):
-    """Class representing formula 8.4 for the calculation of the design anchorage length :math:`l_{bd}` [:math:`mm`]."""
+class Form8Dot10DesignLapLength(Formula):
+    """Class representing formula 8.10 for the calculation of the design lap length :math:`l_{0}` [:math:`mm`]."""
 
-    label = "8.4"
+    label = "8.10"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
         alpha_1: DIMENSIONLESS,
         alpha_2: DIMENSIONLESS,
         alpha_3: DIMENSIONLESS,
-        alpha_4: DIMENSIONLESS,
         alpha_5: DIMENSIONLESS,
+        alpha_6: DIMENSIONLESS,
         l_b_rqd: MM,
-        l_b_min: MM,
+        l_0_min: MM,
     ) -> None:
-        """[:math:`l_{bd}`] Design anchorage length [:math:`mm`].
+        """[:math:`l_{0}`] Design lap length [:math:`mm`].
 
-        NEN-EN 1992-1-1+C2:2011 art.8.4.4(1) - Formula (8.4)
+        NEN-EN 1992-1-1+C2:2011 art.8.7.3(1) - Formula (8.10)
 
         Parameters
         ----------
         alpha_1 : DIMENSIONLESS
             [:math:`α_{1}`] Coefficient for the effect of the form of the bars assuming adequate cover (see figure 8.1) [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1.0` for straight bars in tension.
 
-            :math:`= 1.0 if c_{d} <= 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
+            :math:`= 1.0` if :math:`c_{d} <= 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
 
-            :math:`= 0.7 if c_{d} > 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
+            :math:`= 0.7` if :math:`c_{d} > 3 ⋅ Ø` for bars other than straight in tension (see figure 8.1 (b), (c) and (d)).
 
-            Note: see figure 8.3 for values of :math:`c_{d}`.
+            Note: see figure 8.3 for values of cd.
         alpha_2 : DIMENSIONLESS
             [:math:`α_{2}`] Coefficient for the effect of minimum concrete cover (see figure 8.3) [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1 - 0.15 ⋅ (c_{d} - Ø) / Ø <= 1` with a minimum of 0.7 for straight bars in tension.
 
-            :math:`= 1 - 0.15 ⋅ (c_{d} - 3 ⋅ Ø) / Ø <= 1` with a minimum of 0.7 for bars other than
-            straight in tension (see figure 8.1 (b), (c) and (d)).
+            :math:`= 1 - 0.15 ⋅ (c_{d} - 3 ⋅ Ø) / Ø <= 1` with a minimum of 0.7 for bars other than straight in tension
+            (see figure 8.1 (b), (c) and (d)).
 
             Note: see figure 8.3 for values of :math:`c_{d}`.
         alpha_3 : DIMENSIONLESS
             [:math:`α_{3}`] Coefficient for the effect of confinement by transverse reinforcement [-].
 
             :math:`= 1.0` for bars in compression.
 
             :math:`= 1 - K ⋅ λ <= 1` with a minimum of 0.7 for bars in tension.
 
             Where: :math:`λ = (ΣA_{st} - ΣA_{st,min}) / A_{s}`.
 
-            Where: :math:`ΣA_{st,min}` = cross-sectional area of the minimum transverse
-            reinforcement :math:`= 0,25 ⋅ A_{s}` for beams and 0 for slabs.
-
-            Note: see figure 8.4 for values of :math:`K, A_{s} and A_{st}`.
-        alpha_4 : DIMENSIONLESS
-            [:math:`α_{4}`] Coefficient for the influence of one or more welded transverse bars :math:`(Ø_{t} > 0,6 Ø)` along the design anchorage
-            length :math:`l_{bd}` (see 8.6) [-].
+            Where: :math:`ΣA_{st,min} = A_{s} ⋅ (σ_{sd}/f_{yd})`
 
-            = 0.7 for all types, position and size as specified in figure 8.6 (e) in both tension and compression.
+            With :math:`A_{s}` = area of one lapped bar [mm²].
 
+            Note: see figure 8.4 for values of :math:`K, A_{s}` and :math:`A_{st}`.
         alpha_5 : DIMENSIONLESS
-            [:math:`α_{5}`] Coefficient for the effect of the pressure transverse to the plane of splitting
-            along the design anchorage length :math:`l_{bd}` (see 8.6) [-].
+            [:math:`α_{5}`] Coefficient for the effect of the pressure transverse to the plane of splitting along the design
+            anchorage length :math:`l_{bd}` (see 8.6) [-].
 
             :math:`= 1 - 0.04 ⋅ p <= 1` with a minimum of 0.7 for all types of anchorage in compression.
 
-            Where: p = transverse pressure at ultimate limit state along :math:`l_{bd}` [MPa].
-        l_b_rqd: MM
-            [:math:`l_{b,rqd}`] Basic required anchorage length, for anchoring the force As⋅σsd in a straight bar assuming constant
+            Where: p = transverse pressure at ultimate limit state along :math:`l_{bd}` [:math:`MPa`].
+        alpha_6 : DIMENSIONLESS
+            [:math:`α_{6}`] Coefficient for the effect of reinforcement ratio [-].
+
+            :math:`= (ρ_{1}/25)^{0.5} <= 1.5` with a minimum of 1.0.
+
+            Where: :math:`ρ_{1}` = reinforcement percentage lapped within :math:`0,65 ⋅ l_{0}` from the centre of the lap length
+            considered (see figure 8.8) [-].
+
+            Use your own implementation of this formula or use the :class:`SubForm8Dot10Alpha6` class.
+        l_b_rqd : MM
+            [:math:`l_{b,rqd}`] Basic required anchorage length, for anchoring the force :math:`A_{s} ⋅ σ_{sd}` in a straight bar assuming constant
             bond stress (formula 8.3) [:math:`mm`].
 
             Use your own implementation for this value or use the :class:`Form8Dot3RequiredAnchorageLength` class.
-        l_b_min : MM
-            [:math:`l_{b,min}`] Minimum anchorage length if no other limitation is applied [:math:`mm`].
+        l_0_min : MM
+            [:math:`l_{0,min}`] Minimum design lap length [:math:`mm`].
 
-            :math:`= max(0.3 ⋅ l_{b,rqd}, 10 ⋅ Ø, 100)` for tension anchorage (formula 8.6).
-            :math:`= max(0.6 ⋅ l_{b,rqd}, 10 ⋅ Ø, 100)` for compression anchorage (formula 8.7).
+            :math:`= max(0.3 ⋅ α_{6} ⋅ l_{b,rqd}, 15 ⋅ Ø, 200)` (formula 8.11).
 
-            Use your own implementation of this formula or use the :class:`Form8Dot6MinimumTensionAnchorage` class for tension or
-            :class:`Form8Dot7MinimumCompressionAnchorage` for compression.
-
-        Notes
-        -----
-        NEN-EN 1992-1-1+C2:2011 art.8.4.4(1) - Formula (8.5) prescribes that :math:`(α_{2} ⋅ α_{3} ⋅ α_{5}) >= 0.7`.
+            Use your own implementation of this formula or use :class:`Form8Dot11MinimumDesignLapLength` class.
         """
         super().__init__()
         self.alpha_1 = alpha_1
         self.alpha_2 = alpha_2
         self.alpha_3 = alpha_3
-        self.alpha_4 = alpha_4
         self.alpha_5 = alpha_5
+        self.alpha_6 = alpha_6
         self.l_b_rqd = l_b_rqd
-        self.l_b_min = l_b_min
+        self.l_0_min = l_0_min
 
     @staticmethod
     def _evaluate(
         alpha_1: DIMENSIONLESS,
         alpha_2: DIMENSIONLESS,
         alpha_3: DIMENSIONLESS,
-        alpha_4: DIMENSIONLESS,
         alpha_5: DIMENSIONLESS,
+        alpha_6: DIMENSIONLESS,
         l_b_rqd: MM,
-        l_b_min: MM,
+        l_0_min: MM,
     ) -> MM:
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(
             alpha_1=alpha_1,
             alpha_2=alpha_2,
             alpha_3=alpha_3,
-            alpha_4=alpha_4,
             alpha_5=alpha_5,
+            alpha_6=alpha_6,
             l_b_rqd=l_b_rqd,
-            l_b_min=l_b_min,
+            l_0_min=l_0_min,
+        )
+        return max(alpha_1 * alpha_2 * alpha_3 * alpha_5 * alpha_6 * l_b_rqd, l_0_min)
+
+    def latex(self) -> LatexFormula:
+        """Returns a LatexFormula representation of the formula."""
+        return LatexFormula(
+            return_symbol=r"l_{0}",
+            result=f"{self:.2f}",
+            equation=latex_max_curly_brackets(r"\alpha_1 \cdot \alpha_2 \cdot \alpha_3 \cdot \alpha_5 \cdot \alpha_6 \cdot l_{b,rqd}", r"l_{0,min}"),
+            numeric_equation=latex_max_curly_brackets(
+                rf"{self.alpha_1:.2f} \cdot {self.alpha_2:.2f} \cdot {self.alpha_3:.2f} \cdot "
+                rf"{self.alpha_5:.2f} \cdot {self.alpha_6:.2f} \cdot {self.l_b_rqd:.2f}",
+                f"{self.l_0_min:.2f}",
+            ),
+            comparison_operator_label="=",
+        )
+
+
+class SubForm8Dot10Alpha6(Formula):
+    """Class representing the formula for the calculation of the coefficient :math:`α_{6}`."""
+
+    label = "8.8"
+    source_document = NEN_EN_1992_1_1_C2_2011
+
+    def __init__(self, rho_1: DIMENSIONLESS) -> None:
+        """[:math:`α_{6}`] Coefficient for the effect of reinforcement ratio [-].
+
+        NEN-EN 1992-1-1+C2:2011 art.8.7.3(1) - Formula (8.8)
+
+        Parameters
+        ----------
+        rho_1 : DIMENSIONLESS
+            [:math:`ρ_{1}`] Reinforcement percentage lapped within :math:`0,65 ⋅ l_{0}` from the centre of the lap length
+            considered (see figure 8.8) [-].
+        """
+        super().__init__()
+        self.rho_1 = rho_1
+
+    @staticmethod
+    def _evaluate(rho_1: DIMENSIONLESS) -> DIMENSIONLESS:
+        """Evaluates the formula, for more information see the __init__ method."""
+        raise_if_negative(rho_l=rho_1)
+        value_max_1_5 = min((rho_1 / 25) ** 0.5, 1.5)
+        return max(value_max_1_5, 1)
+
+    def latex(self) -> LatexFormula:
+        """Returns a LatexFormula representation of the formula."""
+        argument_1_formula = r"\left(\frac{\rho_1}{25}\right)^{0.5}"
+        numerical_argument_1 = rf"\left(\frac{{{self.rho_1:.2f}}}{{25}}\right)^{{0.5}}"
+        return LatexFormula(
+            return_symbol=r"\alpha_6",
+            result=f"{self:.2f}",
+            equation=f'{latex_max_curly_brackets(latex_min_curly_brackets(argument_1_formula, "1.5"), "1")}',
+            numeric_equation=f'{latex_max_curly_brackets(latex_min_curly_brackets(numerical_argument_1, "1.5"), "1")}',
+            comparison_operator_label="=",
         )
-        return max(alpha_1 * alpha_2 * alpha_3 * alpha_4 * alpha_5 * l_b_rqd, l_b_min)
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_6.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_16.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-"""Formula 8.6 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+"""Formula 9.16 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
-from blueprints.type_alias import MM
+from blueprints.type_alias import KN, KN_M, M
 from blueprints.validations import raise_if_negative
 
 
-class Form8Dot6MinimumTensionAnchorage(Formula):
-    """Class representing formula 8.6 for the calculation of the minimum anchorage length if no other limitation is applied for anchorage in
-    tension.
-    """
+class Form9Dot16MinimumForceOnInternalBeamLine(Formula):
+    """Class representing the formula 9.16 for calculating the minimum force on an internal beam line for floors without screeds."""
 
-    label = "8.6"
+    label = "9.16"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
-        l_b_rqd: MM,
-        diameter: MM,
+        q_3: KN_M,
+        l_1: M,
+        l_2: M,
+        q_4: KN,
     ) -> None:
-        """[lb,min] Minimum anchorage length if no other limitation is applied for anchorage in tension. [mm].
+        """[Ftie] Minimum force on an internal beam line [kN].
 
-        NEN-EN 1992-1-1+C2:2011 art.8.4.4(1) - Formula (8.6)
+        NEN-EN 1992-1-1+C2:2011 art.9.10.2.3(4) - Formula (9.16)
 
         Parameters
         ----------
-        l_b_rqd: MM
-            [lb,rqd] Basic required anchorage length, for anchoring the force As*σsd in a straight bar assuming constant
-            bond stress (formula 8.3) [mm].
-            Use your own implementation for this value or use the Form8Dot3RequiredAnchorageLength class.
-        diameter: MM
-            [Ø] Diameter of the bar [mm].
+        q_3: KN_M
+            [q3] May be found in national annex, recommended value is 20 [kN/m].
+        l_1: M
+            [l1] span length of floor slabs on either side of the beam, see figure 9.15 [m].
+        l_2: M
+            [l2] span length of floor slabs on either side of the beam, see figure 9.15 [m].
+        q_4: KN
+            [Q4] May be found in national annex, recommended value is 70 [kN].
         """
         super().__init__()
-        self.l_b_rqd = l_b_rqd
-        self.diameter = diameter
+        self.q_3 = q_3
+        self.l_1 = l_1
+        self.l_2 = l_2
+        self.q_4 = q_4
 
     @staticmethod
-    def _evaluate(l_b_rqd: MM, diameter: MM) -> MM:
-        """Evaluates the formula, for more information see the __init__ method."""
-        raise_if_negative(diameter=diameter, l_b_rqd=l_b_rqd)
-        return max(0.3 * l_b_rqd, 10 * diameter, 100)
+    def _evaluate(
+        q_3: KN_M,
+        l_1: M,
+        l_2: M,
+        q_4: KN,
+    ) -> KN:
+        """For more detailed documentation see the class docstring."""
+        raise_if_negative(q_3=q_3, l_1=l_1, l_2=l_2, q_4=q_4)
+        return max(q_3 * (l_1 + l_2) / 2, q_4)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_7.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_7.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Formula 8.7 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
+from blueprints.codes.latex_formula import LatexFormula, latex_max_curly_brackets
 from blueprints.type_alias import MM
 from blueprints.validations import raise_if_negative
 
 
 class Form8Dot7MinimumCompressionAnchorage(Formula):
     """Class representing formula 8.7 for the calculation of the minimum anchorage length if no other limitation is applied for anchorage in
     compression.
@@ -36,7 +38,21 @@
         self.diameter = diameter
 
     @staticmethod
     def _evaluate(l_b_rqd: MM, diameter: MM) -> MM:
         """Evaluates the formula, for more information see the __init__ method."""
         raise_if_negative(diameter=diameter, l_b_rqd=l_b_rqd)
         return max(0.6 * l_b_rqd, 10 * diameter, 100)
+
+    def latex(self) -> LatexFormula:
+        """Returns a LatexFormula object for this formula."""
+        return LatexFormula(
+            return_symbol=r"l_{b,min}",
+            result=f"{self:.2f}",
+            equation=latex_max_curly_brackets(r"0.6 \cdot l_{b,rqd}", r"10 \cdot Ø", r"100 \ \text{mm}"),
+            numeric_equation=latex_max_curly_brackets(
+                rf"0.6 \cdot {self.l_b_rqd:.2f}",
+                rf"10 \cdot {self.diameter}",
+                r"100",
+            ),
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_8n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_8n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Formula 8.8N from NEN-EN 1992-1-1+C2:2011: Chapter 8 - Detailing of reinforcement and prestressing tendons."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DIMENSIONLESS, KN, MM, MPA
 from blueprints.unit_conversion import N_TO_KN
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
 
 
-class Form8Dot8NAnchorageCapacityWeldedTransverseBar(Formula):
+class Form8Dot8nAnchorageCapacityWeldedTransverseBar(Formula):
     """Class representing the formula 8.8N for the calculation of the anchorage capacity of welded transverse bar, welded on the inside of the main
     bar.
     """
 
     label = "8.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
@@ -32,23 +33,23 @@
         Parameters
         ----------
         l_td: MM
             [:math:`l_{td}`] Design length of transverse bar [:math:`mm`].
 
             :math:`= 1.16 ⋅ ø_{t} ⋅ (f_{yd}/σ_{td})^{0.5} ≤ l_{t}`
 
-            Use your own implementation of this formula or use the SubForm8Dot8NDesignLengthOfTransverseBar class.
+            Use your own implementation of this formula or use the SubForm8Dot8nDesignLengthOfTransverseBar class.
         diameter_t: MM
             [:math:`ø_{t}`] Diameter of transverse bar [:math:`mm`].
         sigma_td: MPA
             [:math:`σ_{td}`] Concrete stress [:math:`MPa`].
 
             :math:`=(f_{ctd}+σ_{cm})/y ≤ 3⋅f_{cd}`
 
-            Use your own implementation of this formula or use the SubForm8Dot8NConcreteStress class.
+            Use your own implementation of this formula or use the SubForm8Dot8nConcreteStress class.
         f_wd: KN
             [:math:`F_{wd}`] Design shear strength of weld (specified as a factor times :math:`A_{s}⋅f_{yd}`; say :math:`0.5⋅A_{s}⋅f_{yd}` where
             :math:`A_{s}` is the cross-section of the anchored bar and fyd is its design yield strength)  [kN].
         """
         super().__init__()
         self.l_td = l_td
         self.diameter_t = diameter_t
@@ -68,15 +69,15 @@
             diameter_t=diameter_t,
             sigma_td=sigma_td,
             f_wd=f_wd,
         )
         return min(l_td * diameter_t * sigma_td * N_TO_KN, f_wd)
 
 
-class SubForm8Dot8NDesignLengthOfTransverseBar(Formula):
+class SubForm8Dot8nDesignLengthOfTransverseBar(Formula):
     """Class representing sub-formula for formula 8.8N, which calculates the design length of the transverse bar."""
 
     label = "8.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
@@ -96,15 +97,15 @@
         f_yd: MPA
             [:math:`f_{yd}`] Design yield strength of bar [:math:`MPa`].
         sigma_td: MPA
             [:math:`σ_{td}`] Concrete stress [:math:`MPa`].
 
             :math:`=(f_{ctd}+σ_{cm})/y ≤ 3⋅f_{cd}`
 
-            Use your own implementation of this formula or use the SubForm8Dot8NConcreteStress class.
+            Use your own implementation of this formula or use the SubForm8Dot8nConcreteStress class.
         l_t: MM
             [:math:`l_{t}`] Length of transverse bar, but not more than the spacing of bars to be anchored [:math:`mm`].
         """
         super().__init__()
         self.diameter_t = diameter_t
         self.f_yd = f_yd
         self.sigma_td = sigma_td
@@ -123,15 +124,15 @@
             f_yd=f_yd,
             l_t=l_t,
         )
         raise_if_less_or_equal_to_zero(sigma_td=sigma_td)
         return min(1.16 * diameter_t * (f_yd / sigma_td) ** 0.5, l_t)
 
 
-class SubForm8Dot8NConcreteStress(Formula):
+class SubForm8Dot8nConcreteStress(Formula):
     """Class representing sub-formula for formula 8.8N, which calculates the concrete stress."""
 
     label = "8.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
@@ -151,15 +152,15 @@
         sigma_cm: MPA
             [:math:`σ_{cm}`] Compression in the concrete perpendicular to both bars (mean value) [:math:`MPa`].
         y_function: DIMENSIONLESS
             [y] A function [-]
 
             :math:`= 0.015 + 0.14 ⋅ exp(-0.18⋅x)`
 
-            Use your own implementation of this formula or use the SubForm8Dot8NFunctionY class.
+            Use your own implementation of this formula or use the SubForm8Dot8nFunctionY class.
         f_cd: MPA
             [:math:`f_{cd}`] Design value compressive strength of concrete [:math:`MPa`].
         """
         super().__init__()
         self.f_ctd = f_ctd
         self.sigma_cm = sigma_cm
         self.y_function = y_function
@@ -178,15 +179,15 @@
             sigma_cm=sigma_cm,
             f_cd=f_cd,
         )
         raise_if_less_or_equal_to_zero(y_function=y_function)
         return min((f_ctd + sigma_cm) / y_function, 3 * f_cd)
 
 
-class SubForm8Dot8NFunctionY(Formula):
+class SubForm8Dot8nFunctionY(Formula):
     """Class representing sub-formula for formula 8.8N, which calculates the function y."""
 
     label = "8.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
@@ -199,29 +200,29 @@
         Parameters
         ----------
         x_function: DIMENSIONLESS
             [x] A function accounting for the geometry [-]
 
             :math:`= 2⋅(c/ø_{t}) + 1`
 
-            Use your own implementation of this formula or use the SubForm8Dot8NFunctionX class.
+            Use your own implementation of this formula or use the SubForm8Dot8nFunctionX class.
         """
         super().__init__()
         self.x_function = x_function
 
     @staticmethod
     def _evaluate(
         x_function: DIMENSIONLESS,
     ) -> DIMENSIONLESS:
         """For more detailed documentation see the class docstring."""
         raise_if_negative(x_function=x_function)
         return 0.015 + 0.14 * np.exp(-0.18 * x_function)
 
 
-class SubForm8Dot8NFunctionX(Formula):
+class SubForm8Dot8nFunctionX(Formula):
     """Class representing sub-formula for formula 8.8N, which calculates the function x."""
 
     label = "8.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_9.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_8_detailing_of_reinforcement_and_prestressing_tendons/formula_8_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 8.9 from NEN-EN 1992-1-1+C2:2011: Chapter 8: Detailing of reinforcement and prestressing tendons."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM, MM2, MPA
 from blueprints.unit_conversion import N_TO_KN
 from blueprints.validations import raise_if_less_or_equal_to_zero, raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_10.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_10.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.10 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MM
 from blueprints.validations import raise_if_negative
 
 
 class Form9Dot10MaximumSpacingBentUpBars(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_12n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_12n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Formula 9.12N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM2, MPA
 from blueprints.unit_conversion import KN_TO_N
 from blueprints.validations import raise_if_negative
 
 
-class Form9Dot12NMinimumLongitudinalReinforcementColumns(Formula):
+class Form9Dot12nMinimumLongitudinalReinforcementColumns(Formula):
     """Class representing the formula 9.12N for the calculation of the minimum longitudinal reinforcement for columns."""
 
     label = "9.12N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_13.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_13.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.13 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM
 from blueprints.validations import raise_if_negative
 
 
 class Form9Dot13TensileForceToBeAnchored(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_14.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_14.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.14 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing and specific rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM
 from blueprints.validations import raise_if_negative
 
 
 class Form9Dot14SplittingForceColumnOnRock(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_1n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_6n.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,49 @@
-"""Formula 9.1N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+"""Formula 9.6N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
+import numpy as np
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
-from blueprints.type_alias import MM, MM2, MPA
-from blueprints.validations import raise_if_negative
+from blueprints.type_alias import DEG, MM
+from blueprints.validations import raise_if_greater_than_90, raise_if_negative
 
 
-class Form9Dot1NMinimumTensileReinforcementBeam(Formula):
-    """Class representing the formula 9.1N for the calculation of minimum tensile reinforcement area in longitudinal direction for beams."""
+class Form9Dot6nMaximumDistanceShearReinforcement(Formula):
+    """Class representing the formula 9.6N for the calculation of the maximum distance between shear reinforcement in longitudinal direction."""
 
-    label = "9.1N"
+    label = "9.6N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
-        f_ctm: MPA,
-        f_yk: MPA,
-        b_t: MM,
         d: MM,
+        alpha: DEG,
     ) -> None:
-        """[As,min] Calculates the minimum required tensile reinforcement area in longitudinal direction for beams [mm²].
+        """[sl,max] Maximum distance between shear reinforcement in longitudinal direction [mm].
 
-        NEN-EN 1992-1-1+C2:2011 art.9.2.1.1(1) - Formula (9.1N)
-
-        Notes
-        -----
-        As,min is no less than 0,0013 * bt * d
+        NEN-EN 1992-1-1+C2:2011 art.9.2.2(6) - Formula (9.6N)
 
         Parameters
         ----------
-        f_ctm: MPA
-            [fctm] Mean axial tensile stress concrete [MPa].
-            Should be determined with respect to the relevant strength class according to Table 3.1
-        f_yk: MPA
-            [fyk] Characteristic yield strength reinforcement steel [MPa].
-        b_t: MM
-            [bt] Mean width of the concrete tension zone, for T-beams with a flange under compression only the width of the web is considered for
-            calculating bt [mm].
         d: MM
             [d] Effective height of the cross-section [mm].
+        alpha: DEG
+            [α] The angle between the shear reinforcement and the longitudinal axis of the beam (see 9.2.2(1)) [deg].
         """
         super().__init__()
-        self.f_ctm = f_ctm
-        self.f_yk = f_yk
-        self.b_t = b_t
         self.d = d
+        self.alpha = alpha
 
     @staticmethod
-    def _evaluate(
-        f_ctm: MPA,
-        f_yk: MPA,
-        b_t: MM,
-        d: MM,
-    ) -> MM2:
+    def _evaluate(d: MM, alpha: DEG) -> MM:
         """For more detailed documentation see the class docstring."""
-        raise_if_negative(f_ctm=f_ctm, f_yk=f_yk, b_t=b_t, d=d)
-        return max(0.26 * (f_ctm / f_yk) * b_t * d, 0.0013 * b_t * d)
+        raise_if_negative(d=d, alpha=alpha)
+        raise_if_greater_than_90(alpha=alpha)
+
+        # Convert the angle from degrees to radians
+        alpha_radians = np.deg2rad(alpha)
+
+        # Calculate the cotangent
+        cot_alpha = 1 / np.tan(alpha_radians)
+
+        return 0.75 * d * (1 + cot_alpha)
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_2.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.2 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DEG, MM
 from blueprints.validations import raise_if_greater_than_90, raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_3.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.3 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import KN, MM
 from blueprints.validations import raise_if_negative
 
 
 class Form9Dot3ShiftInMomentDiagram(Formula):
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_4.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Formula 9.4 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DEG, DIMENSIONLESS, MM, MM2
 from blueprints.validations import raise_if_greater_than_90, raise_if_negative
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_5n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_5n.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Formula 9.5N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MPA
 from blueprints.validations import raise_if_negative
 
 
-class Form9Dot5NMinimumShearReinforcementRatio(Formula):
+class Form9Dot5nMinimumShearReinforcementRatio(Formula):
     """Class representing the formula 9.5N for the calculation of the minimum shear reinforcement ratio for beams."""
 
     label = "9.5N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_6n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_9.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-"""Formula 9.6N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+"""Formula 9.9 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DEG, MM
-from blueprints.validations import raise_if_greater_than_90, raise_if_negative
+from blueprints.validations import raise_if_negative
 
 
-class Form9Dot6NMaximumDistanceShearReinforcement(Formula):
-    """Class representing the formula 9.6N for the calculation of the maximum distance between shear reinforcement in longitudinal direction."""
+class Form9Dot9MaximumSpacingSeriesOfLinks(Formula):
+    """Class representing the formula 9.9 for the calculation of the maximum distance between successive series of links in longitudinal direction
+    for slabs.
+    """
 
-    label = "9.6N"
+    label = "9.9"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
         d: MM,
         alpha: DEG,
     ) -> None:
-        """[sl,max] Maximum distance between shear reinforcement in longitudinal direction [mm].
+        """[smax] Maximum distance between successive series of links in longitudinal direction for slabs [mm].
 
-        NEN-EN 1992-1-1+C2:2011 art.9.2.2(6) - Formula (9.6N)
+        NEN-EN 1992-1-1+C2:2011 art.9.3.2(4) - Formula (9.9)
 
         Parameters
         ----------
         d: MM
             [d] Effective height of the cross-section [mm].
         alpha: DEG
-            [α] The angle between the shear reinforcement and the longitudinal axis of the beam (see 9.2.2(1)) [deg].
+            [α] The angle between the shear reinforcement and the longitudinal axis of the slab (see 9.2.2(1)) [deg].
         """
         super().__init__()
         self.d = d
         self.alpha = alpha
 
     @staticmethod
     def _evaluate(d: MM, alpha: DEG) -> MM:
         """For more detailed documentation see the class docstring."""
-        raise_if_negative(d=d, alpha=alpha)
-        raise_if_greater_than_90(alpha=alpha)
+        raise_if_negative(d=d)
 
         # Convert the angle from degrees to radians
         alpha_radians = np.deg2rad(alpha)
 
         # Calculate the cotangent
         cot_alpha = 1 / np.tan(alpha_radians)
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_7n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_7n.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Formula 9.7N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 import numpy as np
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import DEG, MM
 from blueprints.validations import raise_if_greater_than_90, raise_if_negative
 
 
-class Form9Dot7NMaximumDistanceBentUpBars(Formula):
+class Form9Dot7nMaximumDistanceBentUpBars(Formula):
     """Class representing the formula 9.7N for the calculation of the maximum distance between bent-up bars in longitudinal direction."""
 
     label = "9.7N"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_8n.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_8n.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Formula 9.8N from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailing of members and particular rules."""
+
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
 from blueprints.type_alias import MM
 from blueprints.validations import raise_if_negative
 
 
-class Form9Dot8NMaximumTransverseDistanceLegsSeriesShearLinks(Formula):
+class Form9Dot8nMaximumTransverseDistanceLegsSeriesShearLinks(Formula):
     """Class representing the formula 9.8N for the calculation of the maximum distance in transverse direction between legs in a series of shear
     links.
     """
 
     label = "9.8N"
     source_document = NEN_EN_1992_1_1_C2_2011
```

### Comparing `blue-prints-0.0.4/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_9_detailling_and_specific_rules/formula_9_9.py` & `blue_prints-0.0.5/blueprints/codes/eurocode/nen_en_1992_1_1_c2_2011/chapter_5_structural_analysis/formula_5_5.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,70 @@
-"""Formula 9.9 from NEN-EN 1992-1-1+C2:2011: Chapter 9 - Detailling and specific rules."""
-import numpy as np
+"""Formula 5.5 from NEN-EN 1992-1-1+C2:2011: Chapter 5 - Structural Analysis."""
 
 from blueprints.codes.eurocode.nen_en_1992_1_1_c2_2011 import NEN_EN_1992_1_1_C2_2011
 from blueprints.codes.formula import Formula
-from blueprints.type_alias import DEG, MM
+from blueprints.codes.latex_formula import LatexFormula
+from blueprints.type_alias import DIMENSIONLESS, KN
 from blueprints.validations import raise_if_negative
 
 
-class Form9Dot9MaximumSpacingSeriesOfLinks(Formula):
-    """Class representing the formula 9.9 for the calculation of the maximum distance between successive series of links in longitudinal direction
-    for slabs.
+class Form5Dot5TransverseForceEffectFloorDiaphragm(Formula):
+    """Class representing formula 5.5 for the calculation of the effect of the inclination on floor diaphragm, :math:`H_{i}`.
+
+    See Figure 5.1 c1.
     """
 
-    label = "9.9"
+    label = "5.5"
     source_document = NEN_EN_1992_1_1_C2_2011
 
     def __init__(
         self,
-        d: MM,
-        alpha: DEG,
+        theta_i: DIMENSIONLESS,
+        n_a: KN,
+        n_b: KN,
     ) -> None:
-        """[smax] Maximum distance between successive series of links in longitudinal direction for slabs [mm].
+        """[:math:`H_{i}`] Effect of the inclination on floor diaphragm [:math:`kN`].
 
-        NEN-EN 1992-1-1+C2:2011 art.9.3.2(4) - Formula (9.9)
+        NEN-EN 1992-1-1+C2:2011 art.5.2(8) - Formula (5.5)
 
         Parameters
         ----------
-        d: MM
-            [d] Effective height of the cross-section [mm].
-        alpha: DEG
-            [α] The angle between the shear reinforcement and the longitudinal axis of the slab (see 9.2.2(1)) [deg].
+        theta_i : DIMENSIONLESS
+            [:math:`Θ_{i}`] Eccentricity, initial inclination imperfections [-].
+        n_a : KN
+            [:math:`N_{a}`] Axial force in the member [:math:`kN`].
+        n_b : KN
+            [:math:`N_{b}`] Axial force in the member [:math:`kN`].
+
+        Notes
+        -----
+        where :math:`N_{a} and :math:`N_{b}` are longitudinal forces contributing to :math:`H_{i}`.
+        Positive values for compression, tension is not allowed.
         """
         super().__init__()
-        self.d = d
-        self.alpha = alpha
+        self.theta_i = theta_i
+        self.n_a = n_a
+        self.n_b = n_b
 
     @staticmethod
-    def _evaluate(d: MM, alpha: DEG) -> MM:
-        """For more detailed documentation see the class docstring."""
-        raise_if_negative(d=d)
-
-        # Convert the angle from degrees to radians
-        alpha_radians = np.deg2rad(alpha)
-
-        # Calculate the cotangent
-        cot_alpha = 1 / np.tan(alpha_radians)
-
-        return 0.75 * d * (1 + cot_alpha)
+    def _evaluate(
+        theta_i: DIMENSIONLESS,
+        n_a: KN,
+        n_b: KN,
+    ) -> KN:
+        """Evaluates the formula, for more information see the __init__ method."""
+        raise_if_negative(
+            theta_i=theta_i,
+            n_a=n_a,
+            n_b=n_b,
+        )
+        return theta_i * (n_b + n_a) / 2
+
+    def latex(self) -> LatexFormula:
+        """Returns LatexFormula object for formula 5.5."""
+        return LatexFormula(
+            return_symbol=r"H_{i}",
+            result=f"{self:.3f}",
+            equation=r"Θ_{i} \cdot (N_{b} + N_{a}) / 2",
+            numeric_equation=rf"{self.theta_i:.3f} \cdot ({self.n_b:.3f} + {self.n_a:.3f}) / 2",
+            comparison_operator_label="=",
+        )
```

### Comparing `blue-prints-0.0.4/blueprints/codes/formula.py` & `blue_prints-0.0.5/blueprints/codes/formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for the abstract base class Formula."""
+
 from abc import ABC, abstractmethod
 
 
 class Formula(float, ABC):
     """Abstract base class for formulas used in the codes."""
 
     def __new__(cls, *args, **kwargs) -> "Formula":
```

### Comparing `blue-prints-0.0.4/blueprints/type_alias.py` & `blue_prints-0.0.5/blueprints/type_alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to keep track of type aliases used in Blueprints."""
+
 # <editor-fold desc="DISTANCES">
 MM = float
 CM = float
 M = float
 KM = float
 # </editor-fold>
```

### Comparing `blue-prints-0.0.4/blueprints/validations.py` & `blue_prints-0.0.5/blueprints/validations.py`

 * *Files identical despite different names*

### Comparing `blue-prints-0.0.4/pyproject.toml` & `blue_prints-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blue-prints-0.0.4/tests/test_validations.py` & `blue_prints-0.0.5/tests/test_validations.py`

 * *Files identical despite different names*

