# Comparing `tmp/cmem_cmempy-24.1.0.tar.gz` & `tmp/cmem_cmempy-24.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmempy-24.1.0.tar", max compression
+gzip compressed data, was "cmem_cmempy-24.1.1.tar", max compression
```

## Comparing `cmem_cmempy-24.1.0.tar` & `cmem_cmempy-24.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2023-01-18 07:28:45.000000 cmem_cmempy-24.1.0/LICENSE
--rw-r--r--   0        0        0      660 2024-01-22 07:46:42.474850 cmem_cmempy-24.1.0/README-public.md
--rw-r--r--   0        0        0      110 2024-01-22 07:46:42.475418 cmem_cmempy-24.1.0/cmem/__init__.py
--rw-r--r--   0        0        0       40 2024-01-22 07:46:42.475474 cmem_cmempy-24.1.0/cmem/cmempy/__init__.py
--rw-r--r--   0        0        0     4456 2024-01-22 07:46:42.475693 cmem_cmempy-24.1.0/cmem/cmempy/api.py
--rw-r--r--   0        0        0     4970 2024-01-22 07:46:42.475915 cmem_cmempy-24.1.0/cmem/cmempy/config.py
--rw-r--r--   0        0        0     1062 2024-01-22 07:46:42.476013 cmem_cmempy-24.1.0/cmem/cmempy/custom_tasks/__init__.py
--rw-r--r--   0        0        0       36 2024-01-22 07:46:42.476069 cmem_cmempy-24.1.0/cmem/cmempy/dp/__init__.py
--rw-r--r--   0        0        0     1202 2024-01-22 07:46:42.476196 cmem_cmempy-24.1.0/cmem/cmempy/dp/admin/__init__.py
--rw-r--r--   0        0        0     1014 2024-01-22 07:46:42.476255 cmem_cmempy-24.1.0/cmem/cmempy/dp/admin/backup.py
--rw-r--r--   0        0        0       42 2024-01-22 07:46:42.476319 cmem_cmempy-24.1.0/cmem/cmempy/dp/authorization/__init__.py
--rw-r--r--   0        0        0     3806 2024-01-23 20:02:10.440088 cmem_cmempy-24.1.0/cmem/cmempy/dp/authorization/conditions.py
--rw-r--r--   0        0        0      477 2024-01-22 07:46:42.476506 cmem_cmempy-24.1.0/cmem/cmempy/dp/authorization/refresh.py
--rw-r--r--   0        0        0      380 2024-01-22 07:46:42.476594 cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/__init__.py
--rw-r--r--   0        0        0     6289 2024-01-23 20:02:10.440338 cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/graph.py
--rw-r--r--   0        0        0     4159 2024-01-22 07:46:42.476909 cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/sparql.py
--rw-r--r--   0        0        0     1244 2024-01-22 07:46:42.476968 cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/update.py
--rw-r--r--   0        0        0       16 2024-01-23 20:02:10.440929 cmem_cmempy-24.1.0/cmem/cmempy/dp/shacl/__init__.py
--rw-r--r--   0        0        0     1767 2024-01-23 20:02:10.441141 cmem_cmempy-24.1.0/cmem/cmempy/dp/shacl/validation.py
--rw-r--r--   0        0        0     1011 2024-01-22 07:46:42.477631 cmem_cmempy-24.1.0/cmem/cmempy/dp/titles/__init__.py
--rw-r--r--   0        0        0     5905 2024-01-22 07:46:42.477726 cmem_cmempy-24.1.0/cmem/cmempy/health/__init__.py
--rw-r--r--   0        0        0     1807 2024-01-22 07:46:42.477807 cmem_cmempy-24.1.0/cmem/cmempy/keycloak/client.py
--rw-r--r--   0        0        0      519 2024-01-22 07:46:42.478039 cmem_cmempy-24.1.0/cmem/cmempy/keycloak/group.py
--rw-r--r--   0        0        0     4532 2024-01-22 07:46:42.478362 cmem_cmempy-24.1.0/cmem/cmempy/keycloak/user.py
--rw-r--r--   0        0        0       31 2024-01-22 07:46:42.478461 cmem_cmempy-24.1.0/cmem/cmempy/linking/__init__.py
--rw-r--r--   0        0        0     2588 2024-01-22 07:46:42.478522 cmem_cmempy-24.1.0/cmem/cmempy/linking/linkingtask.py
--rw-r--r--   0        0        0       26 2024-01-22 07:46:42.478577 cmem_cmempy-24.1.0/cmem/cmempy/plugins/__init__.py
--rw-r--r--   0        0        0     1939 2024-01-22 07:46:42.478637 cmem_cmempy-24.1.0/cmem/cmempy/plugins/marshalling.py
--rw-r--r--   0        0        0    11190 2024-01-22 07:46:42.478891 cmem_cmempy-24.1.0/cmem/cmempy/queries/__init__.py
--rw-r--r--   0        0        0       33 2024-01-22 07:46:42.479159 cmem_cmempy-24.1.0/cmem/cmempy/transform/__init__.py
--rw-r--r--   0        0        0     1090 2024-01-22 07:46:42.479261 cmem_cmempy-24.1.0/cmem/cmempy/transform/rules/__init__.py
--rw-r--r--   0        0        0     1075 2024-01-22 07:46:42.479335 cmem_cmempy-24.1.0/cmem/cmempy/transform/rules/transformationrule.py
--rw-r--r--   0        0        0     1240 2024-01-22 07:46:42.479392 cmem_cmempy-24.1.0/cmem/cmempy/transform/transformationtask.py
--rw-r--r--   0        0        0     3597 2024-01-22 07:46:42.479462 cmem_cmempy-24.1.0/cmem/cmempy/vocabularies/__init__.py
--rw-r--r--   0        0        0      731 2024-01-22 07:46:42.479907 cmem_cmempy-24.1.0/cmem/cmempy/workflow/__init__.py
--rw-r--r--   0        0        0     4891 2024-01-22 07:46:42.479997 cmem_cmempy-24.1.0/cmem/cmempy/workflow/workflow.py
--rw-r--r--   0        0        0      131 2024-01-22 07:46:42.480049 cmem_cmempy-24.1.0/cmem/cmempy/workflow/workflows.py
--rw-r--r--   0        0        0     1873 2024-01-22 07:46:42.480108 cmem_cmempy-24.1.0/cmem/cmempy/workspace/__init__.py
--rw-r--r--   0        0        0      407 2024-01-23 20:02:10.441528 cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/__init__.py
--rw-r--r--   0        0        0      914 2024-01-22 07:46:42.480478 cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/projectactivities.py
--rw-r--r--   0        0        0     2281 2024-01-22 07:46:42.480534 cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/projectactivity.py
--rw-r--r--   0        0        0     3164 2024-01-22 07:46:42.480590 cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/taskactivities.py
--rw-r--r--   0        0        0     2323 2024-01-22 07:46:42.480637 cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/taskactivity.py
--rw-r--r--   0        0        0      744 2024-01-22 07:46:42.480702 cmem_cmempy-24.1.0/cmem/cmempy/workspace/export_/__init__.py
--rw-r--r--   0        0        0     1540 2024-01-22 07:46:42.480768 cmem_cmempy-24.1.0/cmem/cmempy/workspace/import_/__init__.py
--rw-r--r--   0        0        0      454 2024-01-22 07:46:42.480826 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/__init__.py
--rw-r--r--   0        0        0       45 2024-01-22 07:46:42.480872 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/datasets/__init__.py
--rw-r--r--   0        0        0     5115 2024-01-22 07:46:42.480997 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/datasets/dataset.py
--rw-r--r--   0        0        0      748 2024-01-22 07:46:42.481058 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/export_.py
--rw-r--r--   0        0        0     4945 2024-01-22 07:46:42.481113 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/import_.py
--rw-r--r--   0        0        0     3809 2024-01-22 07:46:42.481370 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/project.py
--rw-r--r--   0        0        0      960 2024-01-22 07:46:42.481471 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/resources/__init__.py
--rw-r--r--   0        0        0     6089 2024-01-22 07:46:42.481649 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/resources/resource.py
--rw-r--r--   0        0        0     2454 2024-01-23 20:02:10.441759 cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/variables/__init__.py
--rw-r--r--   0        0        0     2292 2024-01-22 07:46:42.481941 cmem_cmempy-24.1.0/cmem/cmempy/workspace/python.py
--rw-r--r--   0        0        0     1075 2024-01-22 07:46:42.481996 cmem_cmempy-24.1.0/cmem/cmempy/workspace/search/__init__.py
--rw-r--r--   0        0        0     2087 2024-01-22 07:46:42.483445 cmem_cmempy-24.1.0/cmem/cmempy/workspace/tasks/__init__.py
--rw-r--r--   0        0        0     2272 2024-01-24 07:58:20.715966 cmem_cmempy-24.1.0/pyproject.toml
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 cmem_cmempy-24.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/LICENSE
+-rw-r--r--   0        0        0      660 2023-11-13 07:58:17.000000 cmem_cmempy-24.1.1/README-public.md
+-rw-r--r--   0        0        0      110 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/__init__.py
+-rw-r--r--   0        0        0     4456 2023-04-27 06:10:06.000000 cmem_cmempy-24.1.1/cmem/cmempy/api.py
+-rw-r--r--   0        0        0     4970 2023-04-27 06:10:06.000000 cmem_cmempy-24.1.1/cmem/cmempy/config.py
+-rw-r--r--   0        0        0     1062 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/custom_tasks/__init__.py
+-rw-r--r--   0        0        0       36 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/__init__.py
+-rw-r--r--   0        0        0     1202 2023-11-13 07:58:17.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/admin/__init__.py
+-rw-r--r--   0        0        0     1014 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/admin/backup.py
+-rw-r--r--   0        0        0       42 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/authorization/__init__.py
+-rw-r--r--   0        0        0     3857 2024-04-15 09:37:48.964665 cmem_cmempy-24.1.1/cmem/cmempy/dp/authorization/conditions.py
+-rw-r--r--   0        0        0      477 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/authorization/refresh.py
+-rw-r--r--   0        0        0      380 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/__init__.py
+-rw-r--r--   0        0        0     6287 2024-04-15 09:37:48.964796 cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/graph.py
+-rw-r--r--   0        0        0     4159 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/sparql.py
+-rw-r--r--   0        0        0     1359 2024-04-15 09:37:48.965383 cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/update.py
+-rw-r--r--   0        0        0       16 2024-04-15 09:37:48.965460 cmem_cmempy-24.1.1/cmem/cmempy/dp/shacl/__init__.py
+-rw-r--r--   0        0        0     1756 2024-04-15 09:37:48.965537 cmem_cmempy-24.1.1/cmem/cmempy/dp/shacl/validation.py
+-rw-r--r--   0        0        0     1011 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/dp/titles/__init__.py
+-rw-r--r--   0        0        0     5905 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/health/__init__.py
+-rw-r--r--   0        0        0     1807 2023-09-15 07:05:35.000000 cmem_cmempy-24.1.1/cmem/cmempy/keycloak/client.py
+-rw-r--r--   0        0        0      519 2023-04-27 06:10:06.000000 cmem_cmempy-24.1.1/cmem/cmempy/keycloak/group.py
+-rw-r--r--   0        0        0     4568 2024-04-15 09:37:48.965941 cmem_cmempy-24.1.1/cmem/cmempy/keycloak/user.py
+-rw-r--r--   0        0        0       31 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/linking/__init__.py
+-rw-r--r--   0        0        0     2588 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/linking/linkingtask.py
+-rw-r--r--   0        0        0       26 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/plugins/__init__.py
+-rw-r--r--   0        0        0     1939 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/plugins/marshalling.py
+-rw-r--r--   0        0        0    11213 2024-04-15 09:37:48.966539 cmem_cmempy-24.1.1/cmem/cmempy/queries/__init__.py
+-rw-r--r--   0        0        0       33 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/transform/__init__.py
+-rw-r--r--   0        0        0     1090 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/transform/rules/__init__.py
+-rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/transform/rules/transformationrule.py
+-rw-r--r--   0        0        0     1240 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/transform/transformationtask.py
+-rw-r--r--   0        0        0     3597 2023-01-05 19:05:10.000000 cmem_cmempy-24.1.1/cmem/cmempy/vocabularies/__init__.py
+-rw-r--r--   0        0        0      731 2023-09-15 07:05:35.000000 cmem_cmempy-24.1.1/cmem/cmempy/workflow/__init__.py
+-rw-r--r--   0        0        0     4891 2023-09-15 07:05:35.000000 cmem_cmempy-24.1.1/cmem/cmempy/workflow/workflow.py
+-rw-r--r--   0        0        0      131 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workflow/workflows.py
+-rw-r--r--   0        0        0     1873 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-15 09:37:48.966624 cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/__init__.py
+-rw-r--r--   0        0        0      914 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/projectactivities.py
+-rw-r--r--   0        0        0     2281 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/projectactivity.py
+-rw-r--r--   0        0        0     3164 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/taskactivities.py
+-rw-r--r--   0        0        0     2323 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/taskactivity.py
+-rw-r--r--   0        0        0      744 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/export_/__init__.py
+-rw-r--r--   0        0        0     1540 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/import_/__init__.py
+-rw-r--r--   0        0        0      454 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/datasets/__init__.py
+-rw-r--r--   0        0        0     4987 2024-04-15 09:37:48.966779 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py
+-rw-r--r--   0        0        0      748 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/export_.py
+-rw-r--r--   0        0        0     4945 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/import_.py
+-rw-r--r--   0        0        0     3728 2024-04-15 09:37:48.966919 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/project.py
+-rw-r--r--   0        0        0      960 2023-04-27 06:10:06.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/resources/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-27 06:10:06.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/resources/resource.py
+-rw-r--r--   0        0        0     2424 2024-04-15 09:37:48.967074 cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/variables/__init__.py
+-rw-r--r--   0        0        0     2292 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/python.py
+-rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/search/__init__.py
+-rw-r--r--   0        0        0     2087 2023-09-15 07:05:35.000000 cmem_cmempy-24.1.1/cmem/cmempy/workspace/tasks/__init__.py
+-rw-r--r--   0        0        0     2272 2024-04-15 09:39:59.108771 cmem_cmempy-24.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 cmem_cmempy-24.1.1/PKG-INFO
```

### Comparing `cmem_cmempy-24.1.0/LICENSE` & `cmem_cmempy-24.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/README-public.md` & `cmem_cmempy-24.1.1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/api.py` & `cmem_cmempy-24.1.1/cmem/cmempy/api.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/config.py` & `cmem_cmempy-24.1.1/cmem/cmempy/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/custom_tasks/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/custom_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/admin/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/admin/backup.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/admin/backup.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/authorization/conditions.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/authorization/conditions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 """API for managing conditions in DP."""
 import json
