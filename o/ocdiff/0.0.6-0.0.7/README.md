# Comparing `tmp/ocdiff-0.0.6.tar.gz` & `tmp/ocdiff-0.0.7.tar.gz`

## Comparing `ocdiff-0.0.6.tar` & `ocdiff-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 ocdiff-0.0.6/Cargo.toml
--rw-r--r--   0      501       20     2728 2024-04-08 10:26:05.000000 ocdiff-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0      501       20     3097 2024-04-08 10:26:05.000000 ocdiff-0.0.6/.gitignore
--rw-r--r--   0      501       20     1071 2024-04-08 10:26:05.000000 ocdiff-0.0.6/LICENSE
--rw-r--r--   0      501       20      551 2024-04-08 10:26:05.000000 ocdiff-0.0.6/README.md
--rw-r--r--   0      501       20      139 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/__init__.py
--rw-r--r--   0      501       20      152 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/__init__.pyi
--rw-r--r--   0      501       20     1505 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/helpers.py
--rw-r--r--   0      501       20     8914 2024-04-08 10:26:05.000000 ocdiff-0.0.6/src/lib.rs
--rw-r--r--   0      501       20      788 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/a.json
--rw-r--r--   0      501       20      737 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/b.json
--rw-r--r--   0      501       20     4398 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/expected.html
--rw-r--r--   0      501       20      369 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/test_ocdiff.py
--rw-r--r--   0      501       20     8716 2024-04-08 10:26:05.000000 ocdiff-0.0.6/Cargo.lock
--rw-r--r--   0      501       20     1283 2024-04-08 10:26:05.000000 ocdiff-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 ocdiff-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 ocdiff-0.0.7/Cargo.toml
+-rw-r--r--   0      501       20     2729 2024-04-08 10:29:48.000000 ocdiff-0.0.7/.github/workflows/ci.yml
+-rw-r--r--   0      501       20     3097 2024-04-08 10:29:48.000000 ocdiff-0.0.7/.gitignore
+-rw-r--r--   0      501       20     1071 2024-04-08 10:29:48.000000 ocdiff-0.0.7/LICENSE
+-rw-r--r--   0      501       20      551 2024-04-08 10:29:48.000000 ocdiff-0.0.7/README.md
+-rw-r--r--   0      501       20      139 2024-04-08 10:29:48.000000 ocdiff-0.0.7/python/ocdiff/__init__.py
+-rw-r--r--   0      501       20      152 2024-04-08 10:29:48.000000 ocdiff-0.0.7/python/ocdiff/__init__.pyi
+-rw-r--r--   0      501       20     1505 2024-04-08 10:29:48.000000 ocdiff-0.0.7/python/ocdiff/helpers.py
+-rw-r--r--   0      501       20     8914 2024-04-08 10:29:48.000000 ocdiff-0.0.7/src/lib.rs
+-rw-r--r--   0      501       20      788 2024-04-08 10:29:48.000000 ocdiff-0.0.7/tests/a.json
+-rw-r--r--   0      501       20      737 2024-04-08 10:29:48.000000 ocdiff-0.0.7/tests/b.json
+-rw-r--r--   0      501       20     4398 2024-04-08 10:29:48.000000 ocdiff-0.0.7/tests/expected.html
+-rw-r--r--   0      501       20      369 2024-04-08 10:29:48.000000 ocdiff-0.0.7/tests/test_ocdiff.py
+-rw-r--r--   0      501       20     8716 2024-04-08 10:29:48.000000 ocdiff-0.0.7/Cargo.lock
+-rw-r--r--   0      501       20     1283 2024-04-08 10:29:48.000000 ocdiff-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 ocdiff-0.0.7/PKG-INFO
```

### Comparing `ocdiff-0.0.6/.github/workflows/ci.yml` & `ocdiff-0.0.7/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 jobs:
   build:
     name: build py${{ matrix.python-version }} on ${{ matrix.platform || matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
+          - ubuntu
           - macos
-          - linux
           - windows
         python-version:
           - '3.11'
         include:
           - os: ubuntu
             platform: linux
           - os: windows
```

### Comparing `ocdiff-0.0.6/.gitignore` & `ocdiff-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/LICENSE` & `ocdiff-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/README.md` & `ocdiff-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/python/ocdiff/helpers.py` & `ocdiff-0.0.7/python/ocdiff/helpers.py`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/src/lib.rs` & `ocdiff-0.0.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/tests/a.json` & `ocdiff-0.0.7/tests/a.json`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/tests/b.json` & `ocdiff-0.0.7/tests/b.json`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/tests/expected.html` & `ocdiff-0.0.7/tests/expected.html`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/Cargo.lock` & `ocdiff-0.0.7/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.6/pyproject.toml` & `ocdiff-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ocdiff"
-version = "0.0.6"
+version = "0.0.7"
 description = "difftastic Python wrapper"
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 keywords = ["diff"]
 authors = [{ name = "Oliver Russell", email = "ojhrussell@gmail.com" }]
 maintainers = [{ name = "Oliver Russell", email = "ojhrussell@gmail.com" }]
```

### Comparing `ocdiff-0.0.6/PKG-INFO` & `ocdiff-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ocdiff
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Python
 Requires-Dist: maturin ==1.4.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'dev'
 Requires-Dist: mypy ==1.6.* ; extra == 'dev'
 Requires-Dist: pip ==24.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
```

