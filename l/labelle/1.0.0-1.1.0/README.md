# Comparing `tmp/labelle-1.0.0.tar.gz` & `tmp/labelle-1.1.0.tar.gz`

## Comparing `labelle-1.0.0.tar` & `labelle-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,82 @@
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 labelle-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.0.0/labelle.ini
--rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.0.0/labelle.png
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 labelle-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.0.0/doc/Labelle_example_1.png
--rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.0.0/doc/Labelle_example_2.png
--rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.0.0/doc/Labelle_example_3.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.0.0/src/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/_version.py
--rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/barcode_writer.py
--rwxr-xr-x   0        0        0     7846 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/command_line.py
--rwxr-xr-x   0        0        0     2674 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/constants.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/detect.py
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/dymo_print_engines.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/font_config.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/gui.py
--rwxr-xr-x   0        0        0     7607 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/labeler.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/metadata.py
--rw-r--r--   0        0        0    15286 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/q_dymo_label_widgets.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/q_dymo_labels_list.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/unicode_blocks.py
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/utils.py
--rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/Carlito-Bold.ttf
--rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/Carlito-Italic.ttf
--rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/Carlito-Regular.ttf
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/fonts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/barcode_icon.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/barcode_text_icon.png
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/img_icon.png
--rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/logo_small.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/qr_icon.png
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.0.0/src/labelle/resources/icons/txt_icon.png
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 labelle-1.0.0/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.0.0/LICENSE
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 labelle-1.0.0/README.md
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 labelle-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 labelle-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 labelle-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.1.0/labelle.ini
+-rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.1.0/labelle.png
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 labelle-1.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 labelle-1.1.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 labelle-1.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 labelle-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_1.png
+-rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_2.png
+-rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_3.png
+-rwxr-xr-x   0        0        0      117 2020-02-02 00:00:00.000000 labelle-1.1.0/scripts/gui_dev.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/metadata.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib.pyi
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QHULL
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_STIX
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_YORICK
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/font_manager.py
+-rwxr-xr-x   0        0        0    10454 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/cli/cli.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/common.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/gui.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/q_dymo_label_widgets.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/q_dymo_labels_list.py
+-rwxr-xr-x   0        0        0     4017 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/barcode_writer.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/config_file.py
+-rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/constants.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/detect.py
+-rwxr-xr-x   0        0        0    11650 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/dymo_labeler.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/font_config.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/logger.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/unicode_blocks.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/utils.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/__init__.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/barcode.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/barcode_with_text.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/empty.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/horizontally_combined.py
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/margins.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/picture.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/print_payload.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/print_preview.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/qr.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/render_context.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/render_engine.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/test_pattern.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/text.py
+-rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Bold.ttf
+-rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Italic.ttf
+-rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Regular.ttf
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/barcode_icon.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/barcode_text_icon.png
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/img_icon.png
+-rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/logo_small.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/qr_icon.png
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/txt_icon.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/README.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/vendor.txt
+-rw-r--r--   0        0        0    47308 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/patches/matplotlib.patch
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 labelle-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 labelle-1.1.0/README.md
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 labelle-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 labelle-1.1.0/PKG-INFO
```

### Comparing `labelle-1.0.0/labelle.png` & `labelle-1.1.0/labelle.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/.github/workflows/pypi-publish.yml` & `labelle-1.1.0/.github/workflows/pypi-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Build
       run: |
         python -m pip install --upgrade pip build twine
         python -m build
     - name: Test wheels
```

### Comparing `labelle-1.0.0/.github/workflows/tests.yml` & `labelle-1.1.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
```

### Comparing `labelle-1.0.0/doc/Labelle_example_1.png` & `labelle-1.1.0/doc/Labelle_example_1.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/doc/Labelle_example_2.png` & `labelle-1.1.0/doc/Labelle_example_2.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/doc/Labelle_example_3.png` & `labelle-1.1.0/doc/Labelle_example_3.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/barcode_writer.py` & `labelle-1.1.0/src/labelle/lib/barcode_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,31 +29,30 @@
 
     def calculate_size(self, modules_per_line, number_of_lines, dpi=25.4):
         width = 2 * self.quiet_zone + modules_per_line * self.module_width
         height = self.vertical_margin * 2 + self.module_height * number_of_lines
         return int(mm2px(width, dpi)), int(mm2px(height, dpi))
 
     def render(self, code):
