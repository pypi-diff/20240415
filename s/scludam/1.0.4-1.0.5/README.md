# Comparing `tmp/scludam-1.0.4-py3-none-any.whl.zip` & `tmp/scludam-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 113750 bytes, number of entries: 29
--rw-rw-r--  2.0 unx     2206 b- defN 23-Jun-25 22:01 scludam/__init__.py
+Zip file size: 123870 bytes, number of entries: 33
+-rw-rw-r--  2.0 unx     2230 b- defN 24-Apr-14 22:09 scludam/__init__.py
+-rw-rw-r--  2.0 unx     1216 b- defN 24-Apr-14 22:09 scludam/cli.py
+-rw-rw-r--  2.0 unx    14483 b- defN 24-Apr-14 19:39 scludam/cli_analysis.py
+-rw-rw-r--  2.0 unx     6146 b- defN 24-Apr-14 19:34 scludam/cli_input.py
+-rw-rw-r--  2.0 unx    11802 b- defN 24-Apr-14 19:31 scludam/cli_utils.py
 -rw-rw-r--  2.0 unx    38242 b- defN 23-Nov-30 22:54 scludam/detection.py
 -rw-rw-r--  2.0 unx    24162 b- defN 22-Nov-12 22:56 scludam/fetcher.py
 -rw-rw-r--  2.0 unx    29047 b- defN 23-Nov-30 23:37 scludam/hkde.py
 -rw-rw-r--  2.0 unx     7447 b- defN 22-Oct-08 02:29 scludam/masker.py
 -rw-rw-r--  2.0 unx    18095 b- defN 23-Nov-30 23:23 scludam/membership.py
 -rw-rw-r--  2.0 unx    22184 b- defN 23-Nov-30 23:23 scludam/pipeline.py
 -rw-rw-r--  2.0 unx    28380 b- defN 23-Nov-30 23:41 scludam/plots.py
@@ -19,13 +23,13 @@
 -rw-rw-r--  2.0 unx     9993 b- defN 23-Jun-25 22:01 tests/test_membership.py
 -rw-rw-r--  2.0 unx    10177 b- defN 23-Jun-25 22:01 tests/test_pipeline.py
 -rw-rw-r--  2.0 unx    17500 b- defN 22-Jul-13 00:03 tests/test_shdbscan.py
 -rw-rw-r--  2.0 unx     5054 b- defN 22-Dec-16 04:18 tests/test_stat_tests.py
 -rw-rw-r--  2.0 unx    16673 b- defN 22-Jun-09 03:55 tests/test_synthetic.py
 -rw-rw-r--  2.0 unx     3009 b- defN 22-Aug-27 02:10 tests/test_utils.py
 -rw-rw-r--  2.0 unx      611 b- defN 22-Jul-13 00:03 tests/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Nov-30 23:59 scludam-1.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5384 b- defN 23-Nov-30 23:59 scludam-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Nov-30 23:59 scludam-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Nov-30 23:59 scludam-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2238 b- defN 23-Nov-30 23:59 scludam-1.0.4.dist-info/RECORD
-29 files, 433403 bytes uncompressed, 110268 bytes compressed:  74.6%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-14 22:31 scludam-1.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5384 b- defN 24-Apr-14 22:31 scludam-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-14 22:31 scludam-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-Apr-14 22:31 scludam-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-14 22:31 scludam-1.0.5.dist-info/RECORD
+33 files, 467381 bytes uncompressed, 119930 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,10 +1,22 @@
 Filename: scludam/__init__.py
 Comment: 
 
+Filename: scludam/cli.py
+Comment: 
+
+Filename: scludam/cli_analysis.py
+Comment: 
+
+Filename: scludam/cli_input.py
+Comment: 
+
+Filename: scludam/cli_utils.py
+Comment: 
+
 Filename: scludam/detection.py
 Comment: 
 
 Filename: scludam/fetcher.py
 Comment: 
 
 Filename: scludam/hkde.py
@@ -66,23 +78,23 @@
 
 Filename: tests/test_utils.py
 Comment: 
 
 Filename: tests/utils.py
 Comment: 
 
-Filename: scludam-1.0.4.dist-info/LICENSE
+Filename: scludam-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: scludam-1.0.4.dist-info/METADATA
+Filename: scludam-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: scludam-1.0.4.dist-info/WHEEL
+Filename: scludam-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: scludam-1.0.4.dist-info/top_level.txt
+Filename: scludam-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: scludam-1.0.4.dist-info/RECORD
+Filename: scludam-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scludam/__init__.py

```diff
@@ -40,7 +40,8 @@
 from .detection import CountPeakDetector, default_mask, extend_1dmask
 from .fetcher import Query, search_object, search_objects_near_data, search_table
 from .hkde import HKDE, PluginSelector, RuleOfThumbSelector
 from .membership import DBME
 from .pipeline import DEP
 from .shdbscan import SHDBSCAN
 from .stat_tests import DipDistTest, HopkinsTest, RipleysKTest
+from .cli import launch
```

