# Comparing `tmp/jiebanlp-0.2.1.tar.gz` & `tmp/jiebanlp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jiebanlp-0.2.1.tar", last modified: Mon Apr 15 07:12:14 2024, max compression
+gzip compressed data, was "dist\jiebanlp-1.0.0.tar", last modified: Mon Apr 15 07:14:51 2024, max compression
```

## Comparing `jiebanlp-0.2.1.tar` & `jiebanlp-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      398 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-0.2.1/jiebanlp/__init__.py
--rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-0.2.1/jiebanlp/constant.py
--rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-0.2.1/jiebanlp/manager.py
--rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-0.2.1/jiebanlp/predict.py
--rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-0.2.1/jiebanlp/scheduler.py
--rw-rw-rw-   0        0        0     2137 2024-04-15 07:10:45.000000 jiebanlp-0.2.1/jiebanlp/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/jiebanlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 07:12:14.000000 jiebanlp-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2024-04-15 07:12:07.000000 jiebanlp-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      398 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-1.0.0/jiebanlp/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-1.0.0/jiebanlp/constant.py
+-rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-1.0.0/jiebanlp/manager.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-1.0.0/jiebanlp/predict.py
+-rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-1.0.0/jiebanlp/scheduler.py
+-rw-rw-rw-   0        0        0     1235 2024-04-15 07:14:26.000000 jiebanlp-1.0.0/jiebanlp/service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/jiebanlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:14:51.000000 jiebanlp-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      634 2024-04-15 07:14:45.000000 jiebanlp-1.0.0/setup.py
```

### Comparing `jiebanlp-0.2.1/jiebanlp/constant.py` & `jiebanlp-1.0.0/jiebanlp/constant.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-0.2.1/jiebanlp/manager.py` & `jiebanlp-1.0.0/jiebanlp/manager.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-0.2.1/setup.py` & `jiebanlp-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jiebanlp',
-    version="0.2.1",
+    version="1.0.0",
     packages=find_packages(),
     include_package_data=True,
     author="xl",
     author_email="123456@qq.com",
     description="A short description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
-        'mysql-connector-python',
         'jieba',
         'Flask',
         'APScheduler',
-        'flask-cors'
+        'mysql-connector-python',
     ]
 )
```