-        """Renders the barcode to whatever the inheriting writer provides,
-        using the registered callbacks.
+        """Render the barcode.
+
+        Uses whichever inheriting writer is provided via the registered callbacks.
 
         :parameters:
             code : List
                 List of strings matching the writer spec
                 (only contain 0 or 1).
         """
         if self._callbacks["initialize"] is not None:
             self._callbacks["initialize"](code)
         ypos = self.vertical_margin
         for cc, line in enumerate(code):
-            """
-            Pack line to list give better gfx result, otherwise in can
-            result in aliasing gaps
-            '11010111' -> [2, -1, 1, -1, 3]
-            """
+            # Pack line to list give better gfx result, otherwise in can
+            # result in aliasing gaps
+            # '11010111' -> [2, -1, 1, -1, 3]
             line += " "
             c = 1
             mlist = []
             for i in range(0, len(line) - 1):
                 if line[i] == line[i + 1]:
                     c += 1
                 else:
@@ -86,23 +85,27 @@
 
     def _init(self, code):
         size = self.calculate_size(len(code[0]), len(code), self.dpi)
         self._image = Image.new("1", size, self.background)
         self._draw = ImageDraw.Draw(self._image)
 
     def _paint_module(self, xpos, ypos, width, color):
-        size = [
+        size = (
             (mm2px(xpos, self.dpi), mm2px(ypos, self.dpi)),
             (
                 mm2px(xpos + width, self.dpi),
                 mm2px(ypos + self.module_height, self.dpi),
             ),
-        ]
+        )
+        assert self._draw is not None
         self._draw.rectangle(size, outline=color, fill=color)
 
     def _finish(self):
+        # although Image mode set to "1", draw function writes white as 255
+        assert self._image is not None
+        self._image = self._image.point(lambda x: 1 if x > 0 else 0, mode="1")
         return self._image
 
     def save(self, filename, output):
         filename = f"{filename}.{self.format.lower()}"
         output.save(filename, self.format.upper())
         return filename
```

### Comparing `labelle-1.0.0/src/labelle/command_line.py` & `labelle-1.1.0/src/labelle/cli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,60 @@
 # === LICENSE STATEMENT ===
 # Copyright (c) 2011 Sebastian J. Bronner <waschtl@sbronner.com>
 #
 # Copying and distribution of this file, with or without modification, are
 # permitted in any medium without royalty provided the copyright notice and
 # this notice are preserved.
 # === END LICENSE STATEMENT ===
-
 import argparse
-import os
+import logging
+import webbrowser
+from tempfile import NamedTemporaryFile
 
 from PIL import Image, ImageOps
 
-from . import __version__
-from .constants import (
+from labelle import __version__
+from labelle.lib.constants import (
     AVAILABLE_BARCODES,
     DEFAULT_MARGIN_PX,
     PIXELS_PER_MM,
     USE_QR,
     e_qrcode,
 )
-from .dymo_print_engines import DymoRenderEngine, print_label
-from .font_config import font_filename
-from .metadata import our_metadata
-from .unicode_blocks import image_to_unicode
-from .utils import die
+from labelle.lib.dymo_labeler import DymoLabeler
+from labelle.lib.font_config import NoFontFound, get_available_fonts, get_font_path
+from labelle.lib.logger import configure_logging, is_verbose_env_vars, set_not_verbose
+from labelle.lib.render_engines import (
+    BarcodeRenderEngine,
+    BarcodeWithTextRenderEngine,
+    HorizontallyCombinedRenderEngine,
+    PictureRenderEngine,
+    PrintPayloadRenderEngine,
+    PrintPreviewRenderEngine,
+    QrRenderEngine,
+    RenderContext,
+    TestPatternRenderEngine,
+    TextRenderEngine,
+)
+from labelle.lib.unicode_blocks import image_to_unicode
+from labelle.lib.utils import system_run
+from labelle.metadata import our_metadata
+
+LOG = logging.getLogger(__name__)
+
+FLAG_TO_STYLE = {
+    "r": "regular",
+    "b": "bold",
+    "i": "italic",
+    "n": "narrow",
+}
+
+
+class CommandLineUsageError(Exception):
+    pass
 
 
 def parse_args():
     # check for any text specified on the command line
     parser = argparse.ArgumentParser(description=our_metadata["Summary"])
     parser.add_argument(
         "--version", action="version", version=f"%(prog)s {__version__}"
@@ -36,25 +63,28 @@
         "text",
         nargs="+",
         help="Text Parameter, each parameter gives a new line",
         type=str,
     )
     parser.add_argument(
         "-f",
+        "--frame-width-px",
         action="count",
         help="Draw frame around the text, more arguments for thicker frame",
     )
     parser.add_argument(
         "-s",
+        "--style",
         choices=["r", "b", "i", "n"],
         default="r",
         help="Set fonts style (regular,bold,italic,narrow)",
     )
     parser.add_argument(
         "-a",
+        "--align",
         choices=[
             "left",
             "center",
             "right",
         ],
         default="left",
         help="Align multiline text (left,center,right)",
@@ -86,26 +116,29 @@
         type=int,
         default=None,
         help="Specify fixed label length in mm, error if the label won't fit",
     )
 
     length_options.add_argument(
         "-j",
+        "--justify",
         choices=[
             "left",
             "center",
             "right",
         ],
         default="center",
         help=(
             "Justify content of label if label content is less than the "
             "minimum or fixed length (left, center, right)"
         ),
     )
-    parser.add_argument("-u", nargs="?", help='Set user font, overrides "-s" parameter')
+    parser.add_argument(
+        "-u", "--font", nargs="?", help='Set user font, overrides "-s" parameter'
+    )
     parser.add_argument(
         "-n",
         "--preview",
         action="store_true",
         help="Unicode preview of label, do not send to printer",
     )
     parser.add_argument(
@@ -115,14 +148,19 @@
     )
     parser.add_argument(
         "--imagemagick",
         action="store_true",
         help="Preview label with Imagemagick, do not send to printer",
     )
     parser.add_argument(
+        "--browser",
+        action="store_true",
+        help="Preview label in the browser, do not send to printer",
+    )
+    parser.add_argument(
         "-qr", action="store_true", help="Printing the first text parameter as QR-code"
     )
     parser.add_argument(
         "-c",
         "--barcode",
         choices=AVAILABLE_BARCODES,
         default=False,
@@ -133,133 +171,174 @@
         choices=AVAILABLE_BARCODES,
         default=False,
         help="Printing the first text parameter as barcode and text under it",
     )
     parser.add_argument("-p", "--picture", help="Print the specified picture")
     parser.add_argument(
         "-m",
+        "--margin-px",
         type=int,
         default=DEFAULT_MARGIN_PX,
         help=f"Margin in px (default is {DEFAULT_MARGIN_PX})",
     )
     parser.add_argument(
         "--scale", type=int, default=90, help="Scaling font factor, [0,10] [%%]"
     )
     parser.add_argument(
         "-t",
+        "--tape-size-mm",
         type=int,
         choices=[6, 9, 12, 19],
         default=12,
         help="Tape size: 6,9,12,19 mm, default=12mm",
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Increase logging verbosity",
+    )
     return parser.parse_args()
 
 
 def mm_to_payload_px(mm, margin):
-    """Convert a length in mm to a number of pixels of payload
+    """Convert a length in mm to a number of pixels of payload.
 
-    The print resolution is 7 pixels/mm, and margin is subtracted
-    from each side."""
-    return (mm * PIXELS_PER_MM) - margin * 2
+    The print resolution is 7 pixels/mm, and margin is subtracted from each side.
+    """
+    return max(0, (mm * PIXELS_PER_MM) - margin * 2)
 
 
-def main():
+def run():
     args = parse_args()
-    render_engine = DymoRenderEngine(args.t)
+
+    if (not args.verbose) and (not is_verbose_env_vars()):
+        # Neither --verbose flag nor the environment variable is set.
+        set_not_verbose()
 
     # read config file
-    FONT_FILENAME = font_filename(args.s)
+    style = FLAG_TO_STYLE.get(args.style)
+    try:
+        font_path = get_font_path(font=args.font, style=style)
+    except NoFontFound as e:
+        valid_font_names = [f.stem for f in get_available_fonts()]
+        msg = f"{e}. Valid fonts are: {', '.join(valid_font_names)}"
+        raise CommandLineUsageError(msg) from None
 
     labeltext = args.text
 
-    if args.u is not None:
-        if os.path.isfile(args.u):
-            FONT_FILENAME = args.u
-        else:
-            die("Error: file '%s' not found." % args.u)
-
     # check if barcode, qrcode or text should be printed, use frames only on text
     if args.qr and not USE_QR:
-        die("Error: %s" % e_qrcode)
+        raise CommandLineUsageError(
+            "QR code cannot be used without QR support " "installed"
+        ) from e_qrcode
 
     if args.barcode and args.qr:
-        die("Error: can not print both QR and Barcode on the same label (yet)")
+        raise CommandLineUsageError(
+            "Can not print both QR and Barcode on the same " "label (yet)"
+        )
 
     if args.fixed_length is not None and (
         args.min_length != 0 or args.max_length is not None
     ):
-        die("Error: can't specify min/max and fixed length at the same time")
+        raise CommandLineUsageError(
+            "Cannot't specify min/max and fixed length at the " "same time"
+        )
 
     if args.max_length is not None and args.max_length < args.min_length:
-        die("Error: maximum length is less than minimum length")
+        raise CommandLineUsageError("Maximum length is less than minimum length")
 
-    bitmaps = []
+    render_engines = []
 
     if args.test_pattern:
-        bitmaps.append(render_engine.render_test(args.test_pattern))
+        render_engines.append(TestPatternRenderEngine(args.test_pattern))
 
     if args.qr:
-        bitmaps.append(render_engine.render_qr(labeltext.pop(0)))
+        render_engines.append(QrRenderEngine(labeltext.pop(0)))
 
     elif args.barcode:
-        bitmaps.append(render_engine.render_barcode(labeltext.pop(0), args.barcode))
+        render_engines.append(BarcodeRenderEngine(labeltext.pop(0), args.barcode))
 
     elif args.barcode_text:
-        bitmaps.append(
-            render_engine.render_barcode_with_text(
-                labeltext.pop(0), args.barcode_text, FONT_FILENAME, args.f
+        render_engines.append(
+            BarcodeWithTextRenderEngine(
+                labeltext.pop(0), args.barcode_text, font_path, args.frame_width_px
             )
         )
 
     if labeltext:
-        bitmaps.append(
-            render_engine.render_text(
+        render_engines.append(
+            TextRenderEngine(
                 text_lines=labeltext,
-                font_file_name=FONT_FILENAME,
-                frame_width_px=args.f,
+                font_file_name=font_path,
+                frame_width_px=args.frame_width_px,
                 font_size_ratio=int(args.scale) / 100.0,
-                align=args.a,
+                align=args.align,
             )
         )
 
     if args.picture:
-        bitmaps.append(render_engine.render_picture(args.picture))
-
-    margin = args.m
-    justify = args.j
+        render_engines.append(PictureRenderEngine(args.picture))
 
     if args.fixed_length is not None:
         min_label_mm_len = args.fixed_length
         max_label_mm_len = args.fixed_length
     else:
         min_label_mm_len = args.min_length
         max_label_mm_len = args.max_length
 
-    min_payload_len_px = max(0, mm_to_payload_px(min_label_mm_len, margin))
+    margin_px = args.margin_px
+    min_payload_len_px = mm_to_payload_px(min_label_mm_len, margin_px)
     max_payload_len_px = (
-        mm_to_payload_px(max_label_mm_len, margin)
+        mm_to_payload_px(max_label_mm_len, margin_px)
         if max_label_mm_len is not None
         else None
     )
 
-    label_bitmap = render_engine.merge_render(
-        bitmaps=bitmaps,
-        min_payload_len_px=min_payload_len_px,
-        max_payload_len_px=max_payload_len_px,
-        justify=justify,
+    dymo_labeler = DymoLabeler(tape_size_mm=args.tape_size_mm)
+    render_engine = HorizontallyCombinedRenderEngine(render_engines)
+    render_context = RenderContext(
+        background_color="white",
+        foreground_color="black",
+        height_px=dymo_labeler.height_px,
+        preview_show_margins=False,
     )
 
     # print or show the label
-    if args.preview or args.preview_inverted or args.imagemagick:
-        print("Demo mode: showing label..")
-        # fix size, adding print borders
-        label_image = Image.new(
-            "L", (margin + label_bitmap.width + margin, label_bitmap.height)
+    if args.preview or args.preview_inverted or args.imagemagick or args.browser:
+        render = PrintPreviewRenderEngine(
+            render_engine=render_engine,
+            justify=args.justify,
+            visible_horizontal_margin_px=margin_px,
+            labeler_margin_px=dymo_labeler.labeler_margin_px,
+            max_width_px=max_payload_len_px,
+            min_width_px=min_payload_len_px,
         )
-        label_image.paste(label_bitmap, (margin, 0))
+        bitmap = render.render(render_context)
+        LOG.debug("Demo mode: showing label..")
         if args.preview or args.preview_inverted:
-            label_rotated = label_bitmap.transpose(Image.ROTATE_270)
+            label_rotated = bitmap.transpose(Image.ROTATE_270)
             print(image_to_unicode(label_rotated, invert=args.preview_inverted))
         if args.imagemagick:
-            ImageOps.invert(label_image).show()
+            ImageOps.invert(bitmap).show()
+        if args.browser:
+            with NamedTemporaryFile(suffix=".png", delete=False) as fp:
+                inverted = ImageOps.invert(bitmap.convert("RGB"))
+                ImageOps.invert(inverted).save(fp)
+                webbrowser.open(f"file://{fp.name}")
     else:
-        print_label(label_bitmap, margin_px=args.m, tape_size_mm=args.t)
+        render = PrintPayloadRenderEngine(
+            render_engine=render_engine,
+            justify=args.justify,
+            visible_horizontal_margin_px=margin_px,
+            labeler_margin_px=dymo_labeler.labeler_margin_px,
+            max_width_px=max_payload_len_px,
+            min_width_px=min_payload_len_px,
+        )
+        bitmap, _ = render.render(render_context)
+        dymo_labeler.print(bitmap)
+
+
+def main():
+    configure_logging()
+    with system_run():
+        run()
```

### Comparing `labelle-1.0.0/src/labelle/constants.py` & `labelle-1.1.0/src/labelle/lib/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     e_qrcode = error
     USE_QR = False
     QRCode = None
 
 
 UNCONFIRMED_MESSAGE = (
     "WARNING: This device is not confirmed to work with this software. Please "
-    "report your experiences in https://github.com/computerlyrik/dymoprint/issues/44"
+    "report your experiences in https://github.com/labelle-org/labelle/issues/4"
 )
 SUPPORTED_PRODUCTS = {
     0x0011: "DYMO LabelMANAGER PC",
     0x0015: "LabelPoint 350",
     0x1001: "LabelManager PnP (no mode switch)",
     0x1002: "LabelManager PnP (mode switch)",
     0x1003: f"LabelManager 420P (no mode switch) {UNCONFIRMED_MESSAGE}",
@@ -56,30 +56,21 @@
 ESC = 0x1B
 
 # Synchronization character preceding uncompressed print data
 SYN = 0x16
 
 FONT_SIZERATIO = 7 / 8
 
-DEFAULT_FONT_STYLE = "regular"
-
 DEFAULT_MARGIN_PX = 56
-
-FLAG_TO_STYLE = {
-    "r": "regular",
-    "b": "bold",
-    "i": "italic",
-    "n": "narrow",
-}
+VERTICAL_PREVIEW_MARGIN_PX = 13
 
 DPI = 180
 MM_PER_INCH = 25.4
 PIXELS_PER_MM = DPI / MM_PER_INCH
 
-DEFAULT_FONT_DIR = Path(labelle.resources.fonts.__file__).parent
 ICON_DIR = Path(labelle.resources.icons.__file__).parent
 
 AVAILABLE_BARCODES = [
     "code39",
     "code128",
     "ean",
     "ean13",
```

### Comparing `labelle-1.0.0/src/labelle/q_dymo_label_widgets.py` & `labelle-1.1.0/src/labelle/gui/q_dymo_label_widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,286 +1,306 @@
-import os
+from pathlib import Path
 from typing import Optional
 
 from PyQt6 import QtCore
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import (
     QCheckBox,
     QComboBox,
     QFileDialog,
     QHBoxLayout,
     QLabel,
     QLineEdit,
-    QMessageBox,
     QPlainTextEdit,
     QPushButton,
     QSpinBox,
     QWidget,
 )
 
-from labelle.constants import ICON_DIR
-from labelle.dymo_print_engines import DymoRenderEngine
+from labelle.gui.common import crash_msg_box
+from labelle.lib.constants import AVAILABLE_BARCODES, ICON_DIR
+from labelle.lib.font_config import get_available_fonts
+from labelle.lib.render_engines import (
+    BarcodeRenderEngine,
+    BarcodeWithTextRenderEngine,
+    EmptyRenderEngine,
+    NoContentError,
+    NoPictureFilePath,
+    PictureRenderEngine,
+    QrRenderEngine,
+    RenderContext,
+    TextRenderEngine,
+)
+from labelle.lib.render_engines.render_engine import RenderEngineException
+
 
-from .constants import AVAILABLE_BARCODES
-from .font_config import parse_fonts
+class FontStyle(QComboBox):
+    def __init__(self):
+        super().__init__()
+        # Populate font_style
+        for font_path in get_available_fonts():
+            name = font_path.stem
+            absolute_path = font_path.absolute()
+            self.addItem(name, absolute_path)
+            self.setCurrentText("Carlito-Regular")
 
 
 class BaseDymoLabelWidget(QWidget):
-    """
-    A base class for creating Dymo label widgets.
+    """A base class for creating Dymo label widgets.
+
     Signals:
     --------
     itemRenderSignal : PyQtSignal
         Signal emitted when the content of the label is changed.
-    Methods:
-    --------
+
+    Methods
+    -------
     content_changed()
         Emits the itemRenderSignal when the content of the label is changed.
     render_label()
         Abstract method to be implemented by subclasses for rendering the label.
+
     """
 