## Comparing `scludam-1.0.4.dist-info/LICENSE` & `scludam-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scludam-1.0.4.dist-info/METADATA` & `scludam-1.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scludam
-Version: 1.0.4
+Version: 1.0.5
 Summary: Star cluster detection and membership estimation based on GAIA data.
 Home-page: http://packages.python.org/scludam
 Author: Simón Pedro González
 Author-email: simon.pedro.g@gmail.com
 License: GPL-3
 Keywords: star cluster detection membership probabilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `scludam-1.0.4.dist-info/RECORD` & `scludam-1.0.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-scludam/__init__.py,sha256=qA1uv9DzxQv7J20FImLDZz573KDsx959DWj0Rf4uIm0,2206
+scludam/__init__.py,sha256=K2F0TbLqJj09bSRkLjQgFpf_xhnT_WmCOjP3ogojVBU,2230
+scludam/cli.py,sha256=-XLL8GTjLsG1TkLnsRG4ihFfITyiQ6l-CT14Iqj2I10,1216
+scludam/cli_analysis.py,sha256=m6kaO3c-hzdZJ0NRCwI32nfvEf7wwEtRX6oYw1_FmlM,14483
+scludam/cli_input.py,sha256=RDLU-Th3IZ2rU5AsXAp0hC5YB1yzfbZpe2Jvp9ZIJ6w,6146
+scludam/cli_utils.py,sha256=YoWVcfVwP3mJeMzJ_agPwZOEsNjx_iLfABfIqIvmk6s,11802
 scludam/detection.py,sha256=lLOUf6jyVuEuUOZJLRZvpVj2Bzp10gRWI0ulPL0Ow-g,38242
 scludam/fetcher.py,sha256=gTUdQThPb-4wMxD_SaEbJ3jXOQ4Jnyx-KZUonArbb4A,24162
 scludam/hkde.py,sha256=BBr8dxLbp0OQDh3Xb-DSKzaiNIbM6rfmJK0DWF4D4Nc,29047
 scludam/masker.py,sha256=n0Esyvy8ltK-KC_jKA0lLYtnzLANB8EbcMWD0OhTeW4,7447
 scludam/membership.py,sha256=DwbyyXd4ZomFYcgZJEz7RR1dUf20UZ5E2jjtqdmdVbA,18095
 scludam/pipeline.py,sha256=7A-q7rYT7dwCIV3cmQNPZpSdX-9uPkCXXhLH1fuf6f0,22184
 scludam/plots.py,sha256=8CQ4NtOdpIvPL6UtbWNS8iEmha2N5c65pm20eARGoTM,28380
@@ -18,12 +22,12 @@
 tests/test_membership.py,sha256=bhaGpr2KTGTnFHVzhVC8hBTYvl1K6w4kBAR8S5EouMw,9993
 tests/test_pipeline.py,sha256=A_H6wXnKeunFeVm4UHk5T4J2d_AM3aXMAiY1kQgAtEI,10177
 tests/test_shdbscan.py,sha256=CM8FIqpfXDTUn2OOH8jdH6aIyR9fk5lA9Qx8foITmHs,17500
 tests/test_stat_tests.py,sha256=PMlJVP8lw8llm_BCawk0EewdUGUy_Wq769WMaMgAsbo,5054
 tests/test_synthetic.py,sha256=0YeYIjRM4kWCKAeVvtIWNpIxgg2iDrYqEDbQUitZqmE,16673
 tests/test_utils.py,sha256=oCXOmGRvnWWVTVGnO44AYm0N9S8weLQWLPbwo9AYTkM,3009
 tests/utils.py,sha256=dEG0wWDV1twH_epZACm7WMeq5Sp-RNmW92la4BfMqno,611
-scludam-1.0.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-scludam-1.0.4.dist-info/METADATA,sha256=RiCjoMkvsMpKj8YwgQCIvOquT2WDbEiE3UUMLtz4m1s,5384
-scludam-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-scludam-1.0.4.dist-info/top_level.txt,sha256=o1ZchBQ1yRGNlnzajlmexEPcjlq8wyPsyFafvNVKmqw,14
-scludam-1.0.4.dist-info/RECORD,,
+scludam-1.0.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+scludam-1.0.5.dist-info/METADATA,sha256=TR4OAd5mKIqDDM6hNg6w4ezbPRfI8Aft2l-MdlymTBw,5384
+scludam-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+scludam-1.0.5.dist-info/top_level.txt,sha256=o1ZchBQ1yRGNlnzajlmexEPcjlq8wyPsyFafvNVKmqw,14
+scludam-1.0.5.dist-info/RECORD,,
```

