# Comparing `tmp/ckanext-files-0.2.3.tar.gz` & `tmp/ckanext_files-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-files-0.2.3.tar", last modified: Sun Apr  7 16:20:42 2024, max compression
+gzip compressed data, was "ckanext_files-0.2.4.tar", last modified: Mon Apr 15 14:23:49 2024, max compression
```

## Comparing `ckanext-files-0.2.3.tar` & `ckanext_files-0.2.4.tar`

### file list

```diff
@@ -1,102 +1,107 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/file_manager/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext-files-0.2.3/ckanext/file_manager/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/collection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      185 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/resource.config
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8250 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    26019 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--queue.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    44982 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--shared.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/styles/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/styles/files--style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      358 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10850 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4113 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/exceptions.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9684 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2159 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/files/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/migration/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/migration/files/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/migration/files/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/migration/files/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/model/file.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7500 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/storage/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10667 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/storage/google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4465 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/storage/redis.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/files/templates/files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5129 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/file_table.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2045 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/uploader_v1.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/files/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/user/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      793 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/user/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_redis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12019 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4069 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4293 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/ckanext_files.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2987 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.896156 ckanext_files-0.2.4/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-15 14:23:49.896156 ckanext_files-0.2.4/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/file_manager/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext_files-0.2.4/ckanext/file_manager/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/file_manager/collection.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/file_manager/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/file_manager/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/files/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-04-09 01:54:26.000000 ckanext_files-0.2.4/ckanext/files/assets/resource.config
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/files/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8237 2024-04-15 14:21:37.000000 ckanext_files-0.2.4/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    37143 2024-04-15 14:21:37.000000 ckanext_files-0.2.4/ckanext/files/assets/scripts/files--modules.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.4/ckanext/files/assets/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    44969 2024-04-15 14:21:37.000000 ckanext_files-0.2.4/ckanext/files/assets/scripts/files--shared.js
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/files/assets/styles/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      197 2024-04-09 02:46:04.000000 ckanext_files-0.2.4/ckanext/files/assets/styles/files--style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      360 2024-04-09 01:54:34.000000 ckanext_files-0.2.4/ckanext/files/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14339 2024-04-15 14:22:47.000000 ckanext_files-0.2.4/ckanext/files/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext_files-0.2.4/ckanext/files/command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4481 2024-04-15 14:21:38.000000 ckanext_files-0.2.4/ckanext/files/exceptions.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.886156 ckanext_files-0.2.4/ckanext/files/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9684 2024-04-09 02:24:32.000000 ckanext_files-0.2.4/ckanext/files/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext_files-0.2.4/ckanext/files/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext_files-0.2.4/ckanext/files/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2024-04-15 14:22:08.000000 ckanext_files-0.2.4/ckanext/files/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.882823 ckanext_files-0.2.4/ckanext/files/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/migration/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/migration/files/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/migration/files/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/migration/files/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext_files-0.2.4/ckanext/files/model/file.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/model/owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.882823 ckanext_files-0.2.4/ckanext/files/public/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.882823 ckanext_files-0.2.4/ckanext/files/public/ckanext-files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/public/ckanext-files/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.4/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7410 2024-04-09 11:03:43.000000 ckanext_files-0.2.4/ckanext/files/storage/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10683 2024-04-09 11:03:53.000000 ckanext_files-0.2.4/ckanext/files/storage/google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4719 2024-04-15 14:21:38.000000 ckanext_files-0.2.4/ckanext/files/storage/redis.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.882823 ckanext_files-0.2.4/ckanext/files/templates/files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/templates/files/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/templates/files/snippets/_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/templates/files/snippets/_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5167 2024-04-09 03:20:53.000000 ckanext_files-0.2.4/ckanext/files/templates/files/snippets/file_table.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2451 2024-04-09 05:48:11.000000 ckanext_files-0.2.4/ckanext/files/templates/files/snippets/uploader_v1.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/templates/files/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/templates/files/user/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      847 2024-04-09 05:48:21.000000 ckanext_files-0.2.4/ckanext/files/templates/files/user/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext_files-0.2.4/ckanext/files/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.889490 ckanext_files-0.2.4/ckanext/files/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/ckanext/files/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.892823 ckanext_files-0.2.4/ckanext/files/tests/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/storage/test_fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/storage/test_google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/storage/test_redis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11805 2024-04-09 11:08:13.000000 ckanext_files-0.2.4/ckanext/files/tests/test_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/test_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/ckanext/files/types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5490 2024-04-15 14:21:38.000000 ckanext_files-0.2.4/ckanext/files/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4347 2024-04-09 03:19:07.000000 ckanext_files-0.2.4/ckanext/files/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-15 14:23:49.892823 ckanext_files-0.2.4/ckanext_files.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3113 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-15 14:23:49.000000 ckanext_files-0.2.4/ckanext_files.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext_files-0.2.4/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-15 14:23:49.896156 ckanext_files-0.2.4/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext_files-0.2.4/setup.py
```

### Comparing `ckanext-files-0.2.3/LICENSE` & `ckanext_files-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/PKG-INFO` & `ckanext_files-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-files-0.2.3/README.md` & `ckanext_files-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/file_manager/collection.py` & `ckanext_files-0.2.4/ckanext/file_manager/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/file_manager/plugin.py` & `ckanext_files-0.2.4/ckanext/file_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/file_manager/views.py` & `ckanext_files-0.2.4/ckanext/file_manager/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js` & `ckanext_files-0.2.4/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,7 @@
-"use strict";
 var ckan;
 (function(ckan) {
     let CKANEXT_FILES;
     (function(CKANEXT_FILES) {
         let adapters;
         (function(adapters) {
             class GCSMultipart extends adapters.Multipart {
@@ -43,8 +42,8 @@
                     });
                 }
             }
             adapters.GCSMultipart = GCSMultipart;
         })(adapters = CKANEXT_FILES.adapters || (CKANEXT_FILES.adapters = {}));
     })(CKANEXT_FILES = ckan.CKANEXT_FILES || (ckan.CKANEXT_FILES = {}));
 })(ckan || (ckan = {}));
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLWdvb2dsZS1jbG91ZC1zdG9yYWdlLXVwbG9hZGVyLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vdHMvZmlsZXMtLWdvb2dsZS1jbG91ZC1zdG9yYWdlLXVwbG9hZGVyLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7QUFBQSxJQUFVLElBQUksQ0FvRWI7QUFwRUQsV0FBVSxJQUFJO0lBQ1osSUFBaUIsYUFBYSxDQWtFN0I7SUFsRUQsV0FBaUIsYUFBYTtRQUM1QixJQUFpQixRQUFRLENBZ0V4QjtRQWhFRCxXQUFpQixRQUFRO1lBS3ZCLE1BQWEsWUFBYSxTQUFRLFNBQUEsU0FBUztnQkFDekMsS0FBSyxDQUFDLFlBQVksQ0FDaEIsSUFBbUIsRUFDbkIsSUFBVSxFQUNWLEtBQWE7b0JBRWIsSUFBSSxDQUFDLElBQUksQ0FBQyxJQUFJLEVBQUUsQ0FBQzt3QkFDZixNQUFNLElBQUksS0FBSyxDQUFDLGlDQUFpQyxDQUFDLENBQUM7b0JBQ3JELENBQUM7b0JBRUQsTUFBTSxPQUFPLEdBQUcsSUFBSSxjQUFjLEVBQUUsQ0FBQztvQkFFckMsT0FBTyxDQUFDLElBQUksQ0FBQyxLQUFLLEVBQUUsSUFBSSxDQUFDLFlBQVksQ0FBQyxXQUFXLENBQUMsQ0FBQztvQkFDbkQsT0FBTyxDQUFDLGdCQUFnQixDQUN0QixlQUFlLEVBQ2YsU0FBUyxLQUFLLElBQUksS0FBSyxHQUFHLElBQUksQ0FBQyxJQUFJLEdBQUcsQ0FBQyxJQUFJLElBQUksQ0FBQyxZQUFZLENBQUMsSUFBSSxFQUFFLENBQ3BFLENBQUM7b0JBQ0YsT0FBTyxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztvQkFFbkIsTUFBTSxJQUFJLEdBQVEsTUFBTSxJQUFJLE9BQU8sQ0FBQyxDQUFDLElBQUksRUFBRSxJQUFJLEVBQUUsRUFBRTt3QkFDakQsT0FBTyxDQUFDLGdCQUFnQixDQUFDLE1BQU0sRUFBRSxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsSUFBSSxDQUFDLE9BQU8sQ0FBQyxDQUFDLENBQUM7b0JBQzdELENBQUMsQ0FBQyxDQUFDO29CQUNILElBQUksUUFBUSxDQUFDO29CQUViLElBQUksQ0FBQyxHQUFHLEVBQUUsR0FBRyxDQUFDLENBQUMsUUFBUSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsRUFBRSxDQUFDO3dCQUNyQyxRQUFRLEdBQUcsSUFBSSxDQUFDLFlBQVksQ0FBQyxJQUFJLENBQUM7b0JBQ3BDLENBQUM7eUJBQU0sSUFBSSxJQUFJLENBQUMsTUFBTSxLQUFLLEdBQUcsRUFBRSxDQUFDO3dCQUMvQixNQUFNLEtBQUssR0FBRyxJQUFJLENBQUMsaUJBQWlCLENBQUMsT0FBTyxDQUFDLENBQUM7d0JBQzlDLFFBQVEsR0FBRyxNQUFNLENBQUMsS0FBSyxDQUFDLEtBQUssQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDLENBQUMsQ0FBQyxLQUFLLENBQUMsR0FBRyxDQUFDLENBQUMsQ0FBQyxDQUFDLENBQUMsR0FBRyxDQUFDLENBQUM7b0JBQzNELENBQUM7eUJBQU0sQ0FBQzt3QkFDTixNQUFNLElBQUksS0FBSyxDQUFDLE1BQU0sSUFBSSxDQUFDLFlBQVksQ0FBQyxDQUFDO29CQUMzQyxDQUFDO29CQUVELElBQUksQ0FBQyxNQUFNLENBQUMsU0FBUyxDQUFDLFFBQVEsQ0FBQyxFQUFFLENBQUM7d0JBQ2hDLE1BQU0sSUFBSSxLQUFLLENBQUMseUJBQXlCLFFBQVEsRUFBRSxDQUFDLENBQUM7b0JBQ3ZELENBQUM7b0JBRUQsT0FBTyxJQUFJLE9BQU8sQ0FBQyxDQUFDLElBQUksRUFBRSxJQUFJLEVBQUUsRUFBRTt3QkFDaEMsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsSUFBSSxDQUN0QixNQUFNLEVBQ04scUJBQXFCLEVBQ3JCOzRCQUNFLEVBQUUsRUFBRSxJQUFJLENBQUMsRUFBRTs0QkFDWCxRQUFRO3lCQUNULEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTs0QkFDWixJQUFJLENBQUMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxDQUFDO3dCQUNwQixDQUFDLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTs0QkFDWixJQUFJLENBQ0YsT0FBTyxJQUFJLENBQUMsWUFBWSxLQUFLLFFBQVE7Z0NBQ25DLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWTtnQ0FDbkIsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUM1QixDQUFDO3dCQUNKLENBQUMsQ0FDRixDQUFDO29CQUNKLENBQUMsQ0FBQyxDQUFDO2dCQUNMLENBQUM7YUFDRjtZQTFEWSxxQkFBWSxlQTBEeEIsQ0FBQTtRQUNILENBQUMsRUFoRWdCLFFBQVEsR0FBUixzQkFBUSxLQUFSLHNCQUFRLFFBZ0V4QjtJQUNILENBQUMsRUFsRWdCLGFBQWEsR0FBYixrQkFBYSxLQUFiLGtCQUFhLFFBa0U3QjtBQUNILENBQUMsRUFwRVMsSUFBSSxLQUFKLElBQUksUUFvRWIiLCJzb3VyY2VzQ29udGVudCI6WyJuYW1lc3BhY2UgY2thbiB7XG4gIGV4cG9ydCBuYW1lc3BhY2UgQ0tBTkVYVF9GSUxFUyB7XG4gICAgZXhwb3J0IG5hbWVzcGFjZSBhZGFwdGVycyB7XG4gICAgICBleHBvcnQgdHlwZSBHQ1NVcGxvYWRJbmZvID0gVXBsb2FkSW5mbyAmIHtcbiAgICAgICAgc3RvcmFnZV9kYXRhOiBTdG9yYWdlRGF0YSAmIHsgc2Vzc2lvbl91cmw6IHN0cmluZyB9O1xuICAgICAgfTtcblxuICAgICAgZXhwb3J0IGNsYXNzIEdDU011bHRpcGFydCBleHRlbmRzIE11bHRpcGFydCB7XG4gICAgICAgIGFzeW5jIF91cGxvYWRDaHVuayhcbiAgICAgICAgICBpbmZvOiBHQ1NVcGxvYWRJbmZvLFxuICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgc3RhcnQ6IG51bWJlcixcbiAgICAgICAgKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgaWYgKCFwYXJ0LnNpemUpIHtcbiAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIjAtbGVuZ3RoIGNodW5rcyBhcmUgbm90IGFsbG93ZWRcIik7XG4gICAgICAgICAgfVxuXG4gICAgICAgICAgY29uc3QgcmVxdWVzdCA9IG5ldyBYTUxIdHRwUmVxdWVzdCgpO1xuXG4gICAgICAgICAgcmVxdWVzdC5vcGVuKFwiUFVUXCIsIGluZm8uc3RvcmFnZV9kYXRhLnNlc3Npb25fdXJsKTtcbiAgICAgICAgICByZXF1ZXN0LnNldFJlcXVlc3RIZWFkZXIoXG4gICAgICAgICAgICBcImNvbnRlbnQtcmFuZ2VcIixcbiAgICAgICAgICAgIGBieXRlcyAke3N0YXJ0fS0ke3N0YXJ0ICsgcGFydC5zaXplIC0gMX0vJHtpbmZvLnN0b3JhZ2VfZGF0YS5zaXplfWAsXG4gICAgICAgICAgKTtcbiAgICAgICAgICByZXF1ZXN0LnNlbmQocGFydCk7XG5cbiAgICAgICAgICBjb25zdCByZXNwOiBhbnkgPSBhd2FpdCBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IGRvbmUocmVxdWVzdCkpO1xuICAgICAgICAgIH0pO1xuICAgICAgICAgIGxldCB1cGxvYWRlZDtcblxuICAgICAgICAgIGlmIChbMjAwLCAyMDFdLmluY2x1ZGVzKHJlc3Auc3RhdHVzKSkge1xuICAgICAgICAgICAgdXBsb2FkZWQgPSBpbmZvLnN0b3JhZ2VfZGF0YS5zaXplO1xuICAgICAgICAgIH0gZWxzZSBpZiAocmVzcC5zdGF0dXMgPT09IDMwOCkge1xuICAgICAgICAgICAgY29uc3QgcmFuZ2UgPSByZXNwLmdldFJlc3BvbnNlSGVhZGVyKFwicmFuZ2VcIik7XG4gICAgICAgICAgICB1cGxvYWRlZCA9IE51bWJlcihyYW5nZS5zcGxpdChcIj1cIilbMV0uc3BsaXQoXCItXCIpWzFdKSArIDE7XG4gICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihhd2FpdCByZXNwLnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgfVxuXG4gICAgICAgICAgaWYgKCFOdW1iZXIuaXNJbnRlZ2VyKHVwbG9hZGVkKSkge1xuICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGBJbnZhbGlkIHVwbG9hZGVkIHNpemUgJHt1cGxvYWRlZH1gKTtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX3VwZGF0ZVwiLFxuICAgICAgICAgICAgICB7XG4gICAgICAgICAgICAgICAgaWQ6IGluZm8uaWQsXG4gICAgICAgICAgICAgICAgdXBsb2FkZWQsXG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuICAgICAgICAgIH0pO1xuICAgICAgICB9XG4gICAgICB9XG4gICAgfVxuICB9XG59XG4iXX0=
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLWdvb2dsZS1jbG91ZC1zdG9yYWdlLXVwbG9hZGVyLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vdHMvZmlsZXMtLWdvb2dsZS1jbG91ZC1zdG9yYWdlLXVwbG9hZGVyLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiJBQUFBLElBQVUsSUFBSSxDQW9FYjtBQXBFRCxXQUFVLElBQUk7SUFDWixJQUFpQixhQUFhLENBa0U3QjtJQWxFRCxXQUFpQixhQUFhO1FBQzVCLElBQWlCLFFBQVEsQ0FnRXhCO1FBaEVELFdBQWlCLFFBQVE7WUFLdkIsTUFBYSxZQUFhLFNBQVEsU0FBQSxTQUFTO2dCQUN6QyxLQUFLLENBQUMsWUFBWSxDQUNoQixJQUFtQixFQUNuQixJQUFVLEVBQ1YsS0FBYTtvQkFFYixJQUFJLENBQUMsSUFBSSxDQUFDLElBQUksRUFBRSxDQUFDO3dCQUNmLE1BQU0sSUFBSSxLQUFLLENBQUMsaUNBQWlDLENBQUMsQ0FBQztvQkFDckQsQ0FBQztvQkFFRCxNQUFNLE9BQU8sR0FBRyxJQUFJLGNBQWMsRUFBRSxDQUFDO29CQUVyQyxPQUFPLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRSxJQUFJLENBQUMsWUFBWSxDQUFDLFdBQVcsQ0FBQyxDQUFDO29CQUNuRCxPQUFPLENBQUMsZ0JBQWdCLENBQ3RCLGVBQWUsRUFDZixTQUFTLEtBQUssSUFBSSxLQUFLLEdBQUcsSUFBSSxDQUFDLElBQUksR0FBRyxDQUFDLElBQUksSUFBSSxDQUFDLFlBQVksQ0FBQyxJQUFJLEVBQUUsQ0FDcEUsQ0FBQztvQkFDRixPQUFPLENBQUMsSUFBSSxDQUFDLElBQUksQ0FBQyxDQUFDO29CQUVuQixNQUFNLElBQUksR0FBUSxNQUFNLElBQUksT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLElBQUksRUFBRSxFQUFFO3dCQUNqRCxPQUFPLENBQUMsZ0JBQWdCLENBQUMsTUFBTSxFQUFFLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FBQyxJQUFJLENBQUMsT0FBTyxDQUFDLENBQUMsQ0FBQztvQkFDN0QsQ0FBQyxDQUFDLENBQUM7b0JBQ0gsSUFBSSxRQUFRLENBQUM7b0JBRWIsSUFBSSxDQUFDLEdBQUcsRUFBRSxHQUFHLENBQUMsQ0FBQyxRQUFRLENBQUMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxFQUFFLENBQUM7d0JBQ3JDLFFBQVEsR0FBRyxJQUFJLENBQUMsWUFBWSxDQUFDLElBQUksQ0FBQztvQkFDcEMsQ0FBQzt5QkFBTSxJQUFJLElBQUksQ0FBQyxNQUFNLEtBQUssR0FBRyxFQUFFLENBQUM7d0JBQy9CLE1BQU0sS0FBSyxHQUFHLElBQUksQ0FBQyxpQkFBaUIsQ0FBQyxPQUFPLENBQUMsQ0FBQzt3QkFDOUMsUUFBUSxHQUFHLE1BQU0sQ0FBQyxLQUFLLENBQUMsS0FBSyxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUMsQ0FBQyxDQUFDLEtBQUssQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDLENBQUMsQ0FBQyxHQUFHLENBQUMsQ0FBQztvQkFDM0QsQ0FBQzt5QkFBTSxDQUFDO3dCQUNOLE1BQU0sSUFBSSxLQUFLLENBQUMsTUFBTSxJQUFJLENBQUMsWUFBWSxDQUFDLENBQUM7b0JBQzNDLENBQUM7b0JBRUQsSUFBSSxDQUFDLE1BQU0sQ0FBQyxTQUFTLENBQUMsUUFBUSxDQUFDLEVBQUUsQ0FBQzt3QkFDaEMsTUFBTSxJQUFJLEtBQUssQ0FBQyx5QkFBeUIsUUFBUSxFQUFFLENBQUMsQ0FBQztvQkFDdkQsQ0FBQztvQkFFRCxPQUFPLElBQUksT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLElBQUksRUFBRSxFQUFFO3dCQUNoQyxJQUFJLENBQUMsT0FBTyxDQUFDLE1BQU0sQ0FBQyxJQUFJLENBQ3RCLE1BQU0sRUFDTixxQkFBcUIsRUFDckI7NEJBQ0UsRUFBRSxFQUFFLElBQUksQ0FBQyxFQUFFOzRCQUNYLFFBQVE7eUJBQ1QsRUFDRCxDQUFDLElBQVMsRUFBRSxFQUFFOzRCQUNaLElBQUksQ0FBQyxJQUFJLENBQUMsTUFBTSxDQUFDLENBQUM7d0JBQ3BCLENBQUMsRUFDRCxDQUFDLElBQVMsRUFBRSxFQUFFOzRCQUNaLElBQUksQ0FDRixPQUFPLElBQUksQ0FBQyxZQUFZLEtBQUssUUFBUTtnQ0FDbkMsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZO2dDQUNuQixDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVksQ0FBQyxLQUFLLENBQzVCLENBQUM7d0JBQ0osQ0FBQyxDQUNGLENBQUM7b0JBQ0osQ0FBQyxDQUFDLENBQUM7Z0JBQ0wsQ0FBQzthQUNGO1lBMURZLHFCQUFZLGVBMER4QixDQUFBO1FBQ0gsQ0FBQyxFQWhFZ0IsUUFBUSxHQUFSLHNCQUFRLEtBQVIsc0JBQVEsUUFnRXhCO0lBQ0gsQ0FBQyxFQWxFZ0IsYUFBYSxHQUFiLGtCQUFhLEtBQWIsa0JBQWEsUUFrRTdCO0FBQ0gsQ0FBQyxFQXBFUyxJQUFJLEtBQUosSUFBSSxRQW9FYiIsInNvdXJjZXNDb250ZW50IjpbIm5hbWVzcGFjZSBja2FuIHtcbiAgZXhwb3J0IG5hbWVzcGFjZSBDS0FORVhUX0ZJTEVTIHtcbiAgICBleHBvcnQgbmFtZXNwYWNlIGFkYXB0ZXJzIHtcbiAgICAgIGV4cG9ydCB0eXBlIEdDU1VwbG9hZEluZm8gPSBVcGxvYWRJbmZvICYge1xuICAgICAgICBzdG9yYWdlX2RhdGE6IFN0b3JhZ2VEYXRhICYgeyBzZXNzaW9uX3VybDogc3RyaW5nIH07XG4gICAgICB9O1xuXG4gICAgICBleHBvcnQgY2xhc3MgR0NTTXVsdGlwYXJ0IGV4dGVuZHMgTXVsdGlwYXJ0IHtcbiAgICAgICAgYXN5bmMgX3VwbG9hZENodW5rKFxuICAgICAgICAgIGluZm86IEdDU1VwbG9hZEluZm8sXG4gICAgICAgICAgcGFydDogQmxvYixcbiAgICAgICAgICBzdGFydDogbnVtYmVyLFxuICAgICAgICApOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICBpZiAoIXBhcnQuc2l6ZSkge1xuICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiMC1sZW5ndGggY2h1bmtzIGFyZSBub3QgYWxsb3dlZFwiKTtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG5cbiAgICAgICAgICByZXF1ZXN0Lm9wZW4oXCJQVVRcIiwgaW5mby5zdG9yYWdlX2RhdGEuc2Vzc2lvbl91cmwpO1xuICAgICAgICAgIHJlcXVlc3Quc2V0UmVxdWVzdEhlYWRlcihcbiAgICAgICAgICAgIFwiY29udGVudC1yYW5nZVwiLFxuICAgICAgICAgICAgYGJ5dGVzICR7c3RhcnR9LSR7c3RhcnQgKyBwYXJ0LnNpemUgLSAxfS8ke2luZm8uc3RvcmFnZV9kYXRhLnNpemV9YCxcbiAgICAgICAgICApO1xuICAgICAgICAgIHJlcXVlc3Quc2VuZChwYXJ0KTtcblxuICAgICAgICAgIGNvbnN0IHJlc3A6IGFueSA9IGF3YWl0IG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PiB7XG4gICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJsb2FkXCIsIChldmVudCkgPT4gZG9uZShyZXF1ZXN0KSk7XG4gICAgICAgICAgfSk7XG4gICAgICAgICAgbGV0IHVwbG9hZGVkO1xuXG4gICAgICAgICAgaWYgKFsyMDAsIDIwMV0uaW5jbHVkZXMocmVzcC5zdGF0dXMpKSB7XG4gICAgICAgICAgICB1cGxvYWRlZCA9IGluZm8uc3RvcmFnZV9kYXRhLnNpemU7XG4gICAgICAgICAgfSBlbHNlIGlmIChyZXNwLnN0YXR1cyA9PT0gMzA4KSB7XG4gICAgICAgICAgICBjb25zdCByYW5nZSA9IHJlc3AuZ2V0UmVzcG9uc2VIZWFkZXIoXCJyYW5nZVwiKTtcbiAgICAgICAgICAgIHVwbG9hZGVkID0gTnVtYmVyKHJhbmdlLnNwbGl0KFwiPVwiKVsxXS5zcGxpdChcIi1cIilbMV0pICsgMTtcbiAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGF3YWl0IHJlc3AucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICBpZiAoIU51bWJlci5pc0ludGVnZXIodXBsb2FkZWQpKSB7XG4gICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoYEludmFsaWQgdXBsb2FkZWQgc2l6ZSAke3VwbG9hZGVkfWApO1xuICAgICAgICAgIH1cblxuICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgXCJmaWxlc191cGxvYWRfdXBkYXRlXCIsXG4gICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICBpZDogaW5mby5pZCxcbiAgICAgICAgICAgICAgICB1cGxvYWRlZCxcbiAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgKGRhdGE6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgIGRvbmUoZGF0YS5yZXN1bHQpO1xuICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgZmFpbChcbiAgICAgICAgICAgICAgICAgIHR5cGVvZiByZXNwLnJlc3BvbnNlSlNPTiA9PT0gXCJzdHJpbmdcIlxuICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgIDogcmVzcC5yZXNwb25zZUpTT04uZXJyb3IsXG4gICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICk7XG4gICAgICAgICAgfSk7XG4gICAgICAgIH1cbiAgICAgIH1cbiAgICB9XG4gIH1cbn1cbiJdfQ==
```

### Comparing `ckanext-files-0.2.3/ckanext/files/assets/scripts/files--shared.js` & `ckanext_files-0.2.4/ckanext/files/assets/scripts/files--shared.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,7 @@
-"use strict";
 var ckan;
 (function(ckan) {
     let CKANEXT_FILES;
     (function(CKANEXT_FILES) {
         CKANEXT_FILES.topics = {
             addFileToQueue: "ckanext:files:queue:file:add",
             restoreFileInQueue: "ckanext:files:queue:file:restore",
@@ -273,8 +272,8 @@
             Multipart.defaultSettings = {
                 chunkSize: 1024 * 1024 * 5
             };
             adapters.Multipart = Multipart;
         })(adapters = CKANEXT_FILES.adapters || (CKANEXT_FILES.adapters = {}));
     })(CKANEXT_FILES = ckan.CKANEXT_FILES || (ckan.CKANEXT_FILES = {}));
 })(ckan || (ckan = {}));
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IjtBQUFBLElBQVUsSUFBSSxDQXlZYjtBQXpZRCxXQUFVLElBQUk7SUFLVixJQUFpQixhQUFhLENBbVk3QjtJQW5ZRCxXQUFpQixhQUFhO1FBTWIsb0JBQU0sR0FBRztZQUNsQixjQUFjLEVBQUUsOEJBQThCO1lBQzlDLGtCQUFrQixFQUFFLGtDQUFrQztZQUN0RCxpQkFBaUIsRUFBRSxtQ0FBbUM7U0FDekQsQ0FBQztRQUVXLDZCQUFlLEdBQUc7WUFDM0IsT0FBTyxFQUFFLFNBQVM7U0FDckIsQ0FBQztRQUVGLFNBQVMsTUFBTSxDQUNYLElBQVUsRUFDVixXQUEwQixZQUFZLENBQUMsVUFBVSxDQUFDO1lBRWxELE9BQU8sUUFBUSxDQUFDLE1BQU0sQ0FBQyxJQUFJLENBQUMsQ0FBQztRQUNqQyxDQUFDO1FBRUQsU0FBUyxZQUFZLENBQUMsT0FBZSxFQUFFLEdBQUcsT0FBWTtZQUNsRCxNQUFNLE9BQU8sR0FBNkMsUUFBUyxDQUMvRCxPQUFPLENBQ1YsQ0FBQztZQUNGLElBQUksQ0FBQyxPQUFPLEVBQUUsQ0FBQztnQkFDWCxNQUFNLElBQUksS0FBSyxDQUFDLFlBQVksT0FBTyxvQkFBb0IsQ0FBQyxDQUFDO1lBQzdELENBQUM7WUFDRCxPQUFPLElBQUksT0FBTyxDQUFDLEdBQUcsT0FBTyxDQUFDLENBQUM7UUFDbkMsQ0FBQztRQUVELElBQUksQ0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLEVBQUUsS0FBSyxFQUFFLEVBQUUsTUFBTSxFQUFFLFlBQVksRUFBRSxFQUFFLENBQUMsQ0FBQztRQUV6RCxJQUFpQixRQUFRLENBK1Z4QjtRQS9WRCxXQUFpQixRQUFRO1lBV3JCLE1BQWEsSUFBSyxTQUFRLFdBQVc7Z0JBTWpDLFlBQVksUUFBUSxHQUFHLEVBQUU7b0JBQ3JCLEtBQUssRUFBRSxDQUFDO29C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LENBQUMsT0FBTyxDQUFDLE1BQU0sQ0FBQyxJQUFJLENBQ3BCLE1BQU0sRUFDTix1QkFBdUIsRUFDdkIsTUFBTSxDQUFDLE1BQU0sQ0FDVCxFQUFFLEVBQ0YsSUFBSSxDQUFDLFFBQVEsQ0FBQyxlQUFlLElBQUksRUFBRSxFQUNuQzt3QkFDSSxFQUFFLEVBQUUsSUFBSSxDQUFDLEVBQUU7cUJBQ2QsQ0FDSixFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsQ0FBQztvQkFDdEIsQ0FBQyxFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUNBLE9BQU8sSUFBSSxDQUFDLFlBQVksS0FBSyxRQUFROzRCQUNqQyxDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVk7NEJBQ25CLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWSxDQUFDLEtBQUssQ0FDaEMsQ0FBQztvQkFDTixDQUFDLENBQ0osQ0FDSixDQUFDO2dCQUNOLENBQUM7O1lBOU1NLHlCQUFlLEdBQUcsRUFBRSxTQUFTLEVBQUUsSUFBSSxHQUFHLElBQUksR0FBRyxDQUFDLEVBQUUsQUFBakMsQ0FBa0M7WUFEL0Msa0JBQVMsWUFnTnJCLENBQUE7UUFDTCxDQUFDLEVBL1ZnQixRQUFRLEdBQVIsc0JBQVEsS0FBUixzQkFBUSxRQStWeEI7SUFDTCxDQUFDLEVBbllnQixhQUFhLEdBQWIsa0JBQWEsS0FBYixrQkFBYSxRQW1ZN0I7QUFDTCxDQUFDLEVBellTLElBQUksS0FBSixJQUFJLFFBeVliIiwic291cmNlc0NvbnRlbnQiOlsibmFtZXNwYWNlIGNrYW4ge1xuICAgIGV4cG9ydCB2YXIgc2FuZGJveDogYW55O1xuICAgIGV4cG9ydCB2YXIgcHVic3ViOiBhbnk7XG4gICAgZXhwb3J0IHZhciBtb2R1bGU6IChuYW1lOiBzdHJpbmcsIGluaXRpYWxpemVyOiAoJDogYW55KSA9PiBhbnkpID0+IGFueTtcblxuICAgIGV4cG9ydCBuYW1lc3BhY2UgQ0tBTkVYVF9GSUxFUyB7XG4gICAgICAgIHR5cGUgVXBsb2FkZXJTZXR0aW5ncyA9IHtcbiAgICAgICAgICAgIHN0b3JhZ2U6IHN0cmluZztcbiAgICAgICAgICAgIFtrZXk6IHN0cmluZ106IGFueTtcbiAgICAgICAgfTtcblxuICAgICAgICBleHBvcnQgY29uc3QgdG9waWNzID0ge1xuICAgICAgICAgICAgYWRkRmlsZVRvUXVldWU6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOmFkZFwiLFxuICAgICAgICAgICAgcmVzdG9yZUZpbGVJblF1ZXVlOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTpyZXN0b3JlXCIsXG4gICAgICAgICAgICBxdWV1ZUl0ZW1VcGxvYWRlZDogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6dXBsb2FkZWRcIixcbiAgICAgICAgfTtcblxuICAgICAgICBleHBvcnQgY29uc3QgZGVmYXVsdFNldHRpbmdzID0ge1xuICAgICAgICAgICAgc3RvcmFnZTogXCJkZWZhdWx0XCIsXG4gICAgICAgIH07XG5cbiAgICAgICAgZnVuY3Rpb24gdXBsb2FkKFxuICAgICAgICAgICAgZmlsZTogRmlsZSxcbiAgICAgICAgICAgIHVwbG9hZGVyOiBhZGFwdGVycy5CYXNlID0gbWFrZVVwbG9hZGVyKFwiU3RhbmRhcmRcIiksXG4gICAgICAgICkge1xuICAgICAgICAgICAgcmV0dXJuIHVwbG9hZGVyLnVwbG9hZChmaWxlKTtcbiAgICAgICAgfVxuXG4gICAgICAgIGZ1bmN0aW9uIG1ha2VVcGxvYWRlcihhZGFwdGVyOiBzdHJpbmcsIC4uLm9wdGlvbnM6IGFueSkge1xuICAgICAgICAgICAgY29uc3QgZmFjdG9yeSA9ICg8eyBba2V5OiBzdHJpbmddOiB0eXBlb2YgYWRhcHRlcnMuQmFzZSB9PmFkYXB0ZXJzKVtcbiAgICAgICAgICAgICAgICBhZGFwdGVyXG4gICAgICAgICAgICBdO1xuICAgICAgICAgICAgaWYgKCFmYWN0b3J5KSB7XG4gICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGBVcGxvYWRlciAke2FkYXB0ZXJ9IGlzIG5vdCByZWdpc3RlcmVkYCk7XG4gICAgICAgICAgICB9XG4gICAgICAgICAgICByZXR1cm4gbmV3IGZhY3RvcnkoLi4ub3B0aW9ucyk7XG4gICAgICAgIH1cblxuICAgICAgICBja2FuLnNhbmRib3guZXh0ZW5kKHsgZmlsZXM6IHsgdXBsb2FkLCBtYWtlVXBsb2FkZXIgfSB9KTtcblxuICAgICAgICBleHBvcnQgbmFtZXNwYWNlIGFkYXB0ZXJzIHtcbiAgICAgICAgICAgIGV4cG9ydCB0eXBlIFN0b3JhZ2VEYXRhID0ge1xuICAgICAgICAgICAgICAgIHVwbG9hZGVkOiBudW1iZXI7XG4gICAgICAgICAgICAgICAgc2l6ZTogbnVtYmVyO1xuICAgICAgICAgICAgfTtcblxuICAgICAgICAgICAgZXhwb3J0IHR5cGUgVXBsb2FkSW5mbyA9IHtcbiAgICAgICAgICAgICAgICBpZDogc3RyaW5nO1xuICAgICAgICAgICAgICAgIHN0b3JhZ2VfZGF0YTogU3RvcmFnZURhdGE7XG4gICAgICAgICAgICB9O1xuXG4gICAgICAgICAgICBleHBvcnQgY2xhc3MgQmFzZSBleHRlbmRzIEV2ZW50VGFyZ2V0IHtcbiAgICAgICAgICAgICAgICBzdGF0aWMgZGVmYXVsdFNldHRpbmdzOiBPYmplY3QgPSB7fTtcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgc2V0dGluZ3M6IFVwbG9hZGVyU2V0dGluZ3M7XG4gICAgICAgICAgICAgICAgcHJvdGVjdGVkIHNhbmRib3g6IGFueTtcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgY3NyZlRva2VuOiBzdHJpbmc7XG5cbiAgICAgICAgICAgICAgICBjb25zdHJ1Y3RvcihzZXR0aW5ncyA9IHt9KSB7XG4gICAgICAgICAgICAgICAgICAgIHN1cGVyKCk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MgPSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAuLi5kZWZhdWx0U2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgICAgICAuLi4odGhpcy5jb25zdHJ1Y3RvciBhcyB0eXBlb2YgQmFzZSkuZGVmYXVsdFNldHRpbmdzLFxuICAgICAgICAgICAgICAgICAgICAgICAgLi4uc2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgIH07XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveCA9IGNrYW4uc2FuZGJveCgpO1xuXG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGNzcmZGaWVsZCA9XG4gICAgICAgICAgICAgICAgICAgICAgICBkb2N1bWVudFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5xdWVyeVNlbGVjdG9yKFwibWV0YVtuYW1lPWNzcmZfZmllbGRfbmFtZV1cIilcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICA/LmdldEF0dHJpYnV0ZShcImNvbnRlbnRcIikgPz8gXCJfY3NyZl90b2tlblwiO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmNzcmZUb2tlbiA9XG4gICAgICAgICAgICAgICAgICAgICAgICBkb2N1bWVudFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5xdWVyeVNlbGVjdG9yKGBtZXRhW25hbWU9JHtjc3JmRmllbGR9XWApXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgPy5nZXRBdHRyaWJ1dGUoXCJjb250ZW50XCIpIHx8IFwiXCI7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiQmFzZS51cGxvYWQgaXMgbm90IGltcGxlbWVudGVkXCIpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIHJlc3VtZShmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIkJhc2UucmVzdW1lIGlzIG5vdCBpbXBsZW1lbnRlZFwiKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBkaXNwYXRjaFN0YXJ0KGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwic3RhcnRcIiwgeyBkZXRhaWw6IHsgZmlsZSB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaENvbW1pdChmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImNvbW1pdFwiLCB7IGRldGFpbDogeyBmaWxlLCBpZCB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaFByb2dyZXNzKGZpbGU6IEZpbGUsIGxvYWRlZDogbnVtYmVyLCB0b3RhbDogbnVtYmVyKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcInByb2dyZXNzXCIsIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBkZXRhaWw6IHsgZmlsZSwgbG9hZGVkLCB0b3RhbCB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoRmluaXNoKGZpbGU6IEZpbGUsIHJlc3VsdDogT2JqZWN0KSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImZpbmlzaFwiLCB7IGRldGFpbDogeyBmaWxlLCByZXN1bHQgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hGYWlsKGZpbGU6IEZpbGUsIHJlYXNvbnM6IHsgW2tleTogc3RyaW5nXTogc3RyaW5nW10gfSkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJmYWlsXCIsIHsgZGV0YWlsOiB7IGZpbGUsIHJlYXNvbnMgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hFcnJvcihmaWxlOiBGaWxlLCBtZXNzYWdlOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZXJyb3JcIiwgeyBkZXRhaWw6IHsgZmlsZSwgbWVzc2FnZSB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgZXhwb3J0IGNsYXNzIFN0YW5kYXJkIGV4dGVuZHMgQmFzZSB7XG4gICAgICAgICAgICAgICAgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVxdWVzdCA9IG5ldyBYTUxIdHRwUmVxdWVzdCgpO1xuICAgICAgICAgICAgICAgICAgICBjb25zdCBwcm9taXNlID0gdGhpcy5fYWRkTGlzdGVuZXJzKHJlcXVlc3QsIGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLl9wcmVwYXJlUmVxdWVzdChyZXF1ZXN0LCBmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBwcm9taXNlO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9hZGRMaXN0ZW5lcnMoXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LFxuICAgICAgICAgICAgICAgICAgICBmaWxlOiBGaWxlLFxuICAgICAgICAgICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnVwbG9hZC5hZGRFdmVudExpc3RlbmVyKFwibG9hZHN0YXJ0XCIsIChldmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnVwbG9hZC5hZGRFdmVudExpc3RlbmVyKFwicHJvZ3Jlc3NcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIGV2ZW50LmxvYWRlZCwgZXZlbnQudG90YWwpLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBKU09OLnBhcnNlKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZiAocmVzdWx0LnN1Y2Nlc3MpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaENvbW1pdChmaWxlLCByZXN1bHQucmVzdWx0LmlkKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZpbmlzaChmaWxlLCByZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShyZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmFpbChmaWxlLCByZXN1bHQuZXJyb3IpO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwocmVzdWx0LmVycm9yKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwiZXJyb3JcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuICAgICAgICAgICAgICAgICAgICB9KTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfcHJlcGFyZVJlcXVlc3QocmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsIGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5vcGVuKFxuICAgICAgICAgICAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LnVybChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIi9hcGkvYWN0aW9uL2ZpbGVzX2ZpbGVfY3JlYXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLmNzcmZUb2tlbikge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZXRSZXF1ZXN0SGVhZGVyKFwiWC1DU1JGVG9rZW5cIiwgdGhpcy5jc3JmVG9rZW4pO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3NlbmRSZXF1ZXN0KHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LCBmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGRhdGEgPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICAgICAgICAgICAgZGF0YS5hcHBlbmQoXCJ1cGxvYWRcIiwgZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgZGF0YS5hcHBlbmQoXCJzdG9yYWdlXCIsIHRoaXMuc2V0dGluZ3Muc3RvcmFnZSk7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2VuZChkYXRhKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGV4cG9ydCBjbGFzcyBNdWx0aXBhcnQgZXh0ZW5kcyBCYXNlIHtcbiAgICAgICAgICAgICAgICBzdGF0aWMgZGVmYXVsdFNldHRpbmdzID0geyBjaHVua1NpemU6IDEwMjQgKiAxMDI0ICogNSB9O1xuXG4gICAgICAgICAgICAgICAgcHJpdmF0ZSBfYWN0aXZlID0gbmV3IFNldDxGaWxlPigpO1xuXG4gICAgICAgICAgICAgICAgY29uc3RydWN0b3Ioc2V0dGluZ3M6IE9iamVjdCkge1xuICAgICAgICAgICAgICAgICAgICBzdXBlcihzZXR0aW5ncyk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuX2FjdGl2ZS5oYXMoZmlsZSkpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUud2FybihcIkZpbGUgdXBsb2FkIGluIHByb2dyZXNzXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5hZGQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgbGV0IGluZm87XG5cbiAgICAgICAgICAgICAgICAgICAgdHJ5IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9pbml0aWFsaXplVXBsb2FkKGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB9IGNhdGNoIChlcnIpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICh0eXBlb2YgZXJyID09PSBcInN0cmluZ1wiKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIGVycik7XG4gICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGYWlsKGZpbGUsIGVyciBhcyBhbnkpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaENvbW1pdChmaWxlLCBpbmZvLmlkKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGFzeW5jIHJlc3VtZShmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBjb25zb2xlLndhcm4oXCJGaWxlIHVwbG9hZCBpbiBwcm9ncmVzc1wiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9hY3RpdmUuYWRkKGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIGxldCBpbmZvID0gYXdhaXQgdGhpcy5fc2hvd1VwbG9hZChpZCk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9kb1VwbG9hZChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBwYXVzZShmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5kZWxldGUoZmlsZSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgX2RvVXBsb2FkKGZpbGU6IEZpbGUsIGluZm86IFVwbG9hZEluZm8pIHtcbiAgICAgICAgICAgICAgICAgICAgbGV0IHN0YXJ0ID0gaW5mby5zdG9yYWdlX2RhdGEudXBsb2FkZWQgfHwgMDtcblxuICAgICAgICAgICAgICAgICAgICB3aGlsZSAoc3RhcnQgPCBmaWxlLnNpemUpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICghdGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUuaW5mbyhcIkZpbGUgdXBsb2FkIGlzIHBhdXNlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl91cGxvYWRDaHVuayhcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpbmZvLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZpbGUuc2xpY2Uoc3RhcnQsIHN0YXJ0ICsgdGhpcy5zZXR0aW5ncy5jaHVua1NpemUpLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHN0YXJ0LFxuICAgICAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgdXBsb2FkZWQgPSBpbmZvLnN0b3JhZ2VfZGF0YS51cGxvYWRlZDtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICh1cGxvYWRlZCA8PSBzdGFydCkge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIlVwbG9hZGVkIHNpemUgaXMgcmVkdWNlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIHVwbG9hZGVkLCBmaWxlLnNpemUpO1xuICAgICAgICAgICAgICAgICAgICAgICAgc3RhcnQgPSB1cGxvYWRlZDtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hQcm9ncmVzcyhmaWxlLCBmaWxlLnNpemUsIGZpbGUuc2l6ZSk7XG4gICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9jb21wbGV0ZVVwbG9hZChpbmZvKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZpbmlzaChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfaW5pdGlhbGl6ZVVwbG9hZChmaWxlOiBGaWxlKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcImZpbGVzX3VwbG9hZF9pbml0aWFsaXplXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuaW5pdGlhbGl6ZVBheWxvYWQgfHwge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHN0b3JhZ2U6IHRoaXMuc2V0dGluZ3Muc3RvcmFnZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIG5hbWU6IGZpbGUubmFtZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHNpemU6IGZpbGUuc2l6ZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfc2hvd1VwbG9hZChpZDogc3RyaW5nKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIkdFVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX3Nob3dcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBgP2lkPSR7aWR9YCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAoZGF0YTogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUoZGF0YS5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdHlwZW9mIHJlc3AucmVzcG9uc2VKU09OID09PSBcInN0cmluZ1wiXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIDogcmVzcC5yZXNwb25zZUpTT04uZXJyb3IsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICAgICAgICBpbmZvOiBVcGxvYWRJbmZvLFxuICAgICAgICAgICAgICAgICAgICBwYXJ0OiBCbG9iLFxuICAgICAgICAgICAgICAgICAgICBzdGFydDogbnVtYmVyLFxuICAgICAgICAgICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICBpZiAoIXBhcnQuc2l6ZSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiMC1sZW5ndGggY2h1bmtzIGFyZSBub3QgYWxsb3dlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG5cbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gbmV3IFByb21pc2U8VXBsb2FkSW5mbz4oKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gSlNPTi5wYXJzZShyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHJlc3VsdC5zdWNjZXNzKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUocmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJlcnJvclwiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXF1ZXN0LnJlc3BvbnNlVGV4dCksXG4gICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiL2FwaS9hY3Rpb24vZmlsZXNfdXBsb2FkX3VwZGF0ZVwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5jc3JmVG9rZW4pIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2V0UmVxdWVzdEhlYWRlcihcIlgtQ1NSRlRva2VuXCIsIHRoaXMuY3NyZlRva2VuKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3NlbmRSZXF1ZXN0KHJlcXVlc3QsIHBhcnQsIHN0YXJ0LCBpbmZvLmlkKTtcblxuICAgICAgICAgICAgICAgICAgICByZXR1cm4gcmVzdWx0O1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zZW5kUmVxdWVzdChcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsXG4gICAgICAgICAgICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgICAgICAgICAgIHBvc2l0aW9uOiBudW1iZXIsXG4gICAgICAgICAgICAgICAgICAgIGlkOiBzdHJpbmcsXG4gICAgICAgICAgICAgICAgKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGZvcm0gPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJ1cGxvYWRcIiwgcGFydCk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwicG9zaXRpb25cIiwgU3RyaW5nKHBvc2l0aW9uKSk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwiaWRcIiwgaWQpO1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNlbmQoZm9ybSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX2NvbXBsZXRlVXBsb2FkKGluZm86IFVwbG9hZEluZm8pOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2NvbXBsZXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuY29tcGxldGVQYXlsb2FkIHx8IHt9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZDogaW5mby5pZCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG4gICAgICAgIH1cbiAgICB9XG59XG4iXX0=
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IkFBQUEsSUFBVSxJQUFJLENBeVliO0FBellELFdBQVUsSUFBSTtJQUtWLElBQWlCLGFBQWEsQ0FtWTdCO0lBbllELFdBQWlCLGFBQWE7UUFNYixvQkFBTSxHQUFHO1lBQ2xCLGNBQWMsRUFBRSw4QkFBOEI7WUFDOUMsa0JBQWtCLEVBQUUsa0NBQWtDO1lBQ3RELGlCQUFpQixFQUFFLG1DQUFtQztTQUN6RCxDQUFDO1FBRVcsNkJBQWUsR0FBRztZQUMzQixPQUFPLEVBQUUsU0FBUztTQUNyQixDQUFDO1FBRUYsU0FBUyxNQUFNLENBQ1gsSUFBVSxFQUNWLFdBQTBCLFlBQVksQ0FBQyxVQUFVLENBQUM7WUFFbEQsT0FBTyxRQUFRLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQ2pDLENBQUM7UUFFRCxTQUFTLFlBQVksQ0FBQyxPQUFlLEVBQUUsR0FBRyxPQUFZO1lBQ2xELE1BQU0sT0FBTyxHQUE2QyxRQUFTLENBQy9ELE9BQU8sQ0FDVixDQUFDO1lBQ0YsSUFBSSxDQUFDLE9BQU8sRUFBRSxDQUFDO2dCQUNYLE1BQU0sSUFBSSxLQUFLLENBQUMsWUFBWSxPQUFPLG9CQUFvQixDQUFDLENBQUM7WUFDN0QsQ0FBQztZQUNELE9BQU8sSUFBSSxPQUFPLENBQUMsR0FBRyxPQUFPLENBQUMsQ0FBQztRQUNuQyxDQUFDO1FBRUQsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsRUFBRSxLQUFLLEVBQUUsRUFBRSxNQUFNLEVBQUUsWUFBWSxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRXpELElBQWlCLFFBQVEsQ0ErVnhCO1FBL1ZELFdBQWlCLFFBQVE7WUFXckIsTUFBYSxJQUFLLFNBQVEsV0FBVztnQkFNakMsWUFBWSxRQUFRLEdBQUcsRUFBRTtvQkFDckIsS0FBSyxFQUFFLENBQUM7b0JB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Q0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLElBQUksQ0FDcEIsTUFBTSxFQUNOLHVCQUF1QixFQUN2QixNQUFNLENBQUMsTUFBTSxDQUNULEVBQUUsRUFDRixJQUFJLENBQUMsUUFBUSxDQUFDLGVBQWUsSUFBSSxFQUFFLEVBQ25DO3dCQUNJLEVBQUUsRUFBRSxJQUFJLENBQUMsRUFBRTtxQkFDZCxDQUNKLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQUMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxDQUFDO29CQUN0QixDQUFDLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQ0EsT0FBTyxJQUFJLENBQUMsWUFBWSxLQUFLLFFBQVE7NEJBQ2pDLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWTs0QkFDbkIsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUNoQyxDQUFDO29CQUNOLENBQUMsQ0FDSixDQUNKLENBQUM7Z0JBQ04sQ0FBQzs7WUE5TU0seUJBQWUsR0FBRyxFQUFFLFNBQVMsRUFBRSxJQUFJLEdBQUcsSUFBSSxHQUFHLENBQUMsRUFBRSxBQUFqQyxDQUFrQztZQUQvQyxrQkFBUyxZQWdOckIsQ0FBQTtRQUNMLENBQUMsRUEvVmdCLFFBQVEsR0FBUixzQkFBUSxLQUFSLHNCQUFRLFFBK1Z4QjtJQUNMLENBQUMsRUFuWWdCLGFBQWEsR0FBYixrQkFBYSxLQUFiLGtCQUFhLFFBbVk3QjtBQUNMLENBQUMsRUF6WVMsSUFBSSxLQUFKLElBQUksUUF5WWIiLCJzb3VyY2VzQ29udGVudCI6WyJuYW1lc3BhY2UgY2thbiB7XG4gICAgZXhwb3J0IHZhciBzYW5kYm94OiBhbnk7XG4gICAgZXhwb3J0IHZhciBwdWJzdWI6IGFueTtcbiAgICBleHBvcnQgdmFyIG1vZHVsZTogKG5hbWU6IHN0cmluZywgaW5pdGlhbGl6ZXI6ICgkOiBhbnkpID0+IGFueSkgPT4gYW55O1xuXG4gICAgZXhwb3J0IG5hbWVzcGFjZSBDS0FORVhUX0ZJTEVTIHtcbiAgICAgICAgdHlwZSBVcGxvYWRlclNldHRpbmdzID0ge1xuICAgICAgICAgICAgc3RvcmFnZTogc3RyaW5nO1xuICAgICAgICAgICAgW2tleTogc3RyaW5nXTogYW55O1xuICAgICAgICB9O1xuXG4gICAgICAgIGV4cG9ydCBjb25zdCB0b3BpY3MgPSB7XG4gICAgICAgICAgICBhZGRGaWxlVG9RdWV1ZTogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6YWRkXCIsXG4gICAgICAgICAgICByZXN0b3JlRmlsZUluUXVldWU6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOnJlc3RvcmVcIixcbiAgICAgICAgICAgIHF1ZXVlSXRlbVVwbG9hZGVkOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTp1cGxvYWRlZFwiLFxuICAgICAgICB9O1xuXG4gICAgICAgIGV4cG9ydCBjb25zdCBkZWZhdWx0U2V0dGluZ3MgPSB7XG4gICAgICAgICAgICBzdG9yYWdlOiBcImRlZmF1bHRcIixcbiAgICAgICAgfTtcblxuICAgICAgICBmdW5jdGlvbiB1cGxvYWQoXG4gICAgICAgICAgICBmaWxlOiBGaWxlLFxuICAgICAgICAgICAgdXBsb2FkZXI6IGFkYXB0ZXJzLkJhc2UgPSBtYWtlVXBsb2FkZXIoXCJTdGFuZGFyZFwiKSxcbiAgICAgICAgKSB7XG4gICAgICAgICAgICByZXR1cm4gdXBsb2FkZXIudXBsb2FkKGZpbGUpO1xuICAgICAgICB9XG5cbiAgICAgICAgZnVuY3Rpb24gbWFrZVVwbG9hZGVyKGFkYXB0ZXI6IHN0cmluZywgLi4ub3B0aW9uczogYW55KSB7XG4gICAgICAgICAgICBjb25zdCBmYWN0b3J5ID0gKDx7IFtrZXk6IHN0cmluZ106IHR5cGVvZiBhZGFwdGVycy5CYXNlIH0+YWRhcHRlcnMpW1xuICAgICAgICAgICAgICAgIGFkYXB0ZXJcbiAgICAgICAgICAgIF07XG4gICAgICAgICAgICBpZiAoIWZhY3RvcnkpIHtcbiAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoYFVwbG9hZGVyICR7YWRhcHRlcn0gaXMgbm90IHJlZ2lzdGVyZWRgKTtcbiAgICAgICAgICAgIH1cbiAgICAgICAgICAgIHJldHVybiBuZXcgZmFjdG9yeSguLi5vcHRpb25zKTtcbiAgICAgICAgfVxuXG4gICAgICAgIGNrYW4uc2FuZGJveC5leHRlbmQoeyBmaWxlczogeyB1cGxvYWQsIG1ha2VVcGxvYWRlciB9IH0pO1xuXG4gICAgICAgIGV4cG9ydCBuYW1lc3BhY2UgYWRhcHRlcnMge1xuICAgICAgICAgICAgZXhwb3J0IHR5cGUgU3RvcmFnZURhdGEgPSB7XG4gICAgICAgICAgICAgICAgdXBsb2FkZWQ6IG51bWJlcjtcbiAgICAgICAgICAgICAgICBzaXplOiBudW1iZXI7XG4gICAgICAgICAgICB9O1xuXG4gICAgICAgICAgICBleHBvcnQgdHlwZSBVcGxvYWRJbmZvID0ge1xuICAgICAgICAgICAgICAgIGlkOiBzdHJpbmc7XG4gICAgICAgICAgICAgICAgc3RvcmFnZV9kYXRhOiBTdG9yYWdlRGF0YTtcbiAgICAgICAgICAgIH07XG5cbiAgICAgICAgICAgIGV4cG9ydCBjbGFzcyBCYXNlIGV4dGVuZHMgRXZlbnRUYXJnZXQge1xuICAgICAgICAgICAgICAgIHN0YXRpYyBkZWZhdWx0U2V0dGluZ3M6IE9iamVjdCA9IHt9O1xuICAgICAgICAgICAgICAgIHByb3RlY3RlZCBzZXR0aW5nczogVXBsb2FkZXJTZXR0aW5ncztcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgc2FuZGJveDogYW55O1xuICAgICAgICAgICAgICAgIHByb3RlY3RlZCBjc3JmVG9rZW46IHN0cmluZztcblxuICAgICAgICAgICAgICAgIGNvbnN0cnVjdG9yKHNldHRpbmdzID0ge30pIHtcbiAgICAgICAgICAgICAgICAgICAgc3VwZXIoKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncyA9IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIC4uLmRlZmF1bHRTZXR0aW5ncyxcbiAgICAgICAgICAgICAgICAgICAgICAgIC4uLih0aGlzLmNvbnN0cnVjdG9yIGFzIHR5cGVvZiBCYXNlKS5kZWZhdWx0U2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgICAgICAuLi5zZXR0aW5ncyxcbiAgICAgICAgICAgICAgICAgICAgfTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94ID0gY2thbi5zYW5kYm94KCk7XG5cbiAgICAgICAgICAgICAgICAgICAgY29uc3QgY3NyZkZpZWxkID1cbiAgICAgICAgICAgICAgICAgICAgICAgIGRvY3VtZW50XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLnF1ZXJ5U2VsZWN0b3IoXCJtZXRhW25hbWU9Y3NyZl9maWVsZF9uYW1lXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgICAgID8uZ2V0QXR0cmlidXRlKFwiY29udGVudFwiKSA/PyBcIl9jc3JmX3Rva2VuXCI7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuY3NyZlRva2VuID1cbiAgICAgICAgICAgICAgICAgICAgICAgIGRvY3VtZW50XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLnF1ZXJ5U2VsZWN0b3IoYG1ldGFbbmFtZT0ke2NzcmZGaWVsZH1dYClcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICA/LmdldEF0dHJpYnV0ZShcImNvbnRlbnRcIikgfHwgXCJcIjtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCJCYXNlLnVwbG9hZCBpcyBub3QgaW1wbGVtZW50ZWRcIik7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgcmVzdW1lKGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiQmFzZS5yZXN1bWUgaXMgbm90IGltcGxlbWVudGVkXCIpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGRpc3BhdGNoU3RhcnQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJzdGFydFwiLCB7IGRldGFpbDogeyBmaWxlIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoQ29tbWl0KGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiY29tbWl0XCIsIHsgZGV0YWlsOiB7IGZpbGUsIGlkIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoUHJvZ3Jlc3MoZmlsZTogRmlsZSwgbG9hZGVkOiBudW1iZXIsIHRvdGFsOiBudW1iZXIpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwicHJvZ3Jlc3NcIiwge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRldGFpbDogeyBmaWxlLCBsb2FkZWQsIHRvdGFsIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hGaW5pc2goZmlsZTogRmlsZSwgcmVzdWx0OiBPYmplY3QpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZmluaXNoXCIsIHsgZGV0YWlsOiB7IGZpbGUsIHJlc3VsdCB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaEZhaWwoZmlsZTogRmlsZSwgcmVhc29uczogeyBba2V5OiBzdHJpbmddOiBzdHJpbmdbXSB9KSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImZhaWxcIiwgeyBkZXRhaWw6IHsgZmlsZSwgcmVhc29ucyB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaEVycm9yKGZpbGU6IEZpbGUsIG1lc3NhZ2U6IHN0cmluZykge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJlcnJvclwiLCB7IGRldGFpbDogeyBmaWxlLCBtZXNzYWdlIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICBleHBvcnQgY2xhc3MgU3RhbmRhcmQgZXh0ZW5kcyBCYXNlIHtcbiAgICAgICAgICAgICAgICB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IHByb21pc2UgPSB0aGlzLl9hZGRMaXN0ZW5lcnMocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3ByZXBhcmVSZXF1ZXN0KHJlcXVlc3QsIGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLl9zZW5kUmVxdWVzdChyZXF1ZXN0LCBmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIHByb21pc2U7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX2FkZExpc3RlbmVycyhcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsXG4gICAgICAgICAgICAgICAgICAgIGZpbGU6IEZpbGUsXG4gICAgICAgICAgICAgICAgKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3QudXBsb2FkLmFkZEV2ZW50TGlzdGVuZXIoXCJsb2Fkc3RhcnRcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3QudXBsb2FkLmFkZEV2ZW50TGlzdGVuZXIoXCJwcm9ncmVzc1wiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgZXZlbnQubG9hZGVkLCBldmVudC50b3RhbCksXG4gICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJsb2FkXCIsIChldmVudCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGNvbnN0IHJlc3VsdCA9IEpTT04ucGFyc2UocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGlmIChyZXN1bHQuc3VjY2Vzcykge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIHJlc3VsdC5yZXN1bHQuaWQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmluaXNoKGZpbGUsIHJlc3VsdC5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKHJlc3VsdC5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGYWlsKGZpbGUsIHJlc3VsdC5lcnJvcik7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJlcnJvclwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXJyb3IoZmlsZSwgcmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfSk7XG4gICAgICAgICAgICAgICAgICAgIH0pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9wcmVwYXJlUmVxdWVzdChyZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCwgZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiL2FwaS9hY3Rpb24vZmlsZXNfZmlsZV9jcmVhdGVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuY3NyZlRva2VuKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNldFJlcXVlc3RIZWFkZXIoXCJYLUNTUkZUb2tlblwiLCB0aGlzLmNzcmZUb2tlbik7XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfc2VuZFJlcXVlc3QocmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsIGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgZGF0YSA9IG5ldyBGb3JtRGF0YSgpO1xuICAgICAgICAgICAgICAgICAgICBkYXRhLmFwcGVuZChcInVwbG9hZFwiLCBmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICBkYXRhLmFwcGVuZChcInN0b3JhZ2VcIiwgdGhpcy5zZXR0aW5ncy5zdG9yYWdlKTtcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZW5kKGRhdGEpO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgZXhwb3J0IGNsYXNzIE11bHRpcGFydCBleHRlbmRzIEJhc2Uge1xuICAgICAgICAgICAgICAgIHN0YXRpYyBkZWZhdWx0U2V0dGluZ3MgPSB7IGNodW5rU2l6ZTogMTAyNCAqIDEwMjQgKiA1IH07XG5cbiAgICAgICAgICAgICAgICBwcml2YXRlIF9hY3RpdmUgPSBuZXcgU2V0PEZpbGU+KCk7XG5cbiAgICAgICAgICAgICAgICBjb25zdHJ1Y3RvcihzZXR0aW5nczogT2JqZWN0KSB7XG4gICAgICAgICAgICAgICAgICAgIHN1cGVyKHNldHRpbmdzKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBhc3luYyB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgY29uc29sZS53YXJuKFwiRmlsZSB1cGxvYWQgaW4gcHJvZ3Jlc3NcIik7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fYWN0aXZlLmFkZChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICBsZXQgaW5mbztcblxuICAgICAgICAgICAgICAgICAgICB0cnkge1xuICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX2luaXRpYWxpemVVcGxvYWQoZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIH0gY2F0Y2ggKGVycikge1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHR5cGVvZiBlcnIgPT09IFwic3RyaW5nXCIpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXJyb3IoZmlsZSwgZXJyKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZhaWwoZmlsZSwgZXJyIGFzIGFueSk7XG4gICAgICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIGluZm8uaWQpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoU3RhcnQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fZG9VcGxvYWQoZmlsZSwgaW5mbyk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgcmVzdW1lKGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuX2FjdGl2ZS5oYXMoZmlsZSkpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUud2FybihcIkZpbGUgdXBsb2FkIGluIHByb2dyZXNzXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5hZGQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgbGV0IGluZm8gPSBhd2FpdCB0aGlzLl9zaG93VXBsb2FkKGlkKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIHBhdXNlKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fYWN0aXZlLmRlbGV0ZShmaWxlKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBhc3luYyBfZG9VcGxvYWQoZmlsZTogRmlsZSwgaW5mbzogVXBsb2FkSW5mbykge1xuICAgICAgICAgICAgICAgICAgICBsZXQgc3RhcnQgPSBpbmZvLnN0b3JhZ2VfZGF0YS51cGxvYWRlZCB8fCAwO1xuXG4gICAgICAgICAgICAgICAgICAgIHdoaWxlIChzdGFydCA8IGZpbGUuc2l6ZSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKCF0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc29sZS5pbmZvKFwiRmlsZSB1cGxvYWQgaXMgcGF1c2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGluZm8sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmlsZS5zbGljZShzdGFydCwgc3RhcnQgKyB0aGlzLnNldHRpbmdzLmNodW5rU2l6ZSksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgc3RhcnQsXG4gICAgICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICBjb25zdCB1cGxvYWRlZCA9IGluZm8uc3RvcmFnZV9kYXRhLnVwbG9hZGVkO1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHVwbG9hZGVkIDw9IHN0YXJ0KSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiVXBsb2FkZWQgc2l6ZSBpcyByZWR1Y2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgdXBsb2FkZWQsIGZpbGUuc2l6ZSk7XG4gICAgICAgICAgICAgICAgICAgICAgICBzdGFydCA9IHVwbG9hZGVkO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIGZpbGUuc2l6ZSwgZmlsZS5zaXplKTtcbiAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX2NvbXBsZXRlVXBsb2FkKGluZm8pO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmluaXNoKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9pbml0aWFsaXplVXBsb2FkKGZpbGU6IEZpbGUpOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2luaXRpYWxpemVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBPYmplY3QuYXNzaWduKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncy5pbml0aWFsaXplUGF5bG9hZCB8fCB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgc3RvcmFnZTogdGhpcy5zZXR0aW5ncy5zdG9yYWdlLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgbmFtZTogZmlsZS5uYW1lLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgc2l6ZTogZmlsZS5zaXplLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKGRhdGE6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChyZXNwOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHR5cGVvZiByZXNwLnJlc3BvbnNlSlNPTiA9PT0gXCJzdHJpbmdcIlxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgID8gcmVzcC5yZXNwb25zZVRleHRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zaG93VXBsb2FkKGlkOiBzdHJpbmcpOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiR0VUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJmaWxlc191cGxvYWRfc2hvd1wiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGA/aWQ9JHtpZH1gLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfdXBsb2FkQ2h1bmsoXG4gICAgICAgICAgICAgICAgICAgIGluZm86IFVwbG9hZEluZm8sXG4gICAgICAgICAgICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgICAgICAgICAgIHN0YXJ0OiBudW1iZXIsXG4gICAgICAgICAgICAgICAgKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIGlmICghcGFydC5zaXplKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCIwLWxlbmd0aCBjaHVua3MgYXJlIG5vdCBhbGxvd2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IHJlcXVlc3QgPSBuZXcgWE1MSHR0cFJlcXVlc3QoKTtcblxuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBuZXcgUHJvbWlzZTxVcGxvYWRJbmZvPigoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBKU09OLnBhcnNlKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZiAocmVzdWx0LnN1Y2Nlc3MpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShyZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlc3VsdC5lcnJvcik7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICAgICAgfSk7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImVycm9yXCIsIChldmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlcXVlc3QucmVzcG9uc2VUZXh0KSxcbiAgICAgICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Qub3BlbihcbiAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC51cmwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCIvYXBpL2FjdGlvbi9maWxlc191cGxvYWRfdXBkYXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLmNzcmZUb2tlbikge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZXRSZXF1ZXN0SGVhZGVyKFwiWC1DU1JGVG9rZW5cIiwgdGhpcy5jc3JmVG9rZW4pO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgcGFydCwgc3RhcnQsIGluZm8uaWQpO1xuXG4gICAgICAgICAgICAgICAgICAgIHJldHVybiByZXN1bHQ7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3NlbmRSZXF1ZXN0KFxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCxcbiAgICAgICAgICAgICAgICAgICAgcGFydDogQmxvYixcbiAgICAgICAgICAgICAgICAgICAgcG9zaXRpb246IG51bWJlcixcbiAgICAgICAgICAgICAgICAgICAgaWQ6IHN0cmluZyxcbiAgICAgICAgICAgICAgICApIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgZm9ybSA9IG5ldyBGb3JtRGF0YSgpO1xuICAgICAgICAgICAgICAgICAgICBmb3JtLmFwcGVuZChcInVwbG9hZFwiLCBwYXJ0KTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJwb3NpdGlvblwiLCBTdHJpbmcocG9zaXRpb24pKTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJpZFwiLCBpZCk7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2VuZChmb3JtKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfY29tcGxldGVVcGxvYWQoaW5mbzogVXBsb2FkSW5mbyk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LmNhbGwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJmaWxlc191cGxvYWRfY29tcGxldGVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBPYmplY3QuYXNzaWduKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncy5jb21wbGV0ZVBheWxvYWQgfHwge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGlkOiBpbmZvLmlkLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKGRhdGE6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChyZXNwOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHR5cGVvZiByZXNwLnJlc3BvbnNlSlNPTiA9PT0gXCJzdHJpbmdcIlxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgID8gcmVzcC5yZXNwb25zZVRleHRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cbiAgICAgICAgfVxuICAgIH1cbn1cbiJdfQ==
```

### Comparing `ckanext-files-0.2.3/ckanext/files/cli.py` & `ckanext_files-0.2.4/ckanext/files/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/command.py` & `ckanext_files-0.2.4/ckanext/files/command.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/config.py` & `ckanext_files-0.2.4/ckanext/files/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/exceptions.py` & `ckanext_files-0.2.4/ckanext/files/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,15 +93,30 @@
 
     def __init__(self, storage, filename):
         # type: (str, str) -> None
         self.storage = storage
         self.filename = filename
 
     def __str__(self):