+    render_context: RenderContext
+
     itemRenderSignal = QtCore.pyqtSignal(name="itemRenderSignal")
 
     def content_changed(self):
-        """
-        Emits the itemRenderSignal when the content of the label is changed.
-        """
+        """Emit the itemRenderSignal when the content of the label is changed."""
         self.itemRenderSignal.emit()
 
-    def render_label(self):
-        """
-        Abstract method to be implemented by subclasses for rendering the label.
-        """
+    @property
+    def render_engine_impl(self):
+        """Abstract method for getting the render engine of the label."""
         pass
 
+    @property
+    def render_engine(self):
+        try:
+            return self.render_engine_impl
+        except RenderEngineException as err:
+            crash_msg_box(self, "Render Engine Failed!", err)
+            return EmptyRenderEngine()
+
 
 class TextDymoLabelWidget(BaseDymoLabelWidget):
-    """
-    A widget for rendering text on a Dymo label.
+    """A widget for rendering text on a Dymo label.
+
     Args:
-        render_engine (RenderEngine): The rendering engine to use.
+    ----
+        render_context (RenderContext): The rendering context to use.
         parent (QWidget): The parent widget of this widget.
+
     Attributes:
-        render_engine (RenderEngine): The rendering engine used by this widget.
+    ----------
+        render_context (RenderContext): The rendering context used by this widget.
         label (QPlainTextEdit): The text label to be rendered on the Dymo label.
