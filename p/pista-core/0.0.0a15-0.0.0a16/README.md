# Comparing `tmp/pista_core-0.0.0a15-py3-none-any.whl.zip` & `tmp/pista_core-0.0.0a16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 116451 bytes, number of entries: 73
+Zip file size: 116518 bytes, number of entries: 73
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 14:32 pista/__init__.py
--rw-rw-rw-  2.0 fat    13574 b- defN 24-Apr-12 06:09 pista/conftest.py
+-rw-rw-rw-  2.0 fat    13577 b- defN 24-Apr-15 11:27 pista/conftest.py
 -rw-rw-rw-  2.0 fat     1387 b- defN 24-Apr-11 14:32 pista/pista_config.ini
 -rw-rw-rw-  2.0 fat      881 b- defN 24-Apr-11 14:32 pista/pytest.ini
--rw-rw-rw-  2.0 fat      714 b- defN 24-Apr-11 14:32 pista/requirements.txt
+-rw-rw-rw-  2.0 fat      853 b- defN 24-Apr-15 17:45 pista/requirements.txt
 -rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-11 14:32 pista/root.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 14:32 pista/core/__init__.py
 -rw-rw-rw-  2.0 fat     2005 b- defN 24-Apr-11 14:32 pista/core/_config_manager.py
 -rw-rw-rw-  2.0 fat      935 b- defN 24-Apr-11 14:32 pista/core/_data_manager.py
 -rw-rw-rw-  2.0 fat     5736 b- defN 24-Apr-11 14:32 pista/core/_log_manager.py
 -rw-rw-rw-  2.0 fat     1490 b- defN 24-Apr-11 14:32 pista/core/_root_manager.py
 -rw-rw-rw-  2.0 fat     5973 b- defN 24-Apr-11 14:32 pista/core/_test_enhancer.py
@@ -64,12 +64,12 @@
 -rw-rw-rw-  2.0 fat      745 b- defN 24-Apr-11 14:32 pista/tests/test_Pista_API_ExcelData.py
 -rw-rw-rw-  2.0 fat      874 b- defN 24-Apr-12 16:32 pista/tests/test_Pista_SSH_Xterm.py
 -rw-rw-rw-  2.0 fat      365 b- defN 24-Apr-11 14:32 pista/tests/test_Pista_UI_WebBrowser.py
 -rw-rw-rw-  2.0 fat      650 b- defN 24-Apr-11 14:32 pista/tests/test_Pista_VariableDataFile.py
 -rw-rw-rw-  2.0 fat      699 b- defN 24-Apr-11 14:32 pista/tests/output/log_1308.log
 -rw-rw-rw-  2.0 fat     4444 b- defN 24-Apr-11 14:32 pista/tests/output/log_xterm.log
 -rw-rw-rw-  2.0 fat    50822 b- defN 24-Apr-11 14:32 pista/tests/output/report.html
--rw-rw-rw-  2.0 fat       86 b- defN 24-Apr-15 11:22 pista_core-0.0.0a15.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 11:22 pista_core-0.0.0a15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 11:21 pista_core-0.0.0a15.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6663 b- defN 24-Apr-15 11:22 pista_core-0.0.0a15.dist-info/RECORD
-73 files, 343902 bytes uncompressed, 105691 bytes compressed:  69.3%
+-rw-rw-rw-  2.0 fat       86 b- defN 24-Apr-15 17:46 pista_core-0.0.0a16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 17:46 pista_core-0.0.0a16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 17:46 pista_core-0.0.0a16.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6663 b- defN 24-Apr-15 17:46 pista_core-0.0.0a16.dist-info/RECORD
+73 files, 344044 bytes uncompressed, 105758 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -201,20 +201,20 @@
 
 Filename: pista/tests/output/log_xterm.log
 Comment: 
 
 Filename: pista/tests/output/report.html
 Comment: 
 
-Filename: pista_core-0.0.0a15.dist-info/METADATA
+Filename: pista_core-0.0.0a16.dist-info/METADATA
 Comment: 
 
-Filename: pista_core-0.0.0a15.dist-info/WHEEL
+Filename: pista_core-0.0.0a16.dist-info/WHEEL
 Comment: 
 
-Filename: pista_core-0.0.0a15.dist-info/top_level.txt
+Filename: pista_core-0.0.0a16.dist-info/top_level.txt
 Comment: 
 
-Filename: pista_core-0.0.0a15.dist-info/RECORD
+Filename: pista_core-0.0.0a16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pista/conftest.py

```diff
@@ -161,16 +161,16 @@
         if 'true' in _IS_USE_THREAD_DATA_FILE:
             shutil.copy(THREAD_DATA_TEMPLATE_FILE, _THREAD_DATA_RUNTIME_FILE)
 
         '''Invoke yarn for xterm'''
         ssh_serv_provider = str(PISTA_CONFIG.get('ssh', 'ssh_service_provider'))
         is_run_yarn_flag = str(PISTA_CONFIG.get('ssh', 'is_run_yarn_for_xtermjs'))
         if 'xterm' in ssh_serv_provider and 'true' in is_run_yarn_flag:
-            from pista.core.rf_xtermjs_service import RFXtermService
-            RFXtermService._start_node()
+            from pista.core.ssh_xtermjs_service import SshXtermService
+            SshXtermService._start_node()
 
 
 @pytest.fixture(scope='session', autouse=True)
 def pista_session_setup(request, worker_id):
     # print('pista: pista_session_setup')
 
     global _ENV, _TRIGGERED_CMD, _TRIGGERED_ARGS, _TC_MARK
```

