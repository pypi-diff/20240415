# Comparing `tmp/django-flex-report-0.6.6.tar.gz` & `tmp/django-flex-report-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.6.6.tar", last modified: Thu Mar  7 09:42:22 2024, max compression
+gzip compressed data, was "django-flex-report-0.6.7.tar", last modified: Mon Apr 15 12:57:23 2024, max compression
```

## Comparing `django-flex-report-0.6.6.tar` & `django-flex-report-0.6.7.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-03-07 09:42:22.662366 django-flex-report-0.6.6/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-01-02 07:34:11.000000 django-flex-report-0.6.6/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-02-08 12:10:46.000000 django-flex-report-0.6.6/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-03-07 09:42:22.662366 django-flex-report-0.6.6/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-03-07 09:42:22.662366 django-flex-report-0.6.6/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1521 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-03-07 09:42:22.000000 django-flex-report-0.6.6/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-03-07 09:42:22.658349 django-flex-report-0.6.6/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1568 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-03-07 09:42:21.000000 django-flex-report-0.6.6/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-02-16 10:42:31.000000 django-flex-report-0.6.6/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4633 2024-03-07 09:41:52.000000 django-flex-report-0.6.6/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2004 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-02-18 02:45:47.000000 django-flex-report-0.6.6/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3118 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-03-07 09:42:22.658349 django-flex-report-0.6.6/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-02-15 12:31:18.000000 django-flex-report-0.6.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    13176 2024-03-07 09:03:44.000000 django-flex-report-0.6.6/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     7883 2024-02-18 02:45:47.000000 django-flex-report-0.6.6/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-03-07 09:42:22.662366 django-flex-report-0.6.6/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5699 2024-03-07 09:42:11.000000 django-flex-report-0.6.6/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-02-11 11:59:16.000000 django-flex-report-0.6.6/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    24648 2024-02-25 06:16:29.000000 django-flex-report-0.6.6/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11116 2024-02-18 02:45:48.000000 django-flex-report-0.6.6/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-02-08 12:08:37.000000 django-flex-report-0.6.6/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-02-15 11:37:14.000000 django-flex-report-0.6.6/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-03-07 09:42:22.662366 django-flex-report-0.6.6/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-02-08 10:30:09.000000 django-flex-report-0.6.6/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1627 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.000964 django-flex-report-0.6.7/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1568 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4764 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2139 2024-04-15 12:53:15.000000 django-flex-report-0.6.7/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3118 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    13307 2024-04-15 12:54:34.000000 django-flex-report-0.6.7/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8341 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5671 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    24649 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11116 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/setup.py
```

### Comparing `django-flex-report-0.6.6/LICENSE` & `django-flex-report-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/MANIFEST.in` & `django-flex-report-0.6.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/PKG-INFO` & `django-flex-report-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.6.6/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.6.7/django_flex_report.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.6.6/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.6.7/django_flex_report.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,12 @@
 flex_report/migrations/0006_tablebutton_query_strings.py
 flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
 flex_report/migrations/0008_template_buttons.py
 flex_report/migrations/0009_alter_template_buttons.py
 flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
 flex_report/migrations/0011_alter_template_model_user_path.py
 flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+flex_report/migrations/0013_column_column_type.py
+flex_report/migrations/0014_alter_column_column_type.py
 flex_report/migrations/__init__.py
 flex_report/templatetags/__init__.py
 flex_report/templatetags/flex_report_filters.py
```

### Comparing `django-flex-report-0.6.6/flex_report/__init__.py` & `django-flex-report-0.6.7/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/admin.py` & `django-flex-report-0.6.7/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/app_settings.py` & `django-flex-report-0.6.7/flex_report/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         return self._settings("DEFAULT_CELL_VALUE", "&mdash;")
 
     @property
     def EDITORS_GROUP_NAME(self):
         return self._settings("EDITORS_GROUP_NAME", "report_editors")
 
     @property
