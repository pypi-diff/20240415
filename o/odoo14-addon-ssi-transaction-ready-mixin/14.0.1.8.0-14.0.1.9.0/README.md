# Comparing `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54696 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/__init__.py
--rw-r--r--  2.0 unx      543 b- defN 24-Apr-10 00:00 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
--rw-r--r--  2.0 unx     7310 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      804 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
--rw-r--r--  2.0 unx     1846 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD
-11 files, 61870 bytes uncompressed, 52396 bytes compressed:  15.3%
+Zip file size: 54705 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/__init__.py
+-rw-r--r--  2.0 unx      543 b- defN 24-Apr-10 10:42 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      198 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7346 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      804 b- defN 24-Apr-10 10:41 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
+-rw-r--r--  2.0 unx     1846 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-10 10:42 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/RECORD
+11 files, 61906 bytes uncompressed, 52405 bytes compressed:  15.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_ready_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Ready to Process State",
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

## odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py

```diff
@@ -109,15 +109,16 @@
     def _check_ready_policy(self):
         self.ensure_one()
         if self.env.context.get("bypass_policy_check", False):
             return True
 
         if not self.ready_ok:
             error_message = """
-            Context: Stage %s
+            Document Type: %s
+            Context: Stage document
             Database ID: %s
             Problem: Document is not allowed to stage
             Solution: Check stage policy prerequisite
             """ % (
                 self._description.lower(),
                 self.id,
             )
```

## Comparing `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-ready-mixin
-Version: 14.0.1.8.0
+Version: 14.0.1.9.0
 Summary: Transaction Mixin - Ready to Process State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