-from typing import Optional
+from typing import Optional, Union
 
 from cmem.cmempy import config
 
 from cmem.cmempy.api import request
 
 
 def get_authorization_uri():
     """Get graph URI of the authorization conditions graph."""
     path = "/api/authorization"
     return config.get_dp_api_endpoint() + path
 
 
 def get_acls(page: int = 0):
     """GET access conditions."""
-    return request(
-        get_authorization_uri(),
-        method="GET",
-        params={"page": page}
-    )
+    return request(get_authorization_uri(), method="GET", params={"page": page})
 
 
 def fetch_all_acls() -> list:
     """Fetch all the access conditions"""
     acls: list[dict] = []
     page: int = 0
     while True:
         result = get_acls(page=page).json()
-        acls += result['content']
-        if result['last']:
+        acls += result["content"]
+        if result["last"]:
             break
         page += 1
     return acls
 
 
 # pylint: disable-msg=too-many-arguments
 def update_access_condition(
-        iri,
-        name=None,
-        description=None,
-        user=None,
-        groups=None,
-        read_graphs=None,
-        write_graphs=None,
-        actions=None,
+    iri,
+    name=None,
+    description=None,
+    user=None,
+    groups=None,
+    read_graphs=None,
+    write_graphs=None,
+    actions=None,
 ):
     """PUT access conditions."""
     payload = get_access_condition_by_iri(iri=iri).json()
     if name:
         payload["name"] = name
     if description:
         payload["comment"] = description
