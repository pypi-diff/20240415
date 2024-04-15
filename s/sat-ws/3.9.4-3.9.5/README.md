# Comparing `tmp/sat_ws-3.9.4-py3-none-any.whl.zip` & `tmp/sat_ws-3.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 37400 bytes, number of entries: 58
+Zip file size: 37402 bytes, number of entries: 58
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-28 23:00 mx_edi/__init__.py
 -rw-r--r--  2.0 unx      277 b- defN 21-Sep-28 23:00 mx_edi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-28 23:00 mx_edi/connectors/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/__init__.py
 -rw-r--r--  2.0 unx     2929 b- defN 21-Sep-28 23:09 mx_edi/connectors/sat/certificate_handler.py
 -rw-r--r--  2.0 unx      266 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/enums.py
 -rw-r--r--  2.0 unx     2002 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/envelope_signer.py
 -rw-r--r--  2.0 unx     2145 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/package.py
--rw-r--r--  2.0 unx     4038 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/query.py
+-rw-r--r--  2.0 unx     4038 b- defN 21-Oct-20 21:37 mx_edi/connectors/sat/query.py
 -rw-r--r--  2.0 unx     2885 b- defN 21-Sep-28 23:06 mx_edi/connectors/sat/sat_connector.py
 -rw-r--r--  2.0 unx     4708 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/sat_login_handler.py
 -rw-r--r--  2.0 unx     2413 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/utils.py
 -rw-r--r--  2.0 unx       72 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/package_parsers/__init__.py
 -rw-r--r--  2.0 unx      575 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/package_parsers/cfdi_parser.py
 -rw-r--r--  2.0 unx     2016 b- defN 21-Oct-12 20:57 mx_edi/connectors/sat/package_parsers/metadata2cfdi.py
 -rw-r--r--  2.0 unx      190 b- defN 21-Sep-28 23:00 mx_edi/connectors/sat/package_parsers/utils.py
@@ -48,13 +48,13 @@
 -rw-r--r--  2.0 unx    42947 b- defN 21-Oct-12 21:46 tests/conftest.py
 -rw-r--r--  2.0 unx      863 b- defN 21-Sep-21 22:58 tests/test_certificate_handler.py
 -rw-r--r--  2.0 unx      878 b- defN 21-Sep-28 23:00 tests/test_parse.py
 -rw-r--r--  2.0 unx     2451 b- defN 21-Sep-28 23:00 tests/test_processor.py
 -rw-r--r--  2.0 unx     8846 b- defN 21-Sep-28 23:00 tests/test_sat_connector.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Apr-04 22:06 tests/fake_fiel/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Apr-04 22:06 tests/real_fiel/__init__.py
--rw-r--r--  2.0 unx       14 b- defN 21-Oct-20 21:34 sat_ws-3.9.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2113 b- defN 21-Oct-20 21:34 sat_ws-3.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-20 21:34 sat_ws-3.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Oct-20 21:34 sat_ws-3.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5504 b- defN 21-Oct-20 21:34 sat_ws-3.9.4.dist-info/RECORD
-58 files, 107244 bytes uncompressed, 28330 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx       14 b- defN 21-Oct-20 21:38 sat_ws-3.9.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2113 b- defN 21-Oct-20 21:38 sat_ws-3.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Oct-20 21:38 sat_ws-3.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 21-Oct-20 21:38 sat_ws-3.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5504 b- defN 21-Oct-20 21:38 sat_ws-3.9.5.dist-info/RECORD
+58 files, 107244 bytes uncompressed, 28332 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -153,23 +153,23 @@
 
 Filename: tests/fake_fiel/__init__.py
 Comment: 
 
 Filename: tests/real_fiel/__init__.py
 Comment: 
 
-Filename: sat_ws-3.9.4.dist-info/LICENSE.md
+Filename: sat_ws-3.9.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: sat_ws-3.9.4.dist-info/METADATA
+Filename: sat_ws-3.9.5.dist-info/METADATA
 Comment: 
 
-Filename: sat_ws-3.9.4.dist-info/WHEEL
+Filename: sat_ws-3.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: sat_ws-3.9.4.dist-info/top_level.txt
+Filename: sat_ws-3.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sat_ws-3.9.4.dist-info/RECORD
+Filename: sat_ws-3.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mx_edi/connectors/sat/query.py

```diff
@@ -36,15 +36,15 @@
     cfdi_qty: int
     packages: List[Package]
 
     def __init__(
         self,
         download_type: DownloadType,
         request_type: RequestType,
-        /,
+        *,
         start: datetime = None,
         end: datetime = None,
         identifier: str = None,
     ):
         self.download_type = download_type
         self.request_type = request_type
         # Set start as current time in Mexico timezone
```

