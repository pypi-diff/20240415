# Comparing `tmp/CryptoTracker-0.1.0.tar.gz` & `tmp/CryptoTracker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CryptoTracker-0.1.0.tar", last modified: Mon Apr 15 14:40:32 2024, max compression
+gzip compressed data, was "CryptoTracker-0.1.1.tar", last modified: Mon Apr 15 18:14:46 2024, max compression
```

## Comparing `CryptoTracker-0.1.0.tar` & `CryptoTracker-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:40:32.957597 CryptoTracker-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-15 14:40:32.941016 CryptoTracker-0.1.0/CryptoTracker.egg-info/
--rw-rw-rw-   0        0        0     1292 2024-04-15 14:40:32.000000 CryptoTracker-0.1.0/CryptoTracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-15 14:40:32.000000 CryptoTracker-0.1.0/CryptoTracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:40:32.000000 CryptoTracker-0.1.0/CryptoTracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 14:40:32.000000 CryptoTracker-0.1.0/CryptoTracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 14:40:32.000000 CryptoTracker-0.1.0/CryptoTracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1292 2024-04-15 14:40:32.955597 CryptoTracker-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-04-15 02:21:11.000000 CryptoTracker-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 14:40:32.957597 CryptoTracker-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1007 2024-04-15 14:40:06.000000 CryptoTracker-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:40:32.953596 CryptoTracker-0.1.0/tracker/
--rw-rw-rw-   0        0        0        0 2024-04-15 01:22:09.000000 CryptoTracker-0.1.0/tracker/__init__.py
--rw-rw-rw-   0        0        0     3023 2024-04-15 01:21:39.000000 CryptoTracker-0.1.0/tracker/app.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:14:46.555538 CryptoTracker-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:14:46.545908 CryptoTracker-0.1.1/CryptoTracker.egg-info/
+-rw-rw-rw-   0        0        0     1305 2024-04-15 18:14:45.000000 CryptoTracker-0.1.1/CryptoTracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-15 18:14:46.000000 CryptoTracker-0.1.1/CryptoTracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:14:45.000000 CryptoTracker-0.1.1/CryptoTracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 18:14:45.000000 CryptoTracker-0.1.1/CryptoTracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 18:14:45.000000 CryptoTracker-0.1.1/CryptoTracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2024-04-15 18:04:44.000000 CryptoTracker-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1305 2024-04-15 18:14:46.552527 CryptoTracker-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-04-15 02:21:11.000000 CryptoTracker-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 18:14:46.556542 CryptoTracker-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2024-04-15 18:14:03.000000 CryptoTracker-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:14:46.549910 CryptoTracker-0.1.1/tracker/
+-rw-rw-rw-   0        0        0        0 2024-04-15 01:22:09.000000 CryptoTracker-0.1.1/tracker/__init__.py
+-rw-rw-rw-   0        0        0     3023 2024-04-15 01:21:39.000000 CryptoTracker-0.1.1/tracker/app.py
```

### Comparing `CryptoTracker-0.1.0/CryptoTracker.egg-info/PKG-INFO` & `CryptoTracker-0.1.1/CryptoTracker.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: CryptoTracker
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple GUI application to track cryptocurrency projects.
 Author: DanF
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pandas
-Requires-Dist: tkinter
 
 # CryptoTracker
 
 ## Description
 CryptoTracker is a simple GUI application to track cryptocurrency projects including links, deadlines, market caps, Twitter, and Discord information.
 
 ## Installation
```

### Comparing `CryptoTracker-0.1.0/PKG-INFO` & `CryptoTracker-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: CryptoTracker
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple GUI application to track cryptocurrency projects.
 Author: DanF
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pandas
-Requires-Dist: tkinter
 
 # CryptoTracker
 
 ## Description
 CryptoTracker is a simple GUI application to track cryptocurrency projects including links, deadlines, market caps, Twitter, and Discord information.
 
 ## Installation
```

### Comparing `CryptoTracker-0.1.0/README.md` & `CryptoTracker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CryptoTracker-0.1.0/setup.py` & `CryptoTracker-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CryptoTracker',
-    version='0.1.0',
+    version='0.1.1',
     author='DanF',
+    license='MIT',
     description='A simple GUI application to track cryptocurrency projects.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pandas',
-        'tkinter'  # Note: tkinter is usually included with Python's standard library
+        #'tkinter'  # Note: tkinter is usually included with Python's standard library
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `CryptoTracker-0.1.0/tracker/app.py` & `CryptoTracker-0.1.1/tracker/app.py`

 * *Files identical despite different names*

