# Comparing `tmp/panpdf-0.1.8.tar.gz` & `tmp/panpdf-0.2.0.tar.gz`

## Comparing `panpdf-0.1.8.tar` & `panpdf-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.1.8/.gitattributes
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 panpdf-0.1.8/mkdocs.yml
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.1.8/ruff_defaults.toml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.1.8/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.1.8/.devcontainer/postCreate.sh
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.1.8/.devcontainer/starship.toml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.1.8/.devcontainer/features/zotero/devcontainer-feature.json
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.1.8/.devcontainer/features/zotero/install.sh
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/defaults.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/include-after-body.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/include-before-body.tex
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/include-in-header.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/images/figure.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/images/header.tex
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/src/1.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 panpdf-0.1.8/examples/src/2.md
--rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.1.8/notebooks/pdf.ipynb
--rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.1.8/notebooks/pgf.ipynb
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.1.8/notebooks/png.ipynb
--rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.1.8/notebooks/svg.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/formatters.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/main.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/stores.py
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/attribute.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/crossref.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/filter.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/jupyter.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/layout.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/verbatim.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.1.8/src/panpdf/filters/zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/test_converters.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/test_formatters.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/test_main.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/test_stores.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/test_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/conftest.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_attribute.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_crossref.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_filter.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_jupyter.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_layout.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_verbatim.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/filters/test_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/test_nbformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_cite.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_code.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_figure.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_math.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_metadata.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_raw.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_section.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_table.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.1.8/tests/libraries/panflute/test_tex.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.1.8/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.1.8/README.md
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 panpdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.2.0/.gitattributes
+-rw-r--r--   0        0        0    51052 2020-02-02 00:00:00.000000 panpdf-0.2.0/a.tex
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 panpdf-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.2.0/ruff_defaults.toml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/postCreate.sh
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/starship.toml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/features/zotero/devcontainer-feature.json
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/features/zotero/install.sh
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/defaults.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-after-body.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-before-body.tex
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-in-header.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/images/figure.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/images/header.tex
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/src/1.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/src/2.md
+-rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/pdf.ipynb
+-rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/pgf.ipynb
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/png.ipynb
+-rw-r--r--   0        0        0    54307 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/seaborn.ipynb
+-rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/svg.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/__init__.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/formatters.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/main.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/stores.py
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/attribute.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/crossref.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/filter.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/jupyter.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/layout.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/verbatim.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_converters.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_formatters.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_stores.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/conftest.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_attribute.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_crossref.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_filter.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_jupyter.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_layout.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_verbatim.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/test_nbformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_cite.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_code.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_figure.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_math.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_metadata.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_raw.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_section.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_table.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_tex.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.2.0/README.md
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 panpdf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.2.0/PKG-INFO
```

### Comparing `panpdf-0.1.8/mkdocs.yml` & `panpdf-0.2.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,10 @@
   - pymdownx.highlight:
       use_pygments: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
   - pymdownx.tabbed:
       alternate_style: true
+  - mkdocs-typer
 nav:
   - index.md
