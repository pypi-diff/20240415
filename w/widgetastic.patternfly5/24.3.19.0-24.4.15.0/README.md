# Comparing `tmp/widgetastic.patternfly5-24.3.19.0-py3-none-any.whl.zip` & `tmp/widgetastic.patternfly5-24.4.15.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 51988 bytes, number of entries: 44
+Zip file size: 52086 bytes, number of entries: 44
 -rw-r--r--  2.0 unx     4792 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/__init__.py
 -rw-r--r--  2.0 unx     4299 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/ouia.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/charts/__init__.py
 -rw-r--r--  2.0 unx     3737 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/charts/bullet_chart.py
 -rw-r--r--  2.0 unx     2693 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/charts/donut_chart.py
 -rw-r--r--  2.0 unx     2983 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/charts/legend.py
 -rw-r--r--  2.0 unx     3612 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/charts/line_chart.py
@@ -34,13 +34,13 @@
 -rw-r--r--  2.0 unx     2099 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/forms/radio.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/__init__.py
 -rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/context_selector.py
 -rw-r--r--  2.0 unx     9478 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/dropdown.py
 -rw-r--r--  2.0 unx     7949 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/menu.py
 -rw-r--r--  2.0 unx     1029 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/menu_toggle.py
 -rw-r--r--  2.0 unx     1353 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/options_menu.py
--rw-r--r--  2.0 unx     6243 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/select.py
-?rw-r--r--  2.0 unx     6805 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.3.19.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.3.19.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      576 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.3.19.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     4542 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.3.19.0.dist-info/RECORD
-44 files, 147946 bytes uncompressed, 44412 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx     6537 b- defN 20-Feb-02 00:00 widgetastic_patternfly5/components/menus/select.py
+?rw-r--r--  2.0 unx     6857 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.4.15.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.4.15.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      576 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.4.15.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     4542 b- defN 20-Feb-02 00:00 widgetastic.patternfly5-24.4.15.0.dist-info/RECORD
+44 files, 148292 bytes uncompressed, 44510 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -114,20 +114,20 @@
 
 Filename: widgetastic_patternfly5/components/menus/options_menu.py
 Comment: 
 
 Filename: widgetastic_patternfly5/components/menus/select.py
 Comment: 
 
-Filename: widgetastic.patternfly5-24.3.19.0.dist-info/METADATA
+Filename: widgetastic.patternfly5-24.4.15.0.dist-info/METADATA
 Comment: 
 
-Filename: widgetastic.patternfly5-24.3.19.0.dist-info/WHEEL
+Filename: widgetastic.patternfly5-24.4.15.0.dist-info/WHEEL
 Comment: 
 
-Filename: widgetastic.patternfly5-24.3.19.0.dist-info/licenses/LICENSE
+Filename: widgetastic.patternfly5-24.4.15.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: widgetastic.patternfly5-24.3.19.0.dist-info/RECORD
+Filename: widgetastic.patternfly5-24.4.15.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## widgetastic_patternfly5/components/menus/select.py

```diff
@@ -62,15 +62,18 @@
                 "The following items are available and enabled: {}".format(
                     item, repr(self), self.enabled_items
                 )
             )
 
     def fill(self, value):
         """Fills a Select with a value."""
+        if self.read() == value:
+            return False
         self.item_select(value)
+        return True
 
     def read(self):
         """Returns a string of the text of the selected option."""
         return self.browser.text(self.BUTTON_LOCATOR)
 
 
 class Select(BaseSelect, Dropdown):
@@ -132,22 +135,28 @@
     def fill(self, items):
         """Fills a Checkbox with all items.
         Example dictionary: {"foo": True, "bar": False, "baz": True}
 
         Args:
             items: A dictionary containing what items to select (True) or deselect (False)
         """
+        current_values = self.read()
+        has_changed = False
         try:
             for item, value in items.items():
+                if value == current_values.get(item, None):
+                    continue
                 if value:
                     self.item_select(item, close=False)
                 else:
                     self.item_deselect(item, close=False)
+                has_changed = True
         finally:
             self.close()
+        return has_changed
 
     def read(self):
         """Returns a dictionary containing the selected status as bools."""
         selected = {}
         with self.opened():
             for el in self.browser.elements(self.ITEMS_LOCATOR):
                 item = self.browser.text(el)
```

## Comparing `widgetastic.patternfly5-24.3.19.0.dist-info/METADATA` & `widgetastic.patternfly5-24.4.15.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: widgetastic.patternfly5
-Version: 24.3.19.0
+Version: 24.4.15.0
 Summary: Patternfly5 widget library for Widgetastic.
 Project-URL: repository, https://github.com/RedHatQE/widgetastic.patternfly5
 Maintainer-email: Nikhil Dhandre <ndhandre@redhat.com>, Egor Shamardin <eshamard@redhat.com>, Mike Shriver <mshriver@redhat.com>
 License: Copyright 2023 Red Hat, Inc. and/or its affiliates
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -30,14 +30,15 @@
 Requires-Python: >=3.8
 Requires-Dist: widgetastic-core>=1.0.6
 Provides-Extra: dev
 Requires-Dist: codecov; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-rerunfailures; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Description-Content-Type: text/markdown
 
 <h1 align="center"> widgetastic.patternfly5 </h1>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: widgetastic.patternfly5 Version: 24.3.19.0 Summary:
+Metadata-Version: 2.3 Name: widgetastic.patternfly5 Version: 24.4.15.0 Summary:
 Patternfly5 widget library for Widgetastic. Project-URL: repository, https://
 github.com/RedHatQE/widgetastic.patternfly5 Maintainer-email: Nikhil Dhandre
 redhat.com>, Egor Shamardin
 redhat.com>, Mike Shriver
 redhat.com> License: Copyright 2023 Red Hat, Inc. and/or its affiliates
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License. You may obtain a copy of the
@@ -16,17 +16,17 @@
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
 :: Software Development :: Quality Assurance Classifier: Topic :: Software
 Development :: Testing Requires-Python: >=3.8 Requires-Dist: widgetastic-
 core>=1.0.6 Provides-Extra: dev Requires-Dist: codecov; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: pytest-xdist; extra ==
-'dev' Provides-Extra: doc Requires-Dist: sphinx; extra == 'doc' Description-
-Content-Type: text/markdown
+Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: pytest-rerunfailures;
+extra == 'dev' Requires-Dist: pytest-xdist; extra == 'dev' Provides-Extra: doc
+Requires-Dist: sphinx; extra == 'doc' Description-Content-Type: text/markdown
                      ************ wwiiddggeettaassttiicc..ppaatttteerrnnffllyy55 ************
       _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_R_e_d_H_a_t_Q_E_/
 _w_i_d_g_e_t_a_s_t_i_c_._p_a_t_t_e_r_n_f_l_y_5_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_c_W_u_T_X_n_i_I_P_m_]_[_g_i_t_h_u_b_ _a_c_t_i_o_n_s_]_[_C_o_d_e
                            _s_t_y_l_e_:_ _b_l_a_c_k_]_[_p_r_e_:_ _b_l_a_c_k_]
 This library offers Widgetastic Widgets for [PatternFly v5](https://
 www.patternfly.org/), serving as an extended itteration of
 [widgetastic.patternfly4](https://github.com/RedHatQE/widgetastic.patternfly4).
```

## Comparing `widgetastic.patternfly5-24.3.19.0.dist-info/licenses/LICENSE` & `widgetastic.patternfly5-24.4.15.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `widgetastic.patternfly5-24.3.19.0.dist-info/RECORD` & `widgetastic.patternfly5-24.4.15.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 widgetastic_patternfly5/components/forms/radio.py,sha256=9I7P9hsKRojGvTZtSsqVTI_4ek_qIYKEdamSdUfxsMA,2099
 widgetastic_patternfly5/components/menus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 widgetastic_patternfly5/components/menus/context_selector.py,sha256=uMumIPxuY3f_r5o9JrMibiPQgpFjRaFQwwo08_rVeMQ,1150
 widgetastic_patternfly5/components/menus/dropdown.py,sha256=5nCz0HRG4VcrzD1NFC9Hj1m2T4yHihfNf2MNQWnBOEk,9478
 widgetastic_patternfly5/components/menus/menu.py,sha256=0cUb5V1y3RgRpdAB8DlPIL9OOl7IxBC8A1xjcZgfLBA,7949
 widgetastic_patternfly5/components/menus/menu_toggle.py,sha256=PBwNvg6E2RPdCG6ALBUqyTZxCwThJgk5S-9ghTiZ9hM,1029
 widgetastic_patternfly5/components/menus/options_menu.py,sha256=43D0_JHeY-kPORQi54NL9OVmcMyAolVnI4dqHpo5omY,1353
-widgetastic_patternfly5/components/menus/select.py,sha256=xT3Hdoxp9OiH-Vy24m1AMqDXZxvsyfMpUeLPX3l2uOM,6243
-widgetastic.patternfly5-24.3.19.0.dist-info/METADATA,sha256=xMWGocg4rrt9JPwS4go__edPrIwkmtOAo3szSYVt5E8,6805
-widgetastic.patternfly5-24.3.19.0.dist-info/WHEEL,sha256=bq9SyP5NxIRA9EpQgMCd-9RmPHWvbH-4lTDGwxgIR64,87
-widgetastic.patternfly5-24.3.19.0.dist-info/licenses/LICENSE,sha256=nDhhj8jp0XsTdmvWpTWFpOKVn0LPXPb6ecA9zFF3Exk,576
-widgetastic.patternfly5-24.3.19.0.dist-info/RECORD,,
+widgetastic_patternfly5/components/menus/select.py,sha256=D4M5XUsiQVye97dClWra1c6rD0M-HM4wVJ2VdVFM0F0,6537
+widgetastic.patternfly5-24.4.15.0.dist-info/METADATA,sha256=lxzOzvnP6ACqHBqvWNCJ74O3nEAesZJlyiQw5KvtEK0,6857
+widgetastic.patternfly5-24.4.15.0.dist-info/WHEEL,sha256=xl5aZkiJYVTjhVaiADvIe6UeUVylGNomrxKZ0Zda1CE,87
+widgetastic.patternfly5-24.4.15.0.dist-info/licenses/LICENSE,sha256=nDhhj8jp0XsTdmvWpTWFpOKVn0LPXPb6ecA9zFF3Exk,576
+widgetastic.patternfly5-24.4.15.0.dist-info/RECORD,,
```