## Comparing `sat_ws-3.9.4.dist-info/METADATA` & `sat_ws-3.9.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sat-ws
-Version: 3.9.4
+Version: 3.9.5
 Summary: API to connect with SAT ws
 Home-page: https://gitlab.com/HomebrewSoft/sat_ws_api
 Author: Moisés Navarro
 Author-email: moisalejandro@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `sat_ws-3.9.4.dist-info/RECORD` & `sat_ws-3.9.5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 mx_edi/utils.py,sha256=b8Br_QS1Xq-j1ul9mmmL10h8QB7sRROohAuqQeDShjM,277
 mx_edi/connectors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mx_edi/connectors/sat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mx_edi/connectors/sat/certificate_handler.py,sha256=BMgSGkVcEwJ4JKpK8hEBkBdoBjdAv2F4EqjGYkRRa2M,2929
 mx_edi/connectors/sat/enums.py,sha256=Ycc4haib-lXWhTWhRAd50_pQsX_evVYLc5kuLVuntVI,266
 mx_edi/connectors/sat/envelope_signer.py,sha256=8eCOUMjgCSFus_jAJ-NQ3jfXKKLAjl0P00KvXlZI_xc,2002
 mx_edi/connectors/sat/package.py,sha256=gs0ZyMv6mv152cJXSWaTjRLRja9bk7Fos2MfNfdT6s8,2145
-mx_edi/connectors/sat/query.py,sha256=XQLf1axWS5yYama761jVGaa_oddUf1o048Fnyny7f1Q,4038
+mx_edi/connectors/sat/query.py,sha256=f7QhnQ4Yn-M2ivIAU6UkhP2QIybgUGd8JEt8q9HIhLY,4038
 mx_edi/connectors/sat/sat_connector.py,sha256=gB1VvPCGOXBLYjfCtZ-kAcmPLEn3ckmTrvYlynIkfhU,2885
 mx_edi/connectors/sat/sat_login_handler.py,sha256=VKB_5gF5pUCq6bAU2nRgI2aWJCOQnJu6GhbogB5BZ28,4708
 mx_edi/connectors/sat/utils.py,sha256=u4bS-BBeWOb-c8XvLIUvf-l1Yln19ob_fbQojQG95qA,2413
 mx_edi/connectors/sat/package_parsers/__init__.py,sha256=znALjbAgx6cQeOPNEcUz7gFAH1hiA23x0NJ81LFKE_o,72
 mx_edi/connectors/sat/package_parsers/cfdi_parser.py,sha256=dpzZivYXshgGXgy1jprNJFhn5NC-9L_twG3Eylz7ZEs,575
 mx_edi/connectors/sat/package_parsers/metadata2cfdi.py,sha256=f88knstzUhPwx0CO6C_xwa-9nAyIBmPn7AJfZCWlczM,2016
 mx_edi/connectors/sat/package_parsers/utils.py,sha256=mdUNAkZqZG0Lz5gatmiMQs_cEs6rjYW1pyz25vdnCQU,190
@@ -47,12 +47,12 @@
 tests/conftest.py,sha256=TLNbouTJKPO9FArw-Yx9yvlIxPXJ1siuvWCDJYD8GTA,42947
 tests/test_certificate_handler.py,sha256=fNMySI_Rwd5LRI31i9qYJ1UR-k3TCjjRtibEsL6-YVk,863
 tests/test_parse.py,sha256=Pg9hM1JScswALgMW__SGh_H_Gcid_pscWnWbK1Y8YyE,878
 tests/test_processor.py,sha256=JCvedh0hzXM2HELNnDKADfSSho98w9vZiVQ0AmaImZA,2451
 tests/test_sat_connector.py,sha256=mhbhlcqP_tflACX7_3pGUuM2bLgEpmwkNBKorar89cY,8846
 tests/fake_fiel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/real_fiel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sat_ws-3.9.4.dist-info/LICENSE.md,sha256=xi0IUP_h-GBt0RKvcLPryS6l60WoFjaeqneJGOe62VY,14
-sat_ws-3.9.4.dist-info/METADATA,sha256=GYqJLLXHOedrama0793TZ92UDgz_Kbeh31qf_AILIyE,2113
-sat_ws-3.9.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sat_ws-3.9.4.dist-info/top_level.txt,sha256=18KruflwbuXcTPHwBnia3whjHyS8A8LqpZbRPvXbx9I,13
-sat_ws-3.9.4.dist-info/RECORD,,
+sat_ws-3.9.5.dist-info/LICENSE.md,sha256=xi0IUP_h-GBt0RKvcLPryS6l60WoFjaeqneJGOe62VY,14
+sat_ws-3.9.5.dist-info/METADATA,sha256=e7MZOW-qJGSlsN_UfdKvNgRR4yabWVnjKoe3AqZxONA,2113
+sat_ws-3.9.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sat_ws-3.9.5.dist-info/top_level.txt,sha256=18KruflwbuXcTPHwBnia3whjHyS8A8LqpZbRPvXbx9I,13
+sat_ws-3.9.5.dist-info/RECORD,,
```

