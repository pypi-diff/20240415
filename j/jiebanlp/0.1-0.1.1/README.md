# Comparing `tmp/jiebanlp-0.1.tar.gz` & `tmp/jiebanlp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jiebanlp-0.1.tar", last modified: Mon Apr 15 05:53:05 2024, max compression
+gzip compressed data, was "dist\jiebanlp-0.1.1.tar", last modified: Mon Apr 15 06:25:44 2024, max compression
```

## Comparing `jiebanlp-0.1.tar` & `jiebanlp-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 05:53:05.000000 jiebanlp-0.1/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      396 2024-04-15 05:53:05.000000 jiebanlp-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 05:53:05.000000 jiebanlp-0.1/jiebanlp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-0.1/jiebanlp/__init__.py
--rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-0.1/jiebanlp/constant.py
--rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-0.1/jiebanlp/manager.py
--rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-0.1/jiebanlp/predict.py
--rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-0.1/jiebanlp/scheduler.py
--rw-rw-rw-   0        0        0     1235 2024-04-15 03:35:05.000000 jiebanlp-0.1/jiebanlp/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 05:53:05.000000 jiebanlp-0.1/jiebanlp.egg-info/
--rw-rw-rw-   0        0        0      396 2024-04-15 05:53:04.000000 jiebanlp-0.1/jiebanlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-15 05:53:04.000000 jiebanlp-0.1/jiebanlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 05:53:04.000000 jiebanlp-0.1/jiebanlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-15 05:53:04.000000 jiebanlp-0.1/jiebanlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 05:53:04.000000 jiebanlp-0.1/jiebanlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 05:53:05.000000 jiebanlp-0.1/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-04-15 03:13:52.000000 jiebanlp-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      398 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-0.1.1/jiebanlp/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-0.1.1/jiebanlp/constant.py
+-rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-0.1.1/jiebanlp/manager.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-0.1.1/jiebanlp/predict.py
+-rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-0.1.1/jiebanlp/scheduler.py
+-rw-rw-rw-   0        0        0     2097 2024-04-15 06:24:41.000000 jiebanlp-0.1.1/jiebanlp/service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/jiebanlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:25:44.000000 jiebanlp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      655 2024-04-15 06:22:18.000000 jiebanlp-0.1.1/setup.py
```

### Comparing `jiebanlp-0.1/jiebanlp/constant.py` & `jiebanlp-0.1.1/jiebanlp/constant.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-0.1/jiebanlp/manager.py` & `jiebanlp-0.1.1/jiebanlp/manager.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-0.1/setup.py` & `jiebanlp-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jiebanlp',
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     include_package_data=True,
     author="xl",
     author_email="123456@qq.com",
     description="A short description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -15,10 +15,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         'mysql-connector-python',
         'jieba',
         'Flask',
-        'APScheduler'
+        'APScheduler',
+        'flask-cors'
     ]
 )
```