+    def DYNAMIC_FIELD_FUNC_PREFIX(self):
+        return self._settings("DYNAMIC_FIELD_FUNC_PREFIX", "get_dynamic_")
+
+    @property
     def TIME_FORMATS(self):
         dflt = time_formats = {
             models.DateTimeField: "%H:%M %Y/%m/%d",
             models.DateField: "%Y/%m/%d",
             models.TimeField: "%H:%M:%S",
             jmodels.jDateField: "%H:%M:%S",
             jmodels.jDateTimeField: "%H:%M %Y/%m/%d",
```

### Comparing `django-flex-report-0.6.6/flex_report/constants.py` & `django-flex-report-0.6.7/flex_report/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,28 +39,35 @@
         return models[0]
 
 
 class BaseExportFormat:
     formats = {}
     format_slug = None
     format_name = None
+    format_ext = None
 
     @classmethod
     def __str__(cls):
         return cls.format_name
 
     @classmethod
     @property
     @abstractmethod
     def format_slug(cls):
         raise NotImplementedError
 
     @classmethod
     @property
     @abstractmethod
+    def format_ext(cls):
+        raise NotImplementedError
+
+    @classmethod
+    @property
+    @abstractmethod
     def format_name(cls):
         raise NotImplementedError
 
     @classmethod
     def register(cls, format_):
         assert issubclass(format_, BaseExportFormat)
         return cls.formats.update({format_.format_slug: format_})
@@ -79,8 +86,8 @@
     def handle_response(cls, *args, **kwargs):
         raise NotImplementedError
 
 
 class FieldTypes:
     field = "field"
     property = "property"
-    custom = "custom"
+    dynamic = "dynamic"
```

### Comparing `django-flex-report-0.6.6/flex_report/fields.py` & `django-flex-report-0.6.7/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/filterset.py` & `django-flex-report-0.6.7/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/forms.py` & `django-flex-report-0.6.7/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0001_initial.py` & `django-flex-report-0.6.7/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.6.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.6.7/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.6.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.6.7/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.6.7/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.6.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.6.7/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.6.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/mixins.py` & `django-flex-report-0.6.7/flex_report/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,15 +209,17 @@
             self.report_model, list(self.template_searchable_fields.values())
         )(initials)
 
     def apply_user_path(self):
         LOGICAL_OPERATORS = ["()", "&", "|", "!="]
         paths = self.template_object.model_user_path or {}
         path_func = getattr(
-            self.report_model, app_settings.MODEL_USER_PATH_FUNC_NAME, lambda request: {}
+            self.report_model,
+            app_settings.MODEL_USER_PATH_FUNC_NAME,
+            lambda request: {},
         )
 
         accessed_paths = {
             path_name: path_dict
             for path_name, path in paths.items()
             if (
                 path_dict := {
@@ -235,46 +237,42 @@
             else list(filter(partial(ne, "__all__"), accessed_paths))[0]
         )
         if accessed_path == "__all__":
             return
 
         accessed_path, accessed_val = accessed_paths[accessed_path].popitem()
         if not any(map(lambda op: op in accessed_path, LOGICAL_OPERATORS)):
-            self.report_qs = self.report_qs.filter(
-                **{accessed_path: accessed_val}
-            )
+            self.report_qs = self.report_qs.filter(**{accessed_path: accessed_val})
             return
 
-        self.report_qs = self.report_qs.filter(
-            string_to_q(accessed_path, accessed_val)
-        )
-        
+        self.report_qs = self.report_qs.filter(string_to_q(accessed_path, accessed_val))
+
     def _format_used_filter(self, col_name, val):
         formats = {
             **{k: "بله" for k in ["true", "True", True]},
             **{k: "خیر" for k in ["false", "False", False]},
         }
-        
+
         if formatted_val := formats.get(val, False):
             return formatted_val
 
         if choices := get_choice_field_choices(self.report_model, col_name):
             return dict(choices).get(val, val)
 
         return str(val)
 
-    def used_filter_format(self, col_name, val):        
+    def used_filter_format(self, col_name, val):
         if isinstance(val, list):
             return ", ".join(
                 map(
                     lambda v: self._format_used_filter(col_name, v),
                     val,
                 )
             )
-            
+
         return self._format_used_filter(col_name, val) or val
 
     def setup(self, request, *args, **kwargs):
         super().setup(request, *args, **kwargs)
 
         obj = self.template_object
         if not obj:
@@ -282,75 +280,88 @@
             return
 
         self.report_model = obj.model.model_class()
         self.template_columns = get_template_columns(obj)
         self.template_searchable_fields = get_template_columns(obj, searchables=True)
 
         self.get_filters()
-        self.report_qs = methodcaller("none" if self.template_filters.get_filters() else "all")(self.report_model.objects)
+        self.report_qs = methodcaller(
+            "none" if self.template_filters.get_filters() else "all"
+        )(self.report_model.objects)
         self.apply_user_path()
-        
-        if (
-            all(map(methodcaller("get_filters"), [self.filters, self.quicksearch, self.template_filters]))
-            and all(map(methodcaller("is_valid"), [self.filters, self.quicksearch, self.template_filters]))
+
+        if all(
+            map(
+                methodcaller("get_filters"),
+                [self.filters, self.quicksearch, self.template_filters],
+            )
+        ) and all(
+            map(
+                methodcaller("is_valid"),
+                [self.filters, self.quicksearch, self.template_filters],
+            )
         ):
             self.report_qs = self.template_filters.qs.distinct().filter(
                 pk__in=Subquery(
                     (
                         self.quicksearch.qs.distinct() & self.filters.qs.distinct()
                     ).values("pk")
                 )
             )
 
             self.report_qs = self.report_qs.distinct().order_by(
                 *self.report_model._meta.ordering or ["pk"]
             )
-            
+
             cleaned_data = (
                 self.quicksearch.form.cleaned_data | self.filters.form.cleaned_data
             )
             self.used_filters = self.get_used_filters(
                 {
-                    get_column_verbose_name(self.report_model, k): self.used_filter_format(
-                        k, v
-                    )
+                    get_column_verbose_name(
+                        self.report_model, k
+                    ): self.used_filter_format(k, v)
                     for k, v in cleaned_data.items()
                     if bool(v)
                 }
             )
 
     def get_used_filters(self, cleaned_data):
         return _(" and ").join(
             [
                 f'{k} = {",".join(map(str, v)) if isinstance(v, list) else v}'
                 for k, v in cleaned_data.items()
                 if str(k).lower() != "search"
             ]
         )
-        
+
     def _prepare_initial(self, initial):
         if initial.lower() in ["true", "false"]:
             return initial.lower() == "true"
 
-        if (initial.startswith("[") and initial.endswith("]")) or (not initial.startswith("0") and initial.isnumeric()):
+        if (initial.startswith("[") and initial.endswith("]")) or (
+            not initial.startswith("0") and initial.isnumeric()
+        ):
             return ast.literal_eval(initial)
 
     def get_initial_value(self, initial, *, key=""):
         initial = str(initial)
 
         if key.endswith("__in"):
             return list(map(self._prepare_initial, self.request.GET.getlist(key)))
 
         return self._prepare_initial(initial)
 
     def get_initials(self):
         return {
             k: self.get_initial_value(v, key=k)
             for k, v in self.request.GET.dict().items()
-            if str(v) and v.strip() not in self.ignore_search_values and k.lower() != "search"
+            if str(v)
+            and v.strip() not in self.ignore_search_values
+            and k.lower() != "search"
         }
 
     def get_form_classes(self):
         if not self.template_object:
             return []
         return [generate_filterset_form(self.report_model)]
 
@@ -377,15 +388,15 @@
             "templates": self.get_page_templates(),
             "initials": self.get_initials(),
             "pagination": self.pagination,
             "page_template_keyword": self.page_template_keyword,
             "is_page_table": self.is_page_table,
             "have_template": self.have_template,
             "export_formats": [
-                {"name": format_.format_name, "slug": format_.format_slug}
+                {"name": format_.format_name, "slug": format_.format_slug, "ext": (format_.format_ext or format_.format_slug)}
                 for format_ in export_format.formats.values()
             ],
             "page_title": getattr(
                 self.template_object.page, "title", self.template_object.title
             ),
         }
         return context
```

### Comparing `django-flex-report-0.6.6/flex_report/models.py` & `django-flex-report-0.6.7/flex_report/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         return f"/{url}" if url else ""
 
     def __str__(self):
         return f"{self.title}"
 
 
 class Column(models.Model):
+    class COLUMN_TYPES(models.TextChoices):
+        dynamic = "dynamic", _("Dynamic")
+        model = "model", _("model")
+
     title = models.CharField(verbose_name=_("Title"), max_length=150, db_index=True)
     searchable = models.BooleanField(default=False)
     creator = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         related_name="created_columns",
         blank=True,
@@ -60,17 +64,29 @@
         blank=True,
     )
     model = models.ForeignKey(
         ContentType,
         on_delete=models.CASCADE,
         related_name="flex_columns",
     )
+    column_type = models.CharField(
+        verbose_name=_("Column Type"),
+        choices=COLUMN_TYPES.choices,
+        max_length=10,
+        default=COLUMN_TYPES.model,
+    )
 
     objects = ColumnManager()
 
+    def get_column_choices(self):
+        if self.column_type == self.COLUMN_TYPES.model:
+            return {self.id: self.title}
+        
+        return 
+
     def __str__(self):
         return f"{self.model}: {self.title}"
 
     def clean(self):
         if not is_field_valid(self.model.model_class(), self.title):
             raise ValidationError(
                 {
```

### Comparing `django-flex-report-0.6.6/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.6.7/flex_report/templatetags/flex_report_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,23 +121,23 @@
 
 
 @register.filter
 def get_column_verbose_name(obj, column):
     lookup_exprs = list(map(lambda i: f"__{i}", ["in"]))
     for lookup in filter(lambda i: column.endswith(i), lookup_exprs):
         column = column.rstrip(lookup)
-                        
+
     field_col = getattr(field_to_db_field(obj, column), "verbose_name", False)
     if (
         getattr(obj, column, False)
         and not field_col
         and (property_col := getattr(getattr(obj, column), "fget", False))
     ):
         field_col = getattr(property_col, "verbose_name", False)
-    
+
     return mark_safe(field_col or column.replace("_", " ").title())
 
 
 @register.filter
 def get_columns_verbose_names(cols: Iterable, obj):
     return list(map(lambda c: get_column_verbose_name(obj, c), cols))
```

### Comparing `django-flex-report-0.6.6/flex_report/urls.py` & `django-flex-report-0.6.7/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/flex_report/utils.py` & `django-flex-report-0.6.7/flex_report/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 
     field = get_model_property(model, column)
 
     if isinstance(field, property):
         return FieldTypes.property
 
     if callable(field):
-        return FieldTypes.custom
+        return FieldTypes.dynamic
 
     return None
 
 
 def get_fields_lookups(model, fields):
     """
     Takes in a model and a list of fields, and returns a dict where the keys are the field names,
```

### Comparing `django-flex-report-0.6.6/flex_report/views.py` & `django-flex-report-0.6.7/flex_report/views.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.6/pyproject.toml` & `django-flex-report-0.6.7/pyproject.toml`

 * *Files identical despite different names*

