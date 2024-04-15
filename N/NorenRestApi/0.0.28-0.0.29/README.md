# Comparing `tmp/NorenRestApi-0.0.28-py2.py3-none-any.whl.zip` & `tmp/NorenRestApi-0.0.29-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 22292 bytes, number of entries: 7
--rw-rw-r--  2.0 unx    34055 b- defN 24-Apr-08 05:16 NorenRestApiPy/NorenApi.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 05:14 NorenRestApiPy/__init__.py
--rw-rw-r--  2.0 unx      187 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/LICENSE
--rw-rw-r--  2.0 unx    70334 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      581 b- defN 24-Apr-08 06:34 NorenRestApi-0.0.28.dist-info/RECORD
-7 files, 105282 bytes uncompressed, 21256 bytes compressed:  79.8%
+Zip file size: 22293 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx    34055 b- defN 24-Apr-15 10:55 NorenRestApiPy/NorenApi.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-15 10:55 NorenRestApiPy/__init__.py
+-rw-rw-r--  2.0 unx      187 b- defN 24-Apr-15 11:01 NorenRestApi-0.0.29.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    70336 b- defN 24-Apr-15 11:01 NorenRestApi-0.0.29.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-15 11:01 NorenRestApi-0.0.29.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-15 11:01 NorenRestApi-0.0.29.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-15 11:01 NorenRestApi-0.0.29.dist-info/RECORD
+7 files, 105284 bytes uncompressed, 21257 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: NorenRestApiPy/NorenApi.py
 Comment: 
 
 Filename: NorenRestApiPy/__init__.py
 Comment: 
 
-Filename: NorenRestApi-0.0.28.dist-info/LICENSE
+Filename: NorenRestApi-0.0.29.dist-info/LICENSE
 Comment: 
 
-Filename: NorenRestApi-0.0.28.dist-info/METADATA
+Filename: NorenRestApi-0.0.29.dist-info/METADATA
 Comment: 
 
-Filename: NorenRestApi-0.0.28.dist-info/WHEEL
+Filename: NorenRestApi-0.0.29.dist-info/WHEEL
 Comment: 
 
-Filename: NorenRestApi-0.0.28.dist-info/top_level.txt
+Filename: NorenRestApi-0.0.29.dist-info/top_level.txt
 Comment: 
 
-Filename: NorenRestApi-0.0.28.dist-info/RECORD
+Filename: NorenRestApi-0.0.29.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `NorenRestApi-0.0.28.dist-info/METADATA` & `NorenRestApi-0.0.29.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: NorenRestApi
-Version: 0.0.28
+Version: 0.0.29
 Summary: A package for NorenOMS
 Home-page: UNKNOWN
 Author: KumarAnand
 Author-email: kumar.anand@kambala.co.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyYAML ==6.0
+Requires-Dist: PyYAML ==6.0.1
 Requires-Dist: pandas ==1.5.3
 Requires-Dist: requests ==2.28.2
 Requires-Dist: websocket-client ==1.5.1
 
 # NorenApi
 
 Api used to connect to NorenOMS
```

## Comparing `NorenRestApi-0.0.28.dist-info/RECORD` & `NorenRestApi-0.0.29.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 NorenRestApiPy/NorenApi.py,sha256=fJ3EM-Iwy9inYusfTDxiPn_gAdD9g7_TxTGJ0MbsMjs,34055
 NorenRestApiPy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-NorenRestApi-0.0.28.dist-info/LICENSE,sha256=mqXdxwEe__d9rE8OthmQzKK9sCAPBfJvi_5VUdiazls,187
-NorenRestApi-0.0.28.dist-info/METADATA,sha256=52lcfbgdk3Y5ate1z5Ja-iU0rkTKp24QP4Ut_29_nOI,70334
-NorenRestApi-0.0.28.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-NorenRestApi-0.0.28.dist-info/top_level.txt,sha256=T_X85fuNUvAPVEDBEZofFPOpbANpopXmBDcaFW8Q2W0,15
-NorenRestApi-0.0.28.dist-info/RECORD,,
+NorenRestApi-0.0.29.dist-info/LICENSE,sha256=mqXdxwEe__d9rE8OthmQzKK9sCAPBfJvi_5VUdiazls,187
+NorenRestApi-0.0.29.dist-info/METADATA,sha256=cg7Su3zeOujBhLBepRiHNFyk49_wt7DUDnggWYCquxY,70336
+NorenRestApi-0.0.29.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+NorenRestApi-0.0.29.dist-info/top_level.txt,sha256=T_X85fuNUvAPVEDBEZofFPOpbANpopXmBDcaFW8Q2W0,15
+NorenRestApi-0.0.29.dist-info/RECORD,,
```

