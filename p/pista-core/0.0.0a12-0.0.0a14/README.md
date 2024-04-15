# Comparing `tmp/pista_core-0.0.0a12-py3-none-any.whl.zip` & `tmp/pista_core-0.0.0a14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 116689 bytes, number of entries: 74
+Zip file size: 116451 bytes, number of entries: 73
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-15 07:38 pista/__init__.py
 -rw-rw-rw-  2.0 fat    13574 b- defN 24-Apr-15 07:38 pista/conftest.py
 -rw-rw-rw-  2.0 fat     1387 b- defN 24-Apr-15 07:38 pista/pista_config.ini
 -rw-rw-rw-  2.0 fat      881 b- defN 24-Apr-15 07:38 pista/pytest.ini
 -rw-rw-rw-  2.0 fat      714 b- defN 24-Apr-15 07:38 pista/requirements.txt
 -rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-15 07:38 pista/root.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-15 07:38 pista/core/__init__.py
@@ -64,13 +64,12 @@
 -rw-rw-rw-  2.0 fat      745 b- defN 24-Apr-15 07:38 pista/tests/test_Pista_API_ExcelData.py
 -rw-rw-rw-  2.0 fat      874 b- defN 24-Apr-15 07:38 pista/tests/test_Pista_SSH_Xterm.py
 -rw-rw-rw-  2.0 fat      365 b- defN 24-Apr-15 07:38 pista/tests/test_Pista_UI_WebBrowser.py
 -rw-rw-rw-  2.0 fat      650 b- defN 24-Apr-15 07:38 pista/tests/test_Pista_VariableDataFile.py
 -rw-rw-rw-  2.0 fat      699 b- defN 24-Apr-15 07:38 pista/tests/output/log_1308.log
 -rw-rw-rw-  2.0 fat     4444 b- defN 24-Apr-15 07:38 pista/tests/output/log_xterm.log
 -rw-rw-rw-  2.0 fat    50822 b- defN 24-Apr-15 07:38 pista/tests/output/report.html
--rw-rw-rw-  2.0 fat       86 b- defN 24-Apr-15 09:29 pista_core-0.0.0a12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 09:29 pista_core-0.0.0a12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 24-Apr-15 09:29 pista_core-0.0.0a12.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 09:29 pista_core-0.0.0a12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6764 b- defN 24-Apr-15 09:29 pista_core-0.0.0a12.dist-info/RECORD
-74 files, 344027 bytes uncompressed, 105761 bytes compressed:  69.3%
+-rw-rw-rw-  2.0 fat       86 b- defN 24-Apr-15 09:49 pista_core-0.0.0a14.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 09:49 pista_core-0.0.0a14.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 09:49 pista_core-0.0.0a14.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6663 b- defN 24-Apr-15 09:49 pista_core-0.0.0a14.dist-info/RECORD
+73 files, 343902 bytes uncompressed, 105691 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -201,23 +201,20 @@
 
 Filename: pista/tests/output/log_xterm.log
 Comment: 
 
 Filename: pista/tests/output/report.html
 Comment: 
 
-Filename: pista_core-0.0.0a12.dist-info/METADATA
+Filename: pista_core-0.0.0a14.dist-info/METADATA
 Comment: 
 
-Filename: pista_core-0.0.0a12.dist-info/WHEEL
+Filename: pista_core-0.0.0a14.dist-info/WHEEL
 Comment: 
 
-Filename: pista_core-0.0.0a12.dist-info/entry_points.txt
+Filename: pista_core-0.0.0a14.dist-info/top_level.txt
 Comment: 
 
-Filename: pista_core-0.0.0a12.dist-info/top_level.txt
-Comment: 
-
-Filename: pista_core-0.0.0a12.dist-info/RECORD
+Filename: pista_core-0.0.0a14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pista_core-0.0.0a12.dist-info/RECORD` & `pista_core-0.0.0a14.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -63,12 +63,11 @@
 pista/tests/test_Pista_API_ExcelData.py,sha256=St2vwM4nqjhuwu_92fTY21ZgDvLT4A658XUG2TTtn5s,745
 pista/tests/test_Pista_SSH_Xterm.py,sha256=Y_e-AQCZ3HAXDtBAkEst0WTGmLog6b9QT85rVCH3unE,874
 pista/tests/test_Pista_UI_WebBrowser.py,sha256=ddMDb5VkcwVeZKodOz5f_fu9tVTexZVAJwBuYKWffBk,365
 pista/tests/test_Pista_VariableDataFile.py,sha256=ARGsaP_fpnZdAAhh8k0dxexRmMWqx5H1ZRFmQWYb00Q,650
 pista/tests/output/log_1308.log,sha256=9X8DVDojJgvf95rHAHgP0W-NykBqKuLxROjDGF6OerQ,699
 pista/tests/output/log_xterm.log,sha256=pwteOzOPbZem6bMJsiYwZxCVV442jBYGC6sbT-c0cJc,4444
 pista/tests/output/report.html,sha256=0v9Gy3TP7NwKX7CCoOJTwGRW24yADmBI1TM9SYCDI0s,50822
-pista_core-0.0.0a12.dist-info/METADATA,sha256=eCl2DGB9zzQnFiqNUa0KfbtOyOzhCYVeYtJm7wH-bbc,86
-pista_core-0.0.0a12.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pista_core-0.0.0a12.dist-info/entry_points.txt,sha256=PWtXvBMkhfVjhm1eTYuP1aQChFweJmXczhrL3m3ENl0,24
-pista_core-0.0.0a12.dist-info/top_level.txt,sha256=qyaQLDNzBGzsUjPV9CNJyXu_E5jknTVuICWuyYIPlOw,6
-pista_core-0.0.0a12.dist-info/RECORD,,
+pista_core-0.0.0a14.dist-info/METADATA,sha256=_qmYEcOtEU4RC3cGRiqJblbKlTHo0gnu6jlQ_TqnoX4,86
+pista_core-0.0.0a14.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pista_core-0.0.0a14.dist-info/top_level.txt,sha256=qyaQLDNzBGzsUjPV9CNJyXu_E5jknTVuICWuyYIPlOw,6
+pista_core-0.0.0a14.dist-info/RECORD,,
```