```

### Comparing `panpdf-0.1.8/ruff_defaults.toml` & `panpdf-0.2.0/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/.devcontainer/devcontainer.json` & `panpdf-0.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/.devcontainer/starship.toml` & `panpdf-0.2.0/.devcontainer/starship.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/examples/defaults.yaml` & `panpdf-0.2.0/examples/defaults.yaml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/examples/include-in-header.tex` & `panpdf-0.2.0/examples/include-in-header.tex`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/examples/src/1.md` & `panpdf-0.2.0/examples/src/1.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/notebooks/pdf.ipynb` & `panpdf-0.2.0/notebooks/pdf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/notebooks/pgf.ipynb` & `panpdf-0.2.0/notebooks/pgf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/notebooks/png.ipynb` & `panpdf-0.2.0/notebooks/png.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/notebooks/svg.ipynb` & `panpdf-0.2.0/notebooks/svg.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/main.py` & `panpdf-0.2.0/src/panpdf/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
 class OutputFormat(str, Enum):
     latex = "latex"
     pdf = "pdf"
     auto = "auto"
 
 
+app = typer.Typer(add_completion=False)
+
+
+@app.command(name="panpdf")
 def cli(
     files: Annotated[
         Optional[list[Path]],
         Argument(
             help="Input files or directories.",
             show_default=False,
         ),
@@ -143,28 +147,14 @@
         bool,
         Option(
             "--quiet",
             help="Suppress warning messages.",
             is_flag=True,
         ),
     ] = False,
-    # host: Annotated[
-    #     str,
-    #     Option(
-    #         help="IP address.",
-    #         hidden=True,
-    #     ),
-    # ] = "localhost",
-    # port: Annotated[
-    #     int,
-    #     Option(
-    #         help="Port.",
-    #         hidden=True,
-    #     ),
-    # ] = 23119,
     version: Annotated[
         bool,
         Option(
             "--version",
             "-v",
             help="Show version and exit.",
         ),
@@ -301,20 +291,20 @@
 
     typer.echo(f"pandoc {pandoc_version}")
     typer.echo(f"panflute {pf.__version__}")
     typer.echo(f"panpdf {__version__}")
     raise typer.Exit
 
 
-def main():
-    typer.run(cli)  # no cov
+# def main():
+#     typer.run(cli)  # no cov
 
 
-if __name__ == "__main__":
-    main()  # no cov
+# if __name__ == "__main__":
+#     main()  # no cov
 
 # def convert_notebook(path: str):
 #     nb = nbformat.read(path, as_version=4)
 #     ids = get_ids(nb, "fig")
 #     notebook_dir, path = os.path.split(path)
 #     if not notebook_dir:
 #         notebook_dir = "."
```

### Comparing `panpdf-0.1.8/src/panpdf/stores.py` & `panpdf-0.2.0/src/panpdf/stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/tools.py` & `panpdf-0.2.0/src/panpdf/tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/attribute.py` & `panpdf-0.2.0/src/panpdf/filters/attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/crossref.py` & `panpdf-0.2.0/src/panpdf/filters/crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/filter.py` & `panpdf-0.2.0/src/panpdf/filters/filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/jupyter.py` & `panpdf-0.2.0/src/panpdf/filters/jupyter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/layout.py` & `panpdf-0.2.0/src/panpdf/filters/layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/verbatim.py` & `panpdf-0.2.0/src/panpdf/filters/verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/src/panpdf/filters/zotero.py` & `panpdf-0.2.0/src/panpdf/filters/zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/conftest.py` & `panpdf-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/test_converters.py` & `panpdf-0.2.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/test_formatters.py` & `panpdf-0.2.0/tests/test_formatters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import io
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+import seaborn.objects as so
 from IPython.core.formatters import PlainTextFormatter
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.lib.pretty import RepresentationPrinter
 
 mpl.use("agg")
 
 
@@ -40,14 +41,47 @@
 
     elif fmt == "svg":
         xml = function(fig)
         assert isinstance(xml, str)
         assert xml.startswith('<?xml version="1.0"')
 
 
+def test_seaborn_plot(fmt):
+    from panpdf.formatters import FUNCTIONS
+
+    if fmt == "png":
+        return
+
+    functions = FUNCTIONS.get(("seaborn._core.plot", "Plot"))
+    assert functions
+    function = functions.get(fmt)
+    assert function
+
+    p = so.Plot()
+
+    if fmt == "pgf":
+        out = io.StringIO()
+        rp = RepresentationPrinter(out)
+
+        function(p, rp, None)
+        text = out.getvalue()
+        assert text.startswith("%% Creator: Matplotlib, PGF backend")
+        assert text.endswith("\\endgroup%\n")
+
+    elif fmt == "pdf":
+        data = function(p)
+        assert isinstance(data, bytes)
+        assert base64.b64encode(data).decode().startswith("JVBER")
+
+    elif fmt == "svg":
+        xml = function(p)
+        assert isinstance(xml, str)
+        assert xml.startswith('<?xml version="1.0"')
+
+
 def test_set_formatter():
     from panpdf.formatters import matplotlib_figure_to_pgf, set_formatter
 
     ip = InteractiveShell()
     set_formatter("matplotlib", "pgf", ip)
     formatter = ip.display_formatter.formatters["text/plain"]  # type:ignore
     assert isinstance(formatter, PlainTextFormatter)
