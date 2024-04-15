# Comparing `tmp/pyslth-0.0.6.tar.gz` & `tmp/pyslth-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.0.6.tar", last modified: Mon Apr 15 12:08:20 2024, max compression
+gzip compressed data, was "pyslth-0.0.7.tar", last modified: Mon Apr 15 12:22:17 2024, max compression
```

## Comparing `pyslth-0.0.6.tar` & `pyslth-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.012626 pyslth-0.0.6/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.6/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:08:20.012433 pyslth-0.0.6/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.002523 pyslth-0.0.6/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:08:19.000000 pyslth-0.0.6/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)      873 2024-04-15 12:08:19.000000 pyslth-0.0.6/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-15 12:08:19.000000 pyslth-0.0.6/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-15 12:08:19.000000 pyslth-0.0.6/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-15 12:08:19.000000 pyslth-0.0.6/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.6/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-15 12:08:20.012683 pyslth-0.0.6/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-15 12:08:09.000000 pyslth-0.0.6/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.008302 pyslth-0.0.6/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.6/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.6/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.008941 pyslth-0.0.6/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    16159 2024-04-14 02:11:34.000000 pyslth-0.0.6/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.6/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.009304 pyslth-0.0.6/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.009968 pyslth-0.0.6/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.6/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.6/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.010864 pyslth-0.0.6/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.6/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.6/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.011400 pyslth-0.0.6/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.6/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.6/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.6/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.001007 pyslth-0.0.6/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:08:20.012078 pyslth-0.0.6/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.0.6/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.6/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.6/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.6/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1133 2024-04-15 12:05:06.000000 pyslth-0.0.6/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.6/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.877897 pyslth-0.0.7/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.7/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:22:17.877666 pyslth-0.0.7/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.854461 pyslth-0.0.7/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)      873 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.7/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-15 12:22:17.877958 pyslth-0.0.7/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-15 12:21:50.000000 pyslth-0.0.7/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.869133 pyslth-0.0.7/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.7/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.7/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.869747 pyslth-0.0.7/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    16155 2024-04-15 12:21:30.000000 pyslth-0.0.7/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.7/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.870127 pyslth-0.0.7/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.870953 pyslth-0.0.7/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.7/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.7/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.875813 pyslth-0.0.7/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.7/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.7/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.876387 pyslth-0.0.7/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.7/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.7/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.7/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.852867 pyslth-0.0.7/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.877248 pyslth-0.0.7/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.0.7/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.7/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.7/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1133 2024-04-15 12:05:06.000000 pyslth-0.0.7/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.7/slth/views.py
```

### Comparing `pyslth-0.0.6/PKG-INFO` & `pyslth-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.6
+Version: 0.0.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.6/pyslth.egg-info/PKG-INFO` & `pyslth-0.0.7/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.6
+Version: 0.0.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.6/pyslth.egg-info/SOURCES.txt` & `pyslth-0.0.7/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/setup.py` & `pyslth-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.0.6/slth/__init__.py` & `pyslth-0.0.7/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/components.py` & `pyslth-0.0.7/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/conf.py` & `pyslth-0.0.7/slth/conf.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/db/models.py` & `pyslth-0.0.7/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/endpoints.py` & `pyslth-0.0.7/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
     
 class Manifest(Endpoint):
 
     class Meta:
         verbose_name = 'Manifest'
 
     def get(self):
-        return Response(
+        return dict(
             {
                 "name": APPLICATON['title'],
                 "short_name": APPLICATON['title'],
                 "lang": 'pt-BR',
                 "start_url": "/",
                 "scope": "/",
                 "display": "standalone",
```

### Comparing `pyslth-0.0.6/slth/forms.py` & `pyslth-0.0.7/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/management/commands/integration_test.py` & `pyslth-0.0.7/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/management/commands/sync.py` & `pyslth-0.0.7/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/migrations/0001_initial.py` & `pyslth-0.0.7/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.0.7/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/models.py` & `pyslth-0.0.7/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/permissions.py` & `pyslth-0.0.7/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/queryset.py` & `pyslth-0.0.7/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/roles.py` & `pyslth-0.0.7/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/selenium/__init__.py` & `pyslth-0.0.7/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/selenium/browser.py` & `pyslth-0.0.7/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/serializer.py` & `pyslth-0.0.7/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/static/images/logo.png` & `pyslth-0.0.7/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/static/images/logo.svg` & `pyslth-0.0.7/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/statistics.py` & `pyslth-0.0.7/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/tests.py` & `pyslth-0.0.7/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/urls.py` & `pyslth-0.0.7/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/utils.py` & `pyslth-0.0.7/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.6/slth/views.py` & `pyslth-0.0.7/slth/views.py`

 * *Files identical despite different names*

