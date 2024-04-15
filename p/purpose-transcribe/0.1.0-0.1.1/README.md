# Comparing `tmp/purpose_transcribe-0.1.0.tar.gz` & `tmp/purpose_transcribe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpose_transcribe-0.1.0.tar", last modified: Mon Apr 15 19:30:21 2024, max compression
+gzip compressed data, was "purpose_transcribe-0.1.1.tar", last modified: Mon Apr 15 20:05:32 2024, max compression
```

## Comparing `purpose_transcribe-0.1.0.tar` & `purpose_transcribe-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 19:30:21.932706 purpose_transcribe-0.1.0/
--rw-r--r--   0 mo197      (504) staff       (20)     1577 2024-04-15 18:49:51.000000 purpose_transcribe-0.1.0/LICENSE
--rw-r--r--   0 mo197      (504) staff       (20)       33 2024-04-15 18:40:20.000000 purpose_transcribe-0.1.0/MANIFEST.in
--rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 19:30:21.932634 purpose_transcribe-0.1.0/PKG-INFO
--rw-r--r--   0 mo197      (504) staff       (20)     1516 2024-04-15 19:27:17.000000 purpose_transcribe-0.1.0/README.md
--rw-r--r--   0 mo197      (504) staff       (20)      561 2024-04-15 19:30:21.932980 purpose_transcribe-0.1.0/setup.cfg
--rw-r--r--   0 mo197      (504) staff       (20)      992 2024-04-15 18:14:44.000000 purpose_transcribe-0.1.0/setup.py
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 19:30:21.930252 purpose_transcribe-0.1.0/src/
-drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 19:30:21.932405 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/
--rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 mo197      (504) staff       (20)      326 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 mo197      (504) staff       (20)       77 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/entry_points.txt
--rw-r--r--   0 mo197      (504) staff       (20)       21 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/requires.txt
--rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 19:30:21.000000 purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/top_level.txt
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:05:32.579859 purpose_transcribe-0.1.1/
+-rw-r--r--   0 mo197      (504) staff       (20)     1577 2024-04-15 18:49:51.000000 purpose_transcribe-0.1.1/LICENSE
+-rw-r--r--   0 mo197      (504) staff       (20)       33 2024-04-15 18:40:20.000000 purpose_transcribe-0.1.1/MANIFEST.in
+-rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 20:05:32.579781 purpose_transcribe-0.1.1/PKG-INFO
+-rw-r--r--   0 mo197      (504) staff       (20)     1516 2024-04-15 19:27:17.000000 purpose_transcribe-0.1.1/README.md
+-rw-r--r--   0 mo197      (504) staff       (20)      561 2024-04-15 20:05:32.580081 purpose_transcribe-0.1.1/setup.cfg
+-rw-r--r--   0 mo197      (504) staff       (20)      992 2024-04-15 20:05:26.000000 purpose_transcribe-0.1.1/setup.py
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:05:32.577468 purpose_transcribe-0.1.1/src/
+drwxr-xr-x   0 mo197      (504) staff       (20)        0 2024-04-15 20:05:32.579564 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/
+-rw-r--r--   0 mo197      (504) staff       (20)     2183 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 mo197      (504) staff       (20)      326 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 mo197      (504) staff       (20)       77 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/entry_points.txt
+-rw-r--r--   0 mo197      (504) staff       (20)       21 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/requires.txt
+-rw-r--r--   0 mo197      (504) staff       (20)        1 2024-04-15 20:05:32.000000 purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/top_level.txt
```

### Comparing `purpose_transcribe-0.1.0/LICENSE` & `purpose_transcribe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `purpose_transcribe-0.1.0/PKG-INFO` & `purpose_transcribe-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpose_transcribe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool for transcribing audio files
 Author: Mark Okello
 Author-email: markokello55@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `purpose_transcribe-0.1.0/README.md` & `purpose_transcribe-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `purpose_transcribe-0.1.0/setup.cfg` & `purpose_transcribe-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = purpose_transcribe
-version = 0.1.0
+version = 0.1.1
 author = Mark Okello
 author_email = markokello55@gmail.com
 description = Transcription Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

### Comparing `purpose_transcribe-0.1.0/setup.py` & `purpose_transcribe-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='purpose_transcribe',
-    version='0.1.0',
+    version='0.1.1',
     description='A CLI tool for transcribing audio files',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mark Okello',
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
```

### Comparing `purpose_transcribe-0.1.0/src/purpose_transcribe.egg-info/PKG-INFO` & `purpose_transcribe-0.1.1/src/purpose_transcribe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpose_transcribe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool for transcribing audio files
 Author: Mark Okello
 Author-email: markokello55@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