```

### Comparing `panpdf-0.1.8/tests/test_main.py` & `panpdf-0.2.0/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import sys
 from pathlib import Path
 
 import pytest
 import typer
 from typer.testing import CliRunner
 
-from panpdf.main import cli
+from panpdf.main import app
 
 runner = CliRunner()
-app = typer.Typer()
-app.command()(cli)
 
 
 def test_version():
     result = runner.invoke(app, ["--version"])
     assert result.exit_code == 0
     for name in ["pandoc", "panflute", "panpdf"]:
         assert f"{name} " in result.stdout
```

### Comparing `panpdf-0.1.8/tests/test_stores.py` & `panpdf-0.2.0/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/test_tools.py` & `panpdf-0.2.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_attribute.py` & `panpdf-0.2.0/tests/filters/test_attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_crossref.py` & `panpdf-0.2.0/tests/filters/test_crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_filter.py` & `panpdf-0.2.0/tests/filters/test_filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_jupyter.py` & `panpdf-0.2.0/tests/filters/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_layout.py` & `panpdf-0.2.0/tests/filters/test_layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_verbatim.py` & `panpdf-0.2.0/tests/filters/test_verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/filters/test_zotero.py` & `panpdf-0.2.0/tests/filters/test_zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/test_nbformat.py` & `panpdf-0.2.0/tests/libraries/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_cite.py` & `panpdf-0.2.0/tests/libraries/panflute/test_cite.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_code.py` & `panpdf-0.2.0/tests/libraries/panflute/test_code.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_figure.py` & `panpdf-0.2.0/tests/libraries/panflute/test_figure.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_math.py` & `panpdf-0.2.0/tests/libraries/panflute/test_math.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_metadata.py` & `panpdf-0.2.0/tests/libraries/panflute/test_metadata.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_raw.py` & `panpdf-0.2.0/tests/libraries/panflute/test_raw.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_section.py` & `panpdf-0.2.0/tests/libraries/panflute/test_section.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_table.py` & `panpdf-0.2.0/tests/libraries/panflute/test_table.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/tests/libraries/panflute/test_tex.py` & `panpdf-0.2.0/tests/libraries/panflute/test_tex.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/LICENSE.txt` & `panpdf-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/README.md` & `panpdf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.8/pyproject.toml` & `panpdf-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,28 +33,29 @@
 
 [project.urls]
 Documentation = "https://daizutabi.github.io/panpdf"
 Source = "https://github.com/daizutabi/panpdf"
 Issues = "https://github.com/daizutabi/panpdf/issues"
 
 [project.scripts]
-panpdf = "panpdf.main:main"
+panpdf = "panpdf.main:app"
 
 [tool.hatch.version]
 path = "src/panpdf/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github", "/docs"]
 [tool.hatch.build.targets.wheel]
 packages = ["src/panpdf"]
 
 [tool.hatch.envs.test]
 dependencies = [
   "cairosvg",
   "matplotlib",
+  "pandas",
   "pytest-cov",
   "pytest-randomly",
   "seaborn",
 ]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest {args:tests src/panpdf}"
@@ -77,15 +78,15 @@
 [tool.coverage.run]
 omit = ["src/panpdf/__about__.py"]
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "raise NotImplementedError", "if TYPE_CHECKING:"]
 
 [tool.hatch.envs.docs]
-dependencies = ["mkdocs-material"]
+dependencies = ["mkdocs-material", "mkdocs-typer"]
 python = "3.12"
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict {args}"
 serve = "mkdocs serve --dev-addr localhost:8000 {args}"
 deploy = "mkdocs gh-deploy --force"
```

### Comparing `panpdf-0.1.8/PKG-INFO` & `panpdf-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpdf
-Version: 0.1.8
+Version: 0.2.0
 Summary: PDF documentation generator
 Project-URL: Documentation, https://daizutabi.github.io/panpdf
 Project-URL: Source, https://github.com/daizutabi/panpdf
 Project-URL: Issues, https://github.com/daizutabi/panpdf/issues
 Author-email: daizutabi <daizutabi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

