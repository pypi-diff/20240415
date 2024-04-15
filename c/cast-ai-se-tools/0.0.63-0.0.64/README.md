# Comparing `tmp/cast_ai-se-tools-0.0.63.tar.gz` & `tmp/cast_ai-se-tools-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cast_ai-se-tools-0.0.63.tar", last modified: Sun Mar 31 01:37:18 2024, max compression
+gzip compressed data, was "cast_ai-se-tools-0.0.64.tar", last modified: Mon Apr 15 15:40:45 2024, max compression
```

## Comparing `cast_ai-se-tools-0.0.63.tar` & `cast_ai-se-tools-0.0.64.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.438633 cast_ai-se-tools-0.0.63/
--rw-rw-rw-   0        0        0    11546 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/LICENSE
--rw-rw-rw-   0        0        0       66 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/MANIFEST.in
--rw-rw-rw-   0        0        0     2204 2024-03-31 01:37:18.438633 cast_ai-se-tools-0.0.63/PKG-INFO
--rw-rw-rw-   0        0        0     1192 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.396633 cast_ai-se-tools-0.0.63/cast_ai/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.400634 cast_ai-se-tools-0.0.63/cast_ai/se/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/__init__.py
--rw-rw-rw-   0        0        0     2824 2024-03-31 01:36:00.000000 cast_ai-se-tools-0.0.63/cast_ai/se/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.409633 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/__init__.py
--rw-rw-rw-   0        0        0     3547 2024-03-11 21:12:20.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/aks_controller.py
--rw-rw-rw-   0        0        0     4548 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/castai_controller.py
--rw-rw-rw-   0        0        0      395 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/cloud_controller.py
--rw-rw-rw-   0        0        0     4339 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/eks_controller.py
--rw-rw-rw-   0        0        0     2873 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/gke_controller.py
--rw-rw-rw-   0        0        0     5449 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/kubectl_controller.py
--rw-rw-rw-   0        0        0     3845 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/contollers/snapshot_controller.py
--rw-rw-rw-   0        0        0     1264 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/misc_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.416634 cast_ai-se-tools-0.0.63/cast_ai/se/models/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/__init__.py
--rw-rw-rw-   0        0        0     2308 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/cloud_confs.py
--rw-rw-rw-   0        0        0      169 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/exceptions.py
--rw-rw-rw-   0        0        0      160 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/execution_status.py
--rw-rw-rw-   0        0        0      132 2024-03-29 20:09:28.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/misc_data_models.py
--rw-rw-rw-   0        0        0     1638 2024-03-11 01:33:22.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/refined_snapshot.py
--rw-rw-rw-   0        0        0      563 2024-03-11 21:19:46.000000 cast_ai-se-tools-0.0.63/cast_ai/se/models/refined_snapshot_analysis.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.423632 cast_ai-se-tools-0.0.63/cast_ai/se/services/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/__init__.py
--rw-rw-rw-   0        0        0     1709 2024-02-27 13:57:36.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/api_requests_svc.py
--rw-rw-rw-   0        0        0     2095 2024-03-04 14:53:11.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/request_handle_svc.py
--rw-rw-rw-   0        0        0      943 2024-03-29 20:33:46.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_analysis_svc.py
--rw-rw-rw-   0        0        0     6133 2024-03-29 21:40:22.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_refinery_svc.py
--rw-rw-rw-   0        0        0     8657 2024-03-31 01:36:28.000000 cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_reporting_svc.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.429633 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/
--rw-rw-rw-   0        0        0     2204 2024-03-31 01:37:15.000000 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1471 2024-03-31 01:37:18.000000 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 01:37:15.000000 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      253 2024-03-31 01:37:15.000000 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-31 01:37:15.000000 cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/pyproject.toml
--rw-rw-rw-   0        0        0      265 2024-03-29 20:48:05.000000 cast_ai-se-tools-0.0.63/requirements.txt
--rw-rw-rw-   0        0        0      133 2024-03-31 01:37:18.440633 cast_ai-se-tools-0.0.63/setup.cfg
--rw-rw-rw-   0        0        0     1252 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/setup.py
--rw-rw-rw-   0        0        0       11 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/test_requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.431633 cast_ai-se-tools-0.0.63/tests/
--rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.63/tests/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-05 15:55:34.000000 cast_ai-se-tools-0.0.63/tests/test_api_requests_svc.py
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.382632 cast_ai-se-tools-0.0.63/venv/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.382632 cast_ai-se-tools-0.0.63/venv/Lib/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.383632 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.384634 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.384634 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.384634 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.435634 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      156 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.385635 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.385635 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2024-03-31 01:37:18.436633 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      113 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.63/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
--rw-rw-rw-   0        0        0        6 2024-03-31 01:34:47.000000 cast_ai-se-tools-0.0.63/version.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.770822 cast_ai-se-tools-0.0.64/
+-rw-rw-rw-   0        0        0    11546 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/MANIFEST.in
+-rw-rw-rw-   0        0        0     2204 2024-04-15 15:40:45.769824 cast_ai-se-tools-0.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0     1192 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.716823 cast_ai-se-tools-0.0.64/cast_ai/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.720822 cast_ai-se-tools-0.0.64/cast_ai/se/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/__init__.py
+-rw-rw-rw-   0        0        0     2824 2024-03-31 01:36:00.000000 cast_ai-se-tools-0.0.64/cast_ai/se/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.732821 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2024-03-11 21:12:20.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/aks_controller.py
+-rw-rw-rw-   0        0        0     4548 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/castai_controller.py
+-rw-rw-rw-   0        0        0      395 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/cloud_controller.py
+-rw-rw-rw-   0        0        0     4339 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/eks_controller.py
+-rw-rw-rw-   0        0        0     2873 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/gke_controller.py
+-rw-rw-rw-   0        0        0     5449 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/kubectl_controller.py
+-rw-rw-rw-   0        0        0     3845 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/contollers/snapshot_controller.py
+-rw-rw-rw-   0        0        0     1264 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/misc_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.744824 cast_ai-se-tools-0.0.64/cast_ai/se/models/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/__init__.py
+-rw-rw-rw-   0        0        0     2308 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/cloud_confs.py
+-rw-rw-rw-   0        0        0      169 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/exceptions.py
+-rw-rw-rw-   0        0        0      160 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/execution_status.py
+-rw-rw-rw-   0        0        0      132 2024-03-29 20:09:28.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/misc_data_models.py
+-rw-rw-rw-   0        0        0     1710 2024-04-04 14:05:29.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/refined_snapshot.py
+-rw-rw-rw-   0        0        0      563 2024-03-11 21:19:46.000000 cast_ai-se-tools-0.0.64/cast_ai/se/models/refined_snapshot_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.753821 cast_ai-se-tools-0.0.64/cast_ai/se/services/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/__init__.py
+-rw-rw-rw-   0        0        0     1709 2024-02-27 13:57:36.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/api_requests_svc.py
+-rw-rw-rw-   0        0        0     2095 2024-03-04 14:53:11.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/request_handle_svc.py
+-rw-rw-rw-   0        0        0      943 2024-03-29 20:33:46.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_analysis_svc.py
+-rw-rw-rw-   0        0        0     6810 2024-04-04 14:05:29.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_refinery_svc.py
+-rw-rw-rw-   0        0        0     8863 2024-04-04 21:16:42.000000 cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_reporting_svc.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.761827 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/
+-rw-rw-rw-   0        0        0     2204 2024-04-15 15:40:42.000000 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1471 2024-04-15 15:40:45.000000 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:40:42.000000 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      253 2024-04-15 15:40:42.000000 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 15:40:42.000000 cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       93 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/pyproject.toml
+-rw-rw-rw-   0        0        0      265 2024-03-29 20:48:05.000000 cast_ai-se-tools-0.0.64/requirements.txt
+-rw-rw-rw-   0        0        0      133 2024-04-15 15:40:45.771822 cast_ai-se-tools-0.0.64/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/setup.py
+-rw-rw-rw-   0        0        0       11 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/test_requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.763829 cast_ai-se-tools-0.0.64/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:55:33.000000 cast_ai-se-tools-0.0.64/tests/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-05 15:55:34.000000 cast_ai-se-tools-0.0.64/tests/test_api_requests_svc.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.702823 cast_ai-se-tools-0.0.64/venv/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.702823 cast_ai-se-tools-0.0.64/venv/Lib/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.702823 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.703822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.703822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.703822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.767822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      156 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.704822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.704822 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:40:45.768823 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      113 2024-03-29 20:12:19.000000 cast_ai-se-tools-0.0.64/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+-rw-rw-rw-   0        0        0        6 2024-04-04 21:20:02.000000 cast_ai-se-tools-0.0.64/version.txt
```

### Comparing `cast_ai-se-tools-0.0.63/LICENSE` & `cast_ai-se-tools-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/PKG-INFO` & `cast_ai-se-tools-0.0.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast_ai-se-tools
-Version: 0.0.63
+Version: 0.0.64
 Summary: Provides tools for SE projects (e.g. Cloud controllers).
 Author: Dan Amzulescu
 Author-email: dan@cast.ai
 Keywords: cast.ai k8s eks aks gke
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `cast_ai-se-tools-0.0.63/README.md` & `cast_ai-se-tools-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/constants.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/constants.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/aks_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/aks_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/castai_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/castai_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/eks_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/eks_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/gke_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/gke_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/kubectl_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/kubectl_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/contollers/snapshot_controller.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/contollers/snapshot_controller.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/misc_utils.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/misc_utils.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/models/cloud_confs.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/models/cloud_confs.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/models/refined_snapshot.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/models/refined_snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import logging
 
 
 class RefinedSnapshot:
     def __init__(self):
         self.pdbs = []
         self.workloads = WorkloadObject()
+        self.karpenter_flag = False
+        self.windows_flag = False
 
 
 class WorkloadObject:
     def __init__(self):
         self._logger = logging.getLogger(__name__)
         self.deployments = []
         self.replica_sets = []
```

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/models/refined_snapshot_analysis.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/models/refined_snapshot_analysis.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/services/api_requests_svc.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/services/api_requests_svc.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/services/request_handle_svc.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/services/request_handle_svc.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_analysis_svc.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_analysis_svc.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_refinery_svc.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_refinery_svc.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,29 @@
     @property
     def reporter(self):
         return self._reporter
 
     def refine_snapshot(self, snapshot_data: Dict[str, Any]):
         self._refine_snapshot_workloads(snapshot_data)
         self._refine_snapshot_pdbs(snapshot_data)
