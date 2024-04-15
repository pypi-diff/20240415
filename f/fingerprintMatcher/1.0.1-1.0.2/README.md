# Comparing `tmp/fingerprintMatcher-1.0.1-py3-none-any.whl.zip` & `tmp/fingerprintMatcher-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3099 bytes, number of entries: 5
+Zip file size: 3103 bytes, number of entries: 5
 -rw-rw-rw-  2.0 fat     3643 b- defN 24-Apr-14 10:59 fingerprintmatcher.py
--rw-rw-rw-  2.0 fat     2602 b- defN 24-Apr-14 11:56 fingerprintMatcher-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 11:56 fingerprintMatcher-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-14 11:56 fingerprintMatcher-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      420 b- defN 24-Apr-14 11:56 fingerprintMatcher-1.0.1.dist-info/RECORD
-5 files, 6776 bytes uncompressed, 2311 bytes compressed:  65.9%
+-rw-rw-rw-  2.0 fat     2602 b- defN 24-Apr-14 12:03 fingerprintMatcher-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 12:03 fingerprintMatcher-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-14 12:03 fingerprintMatcher-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      420 b- defN 24-Apr-14 12:03 fingerprintMatcher-1.0.2.dist-info/RECORD
+5 files, 6776 bytes uncompressed, 2315 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: fingerprintmatcher.py
 Comment: 
 
-Filename: fingerprintMatcher-1.0.1.dist-info/METADATA
+Filename: fingerprintMatcher-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: fingerprintMatcher-1.0.1.dist-info/WHEEL
+Filename: fingerprintMatcher-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: fingerprintMatcher-1.0.1.dist-info/top_level.txt
+Filename: fingerprintMatcher-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fingerprintMatcher-1.0.1.dist-info/RECORD
+Filename: fingerprintMatcher-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fingerprintMatcher-1.0.1.dist-info/METADATA` & `fingerprintMatcher-1.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fingerprintMatcher
-Version: 1.0.1
+Version: 1.0.2
 Summary: The FingerprintMatcher Python package provides a comprehensive toolkit for fingerprint matching and recognition tasks. With its intuitive interface and powerful functionality, this package enables users to compare fingerprint images, match them against a database of known fingerprints, and determine their similarity with high accuracy.
 Home-page: https://github.com/Tharunk07/fingerprintMatcher
 Author: Tharun K
 Author-email: tharunkkumarasamy@gmail.com
 Project-URL: Bug Tracker, https://github.com/Tharunk07/fingerprintMatcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,30 +30,30 @@
 
 To match two fingerprint images and check if they are similar, you can use the match_fingerprints method:
 
 ```bash
 from fingerprintmatcher import fingerprintMatcher
 
 # Create an instance of the FingerprintMatcher class
-fingerprint_matcher = FingerprintMatcher()
+fingerprint_matcher = fingerprintMatcher()
 
 # Match two fingerprint images
 fingerprint_matcher.match_fingerprints("path/to/image1", "path/to/image2")
 ```
 Replace "path/to/image1" and "path/to/image2" with the file paths of the fingerprint images you want to compare.
 
 # Matching with a database
 
 To match a fingerprint image with a database of fingerprint images, you can use the match_with_database method:
 
 ```bash
 from fingerprintmatcher import fingerprintMatcher
 
 # Create an instance of the FingerprintMatcher class
-fingerprint_matcher = FingerprintMatcher()
+fingerprint_matcher = fingerprintMatcher()
 
 # Match with a database
 fingerprint_matcher.match_with_database("path/to/test_image", "path/to/database_folder")
 ```
 
 Replace "path/to/test_image" and database path "path/to/database_folder" of the fingerprint images and database you want to compare.
```