-        font_style (QComboBox): The font style selection dropdown.
+        font_style (FontStyle): The font style selection dropdown.
         font_size (QSpinBox): The font size selection spinner.
-        draw_frame (QSpinBox): The frame width selection spinner.
+        frame_width_px (QSpinBox): The frame width selection spinner.
     Signals:
         itemRenderSignal: A signal emitted when the content of the label changes.
+
     """
 
-    render_engine: DymoRenderEngine
     align: QComboBox
     label: QPlainTextEdit
-    font_style: QComboBox
+    font_style: FontStyle
     font_size: QSpinBox
-    draw_frame: QSpinBox
+    frame_width_px: QSpinBox
 
-    def __init__(
-        self, render_engine: DymoRenderEngine, parent: Optional[QWidget] = None
-    ):
+    def __init__(self, render_context: RenderContext, parent: Optional[QWidget] = None):
         super().__init__(parent)
-        self.render_engine = render_engine
+        self.render_context = render_context
 
         self.label = QPlainTextEdit("text")
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
-        self.font_style = QComboBox()
+        self.font_style = FontStyle()
         self.font_size = QSpinBox()
         self.font_size.setMaximum(150)
         self.font_size.setMinimum(0)
         self.font_size.setSingleStep(1)
         self.font_size.setValue(90)
-        self.draw_frame = QSpinBox()
+        self.frame_width_px = QSpinBox()
         self.align = QComboBox()
 
         self.align.addItems(["left", "center", "right"])
 
-        for name, font_path in parse_fonts():
-            self.font_style.addItem(name, font_path)
-            if "Regular" in name:
-                self.font_style.setCurrentText(name)
-
         layout = QHBoxLayout()
         item_icon = QLabel()
         item_icon.setPixmap(QIcon(str(ICON_DIR / "txt_icon.png")).pixmap(32, 32))
         item_icon.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
         layout.addWidget(item_icon)
         layout.addWidget(self.label)
         layout.addWidget(QLabel("Font:"))
         layout.addWidget(self.font_style)
         layout.addWidget(QLabel("Size [%]:"))
         layout.addWidget(self.font_size)
         layout.addWidget(QLabel("Frame Width:"))
-        layout.addWidget(self.draw_frame)
+        layout.addWidget(self.frame_width_px)
         layout.addWidget(QLabel("Alignment:"))
         layout.addWidget(self.align)
         self.label.textChanged.connect(self.content_changed)
-        self.draw_frame.valueChanged.connect(self.content_changed)
+        self.frame_width_px.valueChanged.connect(self.content_changed)
         self.font_size.valueChanged.connect(self.content_changed)
         self.font_style.currentTextChanged.connect(self.content_changed)
         self.align.currentTextChanged.connect(self.content_changed)
         self.setLayout(layout)
 
     def content_changed(self):
-        """
-        Updates the height of the label and emits the itemRenderSignal when the
-        content of the label changes.
+        """Manage changes to the label contents.
+
+        In particular, update the height of the label and emit the itemRenderSignal
+        when the content of the label changes.
         """
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
         self.itemRenderSignal.emit()
 
-    def render_label(self):
-        """
-        Renders the label using the current settings.
-        Returns:
-            QImage: The rendered label image.
-        Raises:
-            QMessageBox.warning: If the rendering fails.
+    @property
+    def render_engine_impl(self):
+        """Get the render engine for the text label using the current settings.
+
+        Returns
+        -------
+            TextRenderEngine: The rendered engine.
+
         """
         selected_alignment = self.align.currentText()
         assert selected_alignment in ("left", "center", "right")
-        try:
-            render = self.render_engine.render_text(
-                text_lines=self.label.toPlainText().splitlines(),
-                font_file_name=self.font_style.currentData(),
-                frame_width_px=self.draw_frame.value(),
-                font_size_ratio=self.font_size.value() / 100.0,
-                align=selected_alignment,
-            )
-            return render
-        except BaseException as err:
-            QMessageBox.warning(self, "TextDymoLabelWidget render fail!", f"{err}")
-            return self.render_engine.render_empty()
+        return TextRenderEngine(
+            text_lines=self.label.toPlainText().splitlines(),
+            font_file_name=self.font_style.currentData(),
+            frame_width_px=self.frame_width_px.value(),
+            font_size_ratio=self.font_size.value() / 100.0,
+            align=selected_alignment,
+        )
 
 
 class QrDymoLabelWidget(BaseDymoLabelWidget):
-    """
-    A widget for rendering QR codes on Dymo labels.
+    """A widget for rendering QR codes on Dymo labels.
+
     Args:
-        render_engine (RenderEngine): The render engine to use for rendering
+    ----
+        render_context (RenderContext): The render context to use for rendering
             the QR code.
         parent (QWidget, optional): The parent widget. Defaults to None.
+
     """
 
