# Comparing `tmp/caluma_alexandria-4.0.0.tar.gz` & `tmp/caluma_alexandria-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-4.0.0.tar", max compression
+gzip compressed data, was "caluma_alexandria-4.0.1.tar", max compression
```

## Comparing `caluma_alexandria-4.0.0.tar` & `caluma_alexandria-4.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    23937 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/LICENSE
--rw-r--r--   0        0        0     8517 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/__init__.py
--rw-r--r--   0        0        0     2199 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/api.py
--rw-r--r--   0        0        0      127 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/apps.py
--rw-r--r--   0        0        0    13501 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/factories.py
--rw-r--r--   0        0        0     6937 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/filters.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2394 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/encrypt_files.py
--rw-r--r--   0        0        0      586 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/generate_missing_thumbnails.py
--rw-r--r--   0        0        0     1084 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/set_mime_type_and_size.py
--rw-r--r--   0        0        0    12553 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2840 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0      652 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0007_category_parent.py
--rw-r--r--   0        0        0      397 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0008_document_date.py
--rw-r--r--   0        0        0      466 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0009_file_checksum.py
--rw-r--r--   0        0        0     2973 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0010_mark.py
--rw-r--r--   0        0        0     1205 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0011_tag_uuid.py
--rw-r--r--   0        0        0     1655 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0012_tag_uuid_schema.py
--rw-r--r--   0        0        0     2086 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0013_file_content.py
--rw-r--r--   0        0        0      975 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0014_file_mime_type_size.py
--rw-r--r--   0        0        0     3304 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0015_fix_modified_by_description.py
--rw-r--r--   0        0        0      672 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0016_category_allowed_mime_types.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/models.py
--rw-r--r--   0        0        0     1823 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/presign_urls.py
--rw-r--r--   0        0        0    11317 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/serializers.py
--rw-r--r--   0        0        0      409 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/urls.py
--rw-r--r--   0        0        0     1463 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/validations.py
--rw-r--r--   0        0        0     9113 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/views.py
--rw-r--r--   0        0        0     1363 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/visibilities.py
--rw-r--r--   0        0        0     1703 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/dav.py
--rw-r--r--   0        0        0     4530 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/dav_provider.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     7450 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     5154 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/django.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/backends/__init__.py
--rw-r--r--   0        0        0     1493 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/backends/s3.py
--rw-r--r--   0        0        0     2595 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/fields.py
--rw-r--r--   0        0        0      162 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/urls.py
--rw-r--r--   0        0        0     1048 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/wsgi.py
--rw-r--r--   0        0        0     3265 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    10221 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    24102 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/LICENSE
+-rw-r--r--   0        0        0     8517 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/__init__.py
+-rw-r--r--   0        0        0     2199 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/api.py
+-rw-r--r--   0        0        0      127 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/apps.py
+-rw-r--r--   0        0        0    13501 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/factories.py
+-rw-r--r--   0        0        0     6937 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/filters.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2394 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/encrypt_files.py
+-rw-r--r--   0        0        0      586 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/generate_missing_thumbnails.py
+-rw-r--r--   0        0        0     1084 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/set_mime_type_and_size.py
+-rw-r--r--   0        0        0    12553 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2840 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0      652 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0007_category_parent.py
+-rw-r--r--   0        0        0      397 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0008_document_date.py
+-rw-r--r--   0        0        0      466 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0009_file_checksum.py
+-rw-r--r--   0        0        0     2973 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0010_mark.py
+-rw-r--r--   0        0        0     1205 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0011_tag_uuid.py
+-rw-r--r--   0        0        0     1655 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0012_tag_uuid_schema.py
+-rw-r--r--   0        0        0     2086 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0013_file_content.py
+-rw-r--r--   0        0        0      975 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0014_file_mime_type_size.py
+-rw-r--r--   0        0        0     3304 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0015_fix_modified_by_description.py
+-rw-r--r--   0        0        0      672 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0016_category_allowed_mime_types.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0    10789 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/models.py
+-rw-r--r--   0        0        0     1823 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/presign_urls.py
+-rw-r--r--   0        0        0    11317 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/serializers.py
+-rw-r--r--   0        0        0      409 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1463 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/validations.py
+-rw-r--r--   0        0        0     9113 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/views.py
+-rw-r--r--   0        0        0     1363 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0     1703 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/dav.py
+-rw-r--r--   0        0        0     4530 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/dav_provider.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     7449 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     5154 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/django.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/backends/__init__.py
+-rw-r--r--   0        0        0     1493 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/backends/s3.py
+-rw-r--r--   0        0        0     2595 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/fields.py
+-rw-r--r--   0        0        0      162 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/urls.py
+-rw-r--r--   0        0        0     1048 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/wsgi.py
+-rw-r--r--   0        0        0     3265 2024-04-15 11:55:05.609381 caluma_alexandria-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10221 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.1/PKG-INFO
```

### Comparing `caluma_alexandria-4.0.0/CHANGELOG.md` & `caluma_alexandria-4.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 4.0.1
+### Fix
+* **thumbnails:** Enlarge the thumbnails ([`a80f7b5`](https://github.com/projectcaluma/alexandria/commit/a80f7b535ba21e3c8a3c23318cb95ca4be70f273))
+
 # 4.0.0
 ### Feature
 * **document:** Create document and file in one request! ([`444912d`](https://github.com/projectcaluma/alexandria/commit/444912d4cb584c05096ca8a78dd455b8471e9441))
 
 ### Breaking
 * The document post endpoint now requires the file data to be provided as well. The reason for this change is allowing the frontend to create documents and files in one request, preventing documents with no associated files. Which fixes the problem if the file got rejected for any reason, the application would create an empty document. ([`444912d`](https://github.com/projectcaluma/alexandria/commit/444912d4cb584c05096ca8a78dd455b8471e9441))
```

### Comparing `caluma_alexandria-4.0.0/LICENSE` & `caluma_alexandria-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/README.md` & `caluma_alexandria-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/api.py` & `caluma_alexandria-4.0.1/alexandria/core/api.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/factories.py` & `caluma_alexandria-4.0.1/alexandria/core/factories.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/filters.py` & `caluma_alexandria-4.0.1/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/management/commands/encrypt_files.py` & `caluma_alexandria-4.0.1/alexandria/core/management/commands/encrypt_files.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/management/commands/generate_missing_thumbnails.py` & `caluma_alexandria-4.0.1/alexandria/core/management/commands/generate_missing_thumbnails.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/management/commands/set_mime_type_and_size.py` & `caluma_alexandria-4.0.1/alexandria/core/management/commands/set_mime_type_and_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0007_category_parent.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0007_category_parent.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0010_mark.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0010_mark.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0011_tag_uuid.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0011_tag_uuid.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0012_tag_uuid_schema.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0012_tag_uuid_schema.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0013_file_content.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0013_file_content.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0014_file_mime_type_size.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0014_file_mime_type_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0015_fix_modified_by_description.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0015_fix_modified_by_description.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/migrations/0016_category_allowed_mime_types.py` & `caluma_alexandria-4.0.1/alexandria/core/migrations/0016_category_allowed_mime_types.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/models.py` & `caluma_alexandria-4.0.1/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/presign_urls.py` & `caluma_alexandria-4.0.1/alexandria/core/presign_urls.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/serializers.py` & `caluma_alexandria-4.0.1/alexandria/core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/validations.py` & `caluma_alexandria-4.0.1/alexandria/core/validations.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/views.py` & `caluma_alexandria-4.0.1/alexandria/core/views.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/core/visibilities.py` & `caluma_alexandria-4.0.1/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/dav.py` & `caluma_alexandria-4.0.1/alexandria/dav.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/dav_provider.py` & `caluma_alexandria-4.0.1/alexandria/dav_provider.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-4.0.1/alexandria/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/oidc_auth/models.py` & `caluma_alexandria-4.0.1/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/settings/alexandria.py` & `caluma_alexandria-4.0.1/alexandria/settings/alexandria.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 )
 
 # Thumbnails
 ALEXANDRIA_ENABLE_THUMBNAIL_GENERATION = env.bool(
     "ALEXANDRIA_ENABLE_THUMBNAIL_GENERATION", default=True
 )
 ALEXANDRIA_THUMBNAIL_WIDTH = env.int("ALEXANDRIA_THUMBNAIL_WIDTH", default=None)
-ALEXANDRIA_THUMBNAIL_HEIGHT = env.int("ALEXANDRIA_THUMBNAIL_HEIGHT", default=None)
+ALEXANDRIA_THUMBNAIL_HEIGHT = env.int("ALEXANDRIA_THUMBNAIL_HEIGHT", default=600)
 
 # Checksums
 ALEXANDRIA_ENABLE_CHECKSUM = env.bool("ALEXANDRIA_ENABLE_CHECKSUM", default=True)
 
 # Clamav service
 CLAMD_SOCKET = env.str("ALEXANDRIA_CLAMD_SOCKET", default="/var/run/clamav/clamd.ctl")
 CLAMD_USE_TCP = env.bool("ALEXANDRIA_CLAMD_USE_TCP", default=True)
```

### Comparing `caluma_alexandria-4.0.0/alexandria/settings/django.py` & `caluma_alexandria-4.0.1/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/storages/backends/s3.py` & `caluma_alexandria-4.0.1/alexandria/storages/backends/s3.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/storages/fields.py` & `caluma_alexandria-4.0.1/alexandria/storages/fields.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/alexandria/wsgi.py` & `caluma_alexandria-4.0.1/alexandria/wsgi.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.0/pyproject.toml` & `caluma_alexandria-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "4.0.0"
+version = "4.0.1"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `caluma_alexandria-4.0.0/PKG-INFO` & `caluma_alexandria-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 4.0.0
+Version: 4.0.1
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