-        return "File {} does not exist inside {} storage".format(
+        return "File {} does not exist inside storage {}".format(
+            self.filename,
+            self.storage,
+        )
+
+
+class ExistingFileError(StorageError):
+    """File already exists."""
+
+    def __init__(self, storage, filename):
+        # type: (str, str) -> None
+        self.storage = storage
+        self.filename = filename
+
+    def __str__(self):
+        return "File {} already exists inside storage {}".format(
             self.filename,
             self.storage,
         )
 
 
 class LargeUploadError(UploadError):
     """Storage cannot be initialized due to missing option."""
```

### Comparing `ckanext-files-0.2.3/ckanext/files/helpers.py` & `ckanext_files-0.2.4/ckanext/files/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/interfaces.py` & `ckanext_files-0.2.4/ckanext/files/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/logic/action.py` & `ckanext_files-0.2.4/ckanext/files/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/logic/auth.py` & `ckanext_files-0.2.4/ckanext/files/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/logic/schema.py` & `ckanext_files-0.2.4/ckanext/files/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/alembic.ini` & `ckanext_files-0.2.4/ckanext/files/migration/files/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/env.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py` & `ckanext_files-0.2.4/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/model/file.py` & `ckanext_files-0.2.4/ckanext/files/model/file.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/model/owner.py` & `ckanext_files-0.2.4/ckanext/files/model/owner.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/plugin.py` & `ckanext_files-0.2.4/ckanext/files/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/storage/fs.py` & `ckanext_files-0.2.4/ckanext/files/storage/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     capabilities = utils.combine_capabilities(
         Capability.CREATE,
         Capability.MULTIPART_UPLOAD,
     )
 
     def upload(self, name, upload, extras):
         # type: (str, types.Upload, dict[str, types.Any]) -> FsStorageData
-        filename = self.compute_name(name, extras, upload)
+        filename = self.storage.compute_name(name, extras, upload)
         filepath = os.path.join(self.storage.settings["path"], filename)
 
         reader = HashingReader(upload.stream)
         with open(filepath, "wb") as dest:
             for chunk in reader:
                 dest.write(chunk)
 
@@ -135,20 +135,16 @@
                         ),
                     ],
                 },
             )
 
         with open(filepath, "rb") as src:
             reader = HashingReader(src)