+        self._karpenter_check(snapshot_data)
+        self._windows_check(snapshot_data)
         self._summarize_rs_object_types()
 
+    def _windows_check(self, snapshot_data: Dict[str, Any]) -> None:
+        for node in snapshot_data.get("nodeList", {}).get("items", []):
+            labels = node.get("metadata", {}).get("labels", {})
+            if labels.get("kubernetes.io/os") == "windows":
+                self._refined_snapshot.windows_flag = True
+                break
+
+    def _karpenter_check(self, snapshot_data: Dict[str, Any]) -> None:
+        self._refined_snapshot.karpenter_flag = \
+            ("ec2NodeClassesList" in snapshot_data and bool(snapshot_data["ec2NodeClassesList"]["items"]))
+
     def _refine_snapshot_workloads(self, snapshot_data: Dict[str, Any]) -> None:
         for workload_key in K8S_WORKLOAD_TYPES:
             if snapshot_data[workload_key]["items"]:
                 self._logger.info(f"Starting to analyze workloads ({workload_key})...")
                 for workload in snapshot_data[workload_key]["items"]:
                     if workload["metadata"]["namespace"] in NON_RELEVANT_NAMESPACES:
                         continue
```

### Comparing `cast_ai-se-tools-0.0.63/cast_ai/se/services/snapshot_reporting_svc.py` & `cast_ai-se-tools-0.0.64/cast_ai/se/services/snapshot_reporting_svc.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,18 @@
                     workload_df = pd.DataFrame([data_dict])
                     df = pd.concat([df, workload_df], ignore_index=True)
         df = df.loc[:, df.ne('').any(axis=0)]
         df.to_csv(report_filename, index=False)
 
     def generate_refined_snapshot_report(self, detail_lvl: ReportDetailLevel = ReportDetailLevel.BASIC) -> str:
         report = "┌" + "─" * 52 + f"< {detail_lvl.value} Report >" + "─" * (57 - len(str(detail_lvl.value))) + "┐\n"