@@ -105,20 +101,26 @@
 
 def get_users():
     """GET users."""
     uri = get_authorization_uri() + "/users"
     return request(uri, method="GET")
 
 
-def review_graph_rights(account_iri: str = None, group_iris: list[str] = None):
+def review_graph_rights(
+        account_iri: Union[str, None] = None,
+        group_iris: Union[list[str], None] = None
+):
     """Review access rights for a given account and group."""
     uri = get_authorization_uri() + "/review"
 
     # query parameters
-    params = {"accountIri": account_iri, "groupIris": group_iris}
+    params: dict[str, Union[str, list[str], None]] = {
+        "accountIri": account_iri,
+        "groupIris": group_iris
+    }
     return request(uri, method="GET", params=params)
 
 
 def get_access_condition_by_iri(iri: str):
     """Get access condition by iri."""
     uri = get_authorization_uri() + "/iri"
     params = {"resource": iri}
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/graph.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     with open(file, "rb") as file_handle:
         return request(
             uri, method="POST", files={"file": (os.path.basename(file), file_handle)}
         )
 
 
 def post_streamed(
-        graph, file: Union[str, io.StringIO],
+        graph, file: Union[str, io.BytesIO],
         endpoint_id="default", replace=False,
         content_type="text/turtle"
 ):
     """Upload graph (streamed).
 
     Add the content of triple to a remote graph or replace the remote graph
     with the content of a triple file.
@@ -131,15 +131,15 @@
     Returns:
         requests.Response object
 
     """
     uri = _get_graph_uri(endpoint_id, graph) + "&replace=" + str(replace).lower()
     headers = {"Content-Type": content_type}
     # https://2.python-requests.org/en/master/user/advanced/#streaming-uploads
