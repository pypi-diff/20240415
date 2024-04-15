# Comparing `tmp/exciton-2.5.0-py3-none-any.whl.zip` & `tmp/exciton-2.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -33,13 +33,13 @@
 -rw-rw-r--  2.0 unx       84 b- defN 24-Apr-13 02:01 exciton/nlp/text_matching/__init__.py
 -rw-rw-r--  2.0 unx     2565 b- defN 24-Apr-13 02:01 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       64 b- defN 24-Apr-13 02:01 exciton/nlp/topic_relevance/__init__.py
 -rw-rw-r--  2.0 unx     3672 b- defN 24-Apr-13 02:01 exciton/nlp/topic_relevance/exciton_relevance.py
 -rw-rw-r--  2.0 unx       50 b- defN 24-Apr-13 02:01 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-13 02:01 exciton/nlp/translation/m2m100/__init__.py
 -rw-rw-r--  2.0 unx     4718 b- defN 24-Apr-13 02:01 exciton/nlp/translation/m2m100/service.py
--rw-rw-r--  2.0 unx    11417 b- defN 24-Apr-15 14:58 exciton-2.5.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1726 b- defN 24-Apr-15 14:58 exciton-2.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-15 14:58 exciton-2.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-15 14:58 exciton-2.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3915 b- defN 24-Apr-15 14:58 exciton-2.5.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx    11417 b- defN 24-Apr-15 15:04 exciton-2.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1726 b- defN 24-Apr-15 15:04 exciton-2.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-15 15:04 exciton-2.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-15 15:04 exciton-2.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3915 b- defN 24-Apr-15 15:04 exciton-2.5.1.dist-info/RECORD
 43 files, 93371 bytes uncompressed, 29994 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -108,23 +108,23 @@
 
 Filename: exciton/nlp/translation/m2m100/__init__.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
-Filename: exciton-2.5.0.dist-info/LICENSE
+Filename: exciton-2.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-2.5.0.dist-info/METADATA
+Filename: exciton-2.5.1.dist-info/METADATA
 Comment: 
 
-Filename: exciton-2.5.0.dist-info/WHEEL
+Filename: exciton-2.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-2.5.0.dist-info/top_level.txt
+Filename: exciton-2.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-2.5.0.dist-info/RECORD
+Filename: exciton-2.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `exciton-2.5.0.dist-info/LICENSE` & `exciton-2.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-2.5.0.dist-info/METADATA` & `exciton-2.5.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 2.5.0
+Version: 2.5.1
 Summary: Natural Language Processing by the Exciton Research
 Home-page: https://excitonresearch.com
 Author: The Exciton Research Team
 Author-email: excitonresearch@gmail.com
 License: UNKNOWN
 Keywords: NLP Deep Learning
 Platform: UNKNOWN
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: accelerate (==0.26.0)
+Requires-Dist: accelerate (==0.29.2)
 Requires-Dist: auto-gptq (==0.7.1)
 Requires-Dist: ctranslate2 (==3.11.0)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: optimum (==1.16.0)
 Requires-Dist: pysbd (==0.3.4)
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: sentence-splitter (==1.4)
```

## Comparing `exciton-2.5.0.dist-info/RECORD` & `exciton-2.5.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 exciton/nlp/text_matching/__init__.py,sha256=tgQvyWZupI0QAHlnLAJldpOPBCF01OFq2poLH49tAVg,84
 exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
 exciton/nlp/topic_relevance/__init__.py,sha256=KKE5y3rytEYStxLQ_VVm2zkxnPQ0FuhnXbNGpbdPZpw,64
 exciton/nlp/topic_relevance/exciton_relevance.py,sha256=-T_gTTU1TA58y8AELbwW3Mw-A1RdQJ159sV_UalD8YY,3672
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/translation/m2m100/service.py,sha256=FIXc5sUtZzywzis_CZ2doF6sqrPcKcyMO8EhLgFTwjY,4718
-exciton-2.5.0.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-2.5.0.dist-info/METADATA,sha256=HDLzrZlUq74B4Syy3DVE3fO6oeRLO_JY24vjV7O1h3A,1726
-exciton-2.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-2.5.0.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-2.5.0.dist-info/RECORD,,
+exciton-2.5.1.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-2.5.1.dist-info/METADATA,sha256=uJ75CW0DjiKHwFZQAylEFucfmSmnXo794MT0WhQArNU,1726
+exciton-2.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-2.5.1.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-2.5.1.dist-info/RECORD,,
```