-            it = iter(reader)
-            content_type = magic.from_buffer(next(it, b""), True)
-
-            # exhaust reader to get the checksum
-            for _chunk in it:
-                pass
+            content_type = magic.from_buffer(next(reader, b""), True)
+            reader.exhaust()
 
         return {
             "filename": upload_data["filename"],
             "content_type": content_type,
             "size": size,
             "hash": reader.get_hash(),
         }
```

### Comparing `ckanext-files-0.2.3/ckanext/files/storage/google_cloud.py` & `ckanext_files-0.2.4/ckanext/files/storage/google_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     capabilities = utils.combine_capabilities(
         Capability.CREATE,
         Capability.MULTIPART_UPLOAD,
     )
 
     def upload(self, name, upload, extras):
         # type: (str, types.Upload, dict[str, types.Any]) -> GCStorageData
-        filename = self.compute_name(name, extras, upload)
+        filename = self.storage.compute_name(name, extras, upload)
         filepath = os.path.join(self.storage.settings["path"], filename)
 
         client = self.storage.client
         blob = client.bucket(self.storage.settings["bucket"]).blob(filepath)
 
         blob.upload_from_file(upload.stream)
         filehash = decode(blob.md5_hash)
@@ -67,15 +67,15 @@
             "__extras": [tk.get_validator("ignore")],
         }
         data, errors = tk.navl_validate(extras, schema)
 
         if errors:
             raise tk.ValidationError(errors)
 
