# Comparing `tmp/easys-ordermanager-2.7.0.tar.gz` & `tmp/easys_ordermanager-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easys-ordermanager-2.7.0.tar", last modified: Wed Mar 27 12:04:31 2024, max compression
+gzip compressed data, was "easys_ordermanager-2.8.0.tar", last modified: Mon Apr 15 14:08:51 2024, max compression
```

## Comparing `easys-ordermanager-2.7.0.tar` & `easys_ordermanager-2.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/
--rw-r--r--   0 root         (0) root         (0)    13446 2024-03-27 11:57:05.000000 easys-ordermanager-2.7.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    10832 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/CHANGELOG_SERIALIZER.md
--rw-r--r--   0 root         (0) root         (0)    34940 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      106 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25506 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      547 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/dev/management/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/dev/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1283 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/management/commands/i18n.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/dev/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/dev/tests/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v1/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/dev/tests/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v2/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/dev/tests/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      826 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/dev/tests/v3/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/
--rw-r--r--   0 root         (0) root         (0)      300 2024-03-27 11:57:05.000000 easys-ordermanager-2.7.0/easys_ordermanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      513 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 root         (0) root         (0)      829 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/easys_ordermanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.222131 easys-ordermanager-2.7.0/easys_ordermanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    13144 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93490 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v1/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93587 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v2/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96211 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/v3/serializer.py
--rw-r--r--   0 root         (0) root         (0)     3573 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/easys_ordermanager/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25506 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-27 12:04:31.000000 easys-ordermanager-2.7.0/easys_ordermanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      331 2024-03-27 12:04:31.226131 easys-ordermanager-2.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1251 2024-03-27 11:36:58.000000 easys-ordermanager-2.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/
+-rw-r--r--   0 root         (0) root         (0)    13522 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    10943 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/CHANGELOG_SERIALIZER.md
+-rw-r--r--   0 root         (0) root         (0)    34940 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25693 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      547 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/management/commands/i18n.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/tests/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v1/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/tests/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v2/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/dev/tests/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/dev/tests/v3/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/easys_ordermanager/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 root         (0) root         (0)      829 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/easys_ordermanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.783520 easys_ordermanager-2.8.0/easys_ordermanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    13144 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93490 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v1/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93587 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v2/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96354 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/v3/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/easys_ordermanager/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25693 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-15 14:08:51.000000 easys_ordermanager-2.8.0/easys_ordermanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      331 2024-04-15 14:08:51.787520 easys_ordermanager-2.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1251 2024-04-15 14:05:23.000000 easys_ordermanager-2.8.0/setup.py
```

### Comparing `easys-ordermanager-2.7.0/CHANGELOG.md` & `easys_ordermanager-2.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 2.8.0 (2024-04-12)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.7.0 (2024-03-27)
 * Add tests and support for DRF 3.15
 * Clarify compatibility matrix in README
 
 ## 2.6.0 (2024-03-08)
 * Add tests and support for Django 5.0 and Python 3.12
```

### Comparing `easys-ordermanager-2.7.0/CHANGELOG_SERIALIZER.md` & `easys_ordermanager-2.8.0/CHANGELOG_SERIALIZER.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Serializer changes
 
+## 2.8.0
+
+### v3
+
+#### `DisplayNativeCreativeSerializer`
+
+* Add `NATIVE_VIDEO_AD` (`7`) to `ad_type` choices.
+
 ## 2.5.1
 
 ### v3
 
 #### `OrderLineInAppSerializer`
 
 * Add `gender_targeting` field, optional.
```

### Comparing `easys-ordermanager-2.7.0/LICENSE.md` & `easys_ordermanager-2.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/PKG-INFO` & `easys_ordermanager-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.7.0
+Version: 2.8.0
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -48,14 +48,17 @@
 
 Python 3.10 to 3.12
 DRF 3.14 to 3.15
 
 
 # Changelog
 
+## 2.8.0 (2024-04-12)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.7.0 (2024-03-27)
 * Add tests and support for DRF 3.15
 * Clarify compatibility matrix in README
 
 ## 2.6.0 (2024-03-08)
 * Add tests and support for Django 5.0 and Python 3.12
 
@@ -490,14 +493,22 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.8.0
+
+### v3
+
+#### `DisplayNativeCreativeSerializer`
+
+* Add `NATIVE_VIDEO_AD` (`7`) to `ad_type` choices.
+
 ## 2.5.1
 
 ### v3
 
 #### `OrderLineInAppSerializer`
 
 * Add `gender_targeting` field, optional.
```

### Comparing `easys-ordermanager-2.7.0/README.md` & `easys_ordermanager-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/dev/management/commands/i18n.py` & `easys_ordermanager-2.8.0/dev/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/dev/tests/v3/test_serializer.py` & `easys_ordermanager-2.8.0/dev/tests/v3/test_serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/__pycache__/__init__.cpython-312.pyc` & `easys_ordermanager-2.8.0/easys_ordermanager/__pycache__/__init__.cpython-312.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0x91090466 (Wed Mar 27 11:57:05 2024 UTC)
+moddate:  0x23341d66 (Mon Apr 15 14:05:23 2024 UTC)
 files sz: 300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
@@ -13,15 +13,15 @@
    
      1           2 LOAD_CONST               0 ('easys-ordermanager')
                  4 STORE_NAME               0 (__title__)
    
      2           6 LOAD_CONST               1 ('API definition of RH order manager for EasyS')
                  8 STORE_NAME               1 (__description__)
    
