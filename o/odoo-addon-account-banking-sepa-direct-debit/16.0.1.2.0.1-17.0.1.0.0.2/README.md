# Comparing `tmp/odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1-py3-none-any.whl.zip` & `tmp/odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,56 @@
-Zip file size: 124831 bytes, number of entries: 55
--rw-r--r--  2.0 unx     5623 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/README.rst
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/__manifest__.py
--rw-r--r--  2.0 unx      544 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/account_payment_method.xml
--rw-r--r--  2.0 unx     1755 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml
--rw-r--r--  2.0 unx      799 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/mandate_expire_cron.xml
--rw-r--r--  2.0 unx    47698 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.02.xsd
--rw-r--r--  2.0 unx    49754 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.03.xsd
--rw-r--r--  2.0 unx    48847 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.04.xsd
--rw-r--r--  2.0 unx    25834 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.003.02.xsd
--rw-r--r--  2.0 unx      750 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/data/report_paperformat.xml
--rw-r--r--  2.0 unx     1986 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/demo/sepa_direct_debit_demo.xml
--rw-r--r--  2.0 unx    20807 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/account_banking_sepa_direct_debit.pot
--rw-r--r--  2.0 unx    22079 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/de.po
--rw-r--r--  2.0 unx    28891 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/es.po
--rw-r--r--  2.0 unx    26780 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/es_AR.po
--rw-r--r--  2.0 unx    26781 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/fr.po
--rw-r--r--  2.0 unx    21286 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/hr.po
--rw-r--r--  2.0 unx    21535 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/it.po
--rw-r--r--  2.0 unx    21229 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/nb_NO.po
--rw-r--r--  2.0 unx    26007 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/nl.po
--rw-r--r--  2.0 unx    21489 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/pt_BR.po
--rw-r--r--  2.0 unx    24414 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/i18n/sl.po
--rw-r--r--  2.0 unx      401 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/migrations/16.0.1.0.2/post-migration.py
--rw-r--r--  2.0 unx      242 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/__init__.py
--rw-r--r--  2.0 unx     5555 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py
--rw-r--r--  2.0 unx     2383 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_method.py
--rw-r--r--  2.0 unx     1207 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_mode.py
--rw-r--r--  2.0 unx    13488 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_order.py
--rw-r--r--  2.0 unx      551 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py
--rw-r--r--  2.0 unx     1172 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/models/res_company.py
--rw-r--r--  2.0 unx     1307 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.rst
--rw-r--r--  2.0 unx      396 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      673 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx      132 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.rst
--rw-r--r--  2.0 unx      194 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.rst
--rw-r--r--  2.0 unx      989 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/reports/sepa_direct_debit_mandate.xml
--rw-r--r--  2.0 unx     7840 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.png
--rw-r--r--  2.0 unx    23879 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.svg
--rw-r--r--  2.0 unx    16408 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/static/description/index.html
--rw-r--r--  2.0 unx      518 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/static/src/css/report.css
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/tests/__init__.py
--rw-r--r--  2.0 unx     2474 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/tests/test_mandate.py
--rw-r--r--  2.0 unx    14342 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/tests/test_sdd.py
--rw-r--r--  2.0 unx     4608 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml
--rw-r--r--  2.0 unx      890 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/views/account_payment_mode.xml
--rw-r--r--  2.0 unx    20588 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/views/report_sepa_direct_debit_mandate.xml
--rw-r--r--  2.0 unx      959 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml
--rw-r--r--  2.0 unx       34 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/wizards/__init__.py
--rw-r--r--  2.0 unx      356 b- defN 24-Apr-02 02:55 odoo/addons/account_banking_sepa_direct_debit/wizards/res_config_settings.py
--rw-r--r--  2.0 unx     6337 b- defN 24-Apr-02 02:55 odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 02:55 odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-02 02:55 odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6903 b- defN 24-Apr-02 02:55 odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/RECORD
-55 files, 582622 bytes uncompressed, 112973 bytes compressed:  80.6%
+Zip file size: 124147 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     5652 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/README.rst
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/__manifest__.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/account_payment_method.xml
+-rw-r--r--  2.0 unx     1698 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml
+-rw-r--r--  2.0 unx      799 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/mandate_expire_cron.xml
+-rw-r--r--  2.0 unx    47698 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.02.xsd
+-rw-r--r--  2.0 unx    49754 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.03.xsd
+-rw-r--r--  2.0 unx    48847 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.04.xsd
+-rw-r--r--  2.0 unx    25834 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.003.02.xsd
+-rw-r--r--  2.0 unx      750 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/data/report_paperformat.xml
+-rw-r--r--  2.0 unx     1986 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/demo/sepa_direct_debit_demo.xml
+-rw-r--r--  2.0 unx    20292 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/account_banking_sepa_direct_debit.pot
+-rw-r--r--  2.0 unx    22079 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/de.po
+-rw-r--r--  2.0 unx    28891 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/es.po
+-rw-r--r--  2.0 unx    26780 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/es_AR.po
+-rw-r--r--  2.0 unx    26781 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/fr.po
+-rw-r--r--  2.0 unx    21286 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/hr.po
+-rw-r--r--  2.0 unx    21535 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/it.po
+-rw-r--r--  2.0 unx    21229 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/nb_NO.po
+-rw-r--r--  2.0 unx    26007 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/nl.po
+-rw-r--r--  2.0 unx    21489 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/pt_BR.po
+-rw-r--r--  2.0 unx    24414 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/i18n/sl.po
+-rw-r--r--  2.0 unx      242 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/__init__.py
+-rw-r--r--  2.0 unx     5592 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py
+-rw-r--r--  2.0 unx     2389 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_method.py
+-rw-r--r--  2.0 unx     1207 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_mode.py
+-rw-r--r--  2.0 unx    13488 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_order.py
+-rw-r--r--  2.0 unx      568 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py
+-rw-r--r--  2.0 unx     1172 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/models/res_company.py
+-rw-r--r--  2.0 unx     1354 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.md
+-rw-r--r--  2.0 unx      412 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.md
+-rw-r--r--  2.0 unx      677 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.md
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.md
+-rw-r--r--  2.0 unx      196 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.md
+-rw-r--r--  2.0 unx      989 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/reports/sepa_direct_debit_mandate.xml
+-rw-r--r--  2.0 unx     7840 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.png
+-rw-r--r--  2.0 unx    23879 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.svg
+-rw-r--r--  2.0 unx    16408 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/static/description/index.html
+-rw-r--r--  2.0 unx      518 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/static/src/css/report.css
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/tests/__init__.py
+-rw-r--r--  2.0 unx     2447 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/tests/test_mandate.py
+-rw-r--r--  2.0 unx    14342 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/tests/test_sdd.py
+-rw-r--r--  2.0 unx     4463 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml
+-rw-r--r--  2.0 unx      890 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/views/account_payment_mode.xml
+-rw-r--r--  2.0 unx    20588 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/views/report_sepa_direct_debit_mandate.xml
+-rw-r--r--  2.0 unx      668 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml
+-rw-r--r--  2.0 unx       34 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/wizards/__init__.py
+-rw-r--r--  2.0 unx      356 b- defN 24-Apr-15 06:50 odoo/addons/account_banking_sepa_direct_debit/wizards/res_config_settings.py
+-rw-r--r--  2.0 unx     6343 b- defN 24-Apr-15 06:50 odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       83 b- defN 24-Apr-15 06:50 odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-15 06:50 odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6757 b- defN 24-Apr-15 06:50 odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/RECORD
+54 files, 581194 bytes uncompressed, 112545 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -63,17 +63,14 @@
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/i18n/pt_BR.po
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/i18n/sl.po
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/migrations/16.0.1.0.2/post-migration.py
-Comment: 
-
 Filename: odoo/addons/account_banking_sepa_direct_debit/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py
