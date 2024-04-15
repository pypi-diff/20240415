# Comparing `tmp/comparable_pattern-0.0.3.tar.gz` & `tmp/comparable_pattern-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comparable_pattern-0.0.3.tar", last modified: Mon Apr 15 12:30:41 2024, max compression
+gzip compressed data, was "comparable_pattern-0.0.4.tar", last modified: Mon Apr 15 13:14:09 2024, max compression
```

## Comparing `comparable_pattern-0.0.3.tar` & `comparable_pattern-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.814871 comparable_pattern-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/ci-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/mypy-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/src/_comparable_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/src/comparable_pattern.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 12:30:41.000000 comparable_pattern-0.0.3/src/comparable_pattern.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-15 12:30:41.000000 comparable_pattern-0.0.3/src/comparable_pattern.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:30:41.000000 comparable_pattern-0.0.3/src/comparable_pattern.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 12:30:41.000000 comparable_pattern-0.0.3/src/comparable_pattern.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/src/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 12:30:41.000000 comparable_pattern-0.0.3/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:41.818871 comparable_pattern-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/test/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:30.000000 comparable_pattern-0.0.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.579646 comparable_pattern-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/ci-constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/mypy-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.579646 comparable_pattern-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/src/comparable_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/src/comparable_pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/src/comparable_pattern/_comparable_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/src/comparable_pattern/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 13:14:09.000000 comparable_pattern-0.0.4/src/comparable_pattern/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/src/comparable_pattern.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 13:14:09.000000 comparable_pattern-0.0.4/src/comparable_pattern.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-15 13:14:09.000000 comparable_pattern-0.0.4/src/comparable_pattern.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:14:09.000000 comparable_pattern-0.0.4/src/comparable_pattern.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 13:14:09.000000 comparable_pattern-0.0.4/src/comparable_pattern.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:14:09.583646 comparable_pattern-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/test/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:13:56.000000 comparable_pattern-0.0.4/test-requirements.txt
```

### Comparing `comparable_pattern-0.0.3/.github/workflows/publish.yml` & `comparable_pattern-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `comparable_pattern-0.0.3/.github/workflows/test.yml` & `comparable_pattern-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `comparable_pattern-0.0.3/.gitignore` & `comparable_pattern-0.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 # Pyre type checker
 .pyre/
 
 .idea/
 *.iml
 .vscode/
 
-src/version.py
+version.py
```

### Comparing `comparable_pattern-0.0.3/LICENSE` & `comparable_pattern-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comparable_pattern-0.0.3/PKG-INFO` & `comparable_pattern-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comparable_pattern
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comparable string / regex object for flexible string comparisons.
 Author-email: Rudolf Byker <rudolfbyker@gmail.com>
 Project-URL: repository, https://github.com/AutoActuary/comparable_pattern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `comparable_pattern-0.0.3/README.md` & `comparable_pattern-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `comparable_pattern-0.0.3/pyproject.toml` & `comparable_pattern-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 ]
 requires-python = ">=3.11"  # TODO: Might work with earlier versions. Test it.
 
 [project.urls]
 repository = "https://github.com/AutoActuary/comparable_pattern"
 
 [tool.setuptools_scm]
-write_to = "src/version.py"
+write_to = "src/comparable_pattern/version.py"
```

### Comparing `comparable_pattern-0.0.3/src/_comparable_pattern.py` & `comparable_pattern-0.0.4/src/comparable_pattern/_comparable_pattern.py`

 * *Files identical despite different names*

### Comparing `comparable_pattern-0.0.3/src/comparable_pattern.egg-info/PKG-INFO` & `comparable_pattern-0.0.4/src/comparable_pattern.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comparable_pattern
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comparable string / regex object for flexible string comparisons.
 Author-email: Rudolf Byker <rudolfbyker@gmail.com>
 Project-URL: repository, https://github.com/AutoActuary/comparable_pattern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `comparable_pattern-0.0.3/src/comparable_pattern.egg-info/SOURCES.txt` & `comparable_pattern-0.0.4/src/comparable_pattern.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 mypy.ini
 pyproject.toml
 test-requirements.txt
 .github/workflows/black.yml
 .github/workflows/mypy.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
-src/__init__.py
-src/_comparable_pattern.py
-src/py.typed
-src/version.py
+src/comparable_pattern/__init__.py
+src/comparable_pattern/_comparable_pattern.py
+src/comparable_pattern/py.typed
+src/comparable_pattern/version.py
 src/comparable_pattern.egg-info/PKG-INFO
 src/comparable_pattern.egg-info/SOURCES.txt
 src/comparable_pattern.egg-info/dependency_links.txt
 src/comparable_pattern.egg-info/top_level.txt
 test/__init__.py
 test/test_doctests.py
```

### Comparing `comparable_pattern-0.0.3/test/test_doctests.py` & `comparable_pattern-0.0.4/test/test_doctests.py`

 * *Files identical despite different names*