-        filename = self.compute_name(name, extras)
+        filename = self.storage.compute_name(name, extras)
         filepath = os.path.join(self.storage.settings["path"], filename)
 
         client = self.storage.client
         blob = client.bucket(self.storage.settings["bucket"]).blob(filepath)
 
         max_size = self.storage.max_size
         if max_size and data["size"] > max_size:
```

### Comparing `ckanext-files-0.2.3/ckanext/files/storage/redis.py` & `ckanext_files-0.2.4/ckanext/files/storage/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,54 +32,31 @@
         Capability.COPY,
         Capability.MOVE,
     )
 
     def upload(self, name, upload, extras):
         # type: (str, types.Upload, dict[str, types.Any]) -> RedisStorageData
 
-        filename = self.compute_name(name, extras, upload)
+        filename = self.storage.compute_name(name, extras, upload)
         key = self.storage.settings["prefix"] + filename
 
         self.storage.redis.delete(key)
 
         reader = HashingReader(upload.stream)
+        self.storage.redis.set(key, b"")
         for chunk in reader:
             self.storage.redis.append(key, chunk)
 
         return {
             "filename": filename,
             "content_type": upload.content_type,
             "size": reader.position,
             "hash": reader.get_hash(),
         }
 
-    def copy(self, data, name, extras):
-        # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
-        filename = self.compute_name(name, extras)
-
-        src = self.storage.settings["prefix"] + data["filename"]
-        dest = self.storage.settings["prefix"] + filename
-
-        try:
-            self.storage.redis.copy(src, dest)
-        except AttributeError:
-            self.storage.redis.restore(dest, 0, self.storage.redis.dump(src))
-
-        return RedisStorageData(data, filename=filename)
-
-    def move(self, data, name, extras):
-        # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
-        filename = self.compute_name(name, extras)
-
-        src = self.storage.settings["prefix"] + data["filename"]
-        dest = self.storage.settings["prefix"] + filename
-
-        self.storage.redis.rename(src, dest)
-        return RedisStorageData(data, filename=filename)
-
 
 class RedisReader(Reader):
     storage = None  # type: RedisStorage # pyright: ignore
 
     required_options = ["prefix"]
     capabilities = utils.combine_capabilities(Capability.STREAM)
 
