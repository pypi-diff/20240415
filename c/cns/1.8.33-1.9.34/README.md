# Comparing `tmp/cns-1.8.33-py3-none-any.whl.zip` & `tmp/cns-1.9.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 911572 bytes, number of entries: 26
+Zip file size: 951987 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat   151040 b- defN 23-Sep-24 05:36 cns/DataX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat   189440 b- defN 23-Sep-24 05:36 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   189952 b- defN 23-Sep-24 05:36 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   117248 b- defN 23-Oct-10 13:48 cns/ExcelX.cp36-win32.pyd
@@ -11,18 +11,19 @@
 -rw-rw-rw-  2.0 fat    88064 b- defN 23-Jun-30 02:07 cns/OTPX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-30 02:07 cns/OTPX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     8432 b- defN 24-Mar-25 09:35 cns/ProX.py
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    80896 b- defN 24-Mar-25 09:33 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      588 b- defN 24-Feb-19 06:05 cns/__init__.py
+-rw-rw-rw-  2.0 fat      644 b- defN 24-Apr-15 03:35 cns/__init__.py
 -rw-rw-rw-  2.0 fat    68608 b- defN 23-Aug-11 08:45 cns/cmdX.cp36-win32.pyd
--rw-rw-rw-  2.0 fat   108032 b- defN 24-Apr-13 08:33 cns/cmdX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   108032 b- defN 24-Apr-13 08:42 cns/cmdX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    89088 b- defN 23-Aug-11 08:45 cns/cmdX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    99328 b- defN 24-Feb-20 06:38 cns/sqlX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-13 08:36 cns-1.8.33.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2023 b- defN 24-Apr-13 08:36 cns-1.8.33.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-13 08:36 cns-1.8.33.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-13 08:36 cns-1.8.33.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2146 b- defN 24-Apr-13 08:36 cns-1.8.33.dist-info/RECORD
-26 files, 2063299 bytes uncompressed, 908176 bytes compressed:  56.0%
+-rw-rw-rw-  2.0 fat    93696 b- defN 24-Apr-15 03:34 cns/strX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-15 03:37 cns-1.9.34.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2023 b- defN 24-Apr-15 03:37 cns-1.9.34.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-15 03:37 cns-1.9.34.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-15 03:37 cns-1.9.34.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2231 b- defN 24-Apr-15 03:37 cns-1.9.34.dist-info/RECORD
+27 files, 2157136 bytes uncompressed, 948461 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -57,23 +57,26 @@
 
 Filename: cns/cmdX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/sqlX.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.8.33.dist-info/LICENSE
+Filename: cns/strX.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.8.33.dist-info/METADATA
+Filename: cns-1.9.34.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.8.33.dist-info/WHEEL
+Filename: cns-1.9.34.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.8.33.dist-info/top_level.txt
+Filename: cns-1.9.34.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.8.33.dist-info/RECORD
+Filename: cns-1.9.34.dist-info/top_level.txt
+Comment: 
+
+Filename: cns-1.9.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -5,8 +5,9 @@
 from .DataX import DataX             # 数据处理
 from .TextX import TextX             # 文本处理
 from .SQLstrX import SQLstrX         # RPASQL处理
 from .cmdX import cmdX               # 路径处理(修改文件名等)
 from .OTPX import OTPX               # 动态口令
 from .ExcelX import ExcelX           # EXCEL文件处理
 from .ProX import ProX               # 综合处理
-from .sqlX import sqlX               # SQL处理 
+from .sqlX import sqlX               # SQL处理
+from .strX import strX               # 字符串处理
```

## Comparing `cns-1.8.33.dist-info/METADATA` & `cns-1.9.34.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.8.33
+Version: 1.9.34
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: Rambo
 Author-email: 6566666@qq.com
 License: Copyright (C) 2023 CNS. All Rights Reserved. See LICENSE for license.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.8.33.dist-info/RECORD` & `cns-1.9.34.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 cns/OTPX.cp36-win_amd64.pyd,sha256=cmWUVENEYKVmv6gFHPuuDQ85qARuXDYE8QJa5-qob7M,88064
 cns/OTPX.cp39-win_amd64.pyd,sha256=gifLhBrujnmf-O0ha6QK3lW9bK3SQFZheF8KJqFmFUg,74240
 cns/ProX.py,sha256=AEjXB3X_BUkR9HmpGt3bN3M1Wj-bCifQ8NXli_hCYyA,8432
 cns/SQLstrX.cp36-win_amd64.pyd,sha256=3NLRKJa7q2Dl1sKlzVBbScgYjcgoSgMOClS2BuxDIzI,84992
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
 cns/TextX.cp36-win_amd64.pyd,sha256=PYVrQEs7reVMhs5Incl0q9IYBZDEmOdKA7EDMdKY_Q4,80896
 cns/TextX.cp39-win_amd64.pyd,sha256=tJkutc00Vya2KBtXFWGcCm0wOSt9vvAm_7cZBsB1DgE,65536
-cns/__init__.py,sha256=oJDDFesRF4kSTrangTS_GBH3IOLSM5LbrdxeqM5Tys4,588
+cns/__init__.py,sha256=kVNsQd-UYVdEDtBJzWboWdaq7RD3viepzmx7w8e3b48,644
 cns/cmdX.cp36-win32.pyd,sha256=f4TcE849qF5PUxcmAf3uGHJwNPk0SNk9xilxDv9j7ek,68608
-cns/cmdX.cp36-win_amd64.pyd,sha256=n0IMWpTtGQ26twvX8XicHJOwwJEs_tkIXuE4yjqoc0s,108032
+cns/cmdX.cp36-win_amd64.pyd,sha256=12GapWmmQ-4PijruUOpF-SEwv5jYJOfeF0rZqrJGftg,108032
 cns/cmdX.cp39-win_amd64.pyd,sha256=8o8LoRMpTyJhvxc3bFAGJcJGW7hnKLHW5Ni-ooOvqYQ,89088
 cns/sqlX.cp36-win_amd64.pyd,sha256=OSKg48KYrNQEGtYrsT0rccLtbXH0Udd2BYYiVCZ2wzQ,99328
-cns-1.8.33.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.8.33.dist-info/METADATA,sha256=GCpE8-6SRBF6d2A4fZSoogMCPNHyrSHqI2_7dRRMuLg,2023
-cns-1.8.33.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.8.33.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.8.33.dist-info/RECORD,,
+cns/strX.cp36-win_amd64.pyd,sha256=j3KfXIyCqEix3OGjtwl6KVT6mY-OzddoMOwTRutOuRU,93696
+cns-1.9.34.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.9.34.dist-info/METADATA,sha256=omYtadMoUHP7YJR0YFuQjKJfB1DQxnkJcREpqwmvZF4,2023
+cns-1.9.34.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.9.34.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.9.34.dist-info/RECORD,,
```