@@ -90,27 +87,27 @@
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/models/res_company.py
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.rst
+Filename: odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.md
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.rst
+Filename: odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.md
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.rst
+Filename: odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.md
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.rst
+Filename: odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.md
 Comment: 
 
-Filename: odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.rst
+Filename: odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.md
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/reports/sepa_direct_debit_mandate.xml
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/static/description/icon.png
 Comment: 
@@ -147,20 +144,20 @@
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/wizards/__init__.py
 Comment: 
 
 Filename: odoo/addons/account_banking_sepa_direct_debit/wizards/res_config_settings.py
 Comment: 
 
-Filename: odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/METADATA
+Filename: odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/WHEEL
+Filename: odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/top_level.txt
+Filename: odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/RECORD
+Filename: odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/account_banking_sepa_direct_debit/README.rst

```diff
@@ -3,148 +3,152 @@
 =================================
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:a433755fd2d5cc4c242b073380fd215deb68ea43af0cdef7207c68febe5f8c10
+   !! source digest: sha256:4649f6ba9491ff0cbc494f6c1cd03f80b300902d9782a202619be9894a2128a5
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fbank--payment-lightgray.png?logo=github
-    :target: https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit
+    :target: https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit
     :alt: OCA/bank-payment
 .. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
-    :target: https://translation.odoo-community.org/projects/bank-payment-16-0/bank-payment-16-0-account_banking_sepa_direct_debit
+    :target: https://translation.odoo-community.org/projects/bank-payment-17-0/bank-payment-17-0-account_banking_sepa_direct_debit
     :alt: Translate me on Weblate
 .. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
-    :target: https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&target_branch=16.0
+    :target: https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&target_branch=17.0
     :alt: Try me on Runboat
 
 |badge1| |badge2| |badge3| |badge4| |badge5|
 
 Create SEPA files for Direct Debit
 
 Module to export direct debit payment orders in SEPA XML file format.
 
 SEPA PAIN (PAyment INitiation) is the new european standard for
-Customer-to-Bank payment instructions. This module implements SEPA Direct
-Debit (SDD), more specifically PAIN versions 008.001.02, 008.001.03 and
-008.001.04. It is part of the ISO 20022 standard, available on
-http://www.iso20022.org.
-
-The Implementation Guidelines for SEPA Direct Debit published by the European
-Payments Council (http://http://www.europeanpaymentscouncil.eu) use PAIN
-version 008.001.02. So if you don't know which version your bank supports, you
-should try version 008.001.02 first.
+Customer-to-Bank payment instructions. This module implements SEPA
+Direct Debit (SDD), more specifically PAIN versions 008.001.02,
+008.001.03 and 008.001.04. It is part of the ISO 20022 standard,
+available on http://www.iso20022.org.
+
+The Implementation Guidelines for SEPA Direct Debit published by the
+European Payments Council (http://http://www.europeanpaymentscouncil.eu)
+use PAIN version 008.001.02. So if you don't know which version your
+bank supports, you should try version 008.001.02 first.
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Installation
 ============
 
 This module depends on :
 
-* account_banking_pain_base
-* account_banking_mandate
+-  account_banking_pain_base
+-  account_banking_mandate
 
 This module is part of the OCA/bank-payment suite.
 
 Configuration
 =============
 
 For setting the SEPA creditor identifier:
 
-#. Go to Invoicing/Accounting > Configuration > Settings.
-#. On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*, you can
-   fill the corresponding identifier.
+1. Go to Invoicing/Accounting > Configuration > Settings.
+2. On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*,
+   you can fill the corresponding identifier.
 
 If your country requires several identifiers (like Spain), you must:
 
-#. Go to *Invoicing/Accounting > Configuration > Settings*.
-#. On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
-#. Now go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a payment mode for your specific bank.
-#. Fill the specific identifier on the field "SEPA Creditor Identifier".
+1. Go to *Invoicing/Accounting > Configuration > Settings*.
+2. On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
+3. Now go to *Invoicing/Accounting > Configuration > Management >
+   Payment Modes*.
+4. Create a payment mode for your specific bank.
+5. Fill the specific identifier on the field "SEPA Creditor Identifier".
 
 For defining a payment mode that uses SEPA direct debit:
 
-#. Go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a record.
-#. Select the Payment Method *SEPA Direct Debit for customers* (which is
+1. Go to *Invoicing/Accounting > Configuration > Management > Payment
+   Modes*.
+2. Create a record.
+3. Select the Payment Method *SEPA Direct Debit for customers* (which is
    automatically created upon module installation).
-#. Check that this payment method uses the proper version of PAIN.
-#. If not, go *Invoicing/Accounting > Configuration > Management > Payment Methods*.
-#. Locate the "SEPA Direct Debit for customers" record and open it.
-#. Change the "PAIN version" according your needs.
-#. If you need to handle several PAIN versions, just duplicate the payment
-   method adjusting this field on each for having them.
+4. Check that this payment method uses the proper version of PAIN.
+5. If not, go *Invoicing/Accounting > Configuration > Management >
+   Payment Methods*.
+6. Locate the "SEPA Direct Debit for customers" record and open it.
+7. Change the "PAIN version" according your needs.
+8. If you need to handle several PAIN versions, just duplicate the
+   payment method adjusting this field on each for having them.
 
 Usage
 =====
 
-In the menu *Invoicing/Accounting > Customers > Debit Order*, create a new debit
-order and select the Payment Mode dedicated to SEPA Direct Debit that
-you created during the configuration step.
+In the menu *Invoicing/Accounting > Customers > Debit Order*, create a
+new debit order and select the Payment Mode dedicated to SEPA Direct
+Debit that you created during the configuration step.
 
 Bug Tracker
 ===========
 
 Bugs are tracked on `GitHub Issues <https://github.com/OCA/bank-payment/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-`feedback <https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+`feedback <https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
-~~~~~~~
+-------
 
 * Akretion
 * Tecnativa
 
 Contributors
-~~~~~~~~~~~~
+------------
 
-* Alexis de Lattre <alexis.delattre@akretion.com>
-* Stéphane Bidoul <stephane.bidoul@acsone.eu>
-* Alexandre Fayolle
-* Raphaël Valyi
-* Sandy Carter
-* Antonio Espinosa <antonioea@antiun.com>
-* Marçal Isern <marsal.isern@qubiq.es>
-* `Tecnativa <https://www.tecnativa.com>`__:
-
-  * Pedro M. Baeza
-  * Sergio Teruel
-  * Carlos Roca
-  * Carolina Fernandez
-* Manuel Regidor <manuel.regidor@sygel.es>
+-  Alexis de Lattre <alexis.delattre@akretion.com>
+-  Stéphane Bidoul <stephane.bidoul@acsone.eu>
+-  Alexandre Fayolle
+-  Raphaël Valyi
+-  Sandy Carter
+-  Antonio Espinosa <antonioea@antiun.com>
+-  Marçal Isern <marsal.isern@qubiq.es>
+-  `Tecnativa <https://www.tecnativa.com>`__:
+
+   -  Pedro M. Baeza
+   -  Sergio Teruel
+   -  Carlos Roca
+   -  Carolina Fernandez
+
+-  Manuel Regidor <manuel.regidor@sygel.es>
 
 Maintainers
-~~~~~~~~~~~
+-----------
 
 This module is maintained by the OCA.
 
 .. image:: https://odoo-community.org/logo.png
    :alt: Odoo Community Association
    :target: https://odoo-community.org
 
 OCA, or the Odoo Community Association, is a nonprofit organization whose
 mission is to support the collaborative development of Odoo features and
 promote its widespread use.
 
