# Comparing `tmp/odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54640 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1256 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/__init__.py
--rw-r--r--  2.0 unx      537 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_open_mixin/__manifest__.py
--rw-r--r--  2.0 unx      197 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/models/__init__.py
--rw-r--r--  2.0 unx     7266 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      697 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
--rw-r--r--  2.0 unx     1824 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD
-11 files, 61661 bytes uncompressed, 52366 bytes compressed:  15.1%
+Zip file size: 54643 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1256 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/__init__.py
+-rw-r--r--  2.0 unx      537 b- defN 24-Apr-10 00:00 odoo/addons/ssi_transaction_open_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      197 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7267 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      697 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
+-rw-r--r--  2.0 unx     1824 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/RECORD
+11 files, 61662 bytes uncompressed, 52369 bytes compressed:  15.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_open_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - In Progress State",
-    "version": "14.0.1.8.0",
+    "version": "14.0.1.9.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
     ],
```

## odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py

```diff
@@ -104,15 +104,15 @@
             record._run_pre_open_action()
             record.write(record._prepare_open_data())
             record._run_post_open_check()
             record._run_post_open_action()
 
     def _check_open_policy(self):
         self.ensure_one()
-        if self.env.context.get("bypass_open_policy", False):
+        if self.env.context.get("bypass_policy_check", False):
             return True
 
         if not self.open_ok:
             error_message = """
                 Context: Start %s
                 Database ID: %s
                 Problem: Document is not allowed to start
```

## Comparing `odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-open-mixin
-Version: 14.0.1.8.0
+Version: 14.0.1.9.0
 Summary: Transaction Mixin - In Progress State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_open_mixin/README.rst,sha256=LsaB-c6GP16LpNgw-0pN-2ylD3Q_d3TCg6dHy79wuB8,1256
 odoo/addons/ssi_transaction_open_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_open_mixin/__manifest__.py,sha256=Hpp9IYzGPWRj62fNEsuMd-1PmCck8xoE9BD8LBDPapM,537
+odoo/addons/ssi_transaction_open_mixin/__manifest__.py,sha256=EvLq-u-fxu17b2C3-sHkJPkjcSb24g3CM3Ucq9vTa_w,537
 odoo/addons/ssi_transaction_open_mixin/models/__init__.py,sha256=9Xi4MfyVO72dwQ8dVtgQqU2p4Q6v4223KpaiAf3pS3o,197
-odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py,sha256=qrZoNTzO7ZDFZ0mtNuLCehkkVrq-21CmX366COML71I,7266
+odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py,sha256=Y09rjBIvSHGIwArQgtiKPFdA-FWDpMAfEGr1whJeDGc,7267
 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
 odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml,sha256=hjtYoBYPwswPncZPs4s9SqszrHZuC64BhTYgQ4McBso,697
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA,sha256=MkjJFQyGtzf7SfcwN_V6RhU0g9rd6Uo_tVhAKOpbq_E,1824
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD,,
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/METADATA,sha256=SUU-iC793BIJ5g2kMTOM7BNDNLs5eovBGH2-vUhQRxA,1824
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.9.0.dist-info/RECORD,,
```

