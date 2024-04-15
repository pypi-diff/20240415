# Comparing `tmp/django-l10n-extensions-1.1.tar.gz` & `tmp/django-l10n-extensions-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-l10n-extensions-1.1.tar", last modified: Fri Feb 16 11:57:34 2024, max compression
+gzip compressed data, was "django-l10n-extensions-1.1.1.tar", last modified: Mon Apr 15 12:04:27 2024, max compression
```

## Comparing `django-l10n-extensions-1.1.tar` & `django-l10n-extensions-1.1.1.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      249 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/DESCRIPTION
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      135 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/MANIFEST.in
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      780 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/PKG-INFO
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1405 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/README.md
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       38 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/setup.cfg
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      577 2024-02-16 11:57:13.000000 django-l10n-extensions-1.1/setup.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.866044 django-l10n-extensions-1.1/src/
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.866044 django-l10n-extensions-1.1/src/django_l10n_extensions/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2438 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      113 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/exceptions.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/django_l10n_extensions/forms/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/forms/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1150 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/forms/fields.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      921 2024-02-16 11:16:53.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/l10n_threading.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/django_l10n_extensions/management/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/management/__init__.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/django_l10n_extensions/management/commands/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/management/commands/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2898 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/management/commands/makemessages.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)    10899 2024-02-15 14:08:28.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/measures.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1449 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/mixins.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/django_l10n_extensions/models/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       24 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/models/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     7880 2024-02-16 11:07:44.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/models/fields.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     3958 2024-02-16 10:03:35.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/models/models.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     4785 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/po_utils.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2729 2024-02-16 08:37:45.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/settings.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/django_l10n_extensions/templatetags/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/templatetags/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2290 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/templatetags/inlinetrans.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1102 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/urls.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1033 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/utils.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     4424 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/django_l10n_extensions/views.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.866044 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      780 2024-02-16 11:57:34.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1902 2024-02-16 11:57:34.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        1 2024-02-16 11:57:34.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        1 2024-02-14 13:17:18.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/not-zip-safe
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       38 2024-02-16 11:57:34.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/requires.txt
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       29 2024-02-16 11:57:34.000000 django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/top_level.txt
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2172 2024-02-14 11:06:00.000000 django-l10n-extensions-1.1/src/tests/conftest.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/management/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/management/__init__.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/management/commands/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/management/commands/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1813 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/management/commands/test_make_messages.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/models/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/models/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      734 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/models/test_l10n_units.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     4197 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/models/test_measure_fields.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     4273 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/models/test_trans_fields.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     2594 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/test_measures.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/testapp/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       80 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      119 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/apps.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/testapp/migrations/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1558 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/migrations/0001_initial.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/migrations/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      726 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/models.py
-drwxrwxr-x   0 blankser  (1000) blankser  (1000)        0 2024-02-16 11:57:34.870044 django-l10n-extensions-1.1/src/tests/testapp/scripts/
--rw-rw-r--   0 blankser  (1000) blankser  (1000)        0 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/scripts/__init__.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)       44 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/scripts/sample_script.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1595 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/settings.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)     1378 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/urls.py
--rw-rw-r--   0 blankser  (1000) blankser  (1000)      362 2024-02-14 10:44:56.000000 django-l10n-extensions-1.1/src/tests/testapp/views.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/
+-rw-rw-r--   0 cees      (1000) cees      (1000)      249 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/DESCRIPTION
+-rw-rw-r--   0 cees      (1000) cees      (1000)      135 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/MANIFEST.in
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1405 2022-02-14 13:37:25.000000 django-l10n-extensions-1.1.1/README.md
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/setup.cfg
+-rw-rw-r--   0 cees      (1000) cees      (1000)      577 2024-04-15 11:51:21.000000 django-l10n-extensions-1.1.1/setup.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2438 2024-03-21 10:40:12.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      113 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/exceptions.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/forms/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/forms/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1150 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/forms/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      921 2024-02-16 11:29:24.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/l10n_threading.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2898 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/commands/makemessages.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)    10899 2023-05-12 15:01:09.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/measures.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/migrations/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4378 2024-04-15 11:50:11.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/migrations/0001_initial.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/migrations/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1449 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/mixins.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       24 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     7880 2024-02-16 11:29:24.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     3958 2024-02-16 11:29:24.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/models.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4785 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/po_utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2729 2024-02-16 11:29:24.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/settings.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/django_l10n_extensions/templatetags/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/templatetags/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2290 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/templatetags/inlinetrans.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1102 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1033 2023-05-12 13:35:39.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4424 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions/views.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.203999 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2024-04-15 12:04:27.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2006 2024-04-15 12:04:27.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2024-04-15 12:04:27.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/not-zip-safe
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2024-04-15 12:04:27.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/requires.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)       29 2024-04-15 12:04:27.000000 django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2172 2023-05-12 13:27:15.000000 django-l10n-extensions-1.1.1/src/tests/conftest.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1813 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/management/commands/test_make_messages.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      734 2024-03-21 10:10:05.000000 django-l10n-extensions-1.1.1/src/tests/models/test_l10n_units.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4197 2024-04-15 11:37:19.000000 django-l10n-extensions-1.1.1/src/tests/models/test_measure_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4273 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/models/test_trans_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2594 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/test_measures.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/testapp/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       80 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      119 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/apps.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/testapp/migrations/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1558 2024-04-15 11:47:26.000000 django-l10n-extensions-1.1.1/src/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      726 2024-04-15 11:50:03.000000 django-l10n-extensions-1.1.1/src/tests/testapp/models.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2024-04-15 12:04:27.207999 django-l10n-extensions-1.1.1/src/tests/testapp/scripts/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/scripts/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)       44 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/scripts/sample_script.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1618 2024-04-15 11:46:44.000000 django-l10n-extensions-1.1.1/src/tests/testapp/settings.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1372 2024-04-15 11:44:52.000000 django-l10n-extensions-1.1.1/src/tests/testapp/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      362 2022-02-14 13:06:47.000000 django-l10n-extensions-1.1.1/src/tests/testapp/views.py
```

### Comparing `django-l10n-extensions-1.1/README.md` & `django-l10n-extensions-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/setup.py` & `django-l10n-extensions-1.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django-l10n-extensions',
-    version='1.1',
+    version='1.1.1',
     author=u'Cees van Wieringen',
     author_email='ceesvw@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='./src'),
     include_package_data=True,
     install_requires=['GitPython==1.0.1', 'Django>=2', 'polib>=1.0'],
     url='https://github.com/ceasaro/django-l10n-extensions',
     license='',
     description=open('DESCRIPTION').read(),
