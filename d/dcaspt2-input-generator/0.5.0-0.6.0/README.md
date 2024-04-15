# Comparing `tmp/dcaspt2_input_generator-0.5.0.tar.gz` & `tmp/dcaspt2_input_generator-0.6.0.tar.gz`

## Comparing `dcaspt2_input_generator-0.5.0.tar` & `dcaspt2_input_generator-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.pylintrc
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.github/release-drafter.yml
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.github/scripts/versionup.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.github/workflows/release-pr.yml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.vscode/extensions.json
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/data/.gitignore
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/__main__.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/dcaspt2_input_generator.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/color_settings.py
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/data.py
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/main_window.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/menu_bar.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/multi_process_settings.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/table_summary.py
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/table_widget.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/color_settings_controller.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/multi_process_controller.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/save_default_settings_controller.py
--rw-r--r--   0        0        0     8251 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/widget_controller.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/args.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/dir_info.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/settings.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/utils.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/LICENSE
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/README.md
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.pylintrc
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.vscode/extensions.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/data/.gitignore
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/__main__.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/dcaspt2_input_generator.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/color_settings.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/data.py
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/main_window.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/menu_bar.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/multi_process_settings.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/table_summary.py
+-rw-r--r--   0        0        0    12248 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/table_widget.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/color_settings_controller.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/multi_process_controller.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/save_default_settings_controller.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/widget_controller.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/args.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/dir_info.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/settings.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/utils.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/LICENSE
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/README.md
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.0/PKG-INFO
```

### Comparing `dcaspt2_input_generator-0.5.0/.pylintrc` & `dcaspt2_input_generator-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/.github/release-drafter.yml` & `dcaspt2_input_generator-0.6.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/.github/scripts/versionup.py` & `dcaspt2_input_generator-0.6.0/.github/scripts/versionup.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/.github/workflows/publish.yml` & `dcaspt2_input_generator-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/.github/workflows/release-pr.yml` & `dcaspt2_input_generator-0.6.0/.github/workflows/release-pr.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/dcaspt2_input_generator.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/dcaspt2_input_generator.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/color_settings.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/color_settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/main_window.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 
     def save_input(self):
         def add_nelec(cur_nelec: int, rem_electrons: int) -> int:
             if rem_electrons > 0:
                 cur_nelec += min(rem_electrons, 2)
             return cur_nelec
 
-        output = ""
         inact = 0
         act = 0
         sec = 0
         elec = 0
         idx_caspt2 = 0
         ras1_list = []
         ras2_list = []
@@ -136,22 +135,24 @@
                 is_cas = False
             elif color == colors.secondary.color:
                 debug_print(f"{idx}, secondary")
                 sec += 2
             rem_electrons -= 2
         nroot = max(10, self.table_summary.user_input.selectroot_number.get_value())
 
-        output += f"ninact\n{inact}\n"
+        output = f"ninact\n{inact}\n"
         output += f"nact\n{act}\n"
         output += f"nelec\n{elec}\n"
         output += f"nsec\n{sec}\n"
         output += f"nroot\n{nroot}\n"
         output += f"selectroot\n{self.table_summary.user_input.selectroot_number.get_value()}\n"
         output += f"totsym\n{self.table_summary.user_input.totsym_number.get_value()}\n"
         output += f"diracver\n{self.table_summary.user_input.dirac_ver_number.get_value()}\n"
+        if table_data.header_info.moltra_scheme is not None:
+            output += f"scheme\n{table_data.header_info.moltra_scheme}\n"  # Explicitly set MOLTRA scheme.
 
         if not is_cas:
             ras1_str = create_ras_str(sorted(ras1_list))
             ras2_str = create_ras_str(sorted(ras2_list))
             ras3_str = create_ras_str(sorted(ras3_list))
             output += (
                 ""
```

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/menu_bar.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/menu_bar.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/multi_process_settings.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/multi_process_settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/components/table_summary.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/components/table_summary.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/color_settings_controller.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/color_settings_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/multi_process_controller.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/multi_process_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/save_default_settings_controller.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/save_default_settings_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/controller/widget_controller.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/controller/widget_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,27 +53,28 @@
             elif rem_electrons >= 0:
                 act += 2
             else:
                 sec += 2
             rem_electrons -= 2
 
         # Create standard IVO input
-        output = ""
-        output += "ninact\n0\n"
+        output = "ninact\n0\n"
         output += f"nact\n{act}\n"
         output += f"nsec\n{sec}\n"
         output += f"nelec\n{act}\n"
         if is_gerade_ungerade:
             output += f"noccg\n{nocc['E1g']}\nnoccu\n{nocc['E1u']}\n"
             output += "" if sum(nvcut.values()) == 0 else f"nvcutg\n{nvcut['E1g']}\nnvcutu\n{nvcut['E1u']}\n"
         else:
             output += f"nocc\n{nocc['E1']}\n"
             output += "" if sum(nvcut.values()) == 0 else f"nvcut\n{nvcut['E1']}\n"
         output += f"totsym\n{self.table_summary.user_input.totsym_number.get_value()}\n"
         output += f"diracver\n{self.table_summary.user_input.dirac_ver_number.get_value()}\n"
+        if table_data.header_info.moltra_scheme is not None:
+            output += f"scheme\n{table_data.header_info.moltra_scheme}\n"  # Explicitly set MOLTRA scheme.
         output += "end\n"
 
         # Save standard IVO input (replace active.ivo.inp)
         with open(dir_info.ivo_input_path, "w") as f:
             f.write(output)
 
     def onUserInputChanged(self):
```

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/args.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/args.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/dir_info.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/dir_info.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/settings.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/src/dcaspt2_input_generator/utils/utils.py` & `dcaspt2_input_generator-0.6.0/src/dcaspt2_input_generator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/.gitignore` & `dcaspt2_input_generator-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/LICENSE` & `dcaspt2_input_generator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.5.0/pyproject.toml` & `dcaspt2_input_generator-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["sum_dirac_dfcoef>=4.4.0", "PySide6", "qtpy"]
+dependencies = ["sum_dirac_dfcoef>=5.0.0", "PySide6", "qtpy"]
 
 [project.optional-dependencies]
 dev = ["coverage[toml]>=6.5", "pytest", "black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
 test = ["coverage[toml]>=6.5", "pytest"]
 
 [project.urls]
 Documentation = "https://github.com/RQC-HU/dcaspt2_input_generator#readme"
```

### Comparing `dcaspt2_input_generator-0.5.0/PKG-INFO` & `dcaspt2_input_generator-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dcaspt2_input_generator
-Version: 0.5.0
+Version: 0.6.0
 Summary: This is a GUI tool for supporting the generation of input files for DIRAC_CASPT2 calculation.
 Project-URL: Documentation, https://github.com/RQC-HU/dcaspt2_input_generator#readme
 Project-URL: Issues, https://github.com/RQC-HU/dcaspt2_input_generator/issues
 Project-URL: Source, https://github.com/RQC-HU/dcaspt2_input_generator
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: pyside6
 Requires-Dist: qtpy
-Requires-Dist: sum-dirac-dfcoef>=4.4.0
+Requires-Dist: sum-dirac-dfcoef>=5.0.0
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
 Requires-Dist: coverage[toml]>=6.5; extra == 'dev'
 Requires-Dist: mypy>=1.0.0; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: ruff>=0.0.243; extra == 'dev'
 Provides-Extra: test
```

