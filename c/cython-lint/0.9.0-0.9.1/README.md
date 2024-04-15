# Comparing `tmp/cython_lint-0.9.0.tar.gz` & `tmp/cython_lint-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cython_lint-0.9.0.tar", last modified: Thu Nov 24 15:28:41 2022, max compression
+gzip compressed data, was "cython_lint-0.9.1.tar", last modified: Thu Nov 24 15:35:54 2022, max compression
```

## Comparing `cython_lint-0.9.0.tar` & `cython_lint-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:28:41.522515 cython_lint-0.9.0/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2022-09-23 11:09:52.000000 cython_lint-0.9.0/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3004 2022-11-24 15:28:41.522515 cython_lint-0.9.0/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2442 2022-11-24 15:28:14.000000 cython_lint-0.9.0/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:28:41.522515 cython_lint-0.9.0/cython_lint.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3004 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      248 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      114 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/entry_points.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       47 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/requires.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       12 2022-11-24 15:28:41.000000 cython_lint-0.9.0/cython_lint.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1159 2022-11-24 15:28:41.522515 cython_lint-0.9.0/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       37 2022-09-23 11:09:52.000000 cython_lint-0.9.0/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:35:54.832516 cython_lint-0.9.1/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2022-09-23 11:09:52.000000 cython_lint-0.9.1/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3018 2022-11-24 15:35:54.832516 cython_lint-0.9.1/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2456 2022-11-24 15:35:39.000000 cython_lint-0.9.1/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:35:54.832516 cython_lint-0.9.1/cython_lint/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:21:03.000000 cython_lint-0.9.1/cython_lint/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    23945 2022-11-24 15:19:39.000000 cython_lint-0.9.1/cython_lint/cython_lint.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2535 2022-11-24 15:19:42.000000 cython_lint-0.9.1/cython_lint/string_fixer.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2022-11-24 15:35:54.832516 cython_lint-0.9.1/cython_lint.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3018 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      327 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      121 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/entry_points.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       47 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/requires.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       12 2022-11-24 15:35:54.000000 cython_lint-0.9.1/cython_lint.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1212 2022-11-24 15:35:54.832516 cython_lint-0.9.1/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       37 2022-09-23 11:09:52.000000 cython_lint-0.9.1/setup.py
```

### Comparing `cython_lint-0.9.0/LICENSE` & `cython_lint-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cython_lint-0.9.0/PKG-INFO` & `cython_lint-0.9.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cython_lint
-Version: 0.9.0
-Summary: A linter for Cython files
-Home-page: https://github.com/MarcoGorelli/cython-lint
-Author: Marco Gorelli
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://github.com/MarcoGorelli/cython-lint/workflows/tox/badge.svg)](https://github.com/MarcoGorelli/cython-lint/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcoGorelli/cython-lint)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/cython-lint/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/cython-lint/main)
 
 cython-lint
 ===========
 
@@ -33,18 +17,18 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/MarcoGorelli/cython-lint
-    rev: v0.9.0
+    rev: v0.9.1
     hooks:
     -   id: cython-lint
-    -   id: double-quote-strings
+    -   id: double-quote-cython-strings
 ```
 
 ## Command-line example
 
 ```console
 $ cython-lint my_file_1.pyx my_file_2.pyx
 my_file_1.pyx:54:5: 'get_conversion_factor' imported but unused
@@ -76,10 +60,10 @@
 - ``.strip``, ``.rstrip``, or ``.lstrip`` used with repeated characters
 - comparison between constants
 - late-binding closures https://docs.python-guide.org/writing/gotchas/#late-binding-closures
 - ``pycodestyle`` nitpicks, which you can turn off with ``--no-pycodestyle``
 
 In addition, the following automated fixers are implemented:
 
-- double-quote-strings (replace single quotes with double quotes, like the ``black`` formatter does)
+- double-quote-cython-strings (replace single quotes with double quotes, like the ``black`` formatter does)
 
 More to come! Requests welcome!
