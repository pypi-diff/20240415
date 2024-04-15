# Comparing `tmp/zhmiscellany-1.9.7-py3-none-any.whl.zip` & `tmp/zhmiscellany-1.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 19785 bytes, number of entries: 18
+Zip file size: 19841 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4435 b- defN 24-Mar-30 18:10 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1595 b- defN 24-Mar-03 05:51 zhmiscellany/netio.py
--rw-rw-rw-  2.0 fat     2221 b- defN 24-Apr-15 14:09 zhmiscellany/pipes.py
+-rw-rw-rw-  2.0 fat     2221 b- defN 24-Apr-15 14:14 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18715 b- defN 24-Apr-15 14:09 zhmiscellany-1.9.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 14:09 zhmiscellany-1.9.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 14:09 zhmiscellany-1.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 14:09 zhmiscellany-1.9.7.dist-info/RECORD
-18 files, 60883 bytes uncompressed, 17437 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 14:14 zhmiscellany-1.9.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 14:14 zhmiscellany-1.9.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 14:14 zhmiscellany-1.9.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 14:14 zhmiscellany-1.9.8.dist-info/RECORD
+18 files, 61061 bytes uncompressed, 17493 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-1.9.7.dist-info/METADATA
+Filename: zhmiscellany-1.9.8.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-1.9.7.dist-info/WHEEL
+Filename: zhmiscellany-1.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-1.9.7.dist-info/top_level.txt
+Filename: zhmiscellany-1.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-1.9.7.dist-info/RECORD
+Filename: zhmiscellany-1.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhmiscellany/pipes.py

```diff
@@ -14,15 +14,15 @@
         self.send_thread.start()
 
     def send_data_thread(self):
         pipe_handle = win32pipe.CreateNamedPipe(
             self.pipe_name,
             win32pipe.PIPE_ACCESS_OUTBOUND,
             win32pipe.PIPE_TYPE_MESSAGE | win32pipe.PIPE_READMODE_MESSAGE | win32pipe.PIPE_WAIT,
-            2,  # Max instances
+            1,  # Max instances
             65536,  # Out buffer size
             65536,  # In buffer size
             0,  # Timeout
             None  # Security attributes
         )
         win32pipe.ConnectNamedPipe(pipe_handle, None)
```

## Comparing `zhmiscellany-1.9.7.dist-info/METADATA` & `zhmiscellany-1.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 1.9.7
+Version: 1.9.8
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,16 @@
 [zhmiscellany.string](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanystring) Functions for interacting with/generating strings that I find useful.\
 [zhmiscellany.math](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanymath) Functions for making some calculations easier.\
 [zhmiscellany.netio](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanynetio) Internet related functions that didn't make sense in any other module.\
 [zhmiscellany.image](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanyimage) Functions for quantifying and manipulating images.\
 [zhmiscellany.list](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanylist) Functions for manipulating lists.\
 [zhmiscellany.dict](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanydict) Functions for working with dicts.\
 [zhmiscellany.processing](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanyprocessing) Functions for processing data in threads in a more straight forward way.\
-[zhmiscellany.misc](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanymisc) Miscellaneous functions that didn't fit anywhere else.
+[zhmiscellany.misc](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanymisc) Miscellaneous functions that didn't fit anywhere else.\
+[zhmiscellany.pipes](https://github.com/zen-ham/zhmiscellany/tree/master#zhmiscellanypipes) A pair of classes for effectively using pipes for IPC (Inter-Process Communication)
 
 
 Usage examples
 ===
 A script that caches and prints out the user IDs of all the members in a server.
 ```py
 import zhmiscellany
```

## Comparing `zhmiscellany-1.9.7.dist-info/RECORD` & `zhmiscellany-1.9.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
 zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=n82JEmQSfU8gX-QTRET3ys6cRuU-DDJjkQFyMMH-5Yg,4435
 zhmiscellany/netio.py,sha256=-nUiO3I5nnTZLezt3IOcs2jWPJ-uiWxJXNZRcTEV8ZA,1595
-zhmiscellany/pipes.py,sha256=ZqIRNwly7vxurf9RwHKCSTkhFVnXy6spAu52rgSJ7us,2221
+zhmiscellany/pipes.py,sha256=nJHkbm4Lst7tJH83XYBFJKfZI0JH5zhUEvvR6VEYLRc,2221
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-1.9.7.dist-info/METADATA,sha256=yQjnVy573Nht06D1kIPiNr-9MQMSdKLpmRR-yUigoFU,18715
-zhmiscellany-1.9.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-1.9.7.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-1.9.7.dist-info/RECORD,,
+zhmiscellany-1.9.8.dist-info/METADATA,sha256=5q8cTIJ3K5e04WxKO-srjgx09liKujNEhsTtewnmf28,18893
+zhmiscellany-1.9.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-1.9.8.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-1.9.8.dist-info/RECORD,,
```

