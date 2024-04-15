# Comparing `tmp/zhmiscellany-1.9.1-py3-none-any.whl.zip` & `tmp/zhmiscellany-1.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,20 @@
-Zip file size: 20121 bytes, number of entries: 20
+Zip file size: 19710 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      215 b- defN 23-Nov-12 21:09 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
--rw-rw-rw-  2.0 fat       59 b- defN 23-Dec-03 10:35 zhmiscellany/_py_resources.py
--rw-rw-rw-  2.0 fat        8 b- defN 23-Nov-01 16:36 zhmiscellany/_state.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4435 b- defN 24-Mar-30 18:10 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1595 b- defN 24-Mar-03 05:51 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     1819 b- defN 24-Apr-15 13:29 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18715 b- defN 24-Apr-15 13:30 zhmiscellany-1.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 13:30 zhmiscellany-1.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 13:30 zhmiscellany-1.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1601 b- defN 24-Apr-15 13:30 zhmiscellany-1.9.1.dist-info/RECORD
-20 files, 60687 bytes uncompressed, 17519 bytes compressed:  71.1%
+-rw-rw-rw-  2.0 fat    18715 b- defN 24-Apr-15 13:35 zhmiscellany-1.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 13:35 zhmiscellany-1.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 13:35 zhmiscellany-1.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 13:35 zhmiscellany-1.9.2.dist-info/RECORD
+18 files, 60460 bytes uncompressed, 17362 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -3,20 +3,14 @@
 
 Filename: zhmiscellany/_discord_supportfuncs.py
 Comment: 
 
 Filename: zhmiscellany/_misc_supportfuncs.py
 Comment: 
 
-Filename: zhmiscellany/_py_resources.py
-Comment: 
-
-Filename: zhmiscellany/_state.py
-Comment: 
-
 Filename: zhmiscellany/dict.py
 Comment: 
 
 Filename: zhmiscellany/discord.py
 Comment: 
 
 Filename: zhmiscellany/fileio.py
@@ -42,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-1.9.1.dist-info/METADATA
+Filename: zhmiscellany-1.9.2.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-1.9.1.dist-info/WHEEL
+Filename: zhmiscellany-1.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-1.9.1.dist-info/top_level.txt
+Filename: zhmiscellany-1.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-1.9.1.dist-info/RECORD
+Filename: zhmiscellany-1.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zhmiscellany-1.9.1.dist-info/METADATA` & `zhmiscellany-1.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 1.9.1
+Version: 1.9.2
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zhmiscellany-1.9.1.dist-info/RECORD` & `zhmiscellany-1.9.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 zhmiscellany/__init__.py,sha256=jFvzqbgBwgxQIa40HHWP7wtKfJAiAJ_wqkyURVYnjJs,215
 zhmiscellany/_discord_supportfuncs.py,sha256=OIO40DDGgAPNCifP9VQsHH4p4P_NuLq-RC377k1LTW8,6520
 zhmiscellany/_misc_supportfuncs.py,sha256=H8VZ8vEhH5kC9df488j-MuQmxS8v5Xjc6RHBtE5UrKM,673
-zhmiscellany/_py_resources.py,sha256=e2XxK058kOFEW9bI_UjGn1-ho7jm7djU8X5y-R6ExZ8,59
-zhmiscellany/_state.py,sha256=F-3o0jbloyZrQvSh7e9lX8VuHydDxGwGwLCtKWbkMD0,8
 zhmiscellany/dict.py,sha256=0BZJ5eK-MurAHYV1OPa0jdGTr-QEWos7ZM0npb-tN9I,81
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
 zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=n82JEmQSfU8gX-QTRET3ys6cRuU-DDJjkQFyMMH-5Yg,4435
 zhmiscellany/netio.py,sha256=-nUiO3I5nnTZLezt3IOcs2jWPJ-uiWxJXNZRcTEV8ZA,1595
 zhmiscellany/pipes.py,sha256=EwpUmJPkuoOif8-f-_lZ7OMjAioaBFcwNONZB6hSgi0,1819
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-1.9.1.dist-info/METADATA,sha256=dL09LqcAeIqaaE00OHaFkRBmkOqK0yhLj9WjeMJyaJ4,18715
-zhmiscellany-1.9.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-1.9.1.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-1.9.1.dist-info/RECORD,,
+zhmiscellany-1.9.2.dist-info/METADATA,sha256=b64uluaPhEg4RDH7C60Fod6rEciv_yn-Lj4s4nEsI40,18715
+zhmiscellany-1.9.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-1.9.2.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-1.9.2.dist-info/RECORD,,
```