```

### Comparing `cython_lint-0.9.0/README.md` & `cython_lint-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: cython_lint
+Version: 0.9.1
+Summary: A linter for Cython files
+Home-page: https://github.com/MarcoGorelli/cython-lint
+Author: Marco Gorelli
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Build Status](https://github.com/MarcoGorelli/cython-lint/workflows/tox/badge.svg)](https://github.com/MarcoGorelli/cython-lint/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcoGorelli/cython-lint)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/cython-lint/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/cython-lint/main)
 
 cython-lint
 ===========
 
@@ -17,18 +33,18 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/MarcoGorelli/cython-lint
-    rev: v0.9.0
+    rev: v0.9.1
     hooks:
     -   id: cython-lint
-    -   id: double-quote-strings
+    -   id: double-quote-cython-strings
 ```
 
 ## Command-line example
 
 ```console
 $ cython-lint my_file_1.pyx my_file_2.pyx
 my_file_1.pyx:54:5: 'get_conversion_factor' imported but unused
@@ -60,10 +76,10 @@
 - ``.strip``, ``.rstrip``, or ``.lstrip`` used with repeated characters
 - comparison between constants
 - late-binding closures https://docs.python-guide.org/writing/gotchas/#late-binding-closures
 - ``pycodestyle`` nitpicks, which you can turn off with ``--no-pycodestyle``
 
 In addition, the following automated fixers are implemented:
 
-- double-quote-strings (replace single quotes with double quotes, like the ``black`` formatter does)
+- double-quote-cython-strings (replace single quotes with double quotes, like the ``black`` formatter does)
 
 More to come! Requests welcome!
```

### Comparing `cython_lint-0.9.0/cython_lint.egg-info/PKG-INFO` & `cython_lint-0.9.1/cython_lint.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cython-lint
-Version: 0.9.0
+Version: 0.9.1
 Summary: A linter for Cython files
 Home-page: https://github.com/MarcoGorelli/cython-lint
 Author: Marco Gorelli
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -33,18 +33,18 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/MarcoGorelli/cython-lint
-    rev: v0.9.0
+    rev: v0.9.1
     hooks:
     -   id: cython-lint
-    -   id: double-quote-strings
+    -   id: double-quote-cython-strings
 ```
 
 ## Command-line example
 
 ```console
 $ cython-lint my_file_1.pyx my_file_2.pyx
 my_file_1.pyx:54:5: 'get_conversion_factor' imported but unused
@@ -76,10 +76,10 @@
 - ``.strip``, ``.rstrip``, or ``.lstrip`` used with repeated characters
 - comparison between constants
 - late-binding closures https://docs.python-guide.org/writing/gotchas/#late-binding-closures
 - ``pycodestyle`` nitpicks, which you can turn off with ``--no-pycodestyle``
 
 In addition, the following automated fixers are implemented:
 
-- double-quote-strings (replace single quotes with double quotes, like the ``black`` formatter does)
+- double-quote-cython-strings (replace single quotes with double quotes, like the ``black`` formatter does)
 
 More to come! Requests welcome!
```

### Comparing `cython_lint-0.9.0/setup.cfg` & `cython_lint-0.9.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cython_lint
-version = 0.9.0
+version = 0.9.1
 description = A linter for Cython files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MarcoGorelli/cython-lint
 author = Marco Gorelli
 license = MIT
 license_file = LICENSE
@@ -12,25 +12,30 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
-py_modules = cython_lint
+packages = find:
 install_requires = 
 	cython>=0.29.32
 	pycodestyle
 	tokenize-rt>=3.2.0
 python_requires = >=3.7
 
+[options.packages.find]
+exclude = 
+	tests*
+	testing*
+
 [options.entry_points]
 console_scripts = 
 	cython-lint = cython_lint.cython_lint:main
-	double-quote-strings = cython_lint.string_fixer:main
+	double-quote-cython-strings = cython_lint.string_fixer:main
 
 [bdist_wheel]
 universal = True
 
 [coverage:run]
 plugins = covdefaults
```

