# Comparing `tmp/spreadsheetsmalldemo-0.0.4.tar.gz` & `tmp/spreadsheetsmalldemo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spreadsheetsmalldemo-0.0.4.tar", last modified: Mon Apr  8 12:32:36 2024, max compression
+gzip compressed data, was "spreadsheetsmalldemo-0.0.5.tar", last modified: Mon Apr 15 19:54:23 2024, max compression
```

## Comparing `spreadsheetsmalldemo-0.0.4.tar` & `spreadsheetsmalldemo-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 12:32:36.248197 spreadsheetsmalldemo-0.0.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 spreadsheetsmalldemo-0.0.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1292 2024-04-08 12:32:36.248197 spreadsheetsmalldemo-0.0.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      735 2024-04-07 20:01:50.000000 spreadsheetsmalldemo-0.0.4/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-08 12:32:36.248197 spreadsheetsmalldemo-0.0.4/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1069 2024-04-08 12:32:33.000000 spreadsheetsmalldemo-0.0.4/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 12:32:36.248197 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       55 2024-04-08 12:27:52.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      489 2024-04-08 12:26:11.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo/definition.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 12:32:36.248197 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1292 2024-04-08 12:32:36.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      313 2024-04-08 12:32:36.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-08 12:32:36.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        7 2024-04-08 12:32:36.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-04-08 12:32:36.000000 spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 19:54:23.925763 spreadsheetsmalldemo-0.0.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 spreadsheetsmalldemo-0.0.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1292 2024-04-15 19:54:23.925763 spreadsheetsmalldemo-0.0.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      735 2024-04-07 20:01:50.000000 spreadsheetsmalldemo-0.0.5/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-15 19:54:23.925763 spreadsheetsmalldemo-0.0.5/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1093 2024-04-15 19:54:07.000000 spreadsheetsmalldemo-0.0.5/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 19:54:23.921763 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      106 2024-04-15 19:53:29.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      489 2024-04-08 12:26:11.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/definition.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 19:54:23.925763 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/rpa/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-15 19:53:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/rpa/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 19:54:23.925763 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/rpa/ui/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       50 2024-04-15 19:53:29.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/rpa/ui/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      485 2024-04-15 19:51:43.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo/rpa/ui/ui.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 19:54:23.921763 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1292 2024-04-15 19:54:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      424 2024-04-15 19:54:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-15 19:54:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-04-15 19:54:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-04-15 19:54:23.000000 spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/top_level.txt
```

### Comparing `spreadsheetsmalldemo-0.0.4/LICENSE` & `spreadsheetsmalldemo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spreadsheetsmalldemo-0.0.4/PKG-INFO` & `spreadsheetsmalldemo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheetsmalldemo
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert WebElement into pdf
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spreadsheetsmalldemo-0.0.4/README.md` & `spreadsheetsmalldemo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spreadsheetsmalldemo-0.0.4/setup.py` & `spreadsheetsmalldemo-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Convert WebElement into pdf'
 LONG_DESCRIPTION = 'A package that allows to convert HTML into pdf'
 
 # Setting up
 setup(
     name="spreadsheetsmalldemo",
     version=VERSION,
     author="Daniel Rubens",
     author_email="danielrubensdaniel@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pandas'],
+    install_requires=['pandas', 'rpaframework==28.5.1'],
     keywords=['python', 'rpa', 'robocorp', 'pdf', 'html', 'conversor'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `spreadsheetsmalldemo-0.0.4/spreadsheetsmalldemo.egg-info/PKG-INFO` & `spreadsheetsmalldemo-0.0.5/spreadsheetsmalldemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheetsmalldemo
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert WebElement into pdf
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