-This module is part of the `OCA/bank-payment <https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit>`_ project on GitHub.
+This module is part of the `OCA/bank-payment <https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit>`_ project on GitHub.
 
 You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
```

## odoo/addons/account_banking_sepa_direct_debit/__manifest__.py

```diff
@@ -3,15 +3,15 @@
 # Copyright 2014-2022 Tecnativa - Pedro M. Baeza
 # Copyright 2024 Tecnativa - Carolina Fernandez
 # License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
 
 {
     "name": "Account Banking SEPA Direct Debit",
     "summary": "Create SEPA files for Direct Debit",
-    "version": "16.0.1.2.0",
+    "version": "17.0.1.0.0",
     "license": "AGPL-3",
     "author": "Akretion, Tecnativa, Odoo Community Association (OCA)",
     "website": "https://github.com/OCA/bank-payment",
     "category": "Banking addons",
     "depends": ["account_banking_pain_base", "account_banking_mandate"],
     "assets": {
         "web.report_assets_common": [
```

## odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml

### odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml

```diff
@@ -26,13 +26,12 @@
               <br/>
               Mitchell Admin
             </t>
           </t>
         </p>
       </div>
     </field>
-    <field name="report_template" ref="report_sepa_direct_debit_mandate"/>
-    <field name="report_name">{{ (object.unique_mandate_reference or 'SEPA Mandate').replace('/','_') }}</field>
+    <field name="report_template_ids" eval="[(4, ref('account_banking_sepa_direct_debit.report_sepa_direct_debit_mandate'))]"/>
     <field name="lang">{{ object.partner_id.lang }}</field>
     <field name="auto_delete" eval="True"/>
   </record>
 </odoo>
```

## odoo/addons/account_banking_sepa_direct_debit/i18n/account_banking_sepa_direct_debit.pot

```diff
@@ -1,14 +1,14 @@
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 # 	* account_banking_sepa_direct_debit
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Odoo Server 16.0\n"
+"Project-Id-Version: Odoo Server 17.0\n"
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
@@ -394,15 +394,14 @@
 #. module: account_banking_sepa_direct_debit
 #: model:ir.model.fields,field_description:account_banking_sepa_direct_debit.field_account_banking_mandate__recurrent_sequence_type
 msgid "Sequence Type for Next Debit"
 msgstr ""
 
 #. module: account_banking_sepa_direct_debit
 #: model:ir.actions.server,name:account_banking_sepa_direct_debit.sdd_mandate_expire_cron_ir_actions_server
-#: model:ir.cron,cron_name:account_banking_sepa_direct_debit.sdd_mandate_expire_cron
 msgid "Set SEPA Direct Debit Mandates to Expired"
 msgstr ""
 
 #. module: account_banking_sepa_direct_debit
 #. odoo-python
 #: code:addons/account_banking_sepa_direct_debit/models/account_payment_mode.py:0
 #: code:addons/account_banking_sepa_direct_debit/models/res_company.py:0
@@ -473,19 +472,14 @@
 
 #. module: account_banking_sepa_direct_debit
 #: model:ir.model.fields,field_description:account_banking_sepa_direct_debit.field_account_banking_mandate__unique_mandate_reference
 msgid "Unique Mandate Reference"
 msgstr ""
 
 #. module: account_banking_sepa_direct_debit
-#: model_terms:ir.ui.view,arch_db:account_banking_sepa_direct_debit.view_account_config_settings
-msgid "Write the ICS of your company"
-msgstr ""
-
-#. module: account_banking_sepa_direct_debit
 #: model:ir.model.fields.selection,name:account_banking_sepa_direct_debit.selection__account_payment_method__pain_version__pain_008_001_02
 msgid "pain.008.001.02 (recommended for direct debit)"
 msgstr ""
 
 #. module: account_banking_sepa_direct_debit
 #: model:ir.model.fields.selection,name:account_banking_sepa_direct_debit.selection__account_payment_method__pain_version__pain_008_001_03
 msgid "pain.008.001.03"
@@ -503,13 +497,7 @@
 
 #. module: account_banking_sepa_direct_debit
 #: model_terms:ir.ui.view,arch_db:account_banking_sepa_direct_debit.sepa_direct_debit_mandate_document
 msgid ""
 "to send instructions to your bank to debit your account and (B) your bank to\n"
 "                       debit your account in accordance with the instructions from"
 msgstr ""
-
-#. module: account_banking_sepa_direct_debit
-#: model:mail.template,report_name:account_banking_sepa_direct_debit.email_template_sepa_mandate
-msgid ""
-"{{ (object.unique_mandate_reference or 'SEPA Mandate').replace('/','_') }}"
-msgstr ""
```

## odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py

```diff
@@ -103,15 +103,16 @@
             ]
         )
         if expired_mandates:
             expired_mandates.write({"state": "expired"})
             for mandate in expired_mandates:
                 mandate.message_post(
                     body=_(
-                        "Mandate automatically set to expired after %d months without use."
+                        "Mandate automatically set to"
+                        " expired after %d months without use."
                     )
                     % NUMBER_OF_UNUSED_MONTHS_BEFORE_EXPIRY
                 )
             logger.info(
                 "%d SDD Mandate set to expired: IDs %s"
                 % (len(expired_mandates), expired_mandates.ids)
             )
@@ -121,23 +122,24 @@
     def print_report(self):
         self.ensure_one()
         xmlid = "account_banking_sepa_direct_debit.report_sepa_direct_debit_mandate"
         action = self.env.ref(xmlid).report_action(self)
         return action
 
     def action_mandate_send(self):
-        """Opens a wizard to compose an email, with relevant mail template loaded by default"""
+        """Opens a wizard to compose an email,
+        with relevant mail template loaded by default"""
         self.ensure_one()
         template_id = self.env["ir.model.data"]._xmlid_to_res_id(
             "account_banking_sepa_direct_debit.email_template_sepa_mandate",
             raise_if_not_found=False,
         )
         ctx = {
             "default_model": "account.banking.mandate",
-            "default_res_id": self.id,
+            "default_res_ids": self.ids,
             "default_use_template": bool(template_id),
             "default_template_id": template_id,
             "default_composition_mode": "comment",
             "is_sent": True,
             "force_email": True,
         }
         return {
```

## odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py

```diff
@@ -7,15 +7,15 @@
 
 class AccountPaymentLine(models.Model):
     _inherit = "account.payment.line"
 
     def draft2open_payment_line_check(self):
         res = super().draft2open_payment_line_check()
         sepa_dd_lines = self.filtered(
-            lambda l: l.order_id.payment_method_id.code == "sepa_direct_debit"
+            lambda line: line.order_id.payment_method_id.code == "sepa_direct_debit"
         )
         sepa_dd_lines._check_sepa_direct_debit_ready()
         return res
 
     def _check_sepa_direct_debit_ready(self):
         """
         This method checks whether the payment line(s) are ready to be used
```

## odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py

```diff
@@ -1,16 +1,17 @@
 # Copyright 2024 Tecnativa - Carolina Fernandez
 # License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl).
+import json
 
 from odoo import models
 
 
 class MailComposeMessage(models.TransientModel):
     _inherit = "mail.compose.message"
 
     def _action_send_mail(self, auto_commit=False):
         for wizard in self:
             if self.env.context.get("is_sent"):
-                self.env[wizard.model].sudo().browse(wizard.res_id).is_sent = True
-        return super(MailComposeMessage, self)._action_send_mail(
-            auto_commit=auto_commit
-        )
+                self.env[wizard.model].sudo().browse(
+                    json.loads(wizard.res_ids)
+                ).is_sent = True
+        return super()._action_send_mail(auto_commit=auto_commit)
```

## odoo/addons/account_banking_sepa_direct_debit/static/description/index.html

```diff
@@ -362,28 +362,28 @@
 <div class="document" id="account-banking-sepa-direct-debit">
 <h1 class="title">Account Banking SEPA Direct Debit</h1>
 
 <!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !! This file is generated by oca-gen-addon-readme !!
 !! changes will be overwritten.                   !!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-!! source digest: sha256:a433755fd2d5cc4c242b073380fd215deb68ea43af0cdef7207c68febe5f8c10
+!! source digest: sha256:4649f6ba9491ff0cbc494f6c1cd03f80b300902d9782a202619be9894a2128a5
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
-<p><a class="reference external image-reference" href="https://odoo-community.org/page/development-status"><img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png" /></a> <a class="reference external image-reference" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html"><img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png" /></a> <a class="reference external image-reference" href="https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit"><img alt="OCA/bank-payment" src="https://img.shields.io/badge/github-OCA%2Fbank--payment-lightgray.png?logo=github" /></a> <a class="reference external image-reference" href="https://translation.odoo-community.org/projects/bank-payment-16-0/bank-payment-16-0-account_banking_sepa_direct_debit"><img alt="Translate me on Weblate" src="https://img.shields.io/badge/weblate-Translate%20me-F47D42.png" /></a> <a class="reference external image-reference" href="https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&amp;target_branch=16.0"><img alt="Try me on Runboat" src="https://img.shields.io/badge/runboat-Try%20me-875A7B.png" /></a></p>
+<p><a class="reference external image-reference" href="https://odoo-community.org/page/development-status"><img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png" /></a> <a class="reference external image-reference" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html"><img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png" /></a> <a class="reference external image-reference" href="https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit"><img alt="OCA/bank-payment" src="https://img.shields.io/badge/github-OCA%2Fbank--payment-lightgray.png?logo=github" /></a> <a class="reference external image-reference" href="https://translation.odoo-community.org/projects/bank-payment-17-0/bank-payment-17-0-account_banking_sepa_direct_debit"><img alt="Translate me on Weblate" src="https://img.shields.io/badge/weblate-Translate%20me-F47D42.png" /></a> <a class="reference external image-reference" href="https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&amp;target_branch=17.0"><img alt="Try me on Runboat" src="https://img.shields.io/badge/runboat-Try%20me-875A7B.png" /></a></p>
 <p>Create SEPA files for Direct Debit</p>
 <p>Module to export direct debit payment orders in SEPA XML file format.</p>
 <p>SEPA PAIN (PAyment INitiation) is the new european standard for
-Customer-to-Bank payment instructions. This module implements SEPA Direct
-Debit (SDD), more specifically PAIN versions 008.001.02, 008.001.03 and
-008.001.04. It is part of the ISO 20022 standard, available on
-<a class="reference external" href="http://www.iso20022.org">http://www.iso20022.org</a>.</p>
-<p>The Implementation Guidelines for SEPA Direct Debit published by the European
-Payments Council (<a class="reference external" href="http://http://www.europeanpaymentscouncil.eu">http://http://www.europeanpaymentscouncil.eu</a>) use PAIN
-version 008.001.02. So if you don’t know which version your bank supports, you
-should try version 008.001.02 first.</p>
+Customer-to-Bank payment instructions. This module implements SEPA
+Direct Debit (SDD), more specifically PAIN versions 008.001.02,
+008.001.03 and 008.001.04. It is part of the ISO 20022 standard,
+available on <a class="reference external" href="http://www.iso20022.org">http://www.iso20022.org</a>.</p>
+<p>The Implementation Guidelines for SEPA Direct Debit published by the
+European Payments Council (<a class="reference external" href="http://http://www.europeanpaymentscouncil.eu">http://http://www.europeanpaymentscouncil.eu</a>)
+use PAIN version 008.001.02. So if you don’t know which version your
+bank supports, you should try version 008.001.02 first.</p>
 <p><strong>Table of contents</strong></p>
 <div class="contents local topic" id="contents">
 <ul class="simple">
 <li><a class="reference internal" href="#installation" id="toc-entry-1">Installation</a></li>
 <li><a class="reference internal" href="#configuration" id="toc-entry-2">Configuration</a></li>
 <li><a class="reference internal" href="#usage" id="toc-entry-3">Usage</a></li>
 <li><a class="reference internal" href="#bug-tracker" id="toc-entry-4">Bug Tracker</a></li>
@@ -405,51 +405,54 @@
 <p>This module is part of the OCA/bank-payment suite.</p>
 </div>
 <div class="section" id="configuration">
 <h1><a class="toc-backref" href="#toc-entry-2">Configuration</a></h1>
 <p>For setting the SEPA creditor identifier:</p>
 <ol class="arabic simple">
 <li>Go to Invoicing/Accounting &gt; Configuration &gt; Settings.</li>
-<li>On the field “SEPA Creditor Identifier” in the section <em>SEPA/PAIN</em>, you can
-fill the corresponding identifier.</li>
+<li>On the field “SEPA Creditor Identifier” in the section <em>SEPA/PAIN</em>,
+you can fill the corresponding identifier.</li>
 </ol>
 <p>If your country requires several identifiers (like Spain), you must:</p>
 <ol class="arabic simple">
 <li>Go to <em>Invoicing/Accounting &gt; Configuration &gt; Settings</em>.</li>
 <li>On the section <em>SEPA/PAIN</em>, check the mark “Multiple identifiers”.</li>
-<li>Now go to <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt; Payment Modes</em>.</li>
+<li>Now go to <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt;
+Payment Modes</em>.</li>
 <li>Create a payment mode for your specific bank.</li>
 <li>Fill the specific identifier on the field “SEPA Creditor Identifier”.</li>
 </ol>
 <p>For defining a payment mode that uses SEPA direct debit:</p>
 <ol class="arabic simple">
-<li>Go to <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt; Payment Modes</em>.</li>
+<li>Go to <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt; Payment
+Modes</em>.</li>
 <li>Create a record.</li>
 <li>Select the Payment Method <em>SEPA Direct Debit for customers</em> (which is
 automatically created upon module installation).</li>
 <li>Check that this payment method uses the proper version of PAIN.</li>
-<li>If not, go <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt; Payment Methods</em>.</li>
+<li>If not, go <em>Invoicing/Accounting &gt; Configuration &gt; Management &gt;
+Payment Methods</em>.</li>
 <li>Locate the “SEPA Direct Debit for customers” record and open it.</li>
 <li>Change the “PAIN version” according your needs.</li>
-<li>If you need to handle several PAIN versions, just duplicate the payment
-method adjusting this field on each for having them.</li>
+<li>If you need to handle several PAIN versions, just duplicate the
+payment method adjusting this field on each for having them.</li>
 </ol>
 </div>
 <div class="section" id="usage">
 <h1><a class="toc-backref" href="#toc-entry-3">Usage</a></h1>
-<p>In the menu <em>Invoicing/Accounting &gt; Customers &gt; Debit Order</em>, create a new debit
-order and select the Payment Mode dedicated to SEPA Direct Debit that
-you created during the configuration step.</p>
+<p>In the menu <em>Invoicing/Accounting &gt; Customers &gt; Debit Order</em>, create a
+new debit order and select the Payment Mode dedicated to SEPA Direct
+Debit that you created during the configuration step.</p>
 </div>
 <div class="section" id="bug-tracker">
 <h1><a class="toc-backref" href="#toc-entry-4">Bug Tracker</a></h1>
 <p>Bugs are tracked on <a class="reference external" href="https://github.com/OCA/bank-payment/issues">GitHub Issues</a>.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-<a class="reference external" href="https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>.</p>
+<a class="reference external" href="https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>.</p>
 <p>Do not contact contributors directly about support or help with technical issues.</p>
 </div>
 <div class="section" id="credits">
 <h1><a class="toc-backref" href="#toc-entry-5">Credits</a></h1>
 <div class="section" id="authors">
 <h2><a class="toc-backref" href="#toc-entry-6">Authors</a></h2>
 <ul class="simple">
@@ -480,14 +483,14 @@
 <div class="section" id="maintainers">
 <h2><a class="toc-backref" href="#toc-entry-8">Maintainers</a></h2>
 <p>This module is maintained by the OCA.</p>
 <a class="reference external image-reference" href="https://odoo-community.org"><img alt="Odoo Community Association" src="https://odoo-community.org/logo.png" /></a>
 <p>OCA, or the Odoo Community Association, is a nonprofit organization whose
 mission is to support the collaborative development of Odoo features and
 promote its widespread use.</p>
-<p>This module is part of the <a class="reference external" href="https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit">OCA/bank-payment</a> project on GitHub.</p>
+<p>This module is part of the <a class="reference external" href="https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit">OCA/bank-payment</a> project on GitHub.</p>
 <p>You are welcome to contribute. To learn how please visit <a class="reference external" href="https://odoo-community.org/page/Contribute">https://odoo-community.org/page/Contribute</a>.</p>
 </div>
 </div>
 </div>
 </body>
 </html>
```

## odoo/addons/account_banking_sepa_direct_debit/tests/test_mandate.py

```diff
@@ -36,17 +36,15 @@
     def test_action_mandate_send(self):
         email_ctx = self.mandate.action_mandate_send().get("context", {})
         mail_template = (
             self.env["mail.template"]
             .browse(email_ctx.get("default_template_id"))
             .copy({"auto_delete": False})
         )
-        self.mandate.with_context(**email_ctx).message_post_with_template(
-            mail_template.id
-        )
+        self.mandate.with_context(**email_ctx).message_post_with_source(mail_template)
         mail_message = self.mandate.message_ids[0]
         self.assertEqual(
             self.mandate.partner_id, mail_message.sudo().mail_ids.recipient_ids
         )
         self.assertEqual(self.mandate.state, "draft")
         self.assertTrue(self.mandate.is_sent)
```

## odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml

### odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml

```diff
@@ -9,23 +9,23 @@
 <odoo>
   <record id="view_mandate_form" model="ir.ui.view">
     <field name="name">sdd.mandate.form</field>
     <field name="model">account.banking.mandate</field>
     <field name="inherit_id" ref="account_banking_mandate.view_mandate_form"/>
     <field name="arch" type="xml">
       <button name="validate" position="before">
-        <button name="action_mandate_send" type="object" string="Send by Email" states="draft" class="btn-primary"/>
+        <button name="action_mandate_send" type="object" string="Send by Email" invisible="state != 'draft'" class="btn-primary"/>
         <button name="print_report" type="object" string="Print"/>
       </button>
       <field name="partner_id" position="after">
-        <field name="scheme" attrs="{'invisible': [('format', '!=', 'sepa')],                                          'required': [('format', '=', 'sepa')]}"/>
-        <field name="recurrent_sequence_type" attrs="{'invisible': ['|', ('type', '=', 'oneoff'), ('format', '!=', 'sepa')],                            'required': [('type', '=', 'recurrent')]}"/>
+        <field name="scheme" invisible="format != 'sepa'" required="format == 'sepa'"/>
+        <field name="recurrent_sequence_type" invisible="type == 'oneoff' or format != 'sepa'" required="type == 'recurrent'"/>
       </field>
       <field name="type" position="attributes">
-        <attribute name="attrs">{'required': [('format', '=', 'sepa')]}</attribute>
+        <attribute name="required">format == 'sepa'</attribute>
       </field>
     </field>
   </record>
   <record id="view_mandate_tree" model="ir.ui.view">
     <field name="name">sdd.mandate.tree</field>
     <field name="model">account.banking.mandate</field>
     <field name="inherit_id" ref="account_banking_mandate.view_mandate_tree"/>
```

## odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml

### odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml

```diff
@@ -1,16 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <record id="view_account_config_settings" model="ir.ui.view">
     <field name="name">sepa_direct_debit.account_config_settings.form</field>
     <field name="model">res.config.settings</field>
     <field name="inherit_id" ref="account_banking_pain_base.view_account_config_settings"/>
     <field name="arch" type="xml">
-      <xpath expr="//div[@id='pain']/div/div/div" position="inside">
-        <div class="row mt16">
-          <label for="sepa_creditor_identifier" class="col-md-3 o_light_label"/>
-          <field name="sepa_creditor_identifier" placeholder="Write the ICS of your company"/>
-        </div>
+      <xpath expr="//block[@id='pain']" position="inside">
+        <setting>
+          <field name="sepa_creditor_identifier"/>
+        </setting>
       </xpath>
     </field>
   </record>
 </odoo>
```

## Comparing `odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.rst` & `odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 For setting the SEPA creditor identifier:
 
-#. Go to Invoicing/Accounting > Configuration > Settings.
-#. On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*, you can
-   fill the corresponding identifier.
+1.  Go to Invoicing/Accounting \> Configuration \> Settings.
+2.  On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*,
+    you can fill the corresponding identifier.
 
 If your country requires several identifiers (like Spain), you must:
 
-#. Go to *Invoicing/Accounting > Configuration > Settings*.
-#. On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
-#. Now go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a payment mode for your specific bank.
-#. Fill the specific identifier on the field "SEPA Creditor Identifier".
+1.  Go to *Invoicing/Accounting \> Configuration \> Settings*.
+2.  On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
+3.  Now go to *Invoicing/Accounting \> Configuration \> Management \>
+    Payment Modes*.
+4.  Create a payment mode for your specific bank.
+5.  Fill the specific identifier on the field "SEPA Creditor
+    Identifier".
 
 For defining a payment mode that uses SEPA direct debit:
 
-#. Go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a record.
-#. Select the Payment Method *SEPA Direct Debit for customers* (which is
-   automatically created upon module installation).
-#. Check that this payment method uses the proper version of PAIN.
-#. If not, go *Invoicing/Accounting > Configuration > Management > Payment Methods*.
-#. Locate the "SEPA Direct Debit for customers" record and open it.
-#. Change the "PAIN version" according your needs.
-#. If you need to handle several PAIN versions, just duplicate the payment
-   method adjusting this field on each for having them.
+1.  Go to *Invoicing/Accounting \> Configuration \> Management \>
+    Payment Modes*.
+2.  Create a record.
+3.  Select the Payment Method *SEPA Direct Debit for customers* (which
+    is automatically created upon module installation).
+4.  Check that this payment method uses the proper version of PAIN.
+5.  If not, go *Invoicing/Accounting \> Configuration \> Management \>
+    Payment Methods*.
+6.  Locate the "SEPA Direct Debit for customers" record and open it.
+7.  Change the "PAIN version" according your needs.
+8.  If you need to handle several PAIN versions, just duplicate the
+    payment method adjusting this field on each for having them.
```

## Comparing `odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.rst` & `odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Create SEPA files for Direct Debit
 
 Module to export direct debit payment orders in SEPA XML file format.
 
 SEPA PAIN (PAyment INitiation) is the new european standard for
-Customer-to-Bank payment instructions. This module implements SEPA Direct
-Debit (SDD), more specifically PAIN versions 008.001.02, 008.001.03 and
-008.001.04. It is part of the ISO 20022 standard, available on
-http://www.iso20022.org.
+Customer-to-Bank payment instructions. This module implements SEPA
+Direct Debit (SDD), more specifically PAIN versions 008.001.02,
+008.001.03 and 008.001.04. It is part of the ISO 20022 standard,
+available on <http://www.iso20022.org>.
 
-The Implementation Guidelines for SEPA Direct Debit published by the European
-Payments Council (http://http://www.europeanpaymentscouncil.eu) use PAIN
-version 008.001.02. So if you don't know which version your bank supports, you
+The Implementation Guidelines for SEPA Direct Debit published by the
+European Payments Council
+(<http://http://www.europeanpaymentscouncil.eu>) use PAIN version
+008.001.02. So if you don't know which version your bank supports, you
 should try version 008.001.02 first.
```

## Comparing `odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/METADATA` & `odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,170 +1,171 @@
 Metadata-Version: 2.1
-Name: odoo-addon-account-banking-sepa-direct-debit
-Version: 16.0.1.2.0.1
+Name: odoo-addon-account_banking_sepa_direct_debit
+Version: 17.0.1.0.0.2
+Requires-Python: >=3.10
+Requires-Dist: odoo-addon-account_banking_mandate>=17.0dev,<17.1dev
+Requires-Dist: odoo-addon-account_banking_pain_base>=17.0dev,<17.1dev
+Requires-Dist: odoo>=17.0a,<17.1dev
 Summary: Create SEPA files for Direct Debit
 Home-page: https://github.com/OCA/bank-payment
+License: AGPL-3
 Author: Akretion, Tecnativa, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
-License: AGPL-3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 16.0
+Classifier: Framework :: Odoo :: 17.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.10
-Requires-Dist: odoo-addon-account-banking-mandate <16.1dev,>=16.0dev
-Requires-Dist: odoo-addon-account-banking-pain-base <16.1dev,>=16.0dev
-Requires-Dist: odoo <16.1dev,>=16.0a
 
 =================================
 Account Banking SEPA Direct Debit
 =================================
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:a433755fd2d5cc4c242b073380fd215deb68ea43af0cdef7207c68febe5f8c10
+   !! source digest: sha256:4649f6ba9491ff0cbc494f6c1cd03f80b300902d9782a202619be9894a2128a5
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fbank--payment-lightgray.png?logo=github
-    :target: https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit
+    :target: https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit
     :alt: OCA/bank-payment
 .. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
-    :target: https://translation.odoo-community.org/projects/bank-payment-16-0/bank-payment-16-0-account_banking_sepa_direct_debit
+    :target: https://translation.odoo-community.org/projects/bank-payment-17-0/bank-payment-17-0-account_banking_sepa_direct_debit
     :alt: Translate me on Weblate
 .. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
-    :target: https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&target_branch=16.0
+    :target: https://runboat.odoo-community.org/builds?repo=OCA/bank-payment&target_branch=17.0
     :alt: Try me on Runboat
 
 |badge1| |badge2| |badge3| |badge4| |badge5|
 
 Create SEPA files for Direct Debit
 
 Module to export direct debit payment orders in SEPA XML file format.
 
 SEPA PAIN (PAyment INitiation) is the new european standard for
-Customer-to-Bank payment instructions. This module implements SEPA Direct
-Debit (SDD), more specifically PAIN versions 008.001.02, 008.001.03 and
-008.001.04. It is part of the ISO 20022 standard, available on
-http://www.iso20022.org.
-
-The Implementation Guidelines for SEPA Direct Debit published by the European
-Payments Council (http://http://www.europeanpaymentscouncil.eu) use PAIN
-version 008.001.02. So if you don't know which version your bank supports, you
-should try version 008.001.02 first.
+Customer-to-Bank payment instructions. This module implements SEPA
+Direct Debit (SDD), more specifically PAIN versions 008.001.02,
+008.001.03 and 008.001.04. It is part of the ISO 20022 standard,
+available on http://www.iso20022.org.
+
+The Implementation Guidelines for SEPA Direct Debit published by the
+European Payments Council (http://http://www.europeanpaymentscouncil.eu)
+use PAIN version 008.001.02. So if you don't know which version your
+bank supports, you should try version 008.001.02 first.
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Installation
 ============
 
 This module depends on :
 
-* account_banking_pain_base
-* account_banking_mandate
+-  account_banking_pain_base
+-  account_banking_mandate
 
 This module is part of the OCA/bank-payment suite.
 
 Configuration
 =============
 
 For setting the SEPA creditor identifier:
 
-#. Go to Invoicing/Accounting > Configuration > Settings.
-#. On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*, you can
-   fill the corresponding identifier.
+1. Go to Invoicing/Accounting > Configuration > Settings.
+2. On the field "SEPA Creditor Identifier" in the section *SEPA/PAIN*,
+   you can fill the corresponding identifier.
 
 If your country requires several identifiers (like Spain), you must:
 
-#. Go to *Invoicing/Accounting > Configuration > Settings*.
-#. On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
-#. Now go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a payment mode for your specific bank.
-#. Fill the specific identifier on the field "SEPA Creditor Identifier".
+1. Go to *Invoicing/Accounting > Configuration > Settings*.
+2. On the section *SEPA/PAIN*, check the mark "Multiple identifiers".
+3. Now go to *Invoicing/Accounting > Configuration > Management >
+   Payment Modes*.
+4. Create a payment mode for your specific bank.
+5. Fill the specific identifier on the field "SEPA Creditor Identifier".
 
 For defining a payment mode that uses SEPA direct debit:
 
-#. Go to *Invoicing/Accounting > Configuration > Management > Payment Modes*.
-#. Create a record.
-#. Select the Payment Method *SEPA Direct Debit for customers* (which is
+1. Go to *Invoicing/Accounting > Configuration > Management > Payment
+   Modes*.
+2. Create a record.
+3. Select the Payment Method *SEPA Direct Debit for customers* (which is
    automatically created upon module installation).
-#. Check that this payment method uses the proper version of PAIN.
-#. If not, go *Invoicing/Accounting > Configuration > Management > Payment Methods*.
-#. Locate the "SEPA Direct Debit for customers" record and open it.
-#. Change the "PAIN version" according your needs.
-#. If you need to handle several PAIN versions, just duplicate the payment
-   method adjusting this field on each for having them.
+4. Check that this payment method uses the proper version of PAIN.
+5. If not, go *Invoicing/Accounting > Configuration > Management >
+   Payment Methods*.
+6. Locate the "SEPA Direct Debit for customers" record and open it.
+7. Change the "PAIN version" according your needs.
+8. If you need to handle several PAIN versions, just duplicate the
+   payment method adjusting this field on each for having them.
 
 Usage
 =====
 
-In the menu *Invoicing/Accounting > Customers > Debit Order*, create a new debit
-order and select the Payment Mode dedicated to SEPA Direct Debit that
-you created during the configuration step.
+In the menu *Invoicing/Accounting > Customers > Debit Order*, create a
+new debit order and select the Payment Mode dedicated to SEPA Direct
+Debit that you created during the configuration step.
 
 Bug Tracker
 ===========
 
 Bugs are tracked on `GitHub Issues <https://github.com/OCA/bank-payment/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-`feedback <https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+`feedback <https://github.com/OCA/bank-payment/issues/new?body=module:%20account_banking_sepa_direct_debit%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
-~~~~~~~
+-------
 
 * Akretion
 * Tecnativa
 
 Contributors
-~~~~~~~~~~~~
+------------
 
-* Alexis de Lattre <alexis.delattre@akretion.com>
-* Stéphane Bidoul <stephane.bidoul@acsone.eu>
-* Alexandre Fayolle
-* Raphaël Valyi
-* Sandy Carter
-* Antonio Espinosa <antonioea@antiun.com>
-* Marçal Isern <marsal.isern@qubiq.es>
-* `Tecnativa <https://www.tecnativa.com>`__:
-
-  * Pedro M. Baeza
-  * Sergio Teruel
-  * Carlos Roca
-  * Carolina Fernandez
-* Manuel Regidor <manuel.regidor@sygel.es>
+-  Alexis de Lattre <alexis.delattre@akretion.com>
+-  Stéphane Bidoul <stephane.bidoul@acsone.eu>
+-  Alexandre Fayolle
+-  Raphaël Valyi
+-  Sandy Carter
+-  Antonio Espinosa <antonioea@antiun.com>
+-  Marçal Isern <marsal.isern@qubiq.es>
+-  `Tecnativa <https://www.tecnativa.com>`__:
+
+   -  Pedro M. Baeza
+   -  Sergio Teruel
+   -  Carlos Roca
+   -  Carolina Fernandez
+
+-  Manuel Regidor <manuel.regidor@sygel.es>
 
 Maintainers
-~~~~~~~~~~~
+-----------
 
 This module is maintained by the OCA.
 
 .. image:: https://odoo-community.org/logo.png
    :alt: Odoo Community Association
    :target: https://odoo-community.org
 
 OCA, or the Odoo Community Association, is a nonprofit organization whose
 mission is to support the collaborative development of Odoo features and
 promote its widespread use.
 
-This module is part of the `OCA/bank-payment <https://github.com/OCA/bank-payment/tree/16.0/account_banking_sepa_direct_debit>`_ project on GitHub.
+This module is part of the `OCA/bank-payment <https://github.com/OCA/bank-payment/tree/17.0/account_banking_sepa_direct_debit>`_ project on GitHub.
 
 You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
-
-
```

## Comparing `odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/RECORD` & `odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-odoo/addons/account_banking_sepa_direct_debit/README.rst,sha256=YMiro86nU9vWA0M92hC64TJ79FHxyWyuj16frt3hO-I,5623
+odoo/addons/account_banking_sepa_direct_debit/README.rst,sha256=LFTsg8u9-MLI7TkJqZpAb-xos0YuEu_BHQsDoTty64g,5652
 odoo/addons/account_banking_sepa_direct_debit/__init__.py,sha256=0XNpxETgFdVxFDEw03O8oL3NtTSk3we-HEZW2sPKzIU,43
-odoo/addons/account_banking_sepa_direct_debit/__manifest__.py,sha256=IYTJog3MPsyOeMvRzTxKJ5S49n-eQ0Od45dL4VtbJaI,1295
+odoo/addons/account_banking_sepa_direct_debit/__manifest__.py,sha256=N_8-5xGmvN8eeB6_ZfDtNLoUMkk5NEeOtMtLJju_srM,1295
 odoo/addons/account_banking_sepa_direct_debit/data/account_payment_method.xml,sha256=DY4blWdIakpnp4WYoKn669UwkBOV4F1eFh2uBzzkKIk,544
-odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml,sha256=Cbey9LI-QHa0Q_lSIpX_2BBqVsr-67SBhZSMaaPNWMQ,1755
+odoo/addons/account_banking_sepa_direct_debit/data/mail_template_data.xml,sha256=n97m4NbVMUqko20TI0lmn0SVAjnVvPj-V5sjPyYKoN8,1698
 odoo/addons/account_banking_sepa_direct_debit/data/mandate_expire_cron.xml,sha256=yULX103bQd44aAt5cEvUAJanAWE7PpMKL6Sf66_U1Fg,799
 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.02.xsd,sha256=M-jzRbEQrsB3cAjsKZ1rZTQdZSZaOjF_7qEGT0Gp-8Y,47698
 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.03.xsd,sha256=srckHuFs0AdaweLyFc76YvIRnSulzFzorJptLtLomHI,49754
 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.001.04.xsd,sha256=_w38PbXeiCoWxOonwf3kv2RlW0XmCwvjfxU5_sn-pAk,48847
 odoo/addons/account_banking_sepa_direct_debit/data/pain.008.003.02.xsd,sha256=agvk4SlSBniPxb8hZrNyGKH5Otp296jS40ei7eBBvFE,25834
 odoo/addons/account_banking_sepa_direct_debit/data/report_paperformat.xml,sha256=1tlw2QxKp-YkKcxyPkqvKxrHDYkio04y7BwRjCoqoZw,750
 odoo/addons/account_banking_sepa_direct_debit/demo/sepa_direct_debit_demo.xml,sha256=CbbOiCqiJt-iFi5cfb43fQOR-bjwWxmlM1WPMZnzm3s,1986
-odoo/addons/account_banking_sepa_direct_debit/i18n/account_banking_sepa_direct_debit.pot,sha256=R2uhG-iLQt2MfzM8XDe4TbzoqsWRPPMyq91pLymy13M,20807
+odoo/addons/account_banking_sepa_direct_debit/i18n/account_banking_sepa_direct_debit.pot,sha256=Xrun_4quQA41T7XHzIv1v4KaMt8ZjwKoPgew9GrRW80,20292
 odoo/addons/account_banking_sepa_direct_debit/i18n/de.po,sha256=62ibEP_4CmLx0tWPzc6oRn8a-mctFR7oWlz4oOIZAts,22079
 odoo/addons/account_banking_sepa_direct_debit/i18n/es.po,sha256=x_Oa08p82Dfc496hPGEo-edazI5Tsk2b0yFJ65_Ugek,28891
 odoo/addons/account_banking_sepa_direct_debit/i18n/es_AR.po,sha256=GMJs_TK9xJ-NB36DZhz0VIbHwcxDtJG3TqqmPtYitJc,26780
 odoo/addons/account_banking_sepa_direct_debit/i18n/fr.po,sha256=MYcqtWNoVp3MF8boZFfFNZ7FsMKyskmEttzbi5F4UF0,26781
 odoo/addons/account_banking_sepa_direct_debit/i18n/hr.po,sha256=aJPlhveOI4MPJbbHZ8yPxcigdLcm4yxew_Moqza6Rbw,21286
 odoo/addons/account_banking_sepa_direct_debit/i18n/it.po,sha256=6euC6NkmoERNM33QXBGjY3OVFm2SbiQjUe9OfDJoi6g,21535
 odoo/addons/account_banking_sepa_direct_debit/i18n/nb_NO.po,sha256=Vu2AlzCd9OAuGzcbkkkK_WKgCBTpPro2_0KFHIQ6V6o,21229
 odoo/addons/account_banking_sepa_direct_debit/i18n/nl.po,sha256=ab5zearrs2V_2B44HI9KJvVgcVaJ1-m7lOjGfqYpd_Y,26007
 odoo/addons/account_banking_sepa_direct_debit/i18n/pt_BR.po,sha256=Riqh-InEfOZcR6tr244BlN11UWmOpcwDwKtLRu51gQQ,21489
 odoo/addons/account_banking_sepa_direct_debit/i18n/sl.po,sha256=VQUaT53vul2OkXoUSCN3QlD35yirkyXU7cSCvi7fvNI,24414
-odoo/addons/account_banking_sepa_direct_debit/migrations/16.0.1.0.2/post-migration.py,sha256=tzfaIEUxiAfIEVaHZmovSC1c1359v09FMYz8c2x_TE0,401
 odoo/addons/account_banking_sepa_direct_debit/models/__init__.py,sha256=3SbJd9gsTwMzXhP38VxRs8Y5kbWA0uBE-pOzwc10W_Q,242
-odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py,sha256=kuBe-r65Cn1lyH_DH7_lk40POs5Dv3XEArWykfi-1Mc,5555
-odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py,sha256=bVsefObzFQ31MAlzQyMaHr48iD2zszXal4faYXJh5fE,2383
+odoo/addons/account_banking_sepa_direct_debit/models/account_banking_mandate.py,sha256=dxxkauh2SRESvLbeDJ92PVYHIoDPhbkzSX7XRwqYDbs,5592
+odoo/addons/account_banking_sepa_direct_debit/models/account_payment_line.py,sha256=f_UY9LQvc6f7L3Vi1YRXOKkQKNF8FS6jikwfqXRhJJk,2389
 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_method.py,sha256=AdZKhwMBtQE3nGqh7suoULb70NGRrSazhVvLa7X-a20,1423
 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_mode.py,sha256=_6HmAdhwW4EaSSGzMKCHTgTZnUL3L8e8ezvwad-mAFk,1207
 odoo/addons/account_banking_sepa_direct_debit/models/account_payment_order.py,sha256=c5mMWuQKBJLKhkohtyUrd4vS4EBODKYx7iGiLZtsUCM,13488
-odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py,sha256=6kVhFNRqIJ9gdiKUsCqi4P_7AOS596c0yoFHIsLyV10,551
+odoo/addons/account_banking_sepa_direct_debit/models/mail_compose_message.py,sha256=W0epCy19a0qTrsQbPN-l-xCJ3a66ngs8MrZYxwrhKeE,568
 odoo/addons/account_banking_sepa_direct_debit/models/res_company.py,sha256=OWmXJg2tmwPdKxkuF0HSlVpRAk1grbF2ZwKO45gmNhU,1172
-odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.rst,sha256=3XCJb4HGrTiSmG4GARMCDdPlhc2OA6zR1QtMpyrn7OY,1307
-odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.rst,sha256=7XuL2bzeyuqJjEm6EkkiUB85Oey6n7FlJcQxNGs8I2A,396
-odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.rst,sha256=VeA_476z5yMo2AATnKBVECXkpDVxeZXw43gAQWo-qeo,673
-odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.rst,sha256=42QFe44NJ1XTo-gxQC5UuMsqcE_HRKZ29er_ifstPKo,132
-odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.rst,sha256=PKz_viLs-7ZioiE6irDKtU8cwdqQcknxqn-YFS6BoIc,194
+odoo/addons/account_banking_sepa_direct_debit/readme/CONFIGURE.md,sha256=iQQzZYSoGudo2pZb7uwdpPA3GzGyFRA0lMFxru5JrX8,1354
+odoo/addons/account_banking_sepa_direct_debit/readme/CONTRIBUTORS.md,sha256=ruUnOGRxEVwGMdHRa6wgMTV7ndQsXzW4eBxI6mKcgfI,412
+odoo/addons/account_banking_sepa_direct_debit/readme/DESCRIPTION.md,sha256=pNzR-Mq0ddImQgdol1obTAP3aJgfpai-6se1H1gGX3A,677
+odoo/addons/account_banking_sepa_direct_debit/readme/INSTALL.md,sha256=qMaZ5AXatfD67eTo71TcAx_mdPwaLImGRWi06_oE1bI,132
+odoo/addons/account_banking_sepa_direct_debit/readme/USAGE.md,sha256=CTRVNjFgb0rPbLVuiJFgDDCpAJcDg8FwG5deb-Uh-rw,196
 odoo/addons/account_banking_sepa_direct_debit/reports/sepa_direct_debit_mandate.xml,sha256=XzPudgVhxm9CE3ob-r0bi4eWl38wjH_yMKA8xgMQEEE,989
 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.png,sha256=FlfkHVemKykdTb4lnXu3i3WVBJbnx2E0Nx-YefmYfm0,7840
 odoo/addons/account_banking_sepa_direct_debit/static/description/icon.svg,sha256=3FwnhOblAA2KZZgNW7F_l90xAshSE5jvSbBL6GEUp9w,23879
-odoo/addons/account_banking_sepa_direct_debit/static/description/index.html,sha256=CkTfSxBMVAlIKGf1rYBEc48lw3N9IZSWvsJE_vHVRmI,16408
+odoo/addons/account_banking_sepa_direct_debit/static/description/index.html,sha256=hTPlXRizfN5pVgcIx0SVvXpJzL5LWFAW1IjDVz-PKXs,16408
 odoo/addons/account_banking_sepa_direct_debit/static/src/css/report.css,sha256=BdO3lXcJ2tUsUbDLOdbI0hMjsEa9I43L8ZDIlk2S4o0,518
 odoo/addons/account_banking_sepa_direct_debit/tests/__init__.py,sha256=70uQqx4Z2wRaH1bjObBtPOMkqrgF8dMJkGY784hnGBQ,50
-odoo/addons/account_banking_sepa_direct_debit/tests/test_mandate.py,sha256=WaiVEeZR32WHw16o4VaJjiEiTPvX4PQN2fpgOhE0GnU,2474
+odoo/addons/account_banking_sepa_direct_debit/tests/test_mandate.py,sha256=L3bUlQeetMdz2zD-LmLFtp7qmEeQT6H1OdqpwIbjZVQ,2447
 odoo/addons/account_banking_sepa_direct_debit/tests/test_sdd.py,sha256=sOFsQaaOOQ-ZqfijXFoknOcgc9MRUEo0rWAl6xi2xf4,14342
-odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml,sha256=SvwBzwDMSBo5b0R2tvQMlwOuYLoweVTSvtbGkorFsc0,4608
+odoo/addons/account_banking_sepa_direct_debit/views/account_banking_mandate_view.xml,sha256=oBv7dU4Aa-36_L7jKMbECN8WzwY90tzWwWBRglRJmWs,4463
 odoo/addons/account_banking_sepa_direct_debit/views/account_payment_mode.xml,sha256=cKbgetVsmfIqzAQoVW8QI9BzxxDmJ_HNipIVUxc4FUY,890
 odoo/addons/account_banking_sepa_direct_debit/views/report_sepa_direct_debit_mandate.xml,sha256=XQ4uBvjVJRC_kn3UCrIFfvXHc4irbVdf4Y39R0kMRYM,20588
-odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml,sha256=mLIyINje8T22koDRzTSzwyyFX1p3NqHyX87a_O6oOHM,959
+odoo/addons/account_banking_sepa_direct_debit/views/res_config_settings.xml,sha256=c9MqRHJ5ybE83perbk8bDZHRWumtfWmyU0jXsGjsuEI,668
 odoo/addons/account_banking_sepa_direct_debit/wizards/__init__.py,sha256=zn8FjADxYHOSCCGGXqyQZL8kz_8gruN-Y3oSjlWHQ4I,34
 odoo/addons/account_banking_sepa_direct_debit/wizards/res_config_settings.py,sha256=KloYafjy12hUUDxvQnvdKmXkASxFXZvxdOAZs24ofnY,356
-odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/METADATA,sha256=Yz38hyyhccUqUO-Hy241KnqwYqxDKwVzzPQVEmzQPB4,6337
-odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_account_banking_sepa_direct_debit-16.0.1.2.0.1.dist-info/RECORD,,
+odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/METADATA,sha256=sWrydPAVrc2ZjYZ8k6Q4D-XjXnpJ7AwV8mgCXUm8oRM,6343
+odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
+odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
+odoo_addon_account_banking_sepa_direct_debit-17.0.1.0.0.2.dist-info/RECORD,,
```