-    def __init__(self, render_engine, parent=None):
-        """
-        Initializes the QrDymoLabelWidget.
+    def __init__(self, render_context, parent=None):
+        """Initialize the QrDymoLabelWidget.
+
         Args:
-            render_engine (RenderEngine): The render engine to use for rendering
+        ----
+            render_context (RenderContext): The render context to use for rendering
                 the QR code.
             parent (QWidget, optional): The parent widget. Defaults to None.
+
         """
         super().__init__(parent)
-        self.render_engine = render_engine
+        self.render_context = render_context
 
         self.label = QLineEdit("")
         layout = QHBoxLayout()
         item_icon = QLabel()
         item_icon.setPixmap(QIcon(str(ICON_DIR / "qr_icon.png")).pixmap(32, 32))
         item_icon.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
         layout.addWidget(item_icon)
         layout.addWidget(self.label)
         self.label.textChanged.connect(self.content_changed)
         self.setLayout(layout)
 
-    def render_label(self):
-        """
-        Renders the QR code on the Dymo label.
-        Returns:
-            bytes: The rendered QR code as bytes.
-        Raises:
-            QMessageBox.warning: If the rendering fails.
+    @property
+    def render_engine_impl(self):
+        """Get the render engine for the QR label using the current settings.
+
+        Returns
+        -------
+            QrRenderEngine: The render engine.
+
         """
         try:
-            render = self.render_engine.render_qr(self.label.text())
-            return render
-
-        except BaseException as err:
-            QMessageBox.warning(self, "QrDymoLabelWidget render fail!", f"{err}")
-            return self.render_engine.render_empty()
+            return QrRenderEngine(content=self.label.text())
+        except NoContentError:
+            return EmptyRenderEngine()
 
 
 class BarcodeDymoLabelWidget(BaseDymoLabelWidget):
-    """
-    A widget for rendering barcode labels using the Dymo label printer.
+    """A widget for rendering barcode labels using the Dymo label printer.
+
     Args:
-        render_engine (DymoRenderEngine): An instance of the DymoRenderEngine class.
+    ----
+        render_context (RenderContext): An instance of the RenderContext class.
         parent (QWidget): The parent widget of this widget.
+
     Attributes:
-        render_engine (DymoRenderEngine): An instance of the DymoRenderEngine class.
+    ----------
+        render_context (RenderContext): An instance of the RenderContext class.
         label (QLineEdit): A QLineEdit widget for entering the content of the
             barcode label.
         Type (QComboBox): A QComboBox widget for selecting the type of barcode
             to render.
-        font_style (QComboBox): The font style selection dropdown.
+        font_style (FontStyle): The font style selection dropdown.
         font_size (QSpinBox): The font size selection spinner.
-        draw_frame (QSpinBox): The frame width selection spinner.
+        frame_width_px (QSpinBox): The frame width selection spinner.
     Signals:
         content_changed(): Emitted when the content of the label or the selected
             barcode type changes.
+
     Methods:
-        __init__(self, render_engine, parent=None): Initializes the widget.
-        render_label(self): Renders the barcode label using the current content
+    -------
+        __init__(self, render_context, parent=None): Initializes the widget.
+        render_label_impl(self): Renders the barcode label using the current content
             and barcode type.
+
     """
 
-    render_engine: DymoRenderEngine
     label: QLineEdit
     barcode_type_label: QLabel
     barcode_type: QComboBox
     show_text_label: QLabel
     show_text_checkbox: QCheckBox
-    font_style: QComboBox
+    font_style: FontStyle
     font_size: QSpinBox
-    draw_frame: QSpinBox
+    frame_width_px: QSpinBox
     font_label: QLabel
-    font_style: QComboBox
     size_label: QLabel
-    font_size: QSpinBox
     frame_label: QLabel
-    draw_frame: QSpinBox
     align_label: QLabel
     align: QComboBox
 
-    def __init__(self, render_engine, parent=None):
+    def __init__(self, render_context, parent=None):
         super().__init__(parent)
-        self.render_engine = render_engine
+        self.render_context = render_context
 
         self.label = QLineEdit("")
 
         # Hidable text fields and their labels
         self.font_label = QLabel("Font:")
-        self.font_style = QComboBox()
+        self.font_style = FontStyle()
         self.size_label = QLabel("Size [%]:")
         self.font_size = QSpinBox()
         self.font_size.setMaximum(150)
         self.font_size.setMinimum(0)
         self.font_size.setSingleStep(1)
         self.font_size.setValue(90)
         self.frame_label = QLabel("Frame Width:")
-        self.draw_frame = QSpinBox()
+        self.frame_width_px = QSpinBox()
         self.align_label = QLabel("Alignment:")
         self.align = QComboBox()
         self.item_icon = QLabel()
         self.item_icon.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
 
         self.align.addItems(["left", "center", "right"])
         # Set the default value to "center"
         self.align.setCurrentIndex(1)
 
-        # Populate font_style
-        for name, font_path in parse_fonts():
-            self.font_style.addItem(name, font_path)
-            if "Regular" in name:
-                self.font_style.setCurrentText(name)
-
         self.set_text_fields_visibility(True)
 
         layout = QHBoxLayout()
 
         self.barcode_type_label = QLabel("Type:")
         self.barcode_type = QComboBox()
         self.barcode_type.addItems(AVAILABLE_BARCODES)
@@ -300,34 +320,34 @@
         layout.addWidget(self.show_text_label)
         layout.addWidget(self.show_text_checkbox)
         layout.addWidget(self.font_label)
         layout.addWidget(self.font_style)
         layout.addWidget(self.size_label)
         layout.addWidget(self.font_size)
         layout.addWidget(self.frame_label)
-        layout.addWidget(self.draw_frame)
+        layout.addWidget(self.frame_width_px)
         layout.addWidget(self.align_label)
         layout.addWidget(self.align)
 
         self.label.textChanged.connect(self.content_changed)
-        self.draw_frame.valueChanged.connect(self.content_changed)
+        self.frame_width_px.valueChanged.connect(self.content_changed)
         self.font_size.valueChanged.connect(self.content_changed)
         self.font_style.currentTextChanged.connect(self.content_changed)
         self.align.currentTextChanged.connect(self.content_changed)
         self.barcode_type.currentTextChanged.connect(self.content_changed)
 
         self.setLayout(layout)
 
     def set_text_fields_visibility(self, visible):
         self.font_label.setVisible(visible)
         self.font_style.setVisible(visible)
         self.size_label.setVisible(visible)
         self.font_size.setVisible(visible)
         self.frame_label.setVisible(visible)
-        self.draw_frame.setVisible(visible)
+        self.frame_width_px.setVisible(visible)
         self.align_label.setVisible(visible)
         self.align.setVisible(visible)
         if visible:
             self.item_icon.setPixmap(
                 QIcon(str(ICON_DIR / "barcode_text_icon.png")).pixmap(32, 32)
             )
         else:
@@ -336,89 +356,91 @@
             )
 
     def toggle_text_fields_and_rerender(self):
         is_checked = self.show_text_checkbox.isChecked()
         self.set_text_fields_visibility(is_checked)
         self.content_changed()  # Trigger rerender
 
-    def render_label(self):
-        """
-        Renders the labels with barcode and text below it using the current settings.
-        Returns:
-            QImage: The rendered label image.
-        Raises:
-            QMessageBox.warning: If the rendering fails.
+    @property
+    def render_engine_impl(self):
+        """Get the render engine for the barcode label using the current settings.
+
+        Returns
+        -------
+            RenderEngine: The rendered engine (either BarcodeRenderEngine or
+            BarcodeWithTextRenderEngine).
+
         """
