# Comparing `tmp/danila-lib-1.0.2.tar.gz` & `tmp/danila-lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.0.2.tar", last modified: Mon Apr 15 17:20:07 2024, max compression
+gzip compressed data, was "danila-lib-1.0.3.tar", last modified: Mon Apr 15 17:16:02 2024, max compression
```

## Comparing `danila-lib-1.0.2.tar` & `danila-lib-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.844830 danila-lib-1.0.2/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:20:07.844830 danila-lib-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.783107 danila-lib-1.0.2/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.2/danila/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-15 17:16:00.000000 danila-lib-1.0.2/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.788085 danila-lib-1.0.2/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:20:07.000000 danila-lib-1.0.2/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-15 17:20:07.000000 danila-lib-1.0.2/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:20:07.000000 danila-lib-1.0.2/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1881 2024-04-15 17:20:07.000000 danila-lib-1.0.2/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:20:07.000000 danila-lib-1.0.2/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.789080 danila-lib-1.0.2/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.2/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.790076 danila-lib-1.0.2/data/neuro/
--rw-rw-rw-   0        0        0     3830 2024-04-15 17:05:00.000000 danila-lib-1.0.2/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.2/data/neuro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:20:07.791071 danila-lib-1.0.2/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.2/data/result/Class_im.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.2/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-15 17:20:07.846822 danila-lib-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-15 17:20:01.000000 danila-lib-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.756641 danila-lib-1.0.3/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 17:16:02.756641 danila-lib-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.748677 danila-lib-1.0.3/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.3/danila/__init__.py
+-rw-rw-rw-   0        0        0      404 2024-04-15 17:16:00.000000 danila-lib-1.0.3/danila/danila.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.753654 danila-lib-1.0.3/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1881 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.753654 danila-lib-1.0.3/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.754649 danila-lib-1.0.3/data/neuro/
+-rw-rw-rw-   0        0        0     3830 2024-04-15 17:05:00.000000 danila-lib-1.0.3/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.3/data/neuro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.755645 danila-lib-1.0.3/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.3/data/result/Class_im.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.3/data/result/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:16:02.757636 danila-lib-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-15 17:09:18.000000 danila-lib-1.0.3/setup.py
```

### Comparing `danila-lib-1.0.2/PKG-INFO` & `danila-lib-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.0.2/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.0.3/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.0.2/danila_lib.egg-info/requires.txt` & `danila-lib-1.0.3/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.0.2/data/neuro/Rama_classify_class.py` & `danila-lib-1.0.3/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.0.2/setup.py` & `danila-lib-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.0.2',
+  version='1.0.3',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

