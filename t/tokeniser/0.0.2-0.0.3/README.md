# Comparing `tmp/tokeniser-0.0.2.tar.gz` & `tmp/tokeniser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokeniser-0.0.2.tar", last modified: Tue Feb 13 22:03:30 2024, max compression
+gzip compressed data, was "tokeniser-0.0.3.tar", last modified: Mon Apr 15 09:46:44 2024, max compression
```

## Comparing `tokeniser-0.0.2.tar` & `tokeniser-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-02-13 22:03:30.998181 tokeniser-0.0.2/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-02-13 21:41:18.000000 tokeniser-0.0.2/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1943 2024-02-13 22:03:30.998050 tokeniser-0.0.2/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1465 2024-02-13 22:03:17.000000 tokeniser-0.0.2/README.md
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-02-13 22:03:30.998234 tokeniser-0.0.2/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      674 2024-02-13 21:51:40.000000 tokeniser-0.0.2/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-02-13 22:03:30.997277 tokeniser-0.0.2/tokeniser/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-02-13 21:55:24.000000 tokeniser-0.0.2/tokeniser/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      110 2024-02-13 21:55:53.000000 tokeniser-0.0.2/tokeniser/tokeniser.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-02-13 22:03:30.997849 tokeniser-0.0.2/tokeniser.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1943 2024-02-13 22:03:30.000000 tokeniser-0.0.2/tokeniser.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      203 2024-02-13 22:03:30.000000 tokeniser-0.0.2/tokeniser.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-02-13 22:03:30.000000 tokeniser-0.0.2/tokeniser.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       10 2024-02-13 22:03:30.000000 tokeniser-0.0.2/tokeniser.egg-info/top_level.txt
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-15 09:46:44.194865 tokeniser-0.0.3/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-02-13 21:41:18.000000 tokeniser-0.0.3/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1943 2024-04-15 09:46:44.194701 tokeniser-0.0.3/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1465 2024-02-13 22:03:17.000000 tokeniser-0.0.3/README.md
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-15 09:46:44.194920 tokeniser-0.0.3/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      674 2024-04-15 09:46:39.000000 tokeniser-0.0.3/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-15 09:46:44.193386 tokeniser-0.0.3/tokeniser/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-02-13 21:55:24.000000 tokeniser-0.0.3/tokeniser/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      110 2024-02-13 21:55:53.000000 tokeniser-0.0.3/tokeniser/tokeniser.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-15 09:46:44.194395 tokeniser-0.0.3/tokeniser.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1943 2024-04-15 09:46:44.000000 tokeniser-0.0.3/tokeniser.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      203 2024-04-15 09:46:44.000000 tokeniser-0.0.3/tokeniser.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-15 09:46:44.000000 tokeniser-0.0.3/tokeniser.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       10 2024-04-15 09:46:44.000000 tokeniser-0.0.3/tokeniser.egg-info/top_level.txt
```

### Comparing `tokeniser-0.0.2/LICENSE` & `tokeniser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tokeniser-0.0.2/PKG-INFO` & `tokeniser-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokeniser
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/chigwell/tokeniser
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tokeniser-0.0.2/README.md` & `tokeniser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tokeniser-0.0.2/setup.py` & `tokeniser-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tokeniser',
-    version='0.0.2',
+    version='0.0.3',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/tokeniser',
     packages=find_packages(),
```

### Comparing `tokeniser-0.0.2/tokeniser.egg-info/PKG-INFO` & `tokeniser-0.0.3/tokeniser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokeniser
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/chigwell/tokeniser
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