+        if self._refined_snapshot.karpenter_flag:
+            report += "│ Karpenter Present !\n"
+        if self._refined_snapshot.windows_flag:
+            report += "│ Windows nodes Present !\n"
         report += (f"│ {self._rs_metadata.total_counters['total_workloads']} "
                    f"Workloads with scheduling-challenging settings:\n")
         report = self._add_refinement_metrics_to_report(report)
         report = self._add_workloads_to_report(detail_lvl, report)
         report += "├" + "─" * 120 + "┤\n"
         report += f"│ {self._rs_metadata.total_counters['total_pdbs']} PDBs\n"
         if detail_lvl != ReportDetailLevel.BASIC:
```

### Comparing `cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/PKG-INFO` & `cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast-ai-se-tools
-Version: 0.0.63
+Version: 0.0.64
 Summary: Provides tools for SE projects (e.g. Cloud controllers).
 Author: Dan Amzulescu
 Author-email: dan@cast.ai
 Keywords: cast.ai k8s eks aks gke
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `cast_ai-se-tools-0.0.63/cast_ai_se_tools.egg-info/SOURCES.txt` & `cast_ai-se-tools-0.0.64/cast_ai_se_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/setup.py` & `cast_ai-se-tools-0.0.64/setup.py`

 * *Files identical despite different names*

### Comparing `cast_ai-se-tools-0.0.63/tests/test_api_requests_svc.py` & `cast_ai-se-tools-0.0.64/tests/test_api_requests_svc.py`

 * *Files identical despite different names*