@@ -100,23 +77,51 @@
 class RedisManager(Manager):
     storage = None  # type: RedisStorage # pyright: ignore
 
     required_options = ["prefix"]
     capabilities = utils.combine_capabilities(Capability.REMOVE, Capability.EXISTS)
 
     def remove(self, data):
-        # type: (dict[str, types.Any]) -> bool
+        # type: (RedisStorageData) -> bool
         key = self.storage.settings["prefix"] + data["filename"]
         self.storage.redis.delete(key)
         return True
 
     def exists(self, data):
-        # type: (dict[str, types.Any]) -> bool
+        # type: (RedisStorageData) -> bool
         key = self.storage.settings["prefix"] + data["filename"]
-        return self.storage.redis.exists(key)
+        return bool(self.storage.redis.exists(key))
+
+    def copy(self, data, name, extras):
+        # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
+        src = self.storage.settings["prefix"] + data["filename"]
+        dest = self.storage.settings["prefix"] + name
+
+        if not self.storage.redis.exists(src):
+            raise exceptions.MissingFileError(self.storage.settings["name"], src)
+
+        if self.storage.redis.exists(dest):
+            raise exceptions.ExistingFileError(self.storage.settings["name"], dest)
+
+        try:
+            self.storage.redis.copy(src, dest)
+        except AttributeError:
+            self.storage.redis.restore(dest, 0, self.storage.redis.dump(src))
+
+        return RedisStorageData(data, filename=name)
+
+    def move(self, data, name, extras):
+        # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
+        filename = self.storage.compute_name(name, extras)
+
+        src = self.storage.settings["prefix"] + data["filename"]
+        dest = self.storage.settings["prefix"] + filename
+
+        self.storage.redis.rename(src, dest)
+        return RedisStorageData(data, filename=filename)
 
 
 class RedisStorage(Storage):
     def make_uploader(self):
         return RedisUploader(self)
 
     def make_manager(self):