-    if isinstance(file, io.StringIO):
+    if isinstance(file, io.BytesIO):
         response = request(
             uri, method="POST", headers=headers, data=file, stream=True
         )
     else:
         with open(file, "rb") as opened_file:
             response = request(
                 uri, method="POST", headers=headers, data=opened_file, stream=True
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/sparql.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/sparql.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/proxy/update.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/proxy/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """API for running SPARQL queries on DP proxy endpoints."""
 
 from base64 import b64encode
 
 from cmem.cmempy import config
-
 from cmem.cmempy.api import send_request
 
 
 def get_update_endpoint():
     """Get endpoint URI pattern for a SPARQL update endpoint."""
     return config.get_dp_api_endpoint() + "/proxy/{}/update"
 
@@ -16,17 +15,19 @@
 def post(
     query,
     endpoint_id="default",
     accept="application/sparql-update",
     named_graph_uri=(),
     default_graph_uri=(),
     base64_encoded=False,
+    timeout=None,
 ):
     """POST update / insert query."""
     headers = {"Accept": accept}
+    params = {}
     uri = get_update_endpoint().format(endpoint_id)
 
     if base64_encoded:
         query = b64encode(query.encode())
         data = {"update": query, "base64encoded": "true"}
     else:
         data = {"update": query}
@@ -37,9 +38,14 @@
             data["named-graph-uri"].append(graph)
 
     if default_graph_uri:
         data["default-graph-uri"] = []
         for graph in default_graph_uri:
             data["default-graph-uri"].append(graph)
 
-    response = send_request(uri=uri, method="POST", data=data, headers=headers)
+    if timeout:
+        params["timeout"] = timeout
+
+    response = send_request(
+        uri=uri, method="POST", data=data, params=params, headers=headers
+    )
     return response.decode("utf-8")
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/shacl/validation.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/shacl/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 def get_all_aggregations() -> list[dict]:
     """Get all batch validations (aggregation views)"""
     endpoint = get_validation_api_endpoint() + "/view/aggregation"
     return list(get_json(endpoint))
 
 
 def start(
-        context_graph: str,
-        shape_graph: Union[str, None] = None,
-        query: Union[str, None] = None
+    context_graph: str,
+    shape_graph: Union[str, None] = None,
+    query: Union[str, None] = None,
 ) -> str:
     """Start a single batch validation and return batch ID"""
     params = {"contextGraph": context_graph}
     if shape_graph:
         params["shapeGraph"] = shape_graph
     if query:
         params["query"] = query
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/dp/titles/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/dp/titles/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/health/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/health/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/keycloak/client.py` & `cmem_cmempy-24.1.1/cmem/cmempy/keycloak/client.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/keycloak/group.py` & `cmem_cmempy-24.1.1/cmem/cmempy/keycloak/group.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/keycloak/user.py` & `cmem_cmempy-24.1.1/cmem/cmempy/keycloak/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 API method to manage cmem realm users
 """
 import json
 from json import loads
-from typing import Optional
+from typing import Optional, Union
 
 from cmem.cmempy import config
 from cmem.cmempy.api import send_request
 
 
 def get_users_uri():
     """Get endpoint URI for user list."""
@@ -86,15 +86,15 @@
     username: str,
     first_name: str,
     last_name: str,
     email: str,
     email_verified: Optional[bool] = None,
 ):
     """update user to cmem relam"""
-    data = {
+    data: dict[str, Union[str, bool]] = {
         "username": username,
         "firstName": first_name,
         "lastName": last_name,
         "email": email,
     }
     if email_verified is not None:
         data["emailVerified"] = email_verified
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/linking/linkingtask.py` & `cmem_cmempy-24.1.1/cmem/cmempy/linking/linkingtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/plugins/marshalling.py` & `cmem_cmempy-24.1.1/cmem/cmempy/plugins/marshalling.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/queries/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/queries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 from pyparsing import ParseException
 from rdflib.plugins.sparql import prepareQuery
 from rdflib.plugins.sparql.parser import parseUpdate
 
 from cmem.cmempy.api import get_json, request
 from cmem.cmempy.config import get_cmem_base_uri, get_dp_api_endpoint
-from cmem.cmempy.dp.proxy import sparql
-from cmem.cmempy.dp.proxy import update
+from cmem.cmempy.dp.proxy import sparql, update
 
 # read queries are send to the normal query endpoint
 QUERY_TYPES_READ = ("SELECT", "ASK", "DESCRIBE", "CONSTRUCT")
 # update queries are send to the update query endpoint
 QUERY_TYPES_UPDATE_TRIPLE = ("UPDATE", "DELETE", "INSERT", "CLEAR", "LOAD")
 QUERY_TYPES_UPDATE_GRAPHS = ("CREATE", "DROP", "COPY", "MOVE", "ADD")
 QUERY_TYPES_UPDATE = QUERY_TYPES_UPDATE_TRIPLE + QUERY_TYPES_UPDATE_GRAPHS
@@ -185,16 +184,16 @@
         text = self.text
         for key, value in placeholder.items():
             text = text.replace("{{" + key + "}}", value)
         if self.get_placeholder_keys(text):
             raise ValueError(
                 "Not all placeholders filled for executing the "
                 "following query:\n"
-                f"- Label: {str(self.label)}\n"
-                f"- ID: {str(self.url)}\n"
+                f"- Label: {self.label!s}\n"
+                f"- ID: {self.url!s}\n"
                 f"- Missing parameters: {self.get_placeholder_keys(text)}"
             )
         return text
 
     def get_csv_results(self, placeholder=None, owl_imports_resolution=True):
         """Get results as CSV text."""
         if self.query_type != "SELECT":
@@ -237,15 +236,18 @@
             self.query_type = self.get_query_type(placeholder)
         if replace_placeholder:
             query_text = self.get_filled_text(placeholder)
         else:
             query_text = self.text
         if self.query_type in QUERY_TYPES_UPDATE:
             return update.post(
-                query=query_text, accept=accept, base64_encoded=base64_encoded
+                query=query_text,
+                accept=accept,
+                base64_encoded=base64_encoded,
+                timeout=timeout,
             )
         return sparql.post(
             query=query_text,
             accept=accept,
             base64_encoded=base64_encoded,
             owl_imports_resolution=owl_imports_resolution,
             distinct=distinct,
@@ -270,15 +272,15 @@
         """Initialize the catalog."""
         self.queries = None
 
     def get_query(self, identifier, placeholder=None):
         """Get a query by giving an url, a short_url or a file name."""
         if os.path.isfile(identifier):
             # do not fetch the catalog in case a file is requested
-            with open(identifier, "r", encoding="UTF-8") as file_handle:
+            with open(identifier, encoding="UTF-8") as file_handle:
                 return SparqlQuery(
                     file_handle.read(),
                     label="query from file " + identifier,
                     origin="file",
                     placeholder=placeholder,
                 )
         queries = self.get_queries()
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/transform/rules/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/transform/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/transform/rules/transformationrule.py` & `cmem_cmempy-24.1.1/cmem/cmempy/transform/rules/transformationrule.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/transform/transformationtask.py` & `cmem_cmempy-24.1.1/cmem/cmempy/transform/transformationtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/vocabularies/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workflow/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workflow/workflow.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/projectactivities.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/projectactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/projectactivity.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/projectactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/taskactivities.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/taskactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/activities/taskactivity.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/activities/taskactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/export_/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/export_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/import_/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/import_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/datasets/dataset.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     """Get endpoint URI pattern for a dataset."""
     path = "/workspace/projects/{}/datasets/{}"
     return config.get_di_api_endpoint() + path
 
 
 def get_dataset_file_uri():
     """Get the endpoint URI for a dataset file."""
-    return get_dataset_uri() + '/file'
+    return get_dataset_uri() + "/file"
 
 
 def get_dataset(project_name, dataset_name):
     """GET retrieve single dataset."""
     headers = {"Accept": "application/json"}
     response = send_request(
         get_dataset_uri().format(project_name, dataset_name),
         method="GET",
         headers=headers,
     )
     return json.loads(response.decode("utf-8"))
 
 
 def make_new_dataset(
-        project_name, dataset_name, dataset_type, parameters, autoconfigure
+    project_name, dataset_name, dataset_type, parameters, autoconfigure
 ):
     """PUT create new dataset (deprecated)."""
     data = {
         "id": f"{dataset_name}",
         "type": f"{dataset_type}",
         "parameters": parameters,
     }
@@ -55,21 +55,21 @@
 def delete_dataset(project_name, dataset_name):
     """DELETE remove existing dataset."""
     send_request(get_dataset_uri().format(project_name, dataset_name), method="DELETE")
 
 
 # pylint: disable=too-many-arguments
 def create_dataset(
-        project_id,
-        dataset_type,
-        dataset_id=None,
-        parameter=None,
-        metadata=None,
-        read_only=False,
-        uri_property=None,
+    project_id,
+    dataset_type,
+    dataset_id=None,
+    parameter=None,
+    metadata=None,
+    read_only=False,
+    uri_property=None,
 ):
     """Create a dataset.
 
     In difference to make_new_dataset, this uses the task API and does
     not enforce an ID in advance. Also, it allows for metadata parameters.
     """
     if parameter is None:
@@ -126,40 +126,31 @@
                 endpoint,
                 method="PUT",
                 stream=True,
                 data=file,
             )
         return response
 
-    multipart_encoder = MultipartEncoder(
-        fields=[
-            ("resource-url", resource_url)
-        ]
-    )
-    headers = {
-        "Content-Type": multipart_encoder.content_type
-    }
+    multipart_encoder = MultipartEncoder(fields=[("resource-url", resource_url)])
+    headers = {"Content-Type": multipart_encoder.content_type}
     return request(
         endpoint,
         method="PUT",
         headers=headers,
         data=multipart_encoder,
         stream=True,
     )
 
 
-def get_resource(
-        project_id,
-        dataset_id
-):
+def get_resource(project_id, dataset_id):
     """Get a resource"""
     endpoint = get_dataset_file_uri().format(project_id, dataset_id)
     response = send_request(
         endpoint,
-        method='GET',
+        method="GET",
     )
     return response.decode("utf-8")
 
 
 def update_dataset(
     project_id,
     dataset_id,
@@ -171,21 +162,19 @@
     """Update a dataset"""
     if parameters is None:
         parameters = {}
     if metadata is None:
         metadata = {}
     data = {
         "metadata": metadata,
-        "data":
-            {
-                "readOnly": read_only,
-                "uriProperty": uri_property,
-                "parameters": parameters,
-            }
-
+        "data": {
+            "readOnly": read_only,
+            "uriProperty": uri_property,
+            "parameters": parameters,
+        },
     }
     path = f"/workspace/projects/{project_id}/tasks/{dataset_id}"
     return send_request(
         config.get_di_api_endpoint() + path,
         method="PATCH",
         data=json.dumps(data).encode("utf-8"),
         headers={"Content-Type": "application/json"},
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/export_.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/export_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/import_.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/import_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/project.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,35 +64,25 @@
 
 def make_new_project(name):
     """PUT make new project."""
     response = send_request(get_project_uri().format(name), method="PUT")
     return json.loads(response.decode("utf-8"))
 
 
-def make_new_project_with_metadata(
-        id_: str,
-        label: str = "",
-        description: str = ""
-):
+def make_new_project_with_metadata(id_: str, label: str = "", description: str = ""):
     """POST make new project including metadata"""
     # {"metaData":{"label":"test","description":"eee"},"id":"myid"}
     if label == "":
         label = id_
-    data = {
-        "id": id_,
-        "metaData": {
-            "label": label,
-            "description": description
-        }
-    }
+    data = {"id": id_, "metaData": {"label": label, "description": description}}
     response = send_request(
         get_projects_api_uri(),
         method="POST",
         headers={"Content-Type": "application/json"},
-        data=json.dumps(data)
+        data=json.dumps(data),
     )
     return json.loads(response.decode("utf-8"))
 
 
 def delete_project(name):
     """DELETE remove project."""
     send_request(get_project_uri().format(name), method="DELETE")
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/resources/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/resources/resource.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/resources/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/projects/variables/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/projects/variables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,35 +35,31 @@
 def get_variable(variable_name: str, project_name: str) -> Union[dict, bool]:
     """GET retrieve a single variable.
 
     or False if variable was not found.
     """
     try:
         response = send_request(
-            get_variable_uri().format(variable_name, project_name),
-            method="GET"
+            get_variable_uri().format(variable_name, project_name), method="GET"
         )
     except HTTPError as error:
         if error.response is not None and error.response.status_code == 404:
             return False
         raise error
     return dict(json.loads(response.decode("utf-8")))
 
 
 def delete_variable(variable_name: str, project_name: str):
     """DELETE a single variable."""
     send_request(
-        get_variable_uri().format(variable_name, project_name),
-        method="DELETE"
+        get_variable_uri().format(variable_name, project_name), method="DELETE"
     )
 
 
-def create_or_update_variable(
-        variable_name: str, project_name: str, data: dict
-):
+def create_or_update_variable(variable_name: str, project_name: str, data: dict):
     """PUT create or update a single variable."""
     headers = {"Content-Type": "application/json"}
     send_request(
         get_variable_uri().format(variable_name, project_name),
         method="PUT",
         data=json.dumps(data),
         headers=headers,
```

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/python.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/search/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/search/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/cmem/cmempy/workspace/tasks/__init__.py` & `cmem_cmempy-24.1.1/cmem/cmempy/workspace/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-24.1.0/pyproject.toml` & `cmem_cmempy-24.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmempy"
-version = "24.1.0"
+version = "24.1.1"
 license = "Apache-2.0"
 description = "API for eccenca Corporate Memory"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 maintainers = ["Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -29,21 +29,21 @@
 pyparsing = "^3.1.1"
 rdflib = "^6.3.2"
 requests = "^2.31.0"
 requests-toolbelt = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.2"
-black = "^22.1.0"
+black = "^24.3.0"
 coverage = "^6.3.2"
 coverage-badge = "^1.1.0"
 defusedxml = "^0.7.1"
 flake8 = "^6.0.0"
 genbadge = "^1.1.1"
-mypy = "^0.931"
+mypy = "^1.9.0"
 pip = ">=23.3" # Avoid safety issue 62044 for pip less than 23.3
 pre-commit = "2.20.0"
 pylint = "^2" # https://github.com/rasjani/pylint-junit/issues/1
 pylint-junit = "==0.3.2" # https://github.com/rasjani/pylint-junit/issues/2
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.3.0"
```

### Comparing `cmem_cmempy-24.1.0/PKG-INFO` & `cmem_cmempy-24.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmempy
-Version: 24.1.0
+Version: 24.1.1
 Summary: API for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmempy
 License: Apache-2.0
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
```