-        try:
-            if self.show_text_checkbox.isChecked():
-                render = self.render_engine.render_barcode_with_text(
-                    barcode_input_text=self.label.text(),
-                    bar_code_type=self.barcode_type.currentText(),
-                    font_file_name=self.font_style.currentData(),
-                    frame_width=self.draw_frame.value(),
-                    font_size_ratio=self.font_size.value() / 100.0,
-                    align=self.align.currentText(),
-                )
-            else:
-                render = self.render_engine.render_barcode(
-                    self.label.text(), self.barcode_type.currentText()
-                )
-            return render
-        except BaseException as err:
-            QMessageBox.warning(
-                self, "BarcodeWithTextDymoLabelWidget render fail!", f"{err}"
+        if self.show_text_checkbox.isChecked():
+            render_engine = BarcodeWithTextRenderEngine(
+                content=self.label.text(),
+                barcode_type=self.barcode_type.currentText(),
+                font_file_name=self.font_style.currentData(),
+                frame_width_px=self.frame_width_px.value(),
+                font_size_ratio=self.font_size.value() / 100.0,
+                align=self.align.currentText(),
+            )
+        else:
+            render_engine = BarcodeRenderEngine(
+                content=self.label.text(),
+                barcode_type=self.barcode_type.currentText(),
             )
-            return self.render_engine.render_empty()
+        return render_engine
 
 
 class ImageDymoLabelWidget(BaseDymoLabelWidget):
-    """
-    A widget for rendering image-based Dymo labels.
+    """A widget for rendering image-based Dymo labels.
+
     Args:
-        render_engine (RenderEngine): The render engine to use for rendering the label.
+    ----
+        context (RenderContext): The render context to use for rendering the label.
         parent (QWidget, optional): The parent widget. Defaults to None.
+
     """
 
-    def __init__(self, render_engine, parent=None):
-        """
-        Initializes the ImageDymoLabelWidget.
+    def __init__(self, render_context, parent=None):
+        """Initialize the ImageDymoLabelWidget.
+
         Args:
-            render_engine (RenderEngine): The render engine to use for rendering
+        ----
+            render_context (RenderContext): The render context to use for rendering
                 the label.
             parent (QWidget, optional): The parent widget. Defaults to None.
+
         """
         super().__init__(parent)
-        self.render_engine = render_engine
+        self.render_context = render_context
 
         self.label = QLineEdit("")
         layout = QHBoxLayout()
         item_icon = QLabel()
         item_icon.setPixmap(QIcon(str(ICON_DIR / "img_icon.png")).pixmap(32, 32))
         item_icon.setAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
 
         button = QPushButton("Select file")
         file_dialog = QFileDialog()
         button.clicked.connect(
             lambda: self.label.setText(
-                os.path.abspath(file_dialog.getOpenFileName()[0])
+                str(Path(file_dialog.getOpenFileName()[0]).absolute())
             )
         )
 
         layout.addWidget(item_icon)
         layout.addWidget(self.label)
         layout.addWidget(button)
 
         self.label.textChanged.connect(self.content_changed)
         self.setLayout(layout)
 
-    def render_label(self):
-        """
-        Renders the label using the render engine and the selected image file.
-        Returns:
-            QPixmap: The rendered label as a QPixmap.
+    @property
+    def render_engine_impl(self):
+        """Get the render engine for the image label using the current settings.
+
+        Returns
+        -------
+            PictureRenderEngine: The rendered engine.
+
         """
         try:
-            render = self.render_engine.render_picture(self.label.text())
-            return render
-        except BaseException as err:
-            QMessageBox.warning(self, "ImageDymoLabelWidget render fail!", f"{err}")
-            return self.render_engine.render_empty()
+            return PictureRenderEngine(picture_path=self.label.text())
+        except NoPictureFilePath:
+            return EmptyRenderEngine()
```

### Comparing `labelle-1.0.0/src/labelle/resources/fonts/Carlito-Bold.ttf` & `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf` & `labelle-1.1.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/fonts/Carlito-Italic.ttf` & `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/fonts/Carlito-Regular.ttf` & `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/fonts/LICENSE` & `labelle-1.1.0/src/labelle/resources/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/icons/barcode_icon.png` & `labelle-1.1.0/src/labelle/resources/icons/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/icons/img_icon.png` & `labelle-1.1.0/src/labelle/resources/icons/img_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/icons/logo_small.png` & `labelle-1.1.0/src/labelle/resources/icons/logo_small.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/src/labelle/resources/icons/txt_icon.png` & `labelle-1.1.0/src/labelle/resources/icons/txt_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/LICENSE` & `labelle-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.0.0/README.md` & `labelle-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 # Labelle
 
 [![GitHub Actions (Tests)](https://github.com/labelle-org/labelle/workflows/Tests/badge.svg)](https://github.com/labelle-org/labelle)
 [![PyPI version](https://img.shields.io/pypi/v/labelle.svg)](https://pypi.org/project/labelle/)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/labelle-org/labelle/main.svg)](https://results.pre-commit.ci/latest/github/labelle-org/labelle/main)
+
+<!-- markdownlint-disable MD033 -->
 
 <p align="center">
-  <img src="labelle.png" alt="logo" width="400"></img><br>
+  <img src="labelle.png" alt="logo" width="400"></img>
 </p>
 
+<!-- markdownlint-enable MD033 -->
+
 ## Open-source label printing software
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
-* Cloned to Github and formerly maintained by @computerlyrik and @maresb: <https://github.com/computerlyrik/dymoprint>
-* Migrated to <https://github.com/labelle-org/labelle> and maintained by @tomers, @maresb, and @tomek-szczesny
+* Cloned to Github and maintained by
+  [@computerlyrik](https://github.com/computerlyrik) and later
+  [@maresb](https://github.com/maresb): <https://github.com/computerlyrik/dymoprint>
+* Migrated to `labelle-org` and maintained by
+  [@tomers](https://github.com/tomers), [@maresb](https://github.com/maresb),
+  and [@tomek-szczesny](https://github.com/tomek-szczesny):
+  <https://github.com/labelle-org/labelle>
 
 ## Features
 
 * Text printing
 * QR code printing
 * Barcode printing
 * Image printing
@@ -29,19 +39,21 @@
 * DYMO LabelPoint 350
 * DYMO LabelManager 280
 * DYMO LabelManager 420P
 * DYMO LabelManager Wireless PnP
 
 Labelle is not affiliated with DYMO. Please see the [disclaimer](#disclaimers) below.
 
-For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
+For more information about experimental device support, see [#4](https://github.com/labelle-org/labelle/issues/4).
 
 ## Installation
 
-It is recommended to install Labelle with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
+It is recommended to install Labelle with
+[pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual
+environment:
 
 ```bash
 pipx install labelle
 ```
 
 In case pipx is not already installed, it can be installed on Ubuntu/Debian with
 
@@ -55,72 +67,84 @@
 sudo pacman -S python-pipx
 ```
 
 By default, users don't have permission to access generic USB devices, so you will
 need to add a rule. The first time you run `labelle`, it will give instructions
 about how to do this:
 
+<!-- markdownlint-disable MD013 -->
+
 ```bash
 $ labelle "Hello world"
 ...
 You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
 
   echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-labelle-1001.rules
 ...
 ```
 
+<!-- markdownlint-enable MD013 -->
+
 ## Testing experimental features
 
 To install a test branch, by GitHub user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/labelle@branchname
 ```
 
 To revert back to the release version, run
 
 ```bash
 pipx install --force labelle
 ```
 
-To install a particular release version, specify `labelle==x.y.z` in place of `labelle` in the above command.
+To install a particular release version, specify `labelle==x.y.z` in place of
+`labelle` in the above command.
 
-## Development
+## Development and code style
 
-To install for development, fork and clone this repository, and run (ideally within a venv):
+To install for development, fork and clone this repository, and run (ideally
+within a venv):
 
 ```bash
 pip install --editable .
 ```
 
-This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
+This project uses [pre-commit](https://pre-commit.com/) to run some checks
+before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
 ## Font management
 
-Fonts are managed via [labelle.ini](labelle.ini). This should be placed in your
-config folder (normally `~/.config`). An example file is provided here.
-
-You may choose any TTF Font you like
-
-You may edit the file to point to your favorite font.
+Default fonts are managed via [labelle.ini](labelle.ini).
+This should be placed in your config folder (normally `~/.config`).
+An example file is provided here.
 
 For my Arch-Linux System, fonts are located at e.g.
 
 ```bash
 /usr/share/fonts/TTF/DejaVuSerif.ttf
 ```
 
 It is also possible to Download a font from
 <http://font.ubuntu.com/> and use it.
 
+For font discovery, Labelle contains code excerpts from
+[`matplotlib`](https://github.com/matplotlib/matplotlib/).
+See [here](vendoring/README.md) for more information and
+[LICENSE](src/labelle/_vendor/matplotlib/LICENSE) for the license.
+
+Labelle includes the Carlito font, licensed under the
+[SIL Open Font License](src/labelle/resources/fonts/LICENSE).
+
 ## Modes
 
 ### Print text
 
 ```labelle MyText```
 
 Multilines will be generated on whitespace
@@ -143,23 +167,24 @@
 
 ### Picture printing
 
 Any picture with JPEG standard may be printed. Beware it will be downsized to tape.
 
 ```labelle -p mypic.jpg ""```
 
-Take care of the trailing "" - you may enter text here which gets printed in front of the image
+Take care of the trailing "" - you may enter text here which gets printed in
+front of the image
 
 ## GUI
 
 ### Run Labelle GUI
 
 ```labelle-gui```
 
-#### GUI Features
+### GUI App Features
 
 * Live preview
 * margin settings
 * type size selector
 * visualization of tape color schema
 * the ability to freely arrange the content using the "Node" list
   * Text Node:
@@ -172,16 +197,16 @@
   * BarCode Node:
     * payload text
     * codding selector
   * Image Node:
     * path to file
 
 Nodes can be freely arranged, simply drag&drop rows on the list.
-To add or delete the node from the label - right-click on the list and select the action from the context menu.
-To print - click the print button.
+To add or delete the node from the label - right-click on the list and select
+the action from the context menu. To print - click the print button.
 
 ### Example
 
 Example 1: multiple text + QR code
 
 ![alt](doc/Labelle_example_1.png)
 
@@ -193,22 +218,28 @@
 
 ![alt](doc/Labelle_example_3.png)
 
 ## About the name
 
 The name "Labelle" is a multilingual pun by [@claui](https://github.com/computerlyrik/dymoprint/issues/114#issuecomment-1978982019).
 
+<!-- markdownlint-disable MD013 -->
+
 | Language | Word/Interpretation   | Meaning           | Pronunciation (IPA) | Simplified Phonetic Spelling |
 |----------|-----------------------|-------------------|---------------------|------------------------------|
 | English  | Label                 | A printed sticker | /ˈleɪbəl/           | LAY-buhl                     |
 | French   | La belle              | The beautiful     | /la bɛl/            | lah BEL                      |
 | German   | Libelle (sounds like) | Dragonfly         | /liˈbɛlə/           | lee-BELL-uh                  |
 
+<!-- markdownlint-enable MD013 -->
+
 ## Disclaimers
 
-* This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE) for details.
+* This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE)
+  for details.
 * Labelle is not affiliated, associated, authorized, endorsed by, or in any way
-  officially connected with DYMO Corporation, or any of its subsidiaries or its
-  affiliates. The official DYMO website can be found at <www.dymo.com>. The name DYMO®,
-  as well as related names, marks, emblems, and images, are registered trademarks of
-  their respective owners. Currently, Labelle software is designed to support certain
-  devices manufactured by DYMO; however, no endorsement or partnership is implied.
+  officially connected with DYMO, or any of its subsidiaries or its affiliates.
+  The official DYMO website can be found at [www.dymo.com](www.dymo.com).
+  The name DYMO®, as well as related names, marks, emblems, and images, are registered
+  trademarks of their respective owners. Currently, Labelle software is designed
+  to support certain devices manufactured by DYMO; however, no endorsement or
+  partnership is implied.
```

### Comparing `labelle-1.0.0/PKG-INFO` & `labelle-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labelle
-Version: 1.0.0
+Version: 1.1.0
 Summary: Open-source label printing software
 Project-URL: Homepage, https://github.com/labelle-org/labelle
 Project-URL: source, https://github.com/labelle-org/labelle
 Project-URL: tracker, https://github.com/labelle-org/labelle/issues
 Author-email: "Sebastian J. Bronner" <waschtl@sbronner.com>
 Maintainer-email: Tomer Shalev <tshalev@proofpoint.com>, Ben Mares <services-labelle@tensorial.com>, Tomek Szczęsny <mctom@tlen.pl>
 License-Expression: Apache-2.0
@@ -14,37 +14,48 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Printing
 Requires-Python: <4,>=3.8
-Requires-Dist: appdirs
+Requires-Dist: darkdetect
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: pillow<11,>=8.1.2
+Requires-Dist: platformdirs
 Requires-Dist: pyqrcode<2,>=1.2.1
 Requires-Dist: pyqt6
 Requires-Dist: python-barcode<1,>=0.13.1
 Requires-Dist: pyusb
 Description-Content-Type: text/markdown
 
 # Labelle
 
 [![GitHub Actions (Tests)](https://github.com/labelle-org/labelle/workflows/Tests/badge.svg)](https://github.com/labelle-org/labelle)
 [![PyPI version](https://img.shields.io/pypi/v/labelle.svg)](https://pypi.org/project/labelle/)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/labelle-org/labelle/main.svg)](https://results.pre-commit.ci/latest/github/labelle-org/labelle/main)
+
+<!-- markdownlint-disable MD033 -->
 
 <p align="center">
-  <img src="labelle.png" alt="logo" width="400"></img><br>
+  <img src="labelle.png" alt="logo" width="400"></img>
 </p>
 
+<!-- markdownlint-enable MD033 -->
+
 ## Open-source label printing software
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
-* Cloned to Github and formerly maintained by @computerlyrik and @maresb: <https://github.com/computerlyrik/dymoprint>
-* Migrated to <https://github.com/labelle-org/labelle> and maintained by @tomers, @maresb, and @tomek-szczesny
+* Cloned to Github and maintained by
+  [@computerlyrik](https://github.com/computerlyrik) and later
+  [@maresb](https://github.com/maresb): <https://github.com/computerlyrik/dymoprint>
+* Migrated to `labelle-org` and maintained by
+  [@tomers](https://github.com/tomers), [@maresb](https://github.com/maresb),
+  and [@tomek-szczesny](https://github.com/tomek-szczesny):
+  <https://github.com/labelle-org/labelle>
 
 ## Features
 
 * Text printing
 * QR code printing
 * Barcode printing
 * Image printing
@@ -58,19 +69,21 @@
 * DYMO LabelPoint 350
 * DYMO LabelManager 280
 * DYMO LabelManager 420P
 * DYMO LabelManager Wireless PnP
 
 Labelle is not affiliated with DYMO. Please see the [disclaimer](#disclaimers) below.
 
-For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
+For more information about experimental device support, see [#4](https://github.com/labelle-org/labelle/issues/4).
 
 ## Installation
 
-It is recommended to install Labelle with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
+It is recommended to install Labelle with
+[pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual
+environment:
 
 ```bash
 pipx install labelle
 ```
 
 In case pipx is not already installed, it can be installed on Ubuntu/Debian with
 
@@ -84,72 +97,84 @@
 sudo pacman -S python-pipx
 ```
 
 By default, users don't have permission to access generic USB devices, so you will
 need to add a rule. The first time you run `labelle`, it will give instructions
 about how to do this:
 
+<!-- markdownlint-disable MD013 -->
+
 ```bash
 $ labelle "Hello world"
 ...
 You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
 
   echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-labelle-1001.rules
 ...
 ```
 
+<!-- markdownlint-enable MD013 -->
+
 ## Testing experimental features
 
 To install a test branch, by GitHub user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/labelle@branchname
 ```
 
 To revert back to the release version, run
 
 ```bash
 pipx install --force labelle
 ```
 
-To install a particular release version, specify `labelle==x.y.z` in place of `labelle` in the above command.
+To install a particular release version, specify `labelle==x.y.z` in place of
+`labelle` in the above command.
 
-## Development
+## Development and code style
 
-To install for development, fork and clone this repository, and run (ideally within a venv):
+To install for development, fork and clone this repository, and run (ideally
+within a venv):
 
 ```bash
 pip install --editable .
 ```
 
-This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
+This project uses [pre-commit](https://pre-commit.com/) to run some checks
+before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
 ## Font management
 
-Fonts are managed via [labelle.ini](labelle.ini). This should be placed in your
-config folder (normally `~/.config`). An example file is provided here.
-
-You may choose any TTF Font you like
-
-You may edit the file to point to your favorite font.
+Default fonts are managed via [labelle.ini](labelle.ini).
+This should be placed in your config folder (normally `~/.config`).
+An example file is provided here.
 
 For my Arch-Linux System, fonts are located at e.g.
 
 ```bash
 /usr/share/fonts/TTF/DejaVuSerif.ttf
 ```
 
 It is also possible to Download a font from
 <http://font.ubuntu.com/> and use it.
 
+For font discovery, Labelle contains code excerpts from
+[`matplotlib`](https://github.com/matplotlib/matplotlib/).
+See [here](vendoring/README.md) for more information and
+[LICENSE](src/labelle/_vendor/matplotlib/LICENSE) for the license.
+
+Labelle includes the Carlito font, licensed under the
+[SIL Open Font License](src/labelle/resources/fonts/LICENSE).
+
 ## Modes
 
 ### Print text
 
 ```labelle MyText```
 
 Multilines will be generated on whitespace
@@ -172,23 +197,24 @@
 
 ### Picture printing
 
 Any picture with JPEG standard may be printed. Beware it will be downsized to tape.
 
 ```labelle -p mypic.jpg ""```
 
-Take care of the trailing "" - you may enter text here which gets printed in front of the image
+Take care of the trailing "" - you may enter text here which gets printed in
+front of the image
 
 ## GUI
 
 ### Run Labelle GUI
 
 ```labelle-gui```
 
-#### GUI Features
+### GUI App Features
 
 * Live preview
 * margin settings
 * type size selector
 * visualization of tape color schema
 * the ability to freely arrange the content using the "Node" list
   * Text Node:
@@ -201,16 +227,16 @@
   * BarCode Node:
     * payload text
     * codding selector
   * Image Node:
     * path to file
 
 Nodes can be freely arranged, simply drag&drop rows on the list.
-To add or delete the node from the label - right-click on the list and select the action from the context menu.
-To print - click the print button.
+To add or delete the node from the label - right-click on the list and select
+the action from the context menu. To print - click the print button.
 
 ### Example
 
 Example 1: multiple text + QR code
 
 ![alt](doc/Labelle_example_1.png)
 
@@ -222,22 +248,28 @@
 
 ![alt](doc/Labelle_example_3.png)
 
 ## About the name
 
 The name "Labelle" is a multilingual pun by [@claui](https://github.com/computerlyrik/dymoprint/issues/114#issuecomment-1978982019).
 
+<!-- markdownlint-disable MD013 -->
+
 | Language | Word/Interpretation   | Meaning           | Pronunciation (IPA) | Simplified Phonetic Spelling |
 |----------|-----------------------|-------------------|---------------------|------------------------------|
 | English  | Label                 | A printed sticker | /ˈleɪbəl/           | LAY-buhl                     |
 | French   | La belle              | The beautiful     | /la bɛl/            | lah BEL                      |
 | German   | Libelle (sounds like) | Dragonfly         | /liˈbɛlə/           | lee-BELL-uh                  |
 
+<!-- markdownlint-enable MD013 -->
+
 ## Disclaimers
 
-* This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE) for details.
+* This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE)
+  for details.
 * Labelle is not affiliated, associated, authorized, endorsed by, or in any way
-  officially connected with DYMO Corporation, or any of its subsidiaries or its
-  affiliates. The official DYMO website can be found at <www.dymo.com>. The name DYMO®,
-  as well as related names, marks, emblems, and images, are registered trademarks of
-  their respective owners. Currently, Labelle software is designed to support certain
-  devices manufactured by DYMO; however, no endorsement or partnership is implied.
+  officially connected with DYMO, or any of its subsidiaries or its affiliates.
+  The official DYMO website can be found at [www.dymo.com](www.dymo.com).
+  The name DYMO®, as well as related names, marks, emblems, and images, are registered
+  trademarks of their respective owners. Currently, Labelle software is designed
+  to support certain devices manufactured by DYMO; however, no endorsement or
+  partnership is implied.
```

