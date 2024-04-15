# Comparing `tmp/utubes-0.0.2.tar.gz` & `tmp/utubes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.2.tar", last modified: Mon Apr 15 16:06:31 2024, max compression
+gzip compressed data, was "utubes-0.0.3.tar", last modified: Mon Apr 15 16:46:43 2024, max compression
```

## Comparing `utubes-0.0.2.tar` & `utubes-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.260479 utubes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 16:06:26.000000 utubes-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 16:06:31.260479 utubes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 16:06:26.000000 utubes-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:06:31.260479 utubes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-15 16:06:26.000000 utubes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.260479 utubes-0.0.2/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:46:43.281579 utubes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 16:46:36.000000 utubes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 16:46:43.281579 utubes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 16:46:36.000000 utubes-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:46:43.277579 utubes-0.0.3/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:46:43.277579 utubes-0.0.3/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:46:43.277579 utubes-0.0.3/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 16:46:36.000000 utubes-0.0.3/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:46:43.281579 utubes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-15 16:46:36.000000 utubes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:46:43.281579 utubes-0.0.3/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 16:46:43.000000 utubes-0.0.3/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 16:46:43.000000 utubes-0.0.3/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:46:43.000000 utubes-0.0.3/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:46:43.000000 utubes-0.0.3/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 16:46:43.000000 utubes-0.0.3/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.2/LICENSE` & `utubes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.2/PKG-INFO` & `utubes-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.2
+Version: 0.0.3
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
-Keywords: python,youtube,monisha
+Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.2 Summary: ã¤ Home-page:
-https://github.com/Monisha License: MIT Keywords: python,youtube,monisha
+Metadata-Version: 2.1 Name: utubes Version: 0.0.3 Summary: ã¤ Home-page:
+https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
```

### Comparing `utubes-0.0.2/Utube/functions/function01.py` & `utubes-0.0.3/Utube/functions/function01.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.2/utubes.egg-info/PKG-INFO` & `utubes-0.0.3/utubes.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.2
+Version: 0.0.3
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
-Keywords: python,youtube,monisha
+Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.2 Summary: ã¤ Home-page:
-https://github.com/Monisha License: MIT Keywords: python,youtube,monisha
+Metadata-Version: 2.1 Name: utubes Version: 0.0.3 Summary: ã¤ Home-page:
+https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
```

