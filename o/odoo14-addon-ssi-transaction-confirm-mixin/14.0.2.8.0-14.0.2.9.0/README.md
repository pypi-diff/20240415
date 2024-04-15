# Comparing `tmp/odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 55241 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1288 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/__init__.py
--rw-r--r--  2.0 unx      588 b- defN 24-Apr-10 10:42 odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py
--rw-r--r--  2.0 unx      200 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py
--rw-r--r--  2.0 unx    11882 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     2839 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
--rw-r--r--  2.0 unx     1924 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1314 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/RECORD
-11 files, 68646 bytes uncompressed, 52889 bytes compressed:  23.0%
+Zip file size: 55244 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1288 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/__init__.py
+-rw-r--r--  2.0 unx      588 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      200 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py
+-rw-r--r--  2.0 unx    11965 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     2839 b- defN 24-Apr-15 02:13 odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
+-rw-r--r--  2.0 unx     1924 b- defN 24-Apr-15 02:14 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 02:14 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-15 02:14 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1314 b- defN 24-Apr-15 02:14 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/RECORD
+11 files, 68729 bytes uncompressed, 52892 bytes compressed:  23.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Waiting for Approval State",
-    "version": "14.0.2.8.0",
+    "version": "14.0.2.9.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
         "ssi_multiple_approval_mixin",
```

## odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py

```diff
@@ -119,14 +119,17 @@
             record.write(record._prepare_confirm_data())
             record._run_post_confirm_check()
             record._run_post_confirm_action()
             record.action_request_approval()
 
     def _check_confirm_policy(self):
         self.ensure_one()
+        if not self._automatically_insert_confirm_button:
+            return True
+
         if self.env.context.get("bypass_policy_check", False):
             return True
 
         if not self.confirm_ok:
             error_message = """
                 Document Type: %s
                 Context: Confirm document
```

## Comparing `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-confirm-mixin
-Version: 14.0.2.8.0
+Version: 14.0.2.9.0
 Summary: Transaction Mixin - Waiting for Approval State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_confirm_mixin/README.rst,sha256=LnAs5oFV6kOiX1rOHkZtPpEUaAQUJlcQk1BLL_Dgbg4,1288
 odoo/addons/ssi_transaction_confirm_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py,sha256=oH5nQ5WaQcRLfe7KHCLUxsmHvMrNwIzGRFmh6s9TCC8,588
+odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py,sha256=KWEC7hs4T3z-H7dMvo0oAO5fdwAlYlhNlK6kxWT7xoI,588
 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py,sha256=kJTOEh8MVP031XPCjCUhq32C99VJfwAreZ3lnX7HFxQ,200
-odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py,sha256=HPKzf8cYVQO2o08ClglLIW7Ke95kRToW5rlfJaflGXo,11882
+odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py,sha256=Pq1NnqarTQmxAmRy4FEYDErQOYtJ3CgV6g4cdu4H9qI,11965
 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
 odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml,sha256=gOWK1MYp7R7bQv2WUTXzsug81vEDhMFi80lSgJaMMnM,2839
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/METADATA,sha256=94V-3BPIw31bIqpW6-dkUtzFC1ZRaYb4utysmVzT2t0,1924
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.8.0.dist-info/RECORD,,
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/METADATA,sha256=YBGY660XTP5k7kwMuWXp8JbiDxu7N4NTeGN7vDoL-6E,1924
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.9.0.dist-info/RECORD,,
```

