# Comparing `tmp/crepex_django_util-0.7.4.tar.gz` & `tmp/crepex_django_util-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepex_django_util-0.7.4.tar", max compression
+gzip compressed data, was "crepex_django_util-0.8.0.tar", max compression
```

## Comparing `crepex_django_util-0.7.4.tar` & `crepex_django_util-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      943 2023-09-20 01:37:47.371055 crepex_django_util-0.7.4/README.md
--rw-r--r--   0        0        0      534 2024-03-18 08:46:10.092929 crepex_django_util-0.7.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-12 08:41:16.226704 crepex_django_util-0.7.4/src/crepex_django_util/__init__.py
--rw-r--r--   0        0        0       42 2023-09-14 02:23:35.476452 crepex_django_util-0.7.4/src/crepex_django_util/admin/__init__.py
--rw-r--r--   0        0        0     3153 2024-03-14 05:29:11.288146 crepex_django_util-0.7.4/src/crepex_django_util/admin/actions.py
--rw-r--r--   0        0        0      716 2023-09-15 01:35:36.740796 crepex_django_util-0.7.4/src/crepex_django_util/admin/utils.py
--rw-r--r--   0        0        0      557 2023-09-12 10:21:22.346796 crepex_django_util-0.7.4/src/crepex_django_util/exceptions.py
--rwxr-xr-x   0        0        0     5768 2023-09-26 06:46:55.121097 crepex_django_util-0.7.4/src/crepex_django_util/fields.py
--rw-r--r--   0        0        0      371 2023-09-26 06:49:36.038702 crepex_django_util-0.7.4/src/crepex_django_util/filters.py
--rw-r--r--   0        0        0        0 2023-09-20 08:37:39.972173 crepex_django_util-0.7.4/src/crepex_django_util/models/__init__.py
--rwxr-xr-x   0        0        0     2474 2023-09-20 08:40:02.030333 crepex_django_util-0.7.4/src/crepex_django_util/models/inheritance.py
--rw-r--r--   0        0        0      467 2023-08-19 17:08:16.684864 crepex_django_util-0.7.4/src/crepex_django_util/paginations.py
--rw-r--r--   0        0        0        0 2023-09-25 01:03:37.182593 crepex_django_util-0.7.4/src/crepex_django_util/payments/__init__.py
--rw-r--r--   0        0        0     7043 2024-02-28 05:09:37.286212 crepex_django_util-0.7.4/src/crepex_django_util/payments/payple.py
--rw-r--r--   0        0        0      127 2023-09-25 01:03:37.183714 crepex_django_util-0.7.4/src/crepex_django_util/payments/types.py
--rw-r--r--   0        0        0      253 2023-10-23 09:02:02.565724 crepex_django_util-0.7.4/src/crepex_django_util/permissions.py
--rw-r--r--   0        0        0        0 2023-09-14 09:04:48.762319 crepex_django_util-0.7.4/src/crepex_django_util/serializers/__init__.py
--rw-r--r--   0        0        0      759 2023-09-20 04:30:51.141241 crepex_django_util-0.7.4/src/crepex_django_util/serializers/generics.py
--rw-r--r--   0        0        0     7559 2023-10-26 01:56:23.112950 crepex_django_util-0.7.4/src/crepex_django_util/serializers/mixins.py
--rw-r--r--   0        0        0     1298 2023-09-25 01:03:37.184020 crepex_django_util-0.7.4/src/crepex_django_util/settings.py
--rwxr-xr-x   0        0        0      179 2023-09-14 01:14:37.773476 crepex_django_util-0.7.4/src/crepex_django_util/utils.py
--rw-r--r--   0        0        0      257 2023-09-27 02:40:59.524905 crepex_django_util-0.7.4/src/crepex_django_util/validators.py
--rw-r--r--   0        0        0        0 2023-09-14 02:31:06.146120 crepex_django_util-0.7.4/src/crepex_django_util/views/__init__.py
--rw-r--r--   0        0        0     3111 2023-10-06 09:02:09.132117 crepex_django_util-0.7.4/src/crepex_django_util/views/generics.py
--rw-r--r--   0        0        0     6435 2023-10-06 08:36:00.258302 crepex_django_util-0.7.4/src/crepex_django_util/views/mixins.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 crepex_django_util-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      943 2023-09-20 01:37:47.371055 crepex_django_util-0.8.0/README.md
+-rw-r--r--   0        0        0      534 2024-04-15 05:55:41.249253 crepex_django_util-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-12 08:41:16.226704 crepex_django_util-0.8.0/src/crepex_django_util/__init__.py
+-rw-r--r--   0        0        0       42 2023-09-14 02:23:35.476452 crepex_django_util-0.8.0/src/crepex_django_util/admin/__init__.py
+-rw-r--r--   0        0        0     3153 2024-03-14 05:29:11.288146 crepex_django_util-0.8.0/src/crepex_django_util/admin/actions.py
+-rw-r--r--   0        0        0     2302 2024-03-23 11:12:09.721495 crepex_django_util-0.8.0/src/crepex_django_util/admin/mixins.py
+-rw-r--r--   0        0        0      716 2023-09-15 01:35:36.740796 crepex_django_util-0.8.0/src/crepex_django_util/admin/utils.py
+-rw-r--r--   0        0        0      557 2023-09-12 10:21:22.346796 crepex_django_util-0.8.0/src/crepex_django_util/exceptions.py
+-rwxr-xr-x   0        0        0     5768 2023-09-26 06:46:55.121097 crepex_django_util-0.8.0/src/crepex_django_util/fields.py
+-rw-r--r--   0        0        0      371 2024-03-22 05:45:07.340415 crepex_django_util-0.8.0/src/crepex_django_util/filters.py
+-rw-r--r--   0        0        0        0 2023-09-20 08:37:39.972173 crepex_django_util-0.8.0/src/crepex_django_util/models/__init__.py
+-rwxr-xr-x   0        0        0     2474 2024-03-22 05:44:45.991572 crepex_django_util-0.8.0/src/crepex_django_util/models/inheritance.py
+-rw-r--r--   0        0        0      467 2023-08-19 17:08:16.684864 crepex_django_util-0.8.0/src/crepex_django_util/paginations.py
+-rw-r--r--   0        0        0        0 2023-09-25 01:03:37.182593 crepex_django_util-0.8.0/src/crepex_django_util/payments/__init__.py
+-rw-r--r--   0        0        0     7043 2024-02-28 05:09:37.286212 crepex_django_util-0.8.0/src/crepex_django_util/payments/payple.py
+-rw-r--r--   0        0        0      127 2023-09-25 01:03:37.183714 crepex_django_util-0.8.0/src/crepex_django_util/payments/types.py
+-rw-r--r--   0        0        0      253 2023-10-23 09:02:02.565724 crepex_django_util-0.8.0/src/crepex_django_util/permissions.py
+-rw-r--r--   0        0        0        0 2023-09-14 09:04:48.762319 crepex_django_util-0.8.0/src/crepex_django_util/serializers/__init__.py
+-rw-r--r--   0        0        0      759 2023-09-20 04:30:51.141241 crepex_django_util-0.8.0/src/crepex_django_util/serializers/generics.py
+-rw-r--r--   0        0        0     7559 2023-10-26 01:56:23.112950 crepex_django_util-0.8.0/src/crepex_django_util/serializers/mixins.py
+-rw-r--r--   0        0        0     1298 2023-09-25 01:03:37.184020 crepex_django_util-0.8.0/src/crepex_django_util/settings.py
+-rwxr-xr-x   0        0        0      770 2024-04-15 05:27:50.202140 crepex_django_util-0.8.0/src/crepex_django_util/utils.py
+-rw-r--r--   0        0        0      257 2023-09-27 02:40:59.524905 crepex_django_util-0.8.0/src/crepex_django_util/validators.py
+-rw-r--r--   0        0        0        0 2023-09-14 02:31:06.146120 crepex_django_util-0.8.0/src/crepex_django_util/views/__init__.py
+-rw-r--r--   0        0        0     3111 2023-10-06 09:02:09.132117 crepex_django_util-0.8.0/src/crepex_django_util/views/generics.py
+-rw-r--r--   0        0        0     6435 2023-10-06 08:36:00.258302 crepex_django_util-0.8.0/src/crepex_django_util/views/mixins.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 crepex_django_util-0.8.0/PKG-INFO
```

### Comparing `crepex_django_util-0.7.4/README.md` & `crepex_django_util-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/pyproject.toml` & `crepex_django_util-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crepex-django-util"
-version = "0.7.4"
+version = "0.8.0"
 description = "CrepeX django utilities"
 authors = ["Hyunwoo Shim <hyunwoo.shim@crepe-x.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 crepex-pyutil = ">= 0.14.0 < 1.0.0"
```

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/admin/actions.py` & `crepex_django_util-0.8.0/src/crepex_django_util/admin/actions.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/admin/utils.py` & `crepex_django_util-0.8.0/src/crepex_django_util/admin/utils.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/exceptions.py` & `crepex_django_util-0.8.0/src/crepex_django_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/fields.py` & `crepex_django_util-0.8.0/src/crepex_django_util/fields.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/models/inheritance.py` & `crepex_django_util-0.8.0/src/crepex_django_util/models/inheritance.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/payments/payple.py` & `crepex_django_util-0.8.0/src/crepex_django_util/payments/payple.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/serializers/generics.py` & `crepex_django_util-0.8.0/src/crepex_django_util/serializers/generics.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/serializers/mixins.py` & `crepex_django_util-0.8.0/src/crepex_django_util/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/settings.py` & `crepex_django_util-0.8.0/src/crepex_django_util/settings.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/views/generics.py` & `crepex_django_util-0.8.0/src/crepex_django_util/views/generics.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/src/crepex_django_util/views/mixins.py` & `crepex_django_util-0.8.0/src/crepex_django_util/views/mixins.py`

 * *Files identical despite different names*

### Comparing `crepex_django_util-0.7.4/PKG-INFO` & `crepex_django_util-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepex-django-util
-Version: 0.7.4
+Version: 0.8.0
 Summary: CrepeX django utilities
 Author: Hyunwoo Shim
 Author-email: hyunwoo.shim@crepe-x.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

