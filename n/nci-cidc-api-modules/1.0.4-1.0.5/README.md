# Comparing `tmp/nci_cidc_api_modules-1.0.4.tar.gz` & `tmp/nci_cidc_api_modules-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci_cidc_api_modules-1.0.4.tar", last modified: Thu Apr 11 16:08:56 2024, max compression
+gzip compressed data, was "nci_cidc_api_modules-1.0.5.tar", last modified: Fri Apr 12 17:00:18 2024, max compression
```

## Comparing `nci_cidc_api_modules-1.0.4.tar` & `nci_cidc_api_modules-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.110384 nci_cidc_api_modules-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-11 16:08:56.110384 nci_cidc_api_modules-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.102384 nci_cidc_api_modules-1.0.4/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.106384 nci_cidc_api_modules-1.0.4/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.106384 nci_cidc_api_modules-1.0.4/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.106384 nci_cidc_api_modules-1.0.4/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.106384 nci_cidc_api_modules-1.0.4/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.106384 nci_cidc_api_modules-1.0.4/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.110384 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-11 16:08:56.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-11 16:08:56.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:08:56.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:08:55.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 16:08:56.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 16:08:56.000000 nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:08:56.110384 nci_cidc_api_modules-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:08:56.110384 nci_cidc_api_modules-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-11 16:08:52.000000 nci_cidc_api_modules-1.0.4/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.264310 nci_cidc_api_modules-1.0.5/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.268309 nci_cidc_api_modules-1.0.5/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-1.0.4/LICENSE` & `nci_cidc_api_modules-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/PKG-INFO` & `nci_cidc_api_modules-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.4
+Version: 1.0.5
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
```

### Comparing `nci_cidc_api_modules-1.0.4/README.md` & `nci_cidc_api_modules-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/config/db.py` & `nci_cidc_api_modules-1.0.5/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/config/logging.py` & `nci_cidc_api_modules-1.0.5/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/config/secrets.py` & `nci_cidc_api_modules-1.0.5/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/config/settings.py` & `nci_cidc_api_modules-1.0.5/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/csms/auth.py` & `nci_cidc_api_modules-1.0.5/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/files/details.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/migrations.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/models.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/models/schemas.py` & `nci_cidc_api_modules-1.0.5/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/shared/auth.py` & `nci_cidc_api_modules-1.0.5/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/shared/emails.py` & `nci_cidc_api_modules-1.0.5/cidc_api/shared/emails.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Template functions for CIDC email bodies."""
+
 import html
 import base64
 from functools import wraps
 from typing import Dict, Union
 
 from cidc_schemas.prism import generate_analysis_configs_from_upload_patch
 
@@ -82,18 +83,21 @@
 
     return email
 
 
 @sendable
 def new_upload_alert(upload, full_metadata) -> dict:
     """Alert the CIDC administrators that an upload succeeded."""
-    pipeline_configs: Dict[
-        str, Union[bytes, str]
-    ] = generate_analysis_configs_from_upload_patch(
-        full_metadata, upload.metadata_patch, upload.upload_type, GOOGLE_ACL_DATA_BUCKET
+    pipeline_configs: Dict[str, Union[bytes, str]] = (
+        generate_analysis_configs_from_upload_patch(
+            full_metadata,
+            upload.metadata_patch,
+            upload.upload_type,
+            GOOGLE_ACL_DATA_BUCKET,
+        )
     )
 
     subject = (
         f"[UPLOAD SUCCESS]({ENV}) {upload.upload_type} uploaded to {upload.trial_id}"
     )
 
     html_content = f"""
```

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-1.0.5/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-1.0.5/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.4
+Version: 1.0.5
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
```

### Comparing `nci_cidc_api_modules-1.0.4/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/pyproject.toml` & `nci_cidc_api_modules-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 exclude = "migrations"
-target-version = ["py36"]
+target-version = ["py39"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 # configure a webdriver for testing Dash dashboards
 # addopts = "--webdriver Chrome --headless"
 
 [tool.poetry]
```

### Comparing `nci_cidc_api_modules-1.0.4/setup.py` & `nci_cidc_api_modules-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.4/tests/test_api.py` & `nci_cidc_api_modules-1.0.5/tests/test_api.py`

 * *Files identical despite different names*

