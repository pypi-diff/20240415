# Comparing `tmp/odoo14_addon_ssi_master_data_mixin-14.0.3.1.1-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_master_data_mixin-14.0.4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 53996 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1278 b- defN 24-Feb-25 03:07 odoo/addons/ssi_master_data_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Feb-25 03:07 odoo/addons/ssi_master_data_mixin/__init__.py
--rw-r--r--  2.0 unx      514 b- defN 24-Feb-25 03:08 odoo/addons/ssi_master_data_mixin/__manifest__.py
--rw-r--r--  2.0 unx      192 b- defN 24-Feb-25 03:07 odoo/addons/ssi_master_data_mixin/models/__init__.py
--rw-r--r--  2.0 unx     2066 b- defN 24-Feb-25 03:07 odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Feb-25 03:07 odoo/addons/ssi_master_data_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     2156 b- defN 24-Feb-25 03:08 odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
--rw-r--r--  2.0 unx     1815 b- defN 24-Feb-25 03:09 odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-25 03:09 odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Feb-25 03:09 odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 24-Feb-25 03:09 odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/RECORD
-11 files, 57833 bytes uncompressed, 51868 bytes compressed:  10.3%
+Zip file size: 54205 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1278 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/__init__.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      192 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     2541 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     2405 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
+-rw-r--r--  2.0 unx     1862 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD
+11 files, 58634 bytes uncompressed, 52077 bytes compressed:  11.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_master_data_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/METADATA
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/WHEEL
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/RECORD
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_master_data_mixin/__manifest__.py

```diff
@@ -1,18 +1,19 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Master Data Mixin",
-    "version": "14.0.3.1.1",
+    "version": "14.0.4.0.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "mail",
         "ssi_print_mixin",
+        "ssi_sequence_mixin",
     ],
     "data": [
         "views/mixin_master_data_views.xml",
     ],
 }
```

## odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py

```diff
@@ -8,14 +8,15 @@
 
 class MixinMasterData(models.AbstractModel):
     _name = "mixin.master_data"
     _inherit = [
         "mail.activity.mixin",
         "mail.thread",
         "mixin.print_document",
+        "mixin.sequence",
     ]
     _description = "Mixin for Master Data"
     _field_name_string = "Name"
     _show_code_on_display_name = False
     _automatically_insert_print_button = True
     _print_button_xpath = "/form/header"
     _print_button_position = "inside"
@@ -47,23 +48,37 @@
             default = {}
         if "code" not in default:
             default["code"] = _("%s (copy)", self.code)
         return super(MixinMasterData, self).copy(default=default)
 
     @api.constrains("code")
     def _check_duplicate_code(self):
-        error_msg = _("Duplicate code not allowed")
         for record in self:
             criteria = [
                 ("code", "=", record.code),
                 ("id", "!=", record.id),
+                ("code", "!=", "/"),
             ]
             count_duplicate = self.search_count(criteria)
             if count_duplicate > 0:
-                raise UserError(error_msg)
+                error_message = """
+                Document Type: %s
+                Context: Create or update document
+                Database ID: %s
+                Problem: Dupilicate code
+                Solution: Change code
+                """ % (
+                    self._description.lower(),
+                    self.id,
+                )
+                raise UserError(error_message)
+
+    def action_generate_code(self):
+        for record in self.sudo():
+            record._create_sequence()
 
     def name_get(self):
         result = []
         for record in self:
             if self._show_code_on_display_name:
                 name = "[%s] %s" % (record.code, record.name)
             else:
```

## odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml

### odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml

```diff
@@ -28,15 +28,17 @@
     </field>
   </record>
   <record id="mixin_master_data_view_form" model="ir.ui.view">
     <field name="name">mixin.master_data - form</field>
     <field name="model">mixin.master_data</field>
     <field name="arch" type="xml">
       <form>
-        <header/>
+        <header>
+          <button name="action_generate_code" string="Generate Code" type="object" class="oe_highlight"/>
+        </header>
         <sheet>
           <div name="div_smart_buttons" class="oe_button_box"/>
           <group name="group_1" colspan="4" col="2">
             <field name="name"/>
             <field name="code"/>
             <field name="active" widget="boolean_toggle"/>
           </group>
```

## Comparing `odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/METADATA` & `odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-master-data-mixin
-Version: 14.0.3.1.1
+Version: 14.0.4.0.0
 Summary: Master Data Mixin
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-ssi-print-mixin
+Requires-Dist: odoo14-addon-ssi-sequence-mixin
 Requires-Dist: odoo <14.1dev,>=14.0a
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: AGPL-3
 
 =================
```

## Comparing `odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/RECORD` & `odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_master_data_mixin/README.rst,sha256=lLjXhCxU_VIVtry1OgQuBcHYRjVO-ENZiENQp9GdwFQ,1278
 odoo/addons/ssi_master_data_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_master_data_mixin/__manifest__.py,sha256=_NBnmFmsmc5y-_NuJMaoKPfOo7d230g92SPmAj1uvTM,514
+odoo/addons/ssi_master_data_mixin/__manifest__.py,sha256=Ijj9Kyo-ltyI21i2IR4ToMa0TYvGqH7NSpfbO_GtsD0,544
 odoo/addons/ssi_master_data_mixin/models/__init__.py,sha256=MH-geBjhVAfrd9wgl2Z6Ojz-WndWU4Sxeo-9yfB0hLE,192
-odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py,sha256=JlvqHwnr4GvukVgXBTb2GI0cXclFPmDr9hJsX9kMznY,2066
+odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py,sha256=prhSjF8i8J-BXTNgp6atRjgZaC-FJDXofEUio1Myp0g,2541
 odoo/addons/ssi_master_data_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml,sha256=YUEhuMjwt7WX2M5BmrZild_58W0z_LASTLoDxOF1MYY,2156
-odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/METADATA,sha256=wZNYdlNTsXvpaUAajno_YO3E0mDQI4WO8pKhTNUSFyk,1815
-odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_master_data_mixin-14.0.3.1.1.dist-info/RECORD,,
+odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml,sha256=YUudvAOkcpWzf0XUvvGJYYaSaTC65GfNFZDbRcvWlN0,2405
+odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA,sha256=0Ref6div4mhaPIPRNtmLjVBNuUPb_hQfIYWdEPio-ys,1862
+odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD,,
```

