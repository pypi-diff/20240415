# Comparing `tmp/drfexts-3.8.0.tar.gz` & `tmp/drfexts-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfexts-3.8.0.tar", max compression
+gzip compressed data, was "drfexts-3.8.1.tar", max compression
```

## Comparing `drfexts-3.8.0.tar` & `drfexts-3.8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.0/LICENSE
--rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.0/README.md
--rw-r--r--   0        0        0       22 2024-04-09 09:51:53.219838 drfexts-3.8.0/drfexts/__init__.py
--rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.0/drfexts/authentication.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.0/drfexts/choices.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.0/drfexts/constants.py
--rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.0/drfexts/exceptions.py
--rw-r--r--   0        0        0    14579 2024-02-19 06:44:03.902452 drfexts-3.8.0/drfexts/fields.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.0/drfexts/filtersets/__init__.py
--rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.0/drfexts/filtersets/backends.py
--rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.0/drfexts/filtersets/fields.py
--rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.0/drfexts/filtersets/filters.py
--rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.0/drfexts/filtersets/widgets.py
--rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.0/drfexts/middlewares.py
--rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.0/drfexts/models.py
--rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.0/drfexts/pagination.py
--rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.0/drfexts/paginators.py
--rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.0/drfexts/parsers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.0/drfexts/permissions.py
--rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.0/drfexts/renderers.py
--rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.0/drfexts/routers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.0/drfexts/serializers/__init__.py
--rw-r--r--   0        0        0    11478 2024-04-02 08:08:13.730672 drfexts-3.8.0/drfexts/serializers/fields.py
--rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.0/drfexts/serializers/mixins.py
--rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.0/drfexts/serializers/serializers.py
--rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.0/drfexts/settings.py
--rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.0/drfexts/storages.py
--rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.0/drfexts/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.0/drfexts/utils/encoders.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.0/drfexts/utils/log.py
--rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.0/drfexts/utils/string.py
--rw-r--r--   0        0        0     3769 2024-01-26 07:54:13.389069 drfexts-3.8.0/drfexts/utils/utils.py
--rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.0/drfexts/viewsets.py
--rw-r--r--   0        0        0     1649 2024-04-09 09:51:53.230140 drfexts-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 drfexts-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.1/LICENSE
+-rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-15 02:12:15.440137 drfexts-3.8.1/drfexts/__init__.py
+-rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.1/drfexts/authentication.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.1/drfexts/choices.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.1/drfexts/constants.py
+-rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.1/drfexts/exceptions.py
+-rw-r--r--   0        0        0    14579 2024-02-19 06:44:03.902452 drfexts-3.8.1/drfexts/fields.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.1/drfexts/filtersets/__init__.py
+-rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.1/drfexts/filtersets/backends.py
+-rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.1/drfexts/filtersets/fields.py
+-rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.1/drfexts/filtersets/filters.py
+-rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.1/drfexts/filtersets/widgets.py
+-rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.1/drfexts/middlewares.py
+-rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.1/drfexts/models.py
+-rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.1/drfexts/pagination.py
+-rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.1/drfexts/paginators.py
+-rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.1/drfexts/parsers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.1/drfexts/permissions.py
+-rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.1/drfexts/renderers.py
+-rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.1/drfexts/routers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.1/drfexts/serializers/__init__.py
+-rw-r--r--   0        0        0    11478 2024-04-02 08:08:13.730672 drfexts-3.8.1/drfexts/serializers/fields.py
+-rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.1/drfexts/serializers/mixins.py
+-rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.1/drfexts/serializers/serializers.py
+-rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.1/drfexts/settings.py
+-rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.1/drfexts/storages.py
+-rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.1/drfexts/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.1/drfexts/utils/encoders.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.1/drfexts/utils/log.py
+-rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.1/drfexts/utils/string.py
+-rw-r--r--   0        0        0     3976 2024-04-15 02:12:05.521855 drfexts-3.8.1/drfexts/utils/utils.py
+-rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.1/drfexts/viewsets.py
+-rw-r--r--   0        0        0     1649 2024-04-15 02:12:15.446211 drfexts-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 drfexts-3.8.1/PKG-INFO
```

### Comparing `drfexts-3.8.0/LICENSE` & `drfexts-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/README.md` & `drfexts-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/choices.py` & `drfexts-3.8.1/drfexts/choices.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/constants.py` & `drfexts-3.8.1/drfexts/constants.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/exceptions.py` & `drfexts-3.8.1/drfexts/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/fields.py` & `drfexts-3.8.1/drfexts/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/filtersets/backends.py` & `drfexts-3.8.1/drfexts/filtersets/backends.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/filtersets/fields.py` & `drfexts-3.8.1/drfexts/filtersets/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/filtersets/filters.py` & `drfexts-3.8.1/drfexts/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/filtersets/widgets.py` & `drfexts-3.8.1/drfexts/filtersets/widgets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/middlewares.py` & `drfexts-3.8.1/drfexts/middlewares.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/models.py` & `drfexts-3.8.1/drfexts/models.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/pagination.py` & `drfexts-3.8.1/drfexts/pagination.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/paginators.py` & `drfexts-3.8.1/drfexts/paginators.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/parsers.py` & `drfexts-3.8.1/drfexts/parsers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/renderers.py` & `drfexts-3.8.1/drfexts/renderers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/serializers/fields.py` & `drfexts-3.8.1/drfexts/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/serializers/mixins.py` & `drfexts-3.8.1/drfexts/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/serializers/serializers.py` & `drfexts-3.8.1/drfexts/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/settings.py` & `drfexts-3.8.1/drfexts/settings.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/storages.py` & `drfexts-3.8.1/drfexts/storages.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/drfexts/utils/utils.py` & `drfexts-3.8.1/drfexts/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,21 +104,25 @@
 
 
 def get_error_msg(data: dict | list, default_field_key):
     if isinstance(data, dict):
         if "detail" in data:
             return str(data["detail"])
         elif default_field_key in data:
-            return "/n".join(str(s) for s in data[default_field_key])
+            return "\n".join(str(s) for s in data[default_field_key])
 
         errors = []
         for k, v in data.items():
-            errors.append(f"{k}: {'/n'.join(str(s) for s in v)}")
+            if isinstance(v, dict):
+                errors.append(get_error_msg(v, default_field_key))
+                # errors.append(f"{k}: {'\n'.join(str(s) for s in v.values())}")
+            else:
+                errors.append(f"{k}: " + "\n".join(str(s) for s in v))
 
-        return "/n".join(errors)
+        return "\n".join(errors)
     elif isinstance(data, exceptions.ErrorDetail):
         return str(data)
     elif isinstance(data, list):
         data = data[0]
         return get_error_msg(data, default_field_key)
 
     return str(data)
```

### Comparing `drfexts-3.8.0/drfexts/viewsets.py` & `drfexts-3.8.1/drfexts/viewsets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.0/pyproject.toml` & `drfexts-3.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.commitizen]
-version = "3.8.0"
+version = "3.8.1"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = ["pyproject.toml:version", "drfexts/__init__.py"]
 
 [tool.poetry]
 name = "drfexts"
-version = "3.8.0"
+version = "3.8.1"
 package-mode = true
 readme = "README.md"
 description = "Django Restframework Utils"
 authors = ["aiden <allaher@icloud.com>"]
 keywords = ["django", "restframework"]
 homepage = "https://github.com/aiden520/drfexts"
 repository = "https://github.com/aiden520/drfexts"
```

### Comparing `drfexts-3.8.0/PKG-INFO` & `drfexts-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfexts
-Version: 3.8.0
+Version: 3.8.1
 Summary: Django Restframework Utils
 Home-page: https://github.com/aiden520/drfexts
 License: Apache-2.0
 Keywords: django,restframework
 Author: aiden
 Author-email: allaher@icloud.com
 Requires-Python: >=3.10,<4.0.0
```