```

### Comparing `ckanext-files-0.2.3/ckanext/files/templates/files/snippets/file_table.html` & `ckanext_files-0.2.4/ckanext/files/templates/files/snippets/file_table.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {#
-Displays a list of files.
+    Displays a list of files.
 
-files       - A list of files to display.
-owner_type  - type of the files owner
-owner_id    - ID of the files owner
+    files       - A list of files to display.
+    owner_type  - type of the files owner
+    owner_id    - ID of the files owner
 
-Example:
+    Example:
 
-{% snippet 'files/snippets/file_table.html', files=files %}
+    {% snippet 'files/snippets/file_table.html', files=files %}
 
-#}
+    #}
 {% set columns = [
     {"name": "name", "label": "Name"},
     {"name": "ctime", "label": "Created"},
     {"name": "storage_data.content_type", "label": "Type"},
     {"name": "storage_data.size", "label": "Size"},
-] %}
+    ] %}
 
-{% set params = request.params or request.args %}
+{% set params = request.args or request.params or {} %}
 
 {% block file_table %}
     <table class="table table-striped">
         <thead>
             {% block table_header %}
                 <tr>
                     {% for column in columns %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {# Displays a list of files. files - A list of files to display. owner_type -
 type of the files owner owner_id - ID of the files owner Example: {% snippet
 'files/snippets/file_table.html', files=files %} #} {% set columns = [ {"name":
 "name", "label": "Name"}, {"name": "ctime", "label": "Created"}, {"name":
 "storage_data.content_type", "label": "Type"}, {"name": "storage_data.size",
-"label": "Size"}, ] %} {% set params = request.params or request.args %} {%
-block file_table %}
+"label": "Size"}, ] %} {% set params = request.args or request.params or {} %}
+{% block file_table %}
 {{%% iiff
 ppaarraammss..ssoorrtt ====
 ccoolluummnn..nnaammee
 aanndd
 ppaarraammss..rreevveerrssee
 ==== ''ffaallssee'' %%}}  {{{{ __((""AAccttiioonnss""))
 {{{{ __           }}}}
```

### Comparing `ckanext-files-0.2.3/ckanext/files/templates/files/snippets/uploader_v1.html` & `ckanext_files-0.2.4/ckanext/files/templates/files/snippets/uploader_v1.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 {#
-storage?
-uploader?
-file_attrs?
-#}
+    storage: str | None
+    uploader: str | None
+    file_attrs: dict[str, str] | None
+    with_dropzone: bool | None
+
+    #}
 
 {% import 'macros/form.html' as form %}
 
 {% block uploader %}
     <div class="file-uploader">
         {% block form %}
-            <form action="" method="post" class="file-uploader__form"  data-module="files--scheduler">
+            <form action="" method="post" class="file-uploader__form"
+                data-module="files--scheduler">
                 {{ form.input("upload", label="File", type="file", attrs=dict({
                     "class": "form-control",
                     "data-queue-scheduler": true,
-                }, **file_attrs|default({}))) }}
+                    }, **file_attrs|default({}))) }}
             </form>
         {% endblock form %}
 
