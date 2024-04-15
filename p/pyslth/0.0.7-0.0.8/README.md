# Comparing `tmp/pyslth-0.0.7.tar.gz` & `tmp/pyslth-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.0.7.tar", last modified: Mon Apr 15 12:22:17 2024, max compression
+gzip compressed data, was "pyslth-0.0.8.tar", last modified: Mon Apr 15 12:50:16 2024, max compression
```

## Comparing `pyslth-0.0.7.tar` & `pyslth-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.877897 pyslth-0.0.7/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.7/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:22:17.877666 pyslth-0.0.7/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.854461 pyslth-0.0.7/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)      873 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-15 12:22:17.000000 pyslth-0.0.7/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.7/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-15 12:22:17.877958 pyslth-0.0.7/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-15 12:21:50.000000 pyslth-0.0.7/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.869133 pyslth-0.0.7/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.7/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.7/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.869747 pyslth-0.0.7/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    16155 2024-04-15 12:21:30.000000 pyslth-0.0.7/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.7/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.870127 pyslth-0.0.7/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.870953 pyslth-0.0.7/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.7/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.7/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.875813 pyslth-0.0.7/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.7/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.7/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.876387 pyslth-0.0.7/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.7/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.7/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.7/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.852867 pyslth-0.0.7/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:22:17.877248 pyslth-0.0.7/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.0.7/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.7/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.7/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.7/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1133 2024-04-15 12:05:06.000000 pyslth-0.0.7/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.7/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.893234 pyslth-0.0.8/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.8/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:50:16.892989 pyslth-0.0.8/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.875444 pyslth-0.0.8/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-15 12:50:16.000000 pyslth-0.0.8/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)      873 2024-04-15 12:50:16.000000 pyslth-0.0.8/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-15 12:50:16.000000 pyslth-0.0.8/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-15 12:50:16.000000 pyslth-0.0.8/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-15 12:50:16.000000 pyslth-0.0.8/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.8/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-15 12:50:16.893299 pyslth-0.0.8/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-15 12:50:00.000000 pyslth-0.0.8/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.888427 pyslth-0.0.8/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.8/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.8/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.889126 pyslth-0.0.8/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    16165 2024-04-15 12:43:01.000000 pyslth-0.0.8/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.8/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.889466 pyslth-0.0.8/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.890338 pyslth-0.0.8/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.8/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.8/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.891301 pyslth-0.0.8/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.8/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.8/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.891771 pyslth-0.0.8/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.8/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.8/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.8/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.873347 pyslth-0.0.8/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-15 12:50:16.892554 pyslth-0.0.8/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.0.8/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.8/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.8/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.8/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1133 2024-04-15 12:05:06.000000 pyslth-0.0.8/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.8/slth/views.py
```

### Comparing `pyslth-0.0.7/PKG-INFO` & `pyslth-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.7
+Version: 0.0.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.7/pyslth.egg-info/PKG-INFO` & `pyslth-0.0.8/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.7
+Version: 0.0.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.7/pyslth.egg-info/SOURCES.txt` & `pyslth-0.0.8/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/setup.py` & `pyslth-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.0.7/slth/__init__.py` & `pyslth-0.0.8/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/components.py` & `pyslth-0.0.8/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/conf.py` & `pyslth-0.0.8/slth/conf.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/db/models.py` & `pyslth-0.0.8/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/endpoints.py` & `pyslth-0.0.8/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
 
     def get(self):
         return dict(
             {
                 "name": APPLICATON['title'],
                 "short_name": APPLICATON['title'],
                 "lang": 'pt-BR',
-                "start_url": "/",
+                "start_url": "/app/login/",
                 "scope": "/",
                 "display": "standalone",
                 "icons": [{
                     "src": build_url(self.request, APPLICATON['logo']),
                     "sizes": "192x192",
                     "type": "image/png"
                 }]
```

### Comparing `pyslth-0.0.7/slth/forms.py` & `pyslth-0.0.8/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/management/commands/integration_test.py` & `pyslth-0.0.8/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/management/commands/sync.py` & `pyslth-0.0.8/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/migrations/0001_initial.py` & `pyslth-0.0.8/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.0.8/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/models.py` & `pyslth-0.0.8/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/permissions.py` & `pyslth-0.0.8/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/queryset.py` & `pyslth-0.0.8/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/roles.py` & `pyslth-0.0.8/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/selenium/__init__.py` & `pyslth-0.0.8/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/selenium/browser.py` & `pyslth-0.0.8/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/serializer.py` & `pyslth-0.0.8/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/static/images/logo.png` & `pyslth-0.0.8/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/static/images/logo.svg` & `pyslth-0.0.8/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/statistics.py` & `pyslth-0.0.8/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/tests.py` & `pyslth-0.0.8/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/urls.py` & `pyslth-0.0.8/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/utils.py` & `pyslth-0.0.8/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.7/slth/views.py` & `pyslth-0.0.8/slth/views.py`

 * *Files identical despite different names*

