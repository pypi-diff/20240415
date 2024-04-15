# Comparing `tmp/itk_dev_shared_components-2.1.0.tar.gz` & `tmp/itk_dev_shared_components-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itk_dev_shared_components-2.1.0.tar", last modified: Tue Apr  9 08:15:10 2024, max compression
+gzip compressed data, was "itk_dev_shared_components-2.1.1.tar", last modified: Mon Apr 15 09:33:16 2024, max compression
```

## Comparing `itk_dev_shared_components-2.1.0.tar` & `itk_dev_shared_components-2.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.067278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.067278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/cpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/misc/cpr_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/fmcacov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/gridview_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/opret_kundekontakt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/sap_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/sap_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/itk_dev_shared_components/smtp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/smtp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components/smtp/smtp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 08:15:10.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-09 08:15:10.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:15:10.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 08:15:10.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 08:15:10.000000 itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 08:15:05.000000 itk_dev_shared_components-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:15:10.071278 itk_dev_shared_components-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/cpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/cpr_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/fmcacov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/gridview_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/opret_kundekontakt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/smtp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/setup.cfg
```

### Comparing `itk_dev_shared_components-2.1.0/LICENSE` & `itk_dev_shared_components-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/PKG-INFO` & `itk_dev_shared_components-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 2.1.0
+Version: 2.1.1
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-2.1.0/README.md` & `itk_dev_shared_components-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/authentication.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/graph/mail.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/mail.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/authentication.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/cpr.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/cpr.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_cases.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_cases.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_documents.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_documents.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import mimetypes
 from typing import BinaryIO
 import urllib.parse
 
 import requests
 
 from itk_dev_shared_components.kmd_nova.authentication import NovaAccess
-from itk_dev_shared_components.kmd_nova.nova_objects import Document
+from itk_dev_shared_components.kmd_nova.nova_objects import Document, Caseworker
 from itk_dev_shared_components.kmd_nova. util import datetime_from_iso_string
 
 
 def get_documents(case_uuid: str, nova_access: NovaAccess) -> list[Document]:
     """Get all documents attached to the given case.
     To get the actual document file use download_document_file.
 
@@ -40,37 +40,49 @@
             "title": True,
             "sensitivity": True,
             "documentType": True,
             "description": True,
             "approved": True,
             "documentDate": True,
             "fileExtension": True,
-            "documentCategory": True
+            "documentCategory": True,
+            "caseworker": True
         }
     }
 
     headers = {'Content-Type': 'application/json', 'Authorization': f"Bearer {nova_access.get_bearer_token()}"}
 
     response = requests.put(url, params=params, headers=headers, json=payload, timeout=60)
     response.raise_for_status()
 
     documents = []
     for document_dict in response.json()['documents']:
+
+        if 'caseworker' in document_dict:
+            caseworker = Caseworker(
+                uuid = document_dict['caseworker']['kspIdentity']['novaUserId'],
+                name = document_dict['caseworker']['kspIdentity']['fullName'],
+                ident = document_dict['caseworker']['kspIdentity']['racfId']
+            )
+        else:
+            caseworker = None
+
         doc = Document(
             uuid = document_dict['documentUuid'],
             document_number = document_dict['documentNumber'],
             title = document_dict['title'],
             sensitivity = document_dict['sensitivity'],
             document_type = document_dict['documentType'],
             description = document_dict.get('description', None),
             approved = document_dict['approved'],
             document_date = datetime_from_iso_string(document_dict['documentDate']),
             file_extension = document_dict['fileExtension'],
             category_name = document_dict.get('documentCategoryName'),
-            category_uuid = document_dict.get('documentCategoryUuid')
+            category_uuid = document_dict.get('documentCategoryUuid'),
+            caseworker=caseworker
         )
         documents.append(doc)
 
     return documents
 
 
 def download_document_file(document_uuid: str, nova_access: NovaAccess, checkout: bool = False, checkout_comment: str = None) -> bytes:
@@ -180,10 +192,18 @@
                 "fullName": security_unit_name,
             }
         },
         "approved": document.approved,
         "accessToDocuments": True
     }
 
+    if document.caseworker:
+        payload['caseworker'] = {
+            "kspIdentity": {
+                "racfId": document.caseworker.ident,
+                "fullName": document.caseworker.name
+            }
+        }
+
     headers = {'Content-Type': 'application/json', 'Authorization': f"Bearer {nova_access.get_bearer_token()}"}
     response = requests.post(url, params=params, headers=headers, json=payload, timeout=60)
     response.raise_for_status()
```

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_objects.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     description: str
     approved: bool
     document_number: Optional[str] = None
     document_date: Optional[datetime] = None
     file_extension: Optional[str] = None
     category_name: Optional[str] = None
     category_uuid: Optional[str] = None
+    caseworker: Optional[Caseworker] = None
 
 
 @dataclass(slots=True, kw_only=True)
 class JournalNote:
     """A dataclass representing a KMD Nova journal note."""
     uuid: str
     title: str
```

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/nova_tasks.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_tasks.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/kmd_nova/util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/misc/cpr_util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/cpr_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/fmcacov.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/fmcacov.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/gridview_util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/gridview_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/multi_session.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/multi_session.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/opret_kundekontakt.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/opret_kundekontakt.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/sap_login.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_login.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/sap_util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/sap/tree_util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/tree_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components/smtp/smtp_util.py` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/smtp_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/PKG-INFO` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 2.1.0
+Version: 2.1.1
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-2.1.0/itk_dev_shared_components.egg-info/SOURCES.txt` & `itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.0/pyproject.toml` & `itk_dev_shared_components-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itk_dev_shared_components"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="ITK Development", email="itk-rpa@mkb.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

