# Comparing `tmp/odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54351 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1224 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/__init__.py
--rw-r--r--  2.0 unx      530 b- defN 23-Dec-30 14:52 odoo/addons/ssi_transaction_done_mixin/__manifest__.py
--rw-r--r--  2.0 unx      197 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/models/__init__.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/models/mixin_transaction_done.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      537 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml
--rw-r--r--  2.0 unx     1787 b- defN 23-Dec-30 14:54 odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-30 14:54 odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Dec-30 14:54 odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1273 b- defN 23-Dec-30 14:54 odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/RECORD
-11 files, 60353 bytes uncompressed, 52077 bytes compressed:  13.7%
+Zip file size: 54620 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1224 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/__init__.py
+-rw-r--r--  2.0 unx      530 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_done_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      197 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7258 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/models/mixin_transaction_done.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      738 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml
+-rw-r--r--  2.0 unx     1785 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/RECORD
+11 files, 61616 bytes uncompressed, 52346 bytes compressed:  15.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_done_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_done_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Done State",
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

## odoo/addons/ssi_transaction_done_mixin/models/mixin_transaction_done.py

```diff
@@ -2,15 +2,18 @@
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 
 from inspect import getmembers
 
 from lxml import etree
 
-from odoo import api, fields, models
+from odoo import _, api, fields, models
+from odoo.exceptions import UserError
+
+from odoo.addons.ssi_decorator import ssi_decorator
 
 
 class MixinTransactionDone(models.AbstractModel):
     _name = "mixin.transaction_done"
     _inherit = [
         "mixin.transaction",
     ]
@@ -92,20 +95,38 @@
             if self.is_decorator(func, "_post_done_action"):
                 methods.append(func)
         if methods:
             self.run_decorator_method(methods)
 
     def action_done(self):
         for record in self.sudo():
+            record._check_done_policy()
             record._run_pre_done_check()
             record._run_pre_done_action()
             record.write(record._prepare_done_data())
             record._run_post_done_check()
             record._run_post_done_action()
 
+    def _check_done_policy(self):
+        self.ensure_one()
+        if self.env.context.get("bypass_done_policy", False):
+            return True
+
+        if not self.done_ok:
+            error_message = """
+                Context: Finish %s
+                Database ID: %s
+                Problem: Document is not allowed to finish
+                Solution: Check finish policy prerequisite
+                """ % (
+                self._description.lower(),
+                self.id,
+            )
+            raise UserError(_(error_message))
+
     @api.model
     def fields_view_get(
         self, view_id=None, view_type="form", toolbar=False, submenu=False
     ):
         result = super().fields_view_get(
             view_id=view_id, view_type=view_type, toolbar=toolbar, submenu=submenu
         )
@@ -174,7 +195,18 @@
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_done_mixin.button_done",
                 "/form/header/field[@name='state']",
                 "before",
             )
         return view_arch
+
+    @ssi_decorator.insert_on_tree_view()
+    def _01_view_add_tree_done_button(self, view_arch):
+        if self._automatically_insert_done_button:
+            view_arch = self._add_view_element(
+                view_arch,
+                "ssi_transaction_done_mixin.tree_button_done",
+                "/tree/header",
+                "inside",
+            )
+        return view_arch
```

## odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml

### odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml

```diff
@@ -2,11 +2,14 @@
 <odoo>
   <template id="done_policy_field">
     <field name="done_ok"/>
   </template>
   <template id="button_done">
     <button name="action_done" string="Done" type="object" class="oe_highlight" attrs="{'invisible':[('done_ok','!=',True)]}" confirm="Finish data. Are you sure?"/>
   </template>
+  <template id="tree_button_done">
+    <button name="action_done" string="Done" type="object" confirm="Finish data. Are you sure?"/>
+  </template>
   <template id="done_filter">
     <filter name="dom_done" string="Done" domain="[('state', '=', 'done')]"/>
   </template>
 </odoo>
```

## Comparing `odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-done-mixin
-Version: 14.0.1.8.0
+Version: 14.0.1.9.0
 Summary: Transaction Mixin - Done State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-ssi-transaction-mixin
-Requires-Dist: odoo (<14.1dev,>=14.0a)
+Requires-Dist: odoo <14.1dev,>=14.0a
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: AGPL-3
 
 ==============================
 Transaction Mixin - Done State
```

## Comparing `odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_done_mixin/README.rst,sha256=DS-OJXRCoDosDfteSAlLkCAfTuyvy2ZodOdmxxM5t44,1224
 odoo/addons/ssi_transaction_done_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_done_mixin/__manifest__.py,sha256=SvFEiFVRvOK-pYmJ3DGv3oAiERojwFpT72owPPcNV34,530
+odoo/addons/ssi_transaction_done_mixin/__manifest__.py,sha256=RwpujF-o8b9efj69aRG4o4bNfkYWKwKhgwjSjljNxHs,530
 odoo/addons/ssi_transaction_done_mixin/models/__init__.py,sha256=DRmZ-m-qxZZKBPl1jFWUoYeb-0GzAGhh4SLDAWgBbRU,197
-odoo/addons/ssi_transaction_done_mixin/models/mixin_transaction_done.py,sha256=eACeOFuNB9-uqEgQtWJdORIa6-bxps-qVPGNU3hdjRs,6194
+odoo/addons/ssi_transaction_done_mixin/models/mixin_transaction_done.py,sha256=WLsYfbYShQHlwvvYFW1cBMTX3iGGg-G3YRMr_f-FSew,7258
 odoo/addons/ssi_transaction_done_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml,sha256=dLgL-OuvlkO-_W-VU2bH5aPhj9P4o2yzVdomWnqwkO8,537
-odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/METADATA,sha256=kAu9BiKvXwxcJ07rEZHo1N7OFOKsfLmklRe9QXIB_-k,1787
-odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_done_mixin-14.0.1.8.0.dist-info/RECORD,,
+odoo/addons/ssi_transaction_done_mixin/templates/mixin_transaction_done_templates.xml,sha256=LgZ4Rmz4PfafoL3yi7O_k0Isxbf3s7p_UC9TJymtt24,738
+odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/METADATA,sha256=aGjD4rwCztH3ZwvQP7edmpbjVn2XsPnI_TCBy1OK8Ds,1785
+odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_done_mixin-14.0.1.9.0.dist-info/RECORD,,
```

