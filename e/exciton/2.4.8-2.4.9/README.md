# Comparing `tmp/exciton-2.4.8-py3-none-any.whl.zip` & `tmp/exciton-2.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 70859 bytes, number of entries: 74
+Zip file size: 70861 bytes, number of entries: 74
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5150 b- defN 24-Jan-10 02:54 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     2437 b- defN 24-Jan-04 04:28 exciton/ml/classification/bert/trainer.py
@@ -64,13 +64,13 @@
 -rw-rw-r--  2.0 unx     2565 b- defN 23-May-08 00:57 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       64 b- defN 24-Jan-04 03:48 exciton/nlp/topic_relevance/__init__.py
 -rw-rw-r--  2.0 unx     3672 b- defN 24-Jan-10 16:31 exciton/nlp/topic_relevance/exciton_relevance.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
 -rw-rw-r--  2.0 unx     4718 b- defN 23-May-08 13:23 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 24-Mar-22 03:41 exciton-2.4.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1726 b- defN 24-Mar-22 03:41 exciton-2.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-22 03:41 exciton-2.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Mar-22 03:41 exciton-2.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6975 b- defN 24-Mar-22 03:41 exciton-2.4.8.dist-info/RECORD
-74 files, 187648 bytes uncompressed, 59483 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    11417 b- defN 24-Mar-22 12:48 exciton-2.4.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1726 b- defN 24-Mar-22 12:48 exciton-2.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Mar-22 12:48 exciton-2.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Mar-22 12:48 exciton-2.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6975 b- defN 24-Mar-22 12:48 exciton-2.4.9.dist-info/RECORD
+74 files, 187648 bytes uncompressed, 59485 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -201,23 +201,23 @@
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-2.4.8.dist-info/LICENSE
+Filename: exciton-2.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-2.4.8.dist-info/METADATA
+Filename: exciton-2.4.9.dist-info/METADATA
 Comment: 
 
-Filename: exciton-2.4.8.dist-info/WHEEL
+Filename: exciton-2.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-2.4.8.dist-info/top_level.txt
+Filename: exciton-2.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-2.4.8.dist-info/RECORD
+Filename: exciton-2.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `exciton-2.4.8.dist-info/LICENSE` & `exciton-2.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-2.4.8.dist-info/METADATA` & `exciton-2.4.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 2.4.8
+Version: 2.4.9
 Summary: Natural Language Processing by the Exciton Research
 Home-page: https://excitonresearch.com
 Author: The Exciton Research Team
 Author-email: excitonresearch@gmail.com
 License: UNKNOWN
 Keywords: NLP Deep Learning
 Platform: UNKNOWN
@@ -24,15 +24,15 @@
 Requires-Dist: pysbd (==0.3.4)
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: sentence-splitter (==1.4)
 Requires-Dist: sentencepiece (==0.1.98)
 Requires-Dist: spacy (==3.5.2)
 Requires-Dist: torch (==2.1.0)
 Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: transformers (==4.39.0)
+Requires-Dist: transformers (==4.34.0)
 
 # Exciton NLP - A tool for natural language processing
 
 Exciton NLP is designed and maintained by the Exciton Research for different NLP tasks, including multilingual classification, NER, translation, etc.
 
 ## Installation
 Use ``pip`` to install exciton. Run:
```

## Comparing `exciton-2.4.8.dist-info/RECORD` & `exciton-2.4.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
 exciton/nlp/topic_relevance/__init__.py,sha256=KKE5y3rytEYStxLQ_VVm2zkxnPQ0FuhnXbNGpbdPZpw,64
 exciton/nlp/topic_relevance/exciton_relevance.py,sha256=-T_gTTU1TA58y8AELbwW3Mw-A1RdQJ159sV_UalD8YY,3672
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/translation/m2m100/service.py,sha256=FIXc5sUtZzywzis_CZ2doF6sqrPcKcyMO8EhLgFTwjY,4718
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-2.4.8.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-2.4.8.dist-info/METADATA,sha256=jtGYbnmu_1Su9agAFJM4JamF0JWeAOPAfu3vS0CzbQM,1726
-exciton-2.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-2.4.8.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-2.4.8.dist-info/RECORD,,
+exciton-2.4.9.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-2.4.9.dist-info/METADATA,sha256=vdWeWswJzvDsr2C0xPfyRHn2TgayDlNGorWlpMm0dLA,1726
+exciton-2.4.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-2.4.9.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-2.4.9.dist-info/RECORD,,
```