-    long_description=open('DESCRIPTION').read(),
+    long_description=open('README.md').read(),
     zip_safe=False,
     key_words=['django', 'l10n', ]
 )
```

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/__init__.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/forms/fields.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/l10n_threading.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/l10n_threading.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/management/commands/makemessages.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/measures.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/measures.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/mixins.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/models/fields.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/models/models.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/models/models.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/po_utils.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/po_utils.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/settings.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/templatetags/inlinetrans.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/templatetags/inlinetrans.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/urls.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/urls.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/utils.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions/views.py` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions/views.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/django_l10n_extensions.egg-info/SOURCES.txt` & `django-l10n-extensions-1.1.1/src/django_l10n_extensions.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 src/django_l10n_extensions.egg-info/requires.txt
 src/django_l10n_extensions.egg-info/top_level.txt
 src/django_l10n_extensions/forms/__init__.py
 src/django_l10n_extensions/forms/fields.py
 src/django_l10n_extensions/management/__init__.py
 src/django_l10n_extensions/management/commands/__init__.py
 src/django_l10n_extensions/management/commands/makemessages.py
+src/django_l10n_extensions/migrations/0001_initial.py
+src/django_l10n_extensions/migrations/__init__.py
 src/django_l10n_extensions/models/__init__.py
 src/django_l10n_extensions/models/fields.py
 src/django_l10n_extensions/models/models.py
 src/django_l10n_extensions/templatetags/__init__.py
 src/django_l10n_extensions/templatetags/inlinetrans.py
 src/tests/__init__.py
 src/tests/conftest.py
```

### Comparing `django-l10n-extensions-1.1/src/tests/conftest.py` & `django-l10n-extensions-1.1.1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/management/commands/test_make_messages.py` & `django-l10n-extensions-1.1.1/src/tests/management/commands/test_make_messages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/models/test_l10n_units.py` & `django-l10n-extensions-1.1.1/src/tests/models/test_l10n_units.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/models/test_measure_fields.py` & `django-l10n-extensions-1.1.1/src/tests/models/test_measure_fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/models/test_trans_fields.py` & `django-l10n-extensions-1.1.1/src/tests/models/test_trans_fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/test_measures.py` & `django-l10n-extensions-1.1.1/src/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/testapp/migrations/0001_initial.py` & `django-l10n-extensions-1.1.1/src/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/testapp/models.py` & `django-l10n-extensions-1.1.1/src/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.1/src/tests/testapp/settings.py` & `django-l10n-extensions-1.1.1/src/tests/testapp/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 SECRET_KEY = 'dummy'
 
 INSTALLED_APPS = [
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.admin',
     'django.contrib.sessions',
+    'django.contrib.messages',
     'django_l10n_extensions',
     'tests.testapp',
 ]
 
-MIDDLEWARE_CLASSES = (
+MIDDLEWARE = (
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.locale.LocaleMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
 )
 
 PROJECT_DIR = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `django-l10n-extensions-1.1/src/tests/testapp/urls.py` & `django-l10n-extensions-1.1.1/src/tests/testapp/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.conf.urls import url, include
     2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
 """
 from django.conf.urls import url, include
 from django.contrib import admin
-from django.contrib.auth.views import login, logout
+from django.contrib.auth import login, logout
 from django.views.generic import TemplateView
 
 from tests.testapp.views import TransExampleView
 
 urlpatterns = [
     url(r'^$', TemplateView.as_view(template_name="l10n_extensions/testapp/home.html"),
         name="home"),
```

