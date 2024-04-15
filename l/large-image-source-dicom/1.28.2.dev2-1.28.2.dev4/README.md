# Comparing `tmp/large-image-source-dicom-1.28.2.dev2.tar.gz` & `tmp/large-image-source-dicom-1.28.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.28.2.dev2.tar", last modified: Fri Apr 12 15:22:52 2024, max compression
+gzip compressed data, was "large-image-source-dicom-1.28.2.dev4.tar", last modified: Mon Apr 15 12:54:07 2024, max compression
```

## Comparing `large-image-source-dicom-1.28.2.dev2.tar` & `large-image-source-dicom-1.28.2.dev4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.903277 large-image-source-dicom-1.28.2.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-12 15:22:52.899277 large-image-source-dicom-1.28.2.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.883277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.887277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22975 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/dicom_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/dicom_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/dicomweb_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/girder_plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.891277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.891277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.895277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/assetstoreImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.899277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/AuthOptions.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3469 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/DICOMwebImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.899277 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-12 15:22:52.000000 large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 15:22:52.903277 large-image-source-dicom-1.28.2.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2753 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.899277 large-image-source-dicom-1.28.2.dev2/test_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/test_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/test_dicom/test_web_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:22:52.899277 large-image-source-dicom-1.28.2.dev2/test_dicom/web_client_specs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2024-04-12 15:20:51.000000 large-image-source-dicom-1.28.2.dev2/test_dicom/web_client_specs/dicomWebSpec.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.033767 large-image-source-dicom-1.28.2.dev4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-15 12:54:07.033767 large-image-source-dicom-1.28.2.dev4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.025767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22975 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/dicom_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/dicom_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/dicomweb_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/girder_plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/models/AssetstoreModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/assetstoreImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/AuthOptions.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3469 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/DICOMwebImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-15 12:54:07.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-15 12:54:06.000000 large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-15 12:54:07.033767 large-image-source-dicom-1.28.2.dev4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2753 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/test_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/test_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/test_dicom/test_web_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:54:07.029767 large-image-source-dicom-1.28.2.dev4/test_dicom/web_client_specs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2024-04-15 12:52:04.000000 large-image-source-dicom-1.28.2.dev4/test_dicom/web_client_specs/dicomWebSpec.js
```

### Comparing `large-image-source-dicom-1.28.2.dev2/LICENSE` & `large-image-source-dicom-1.28.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/PKG-INFO` & `large-image-source-dicom-1.28.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.2.dev2
+Version: 1.28.2.dev4
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev2
+Requires-Dist: large-image>=1.28.2.dev4
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev2; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.2.dev2/README.rst` & `large-image-source-dicom-1.28.2.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/__init__.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/assetstore/rest.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/assetstore/rest.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/dicom_metadata.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/dicomweb_utils.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/dicomweb_utils.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/models/AssetstoreModel.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/models/AssetstoreModel.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/package.json` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/package.json`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/routes.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/assetstoreImport.pug` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/assetstoreImport.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/AssetstoresView.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/DICOMwebImportView.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/DICOMwebImportView.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.2.dev2
+Version: 1.28.2.dev4
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev2
+Requires-Dist: large-image>=1.28.2.dev4
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev2; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.2.dev2/large_image_source_dicom.egg-info/SOURCES.txt` & `large-image-source-dicom-1.28.2.dev4/large_image_source_dicom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/setup.py` & `large-image-source-dicom-1.28.2.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/test_dicom/test_web_client.py` & `large-image-source-dicom-1.28.2.dev4/test_dicom/test_web_client.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev2/test_dicom/web_client_specs/dicomWebSpec.js` & `large-image-source-dicom-1.28.2.dev4/test_dicom/web_client_specs/dicomWebSpec.js`

 * *Files identical despite different names*
