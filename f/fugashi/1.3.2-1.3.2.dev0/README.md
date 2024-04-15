# Comparing `tmp/fugashi-1.3.2.tar.gz` & `tmp/fugashi-1.3.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugashi-1.3.2.tar", last modified: Mon Apr 15 12:47:37 2024, max compression
+gzip compressed data, was "fugashi-1.3.2.dev0.tar", last modified: Mon Apr 15 12:34:50 2024, max compression
```

## Comparing `fugashi-1.3.2.tar` & `fugashi-1.3.2.dev0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.023190 fugashi-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.019190 fugashi-1.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/FUNDING.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1577 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/macos-build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.019190 fugashi-1.3.2/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.015190 fugashi-1.3.2/.github/workflows/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.019190 fugashi-1.3.2/.github/workflows/actions/build-manylinux/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/actions/build-manylinux/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.019190 fugashi-1.3.2/.github/workflows/actions/build-manylinux-aarch64/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/actions/build-manylinux-aarch64/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/manylinux1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/osx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/test_manylinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-15 12:46:12.000000 fugashi-1.3.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-15 12:46:12.000000 fugashi-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 12:46:12.000000 fugashi-1.3.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 12:46:12.000000 fugashi-1.3.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 12:46:12.000000 fugashi-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-15 12:46:12.000000 fugashi-1.3.2/LICENSE.mecab
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 12:46:12.000000 fugashi-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-15 12:47:37.023190 fugashi-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-15 12:46:12.000000 fugashi-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.023190 fugashi-1.3.2/fugashi/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14166 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/fugashi.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.015190 fugashi-1.3.2/fugashi/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.023190 fugashi-1.3.2/fugashi/include/mecab/
--rw-r--r--   0 runner    (1001) docker     (127)    42106 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/include/mecab/mecab.h
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/mecab.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.023190 fugashi-1.3.2/fugashi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/tests/test_ipadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi/tests/test_nbest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:47:37.023190 fugashi-1.3.2/fugashi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-15 12:47:36.000000 fugashi-1.3.2/fugashi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-15 12:47:37.000000 fugashi-1.3.2/fugashi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:47:36.000000 fugashi-1.3.2/fugashi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 12:47:36.000000 fugashi-1.3.2/fugashi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 12:47:36.000000 fugashi-1.3.2/fugashi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 12:47:36.000000 fugashi-1.3.2/fugashi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   310109 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi.png
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-15 12:46:12.000000 fugashi-1.3.2/fugashi_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 12:46:12.000000 fugashi-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-15 12:47:37.023190 fugashi-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-15 12:46:12.000000 fugashi-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.964550 fugashi-1.3.2.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/FUNDING.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1577 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/macos-build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.964550 fugashi-1.3.2.dev0/.github/workflows/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/.github/workflows/actions/build-manylinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/actions/build-manylinux/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/.github/workflows/actions/build-manylinux-aarch64/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/actions/build-manylinux-aarch64/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/manylinux1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/osx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/test_manylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/LICENSE.mecab
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/fugashi/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14166 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/fugashi.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.964550 fugashi-1.3.2.dev0/fugashi/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/fugashi/include/mecab/
+-rw-r--r--   0 runner    (1001) docker     (127)    42106 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/include/mecab/mecab.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/mecab.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/fugashi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/tests/test_ipadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi/tests/test_nbest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:34:50.968550 fugashi-1.3.2.dev0/fugashi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 12:34:50.000000 fugashi-1.3.2.dev0/fugashi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   310109 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/fugashi_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-15 12:34:50.972550 fugashi-1.3.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-15 12:32:39.000000 fugashi-1.3.2.dev0/setup.py
```

### Comparing `fugashi-1.3.2/.github/macos-build.sh` & `fugashi-1.3.2.dev0/.github/macos-build.sh`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.github/workflows/entrypoint.sh` & `fugashi-1.3.2.dev0/.github/workflows/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.github/workflows/manylinux1.yml` & `fugashi-1.3.2.dev0/.github/workflows/manylinux1.yml`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.github/workflows/osx.yml` & `fugashi-1.3.2.dev0/.github/workflows/osx.yml`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.github/workflows/test_manylinux.yml` & `fugashi-1.3.2.dev0/.github/workflows/test_manylinux.yml`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.github/workflows/windows.yml` & `fugashi-1.3.2.dev0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/.gitignore` & `fugashi-1.3.2.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/LICENSE` & `fugashi-1.3.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/LICENSE.mecab` & `fugashi-1.3.2.dev0/LICENSE.mecab`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/PKG-INFO` & `fugashi-1.3.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugashi
-Version: 1.3.2
+Version: 1.3.2.dev0
 Summary: A Cython MeCab wrapper for fast, pythonic Japanese tokenization.
 Home-page: https://github.com/polm/fugashi
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
```

### Comparing `fugashi-1.3.2/README.md` & `fugashi-1.3.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/cli.py` & `fugashi-1.3.2.dev0/fugashi/cli.py`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/fugashi.pyx` & `fugashi-1.3.2.dev0/fugashi/fugashi.pyx`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/include/mecab/mecab.h` & `fugashi-1.3.2.dev0/fugashi/include/mecab/mecab.h`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/mecab.pxd` & `fugashi-1.3.2.dev0/fugashi/mecab.pxd`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/tests/test_basic.py` & `fugashi-1.3.2.dev0/fugashi/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/tests/test_ipadic.py` & `fugashi-1.3.2.dev0/fugashi/tests/test_ipadic.py`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi/tests/test_nbest.py` & `fugashi-1.3.2.dev0/fugashi/tests/test_nbest.py`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi.egg-info/PKG-INFO` & `fugashi-1.3.2.dev0/fugashi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugashi
-Version: 1.3.2
+Version: 1.3.2.dev0
 Summary: A Cython MeCab wrapper for fast, pythonic Japanese tokenization.
 Home-page: https://github.com/polm/fugashi
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
```

### Comparing `fugashi-1.3.2/fugashi.egg-info/SOURCES.txt` & `fugashi-1.3.2.dev0/fugashi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi.png` & `fugashi-1.3.2.dev0/fugashi.png`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/fugashi_util.py` & `fugashi-1.3.2.dev0/fugashi_util.py`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/setup.cfg` & `fugashi-1.3.2.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugashi-1.3.2/setup.py` & `fugashi-1.3.2.dev0/setup.py`

 * *Files identical despite different names*

