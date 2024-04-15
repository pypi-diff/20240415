# Comparing `tmp/switchinglogfilehandlers-0.0.4.tar.gz` & `tmp/switchinglogfilehandlers-0.0.5.tar.gz`

## Comparing `switchinglogfilehandlers-0.0.4.tar` & `switchinglogfilehandlers-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-31.log
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-32.log
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-33.log
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2023-08-07-12-22.log
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2023-08-07-12-23.log
--rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit
--rwxr-xr-x   0        0        0     1613 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit2
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit3
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo/bar/baz.2023-08-07-12-31.log
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo/bar/baz.2023-08-07-12-32.log
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/src/switchinglogfilehandlers/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/LICENSE
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-31.log
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-32.log
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-33.log
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo.2023-08-07-12-22.log
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo.2023-08-07-12-23.log
+-rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/testit
+-rwxr-xr-x   0        0        0     1613 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/testit2
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/testit3
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo/bar/baz.2023-08-07-12-31.log
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/foo/bar/baz.2023-08-07-12-32.log
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/src/switchinglogfilehandlers/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.5/PKG-INFO
```

### Comparing `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-31.log` & `switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-31.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-32.log` & `switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-32.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-33.log` & `switchinglogfilehandlers-0.0.5/foo.2022-12-10-21-33.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/foo.2023-08-07-12-22.log` & `switchinglogfilehandlers-0.0.5/foo.2023-08-07-12-22.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/testit` & `switchinglogfilehandlers-0.0.5/testit`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/testit2` & `switchinglogfilehandlers-0.0.5/testit2`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/testit3` & `switchinglogfilehandlers-0.0.5/testit3`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/foo/bar/baz.2023-08-07-12-31.log` & `switchinglogfilehandlers-0.0.5/foo/bar/baz.2023-08-07-12-31.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/src/switchinglogfilehandlers/__init__.py` & `switchinglogfilehandlers-0.0.5/src/switchinglogfilehandlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/LICENSE` & `switchinglogfilehandlers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.4/pyproject.toml` & `switchinglogfilehandlers-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "switchinglogfilehandlers"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Peter J. Holzer", email="hjp@hjp.at" },
 ]
 description = "A collection of switching log file handlers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

