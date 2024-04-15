# Comparing `tmp/zhmiscellany-2.0.0-py3-none-any.whl.zip` & `tmp/zhmiscellany-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 19864 bytes, number of entries: 18
+Zip file size: 19916 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
--rw-rw-rw-  2.0 fat     4440 b- defN 24-Apr-15 15:01 zhmiscellany/misc.py
+-rw-rw-rw-  2.0 fat     4531 b- defN 24-Apr-15 16:39 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1685 b- defN 24-Apr-15 15:15 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     2221 b- defN 24-Apr-15 14:14 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 15:16 zhmiscellany-2.0.0.dist-info/RECORD
-18 files, 61156 bytes uncompressed, 17516 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 16:40 zhmiscellany-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 16:40 zhmiscellany-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 16:40 zhmiscellany-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 16:40 zhmiscellany-2.0.1.dist-info/RECORD
+18 files, 61247 bytes uncompressed, 17568 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-2.0.0.dist-info/METADATA
+Filename: zhmiscellany-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-2.0.0.dist-info/WHEEL
+Filename: zhmiscellany-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-2.0.0.dist-info/top_level.txt
+Filename: zhmiscellany-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-2.0.0.dist-info/RECORD
+Filename: zhmiscellany-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhmiscellany/misc.py

```diff
@@ -1,12 +1,12 @@
 import os, signal, time, importlib
 from ._misc_supportfuncs import set_activity_timeout, activity
 import zhmiscellany.math
 import zhmiscellany.string
-import win32api, win32con, time
+import win32api, win32con, time, hashlib
 
 
 def die():
     os.kill(os.getpid(), signal.SIGTERM)
 
 
 def show_progress(things, total_things, extra_data='', smart_ratelimit=False, max_prints=1000):
@@ -116,16 +116,16 @@
 
 
 def get_mouse_xy():
     x, y = win32api.GetCursorPos()
     return x, y
 
 
-def base62_hash(__obj):
-    return zhmiscellany.string.convert_to_base62(abs(hash(__obj)))
+def base62_hash(data):
+    return zhmiscellany.string.convert_to_base62(int(int(hashlib.md5(data if isinstance(data, bytes) else str(data).encode()).hexdigest(), 16)**0.5))
 
 
 def high_precision_sleep(duration):
     start_time = time.perf_counter()
     while True:
         elapsed_time = time.perf_counter() - start_time
         remaining_time = duration - elapsed_time
```

## Comparing `zhmiscellany-2.0.0.dist-info/METADATA` & `zhmiscellany-2.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 2.0.0
+Version: 2.0.1
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zhmiscellany-2.0.0.dist-info/RECORD` & `zhmiscellany-2.0.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 zhmiscellany/_misc_supportfuncs.py,sha256=H8VZ8vEhH5kC9df488j-MuQmxS8v5Xjc6RHBtE5UrKM,673
 zhmiscellany/dict.py,sha256=0BZJ5eK-MurAHYV1OPa0jdGTr-QEWos7ZM0npb-tN9I,81
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
 zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
-zhmiscellany/misc.py,sha256=pDlnSdBBdaJNhIDMIowSNHbxHMo8agO7XdJ52Wt_VfY,4440
+zhmiscellany/misc.py,sha256=JlibUEtNHc3nHDnlgyOE3050SIQkcMMedPK8WZookNU,4531
 zhmiscellany/netio.py,sha256=4dKBJp-fq_jnuDcwrag6kH7WZncnERPPtuCmGcdFAt0,1685
 zhmiscellany/pipes.py,sha256=nJHkbm4Lst7tJH83XYBFJKfZI0JH5zhUEvvR6VEYLRc,2221
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-2.0.0.dist-info/METADATA,sha256=21FHOFDp1tFWr3N1rmx8PljA7uOVZivOKq1miHxbneA,18893
-zhmiscellany-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-2.0.0.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-2.0.0.dist-info/RECORD,,
+zhmiscellany-2.0.1.dist-info/METADATA,sha256=FKhKHLmnTVBAy6-f1-5GqnfcYJV0AnW6_FPmBlVt_oY,18893
+zhmiscellany-2.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-2.0.1.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-2.0.1.dist-info/RECORD,,
```