-     3          10 LOAD_CONST               2 ('2.7.0')
+     3          10 LOAD_CONST               2 ('2.8.0')
                 12 STORE_NAME               2 (__version__)
    
      4          14 LOAD_CONST               3 ('https://gitlab.herocentral.de/development/easys-ordermanager')
                 16 STORE_NAME               3 (__url__)
    
      5          18 LOAD_CONST               4 ('RegioHelden developers')
                 20 STORE_NAME               4 (__author__)
@@ -31,15 +31,15 @@
    
      7          26 LOAD_CONST               6 ('GPL 3')
                 28 STORE_NAME               6 (__license__)
                 30 PRECALL                  7
    consts
       'easys-ordermanager'
       'API definition of RH order manager for EasyS'
-      '2.7.0'
+      '2.8.0'
       'https://gitlab.herocentral.de/development/easys-ordermanager'
       'RegioHelden developers'
       'opensource@regiohelden.de'
       'GPL 3'
       None
    names      ('__title__', '__description__', '__version__', '__url__', '__author__', '__author_email__', '__license__')
    varnames   ()
```

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/fields.py` & `easys_ordermanager-2.8.0/easys_ordermanager/fields.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po` & `easys_ordermanager-2.8.0/easys_ordermanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/v1/serializer.py` & `easys_ordermanager-2.8.0/easys_ordermanager/v1/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/v2/serializer.py` & `easys_ordermanager-2.8.0/easys_ordermanager/v2/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/v3/serializer.py` & `easys_ordermanager-2.8.0/easys_ordermanager/v3/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,21 +733,23 @@
 
 NATIVE_AD_IN = 1
 NATIVE_AD_OUT = 2
 NATIVE_AD_PROSPECT = 3
 NATIVE_AD_FLOW_AD_IN = 4
 NATIVE_AD_FLOW_AD_OUT = 5
 NATIVE_AD_FLOW_AD_PROSPECT = 6
+NATIVE_VIDEO_AD = 7
 NATIVE_AD_TYPES = Choices(
     (NATIVE_AD_IN, 'native_ad_in', _('AdIn')),
     (NATIVE_AD_OUT, 'native_ad_out', _('AdOut')),
     (NATIVE_AD_PROSPECT, 'native_ad_prospect', _('AdProspect')),
     (NATIVE_AD_FLOW_AD_IN, 'native_ad_flow_ad_in', _('AdFlow (AdIn)')),
     (NATIVE_AD_FLOW_AD_OUT, 'native_ad_flow_ad_out', _('AdFlow (AdOut)')),
     (NATIVE_AD_FLOW_AD_PROSPECT, 'native_ad_flow_ad_prospect', _('AdFlow (AdProspect)')),
+    (NATIVE_VIDEO_AD, 'native_video_ad', _('Video Ad')),
 )
 
 
 class FileSerializer(serializers.Serializer):
     """
     proof of offer file, e.g. pdf with signature, file scan, etc
 
@@ -1344,14 +1346,15 @@
             NATIVE_AD_TYPES.native_ad_prospect: [
                 BILLING_TYPES.cpm,
                 BILLING_TYPES.cpc,
             ],
             NATIVE_AD_TYPES.native_ad_flow_ad_in: [BILLING_TYPES.cpm],
             NATIVE_AD_TYPES.native_ad_flow_ad_out: [BILLING_TYPES.cpm],
             NATIVE_AD_TYPES.native_ad_flow_ad_prospect: [BILLING_TYPES.cpm],
+            NATIVE_AD_TYPES.native_video_ad: [BILLING_TYPES.cpm],
         }
 
         errors = []
         ad_type = data.get('creatives').get('ad_type')
         billing_type = data.get('billing_type')
         if billing_type and billing_type not in BILLING_TYPES_MAP[ad_type]:
             errors.append({'billing_type': '"ad_type" and "billing_type" fields not match each other.'})
```

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager/validators.py` & `easys_ordermanager-2.8.0/easys_ordermanager/validators.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager.egg-info/PKG-INFO` & `easys_ordermanager-2.8.0/easys_ordermanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.7.0
+Version: 2.8.0
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -48,14 +48,17 @@
 
 Python 3.10 to 3.12
 DRF 3.14 to 3.15
 
 
 # Changelog
 
+## 2.8.0 (2024-04-12)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.7.0 (2024-03-27)
 * Add tests and support for DRF 3.15
 * Clarify compatibility matrix in README
 
 ## 2.6.0 (2024-03-08)
 * Add tests and support for Django 5.0 and Python 3.12
 
@@ -490,14 +493,22 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.8.0
+
+### v3
+
+#### `DisplayNativeCreativeSerializer`
+
+* Add `NATIVE_VIDEO_AD` (`7`) to `ad_type` choices.
+
 ## 2.5.1
 
 ### v3
 
 #### `OrderLineInAppSerializer`
 
 * Add `gender_targeting` field, optional.
```

### Comparing `easys-ordermanager-2.7.0/easys_ordermanager.egg-info/SOURCES.txt` & `easys_ordermanager-2.8.0/easys_ordermanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.7.0/setup.py` & `easys_ordermanager-2.8.0/setup.py`

 * *Files identical despite different names*

