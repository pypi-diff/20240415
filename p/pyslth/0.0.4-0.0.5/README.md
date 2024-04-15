# Comparing `tmp/pyslth-0.0.4.tar.gz` & `tmp/pyslth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.0.4.tar", last modified: Sun Apr 14 18:57:07 2024, max compression
+gzip compressed data, was "pyslth-0.0.5.tar", last modified: Sun Apr 14 19:05:24 2024, max compression
```

## Comparing `pyslth-0.0.4.tar` & `pyslth-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.095790 pyslth-0.0.4/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.4/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:57:07.095649 pyslth-0.0.4/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.088636 pyslth-0.0.4/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:57:07.000000 pyslth-0.0.4/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)      845 2024-04-14 18:57:07.000000 pyslth-0.0.4/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-14 18:57:07.000000 pyslth-0.0.4/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-14 18:57:07.000000 pyslth-0.0.4/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-14 18:57:07.000000 pyslth-0.0.4/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.4/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-14 18:57:07.095847 pyslth-0.0.4/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-14 18:56:58.000000 pyslth-0.0.4/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.092985 pyslth-0.0.4/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.4/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2217 2024-04-13 03:34:53.000000 pyslth-0.0.4/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.093499 pyslth-0.0.4/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    16159 2024-04-14 02:11:34.000000 pyslth-0.0.4/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.4/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.093737 pyslth-0.0.4/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.094132 pyslth-0.0.4/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.4/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.4/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.094723 pyslth-0.0.4/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.4/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.4/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.095079 pyslth-0.0.4/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.4/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.4/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.4/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.087682 pyslth-0.0.4/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:57:07.095335 pyslth-0.0.4/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.4/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.4/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)      940 2024-04-09 12:56:09.000000 pyslth-0.0.4/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.4/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.019414 pyslth-0.0.5/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.5/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 19:05:24.019280 pyslth-0.0.5/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.011880 pyslth-0.0.5/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 19:05:23.000000 pyslth-0.0.5/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)      845 2024-04-14 19:05:23.000000 pyslth-0.0.5/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-14 19:05:23.000000 pyslth-0.0.5/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-14 19:05:23.000000 pyslth-0.0.5/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-14 19:05:23.000000 pyslth-0.0.5/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.5/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-14 19:05:24.019454 pyslth-0.0.5/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-14 19:05:18.000000 pyslth-0.0.5/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.016459 pyslth-0.0.5/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.5/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.5/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.016940 pyslth-0.0.5/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    16159 2024-04-14 02:11:34.000000 pyslth-0.0.5/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.5/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.017193 pyslth-0.0.5/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.017676 pyslth-0.0.5/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.5/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.5/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.018337 pyslth-0.0.5/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.5/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.5/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.018707 pyslth-0.0.5/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.5/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.5/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.5/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.010926 pyslth-0.0.5/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 19:05:24.018976 pyslth-0.0.5/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.5/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.5/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)      940 2024-04-09 12:56:09.000000 pyslth-0.0.5/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.5/slth/views.py
```

### Comparing `pyslth-0.0.4/PKG-INFO` & `pyslth-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.4
+Version: 0.0.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.4/pyslth.egg-info/PKG-INFO` & `pyslth-0.0.5/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.4
+Version: 0.0.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.4/pyslth.egg-info/SOURCES.txt` & `pyslth-0.0.5/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/setup.py` & `pyslth-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.0.4/slth/__init__.py` & `pyslth-0.0.5/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/components.py` & `pyslth-0.0.5/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/conf.py` & `pyslth-0.0.5/slth/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,22 +49,20 @@
     REDIS_HOST = os.environ.get('REDIS_HOST', 'redis')
     REDIS_PORT = os.environ.get('REDIS_PORT', 6379)
     REDIS_PASSWORD = os.environ.get('REDIS_PASSWORD', None)
     SESSION_ENGINE = 'django.contrib.sessions.backends.cache'
     SESSION_CACHE_ALIAS = 'default'
   
     CACHES = {
-        "default": {
-            "BACKEND": "django_redis.cache.RedisCache",
-            "LOCATION": "master/{}:{}/0".format(REDIS_HOST, REDIS_PORT),
-            "OPTIONS": {
+        'default': {
+            'BACKEND': 'django_redis.cache.RedisCache',
+            'LOCATION': 'redis://{}:{}/0'.format(REDIS_HOST, REDIS_PORT),
+            'OPTIONS': {
                 "PASSWORD": REDIS_PASSWORD,
-                "ALWAYS_MASTER": True,
-                "CLIENT_CLASS": "pnp.redis.PNPRedisClient",
-                "SENTINEL_TIMEOUT": 3
+                'CLIENT_CLASS': 'django_redis.client.DefaultClient'
             }
         }
     }
 
 
 if os.environ.get('POSTGRES_HOST'):
     DATABASES = {
```

### Comparing `pyslth-0.0.4/slth/db/models.py` & `pyslth-0.0.5/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/endpoints.py` & `pyslth-0.0.5/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/forms.py` & `pyslth-0.0.5/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/management/commands/integration_test.py` & `pyslth-0.0.5/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/management/commands/sync.py` & `pyslth-0.0.5/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/migrations/0001_initial.py` & `pyslth-0.0.5/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.0.5/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/models.py` & `pyslth-0.0.5/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/permissions.py` & `pyslth-0.0.5/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/queryset.py` & `pyslth-0.0.5/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/roles.py` & `pyslth-0.0.5/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/selenium/__init__.py` & `pyslth-0.0.5/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/selenium/browser.py` & `pyslth-0.0.5/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/serializer.py` & `pyslth-0.0.5/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/static/images/logo.svg` & `pyslth-0.0.5/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/statistics.py` & `pyslth-0.0.5/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/tests.py` & `pyslth-0.0.5/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/urls.py` & `pyslth-0.0.5/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/utils.py` & `pyslth-0.0.5/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.4/slth/views.py` & `pyslth-0.0.5/slth/views.py`

 * *Files identical despite different names*