+        {% block dropzone %}
+            {% if with_dropzone %}
+                <div class="file-uploader__dropzone" data-module="files--dropzone" data-module-immediate>
+                    {{ _("Drag a file here") }}
+                </div>
+            {% endif %}
+        {% endblock dropzone%}
+
         {% block progress %}
             <div data-module="files--queue"
-                 {% if storage is defined %} data-module-storage="{{ storage }}"{% endif %}
-                 {% if uploader is defined %} data-module-uploader="{{ uploader }}"{% endif %}
+                {% if storage is defined %} data-module-storage="{{ storage }}"{% endif %}
+                {% if uploader is defined %} data-module-uploader="{{ uploader }}"{% endif %}
             >
 
                 <div data-upload-template hidden class="card file-uploader__queue_item my-1">
                     <div class="card-header">
                         <strong data-item-name></strong>
                     </div>
```

### Comparing `ckanext-files-0.2.3/ckanext/files/templates/files/user/delete.html` & `ckanext_files-0.2.4/ckanext/files/templates/files/user/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/templates/files/user/index.html` & `ckanext_files-0.2.4/ckanext/files/templates/files/user/index.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {#
-storage?
-uploader?
-#}
+    storage: str | None
+    uploader: str | None
+    #}
 
 {% extends "user/read_base.html" %}
 
 {% block page_primary_action %}
 
     {% if (g.userobj or current_user or {}).id == user_dict.id and h.check_access('files_file_create') %}
 
-        {% snippet "files/snippets/uploader_v1.html", storage=storage, uploader=uploader %}
+        {% snippet "files/snippets/uploader_v1.html", storage=storage, uploader=uploader, with_dropzone=true %}
 
     {% endif %}
 {% endblock %}
 
 {% block primary_content_inner %}
     {% block files_list %}
         {% if files.results %}
```

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/conftest.py` & `ckanext_files-0.2.4/ckanext/files/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/logic/test_action.py` & `ckanext_files-0.2.4/ckanext/files/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/logic/test_validators.py` & `ckanext_files-0.2.4/ckanext/files/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/storage/test_fs.py` & `ckanext_files-0.2.4/ckanext/files/tests/storage/test_fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/storage/test_google_cloud.py` & `ckanext_files-0.2.4/ckanext/files/tests/storage/test_google_cloud.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/storage/test_redis.py` & `ckanext_files-0.2.4/ckanext/files/tests/storage/test_redis.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/test_base.py` & `ckanext_files-0.2.4/ckanext/files/tests/test_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -140,83 +140,14 @@
 
         with pytest.raises(NotImplementedError):
             uploader.update_multipart_upload({}, {})
 
         with pytest.raises(NotImplementedError):
             uploader.complete_multipart_upload({}, {})
 
-        with pytest.raises(NotImplementedError):
-            uploader.copy({}, "", {})
-
-        with pytest.raises(NotImplementedError):
-            uploader.move({}, "", {})
-
-    def test_compute_name_uuid(self, uploader, faker):
-        # type: (base.Uploader, Faker) -> None
-        """`uuid`(default) name strategy produces valid UUID."""
-
-        extension = faker.file_extension()
-        name = faker.file_name(extension=extension)
-        result = uploader.compute_name(name, {})
-
-        assert uuid.UUID(result)
-
-    def test_compute_name_uuid_prefix(self, uploader, faker):
-        # type: (base.Uploader, Faker) -> None
-        """`uuid_prefix` name strategy produces valid UUID."""
-        uploader.storage.settings["name_strategy"] = "uuid_prefix"
-        extension = faker.file_extension()
-        name = faker.file_name(extension=extension)
-        result = uploader.compute_name(name, {})
-        assert result.endswith(name)
-        assert uuid.UUID(result[: -len(name)])
-
-    def test_compute_name_uuid_with_extension(self, uploader, faker):
-        # type: (base.Uploader, Faker) -> None
-        """`uuid_with_extension` name strategy produces valid UUID."""
-        uploader.storage.settings["name_strategy"] = "uuid_with_extension"
-        extension = faker.file_extension()
-        name = faker.file_name(extension=extension)
-        result = uploader.compute_name(name, {})
-
-        assert result.endswith(extension)
-        assert uuid.UUID(result[: -len(extension) - 1])
-
-    def test_compute_name_datetime_prefix(self, uploader, faker, files_stopped_time):
-        # type: (base.Uploader, Faker, datetime) -> None
-        """`datetime_prefix` name strategy produces valid UUID."""
-        uploader.storage.settings["name_strategy"] = "datetime_prefix"
-        extension = faker.file_extension()
-        name = faker.file_name(extension=extension)
-        result = uploader.compute_name(name, {})
-
-        assert result == files_stopped_time.isoformat() + name
-
-    def test_compute_name_datetime_with_extension(
-        self,
-        uploader,
-        faker,
-        files_stopped_time,
-    ):
-        # type: (base.Uploader, Faker, datetime) -> None
-        """`datetime_with_extension` name strategy produces valid UUID."""
-        uploader.storage.settings["name_strategy"] = "datetime_with_extension"
-        extension = faker.file_extension()
-        name = faker.file_name(extension=extension)
-        result = uploader.compute_name(name, {})
-
-        assert result == files_stopped_time.isoformat() + "." + extension
-
-    def test_compute_name_with_wrong_strategy(self, uploader):
-        # type: (base.Uploader) -> None
-        """`datetime_with_extension` name strategy produces valid UUID."""
-        uploader.storage.settings["name_strategy"] = "wrong_strategy"
-        with pytest.raises(exceptions.NameStrategyError):
-            uploader.compute_name("test", {})
-
 
 class TestManager:
     @pytest.fixture()
     def manager(self):
         return base.Manager(base.Storage())
 
     def test_abstract_methods(self, manager):
@@ -362,7 +293,76 @@
             storage.remove({})
 
         with pytest.raises(NotImplementedError):
             storage.copy({}, storage, "", {})
 
         with pytest.raises(NotImplementedError):
             storage.move({}, storage, "", {})
+
+    def test_compute_name_uuid(self, faker):
+        # type: (Faker) -> None
+        """`uuid`(default) name strategy produces valid UUID."""
+        storage = Storage()
+
+        extension = faker.file_extension()
+        name = faker.file_name(extension=extension)
+        result = storage.compute_name(name, {})
+
+        assert uuid.UUID(result)
+
+    def test_compute_name_uuid_prefix(self, faker):
+        # type: (Faker) -> None
+        """`uuid_prefix` name strategy produces valid UUID."""
+        storage = Storage()
+
+        storage.settings["name_strategy"] = "uuid_prefix"
+        extension = faker.file_extension()
+        name = faker.file_name(extension=extension)
+        result = storage.compute_name(name, {})
+        assert result.endswith(name)
+        assert uuid.UUID(result[: -len(name)])
+
+    def test_compute_name_uuid_with_extension(self, faker):
+        # type: (Faker) -> None
+        """`uuid_with_extension` name strategy produces valid UUID."""
+        storage = Storage()
+        storage.settings["name_strategy"] = "uuid_with_extension"
+        extension = faker.file_extension()
+        name = faker.file_name(extension=extension)
+        result = storage.compute_name(name, {})
+
+        assert result.endswith(extension)
+        assert uuid.UUID(result[: -len(extension) - 1])
+
+    def test_compute_name_datetime_prefix(self, faker, files_stopped_time):
+        # type: (Faker, datetime) -> None
+        """`datetime_prefix` name strategy produces valid UUID."""
+        storage = Storage()
+        storage.settings["name_strategy"] = "datetime_prefix"
+        extension = faker.file_extension()
+        name = faker.file_name(extension=extension)
+        result = storage.compute_name(name, {})
+
+        assert result == files_stopped_time.isoformat() + name
+
+    def test_compute_name_datetime_with_extension(
+        self,
+        faker,
+        files_stopped_time,
+    ):
+        # type: (Faker, datetime) -> None
+        """`datetime_with_extension` name strategy produces valid UUID."""
+        storage = Storage()
+        storage.settings["name_strategy"] = "datetime_with_extension"
+        extension = faker.file_extension()
+        name = faker.file_name(extension=extension)
+        result = storage.compute_name(name, {})
+
+        assert result == files_stopped_time.isoformat() + "." + extension
+
+    def test_compute_name_with_wrong_strategy(self):
+        # type: () -> None
+        """`datetime_with_extension` name strategy produces valid UUID."""
+        storage = Storage()
+        storage.settings["name_strategy"] = "wrong_strategy"
+        with pytest.raises(exceptions.NameStrategyError):
+            storage.compute_name("test", {})
```

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/test_config.py` & `ckanext_files-0.2.4/ckanext/files/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/tests/test_utils.py` & `ckanext_files-0.2.4/ckanext/files/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/types.py` & `ckanext_files-0.2.4/ckanext/files/types.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/ckanext/files/utils.py` & `ckanext_files-0.2.4/ckanext/files/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 
 Do not use this module outside of the extension and do not import any other
 internal modules except for types and exceptions. Only independent tools are
 stored here, to avoid import cycles.
 
 """
 
+import cgi
+import mimetypes
 import re
+from io import BytesIO
 
+import magic
 import six
+from werkzeug.datastructures import FileStorage
 
 from ckanext.files import exceptions
 
 from ckanext.files import types  # isort: skip # noqa: 401
 
 if six.PY3:
     from typing import TypeVar
@@ -169,7 +174,51 @@
     size, unit = result.groups()
 
     multiplier = UNITS.get(unit.lower())
     if not multiplier:
         raise ValueError(value)
 
     return int(float(size) * multiplier)
+
+
+def make_upload(value):
+    # type: (Any) -> types.Upload
+    """Convert value into werkzeug.FileStorage object"""
+    if isinstance(value, FileStorage):
+        if not value.content_length:
+            value.stream.seek(0, 2)
+            value.headers["content-length"] = str(value.stream.tell())
+            value.stream.seek(0)
+        return value
+
+    if isinstance(value, cgi.FieldStorage):
+        if not value.filename or not value.file:
+            raise ValueError(value)
+
+        mime, _encoding = mimetypes.guess_type(value.filename)
+        if not mime:
+            mime = magic.from_buffer(value.file.read(1024), True)
+            value.file.seek(0)
+        value.file.seek(0, 2)
+        size = value.file.tell()
+        value.file.seek(0)
+
+        return FileStorage(
+            value.file,
+            value.filename,
+            content_type=mime,
+            content_length=size,
+        )
+
+    if isinstance(value, six.text_type):
+        value = value.encode()
+
+    if isinstance(value, (bytes, bytearray)):
+        stream = BytesIO(value)
+        mime = magic.from_buffer(stream.read(1024), True)
+        stream.seek(0, 2)
+        size = stream.tell()
+        stream.seek(0)
+
+        return FileStorage(stream, content_type=mime, content_length=size)
+
+    raise TypeError(type(value))
```

### Comparing `ckanext-files-0.2.3/ckanext/files/views.py` & `ckanext_files-0.2.4/ckanext/files/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     # type: (str, str | None) -> str
     user_dict = tk.get_action("user_show")(
         {},
         {"id": user_id, "include_num_followers": True},
     )
 
     rows = 10
-    params = tk.request.params  # type: ignore
+    params = tk.request.args if tk.check_ckan_version("2.10") else tk.request.params  # type: ignore
     page = tk.h.get_page_number(params)
     start = rows * page - rows
 
     search_dict = {
         "rows": rows,
         "start": start,
         "user": user_id,
```

### Comparing `ckanext-files-0.2.3/ckanext_files.egg-info/PKG-INFO` & `ckanext_files-0.2.4/ckanext_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-files-0.2.3/ckanext_files.egg-info/SOURCES.txt` & `ckanext_files-0.2.4/ckanext_files.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 ckanext/files/shared.py
 ckanext/files/types.py
 ckanext/files/utils.py
 ckanext/files/views.py
 ckanext/files/assets/resource.config
 ckanext/files/assets/webassets.yml
 ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
-ckanext/files/assets/scripts/files--queue.js
+ckanext/files/assets/scripts/files--modules.js
+ckanext/files/assets/scripts/files--shared-uploader.js
 ckanext/files/assets/scripts/files--shared.js
 ckanext/files/assets/styles/files--style.css
 ckanext/files/logic/__init__.py
 ckanext/files/logic/action.py
 ckanext/files/logic/auth.py
 ckanext/files/logic/schema.py
 ckanext/files/logic/validators.py
@@ -44,14 +45,15 @@
 ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
 ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
 ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
 ckanext/files/model/__init__.py
 ckanext/files/model/base.py
 ckanext/files/model/file.py
 ckanext/files/model/owner.py
+ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
 ckanext/files/storage/__init__.py
 ckanext/files/storage/fs.py
 ckanext/files/storage/google_cloud.py
 ckanext/files/storage/redis.py
 ckanext/files/templates/page.html
 ckanext/files/templates/files/snippets/_asset.html
 ckanext/files/templates/files/snippets/_resource.html
```

### Comparing `ckanext-files-0.2.3/pyproject.toml` & `ckanext_files-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.3/setup.cfg` & `ckanext_files-0.2.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-files
-version = 0.2.3
+version = 0.2.4
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-files
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