## pista/requirements.txt

```diff
@@ -1,21 +1,21 @@
 cryptography==42.0.5
 
-### For test framework : Also included in pista_core ###
+### For test framework : Required by pista-core ###
 pytest==7.2.0
 pytest-order==1.0.1
 pytest-dependency==0.5.1
 pytest-xdist==3.1.0
 #pytest-excel==1.6.0
 
 pytest-md-report==0.3.0
 pytest-timeout==2.2.0
 pytest-rerunfailures
 
-### For pytest-reporter-html1==0.8.2 : Also included in pista_core ###
+### For pytest-reporter-html1==0.8.2 : Required by pista-core ###
 Jinja2==3.1.3
 ansi2html==1.8.0
 htmlmin==0.1.12
 docutils==0.19
 pytest_metadata==3.0.0
 
 ### For web ui ###
@@ -33,7 +33,12 @@
 paramiko==3.4.0
 Pillow==10.2.0
 
 ### For json (in api) ###
 jsonpath-ng==1.6.0
 pandas==2.1.3
 numpy==1.26.2
+
+### For core framework : Required by projects ###
+#pista-core=={version}
+#--find-links ./pista/dist
+#--index-url https://test.pypi.org/simple/
```

## Comparing `pista_core-0.0.0a15.dist-info/RECORD` & `pista_core-0.0.0a16.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pista/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pista/conftest.py,sha256=a0QRzkRmPflIPpRTXKKFNY4-uxDBs7suEx5iIwh7rLE,13574
+pista/conftest.py,sha256=XFgNhrrFZzGsGxFRb8kTLooOMMySn_PPcQN8yO02YQU,13577
 pista/pista_config.ini,sha256=LD8OGTTbUlV4dDlgqQkPD9nkILQ6hR81t0sO24JH4iI,1387
 pista/pytest.ini,sha256=3mQ5WIw8S22AyayAhddYYqgwDLaCkCGmwzkQpDUt6ME,881
-pista/requirements.txt,sha256=lujXQMLafiNVpVRom3UQWOfgifrEek69NphqXZpjSpk,714
+pista/requirements.txt,sha256=x4MW3Xp-jE9ZZQUCW-4Zu247ehZQ917OeKYgMVbV_dw,853
 pista/root.py,sha256=ky2NB5RyV2LGN1NYQ8f30iSHbtxkw35Qhgg8fb7xqp8,357
 pista/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pista/core/_config_manager.py,sha256=9Av_pyJH6tx2Grmcn1WQEkW1nUA6dhnV-Qg6rCdwDxg,2005
 pista/core/_data_manager.py,sha256=ihyNgv7T3T36mbQfjiUlFPDlPvmI5Tp2JjvjNbEO30g,935
 pista/core/_log_manager.py,sha256=DbAPceE1Kl_eBLWczht8HFghOn3c0u-Qks2P7uEGT8o,5736
 pista/core/_root_manager.py,sha256=uQbapEfMd_4dIsK2T042eEAErMwEA6T1YxTaRuzo7QE,1490
 pista/core/_test_enhancer.py,sha256=_T5fpX28Pdw8zE2Tdmfm8zOl-ZKK29Zj6btW-MuVjvI,5973
@@ -63,11 +63,11 @@
 pista/tests/test_Pista_API_ExcelData.py,sha256=St2vwM4nqjhuwu_92fTY21ZgDvLT4A658XUG2TTtn5s,745
 pista/tests/test_Pista_SSH_Xterm.py,sha256=Y_e-AQCZ3HAXDtBAkEst0WTGmLog6b9QT85rVCH3unE,874
 pista/tests/test_Pista_UI_WebBrowser.py,sha256=ddMDb5VkcwVeZKodOz5f_fu9tVTexZVAJwBuYKWffBk,365
 pista/tests/test_Pista_VariableDataFile.py,sha256=ARGsaP_fpnZdAAhh8k0dxexRmMWqx5H1ZRFmQWYb00Q,650
 pista/tests/output/log_1308.log,sha256=9X8DVDojJgvf95rHAHgP0W-NykBqKuLxROjDGF6OerQ,699
 pista/tests/output/log_xterm.log,sha256=pwteOzOPbZem6bMJsiYwZxCVV442jBYGC6sbT-c0cJc,4444
 pista/tests/output/report.html,sha256=0v9Gy3TP7NwKX7CCoOJTwGRW24yADmBI1TM9SYCDI0s,50822
-pista_core-0.0.0a15.dist-info/METADATA,sha256=sTG68pm7UeLXuH8WRDBVso6-aWquAi_hgja8rCyQayk,86
-pista_core-0.0.0a15.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pista_core-0.0.0a15.dist-info/top_level.txt,sha256=qyaQLDNzBGzsUjPV9CNJyXu_E5jknTVuICWuyYIPlOw,6
-pista_core-0.0.0a15.dist-info/RECORD,,
+pista_core-0.0.0a16.dist-info/METADATA,sha256=JO5eF-n_YakDvtIWgmM79RNMqM5Cm1LxZNS5futi1Fw,86
+pista_core-0.0.0a16.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pista_core-0.0.0a16.dist-info/top_level.txt,sha256=qyaQLDNzBGzsUjPV9CNJyXu_E5jknTVuICWuyYIPlOw,6
+pista_core-0.0.0a16.dist-info/RECORD,,
```

