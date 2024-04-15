# Comparing `tmp/jupyterlab_translate-1.3.5.tar.gz` & `tmp/jupyterlab_translate-1.3.6.tar.gz`

## Comparing `jupyterlab_translate-1.3.5.tar` & `jupyterlab_translate-1.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/RELEASE.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/package.json
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/yarn.lock
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/.github/workflows/release_publish.yml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/__init__.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/api.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/cli.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/constants.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/contributors.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/converters.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/finder.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/gettext_extract.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/hooks.py
--rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/index.js
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/plugin.py
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/pybabel_config.cfg
--rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/jupyterlab_translate/utils.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/dummy_pkg.patch
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/example.json
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/test_hatch_hook.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/test_utils.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/dummy_pkg/locale/dummy_pkg.pot
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/tests/dummy_pkg/src/documentwidget.ts
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/RELEASE.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/package.json
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/yarn.lock
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.github/workflows/release_publish.yml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/__init__.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/api.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/cli.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/constants.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/contributors.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/converters.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/finder.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/gettext_extract.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/hooks.py
+-rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/index.js
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/plugin.py
+-rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/pybabel_config.cfg
+-rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/utils.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg.patch
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/example.json
+-rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/test_hatch_hook.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/test_utils.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg/locale/dummy_pkg.pot
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg/src/documentwidget.ts
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/README.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/PKG-INFO
```

### Comparing `jupyterlab_translate-1.3.5/CONTRIBUTING.md` & `jupyterlab_translate-1.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/package.json` & `jupyterlab_translate-1.3.6/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/yarn.lock` & `jupyterlab_translate-1.3.6/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/.github/workflows/release_publish.yml` & `jupyterlab_translate-1.3.6/.github/workflows/release_publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 
 permissions:
   contents: write
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    permissions:
+      # IMPORTANT: this permission is mandatory for the release-action
+      contents: write
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.10'
+        python-version: '3.12'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade twine build
     - name: Build release
       run: |
         python -m build
         python -m twine check dist/*
     - name: Create Release
       id: create_release
-      uses: ncipollo/release-action@c4bf6c1ab090090498fb7f3ddc9f99ba5ab619b9
+      uses: ncipollo/release-action@4f8867fa5eec0b3f59ead8f69aeba316c24907b3
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag: ${{ env.GITHUB_REF }}
         name: ${{ env.GITHUB_REF }}
         artifacts: 'dist/*'
         body: Release ${{ env.GITHUB_REF }}
         token: ${{ secrets.GITHUB_TOKEN }}
-    - name: Publish PyPI Package
-      env:
-        TWINE_USERNAME: __token__
-        TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
-      run: |
-        python -m twine upload dist/*
+
+    - name: Publish package distributions to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
+
```

### Comparing `jupyterlab_translate-1.3.5/.github/workflows/tests.yml` & `jupyterlab_translate-1.3.6/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
   pull_request:
     branches: ['main']
 
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install gettext
       run: sudo apt-get install gettext
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.10'
+        python-version: '3.12'
     - name: Install in develop mode
       run: |
         pip install -e ".[test]"
     - name: Style checks
       run: |
         pre-commit run -a
     - name: Run tests
```

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/api.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/cli.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/cli.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/constants.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/contributors.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/contributors.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/converters.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/converters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/finder.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/finder.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/index.js` & `jupyterlab_translate-1.3.6/jupyterlab_translate/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/plugin.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/plugin.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/jupyterlab_translate/utils.py` & `jupyterlab_translate-1.3.6/jupyterlab_translate/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/tests/dummy_pkg.patch` & `jupyterlab_translate-1.3.6/tests/dummy_pkg.patch`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/tests/example.json` & `jupyterlab_translate-1.3.6/tests/example.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/tests/test_hatch_hook.py` & `jupyterlab_translate-1.3.6/tests/test_hatch_hook.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/tests/test_utils.py` & `jupyterlab_translate-1.3.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/tests/dummy_pkg/src/documentwidget.ts` & `jupyterlab_translate-1.3.6/tests/dummy_pkg/src/documentwidget.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/.gitignore` & `jupyterlab_translate-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/LICENSE.txt` & `jupyterlab_translate-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/README.md` & `jupyterlab_translate-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.5/pyproject.toml` & `jupyterlab_translate-1.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 keywords = ["hatch", "jupyterlab", "language", "localization"]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "importlib-metadata>=4.8.3;python_version<\"3.10\"",
     "babel",
     "click",
-    "copier>=7.0.0",
+    "copier>=9.2.0",
     "copier-templates-extensions",
     "crowdin-api-client",
     "hatchling>=1.5",
     "jinja2-time",
     "polib",
-    "pydantic<2.0.0",
+    "pydantic",
     "requests"
 ]
 
 [project.optional-dependencies]
 test = [
     "hatch",
     "pre-commit",
```

### Comparing `jupyterlab_translate-1.3.5/PKG-INFO` & `jupyterlab_translate-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab-translate
-Version: 1.3.5
+Version: 1.3.6
 Summary: JupyterLab Language Pack Translations Helper
 Project-URL: homepage, https://github.com/jupyterlab/jupyterlab-translate
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2020 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -39,21 +39,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: babel
 Requires-Dist: click
 Requires-Dist: copier-templates-extensions
-Requires-Dist: copier>=7.0.0
+Requires-Dist: copier>=9.2.0
 Requires-Dist: crowdin-api-client
 Requires-Dist: hatchling>=1.5
 Requires-Dist: importlib-metadata>=4.8.3; python_version < '3.10'
 Requires-Dist: jinja2-time
 Requires-Dist: polib
-Requires-Dist: pydantic<2.0.0
+Requires-Dist: pydantic
 Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: hatch; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

