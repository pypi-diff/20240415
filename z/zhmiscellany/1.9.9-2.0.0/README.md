# Comparing `tmp/zhmiscellany-1.9.9-py3-none-any.whl.zip` & `tmp/zhmiscellany-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 19847 bytes, number of entries: 18
+Zip file size: 19864 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4440 b- defN 24-Apr-15 15:01 zhmiscellany/misc.py
--rw-rw-rw-  2.0 fat     1595 b- defN 24-Mar-03 05:51 zhmiscellany/netio.py
+-rw-rw-rw-  2.0 fat     1685 b- defN 24-Apr-15 15:15 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     2221 b- defN 24-Apr-15 14:14 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 15:02 zhmiscellany-1.9.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 15:02 zhmiscellany-1.9.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 15:02 zhmiscellany-1.9.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 15:02 zhmiscellany-1.9.9.dist-info/RECORD
-18 files, 61066 bytes uncompressed, 17499 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/RECORD
+18 files, 61156 bytes uncompressed, 17516 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-1.9.9.dist-info/METADATA
+Filename: zhmiscellany-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-1.9.9.dist-info/WHEEL
+Filename: zhmiscellany-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-1.9.9.dist-info/top_level.txt
+Filename: zhmiscellany-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-1.9.9.dist-info/RECORD
+Filename: zhmiscellany-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhmiscellany/netio.py

```diff
@@ -9,16 +9,20 @@
     file_name = file_name.split('?')[0]
     destination_path = f"{destination_folder}/{file_name}"
     if len(destination_path) > 250:
         destination_path = f'{destination_path[:(250 - len(os.path.splitext(destination_path)[1]))]}{os.path.splitext(destination_path)[1]}'
     return destination_path
 
 
-def download_file(url, destination_folder=".", just_return_path=False, headers=None):
-    destination_path = resolve_file(url, destination_folder)
+def download_file(url, destination_folder=".", just_return_path=False, headers=None, file_path=None):
+    if file_path:
+        destination_path = file_path
+    else:
+        destination_path = resolve_file(url, destination_folder)
+
     if os.path.exists(destination_path):
         if just_return_path:
             return destination_path
         return False
     if headers:
         response = requests.get(url, stream=True, headers=headers)
     else:
```

## Comparing `zhmiscellany-1.9.9.dist-info/METADATA` & `zhmiscellany-2.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 1.9.9
+Version: 2.0.0
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zhmiscellany-1.9.9.dist-info/RECORD` & `zhmiscellany-2.0.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 zhmiscellany/dict.py,sha256=0BZJ5eK-MurAHYV1OPa0jdGTr-QEWos7ZM0npb-tN9I,81
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
 zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=pDlnSdBBdaJNhIDMIowSNHbxHMo8agO7XdJ52Wt_VfY,4440
-zhmiscellany/netio.py,sha256=-nUiO3I5nnTZLezt3IOcs2jWPJ-uiWxJXNZRcTEV8ZA,1595
+zhmiscellany/netio.py,sha256=4dKBJp-fq_jnuDcwrag6kH7WZncnERPPtuCmGcdFAt0,1685
 zhmiscellany/pipes.py,sha256=nJHkbm4Lst7tJH83XYBFJKfZI0JH5zhUEvvR6VEYLRc,2221
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-1.9.9.dist-info/METADATA,sha256=7pfKnZavzSf87RHqK3dQb-NC4pGIiWoCDn2r9GmCGGg,18893
-zhmiscellany-1.9.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-1.9.9.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-1.9.9.dist-info/RECORD,,
+zhmiscellany-2.0.0.dist-info/METADATA,sha256=21FHOFDp1tFWr3N1rmx8PljA7uOVZivOKq1miHxbneA,18893
+zhmiscellany-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-2.0.0.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-2.0.0.dist-info/RECORD,,
```

