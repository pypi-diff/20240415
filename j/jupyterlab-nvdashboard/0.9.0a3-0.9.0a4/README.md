# Comparing `tmp/jupyterlab_nvdashboard-0.9.0a3.tar.gz` & `tmp/jupyterlab_nvdashboard-0.9.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nvdashboard-0.9.0a3.tar", last modified: Wed Oct  4 21:20:30 2023, max compression
+gzip compressed data, was "jupyterlab_nvdashboard-0.9.0a4.tar", last modified: Mon Dec  4 16:31:01 2023, max compression
```

## Comparing `jupyterlab_nvdashboard-0.9.0a3.tar` & `jupyterlab_nvdashboard-0.9.0a4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.463581 jupyterlab_nvdashboard-0.9.0a3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-10-04 21:20:30.463581 jupyterlab_nvdashboard-0.9.0a3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2991 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/install.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.455581 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/_version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/cpu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16090 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/gpu.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2724 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/package.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6752 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/remoteEntry.3b54148a5b3606889173.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-10-04 21:20:28.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/style.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1339 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1260 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-10-04 21:20:30.000000 jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2582 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/package.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-10-04 21:20:30.463581 jupyterlab_nvdashboard-0.9.0a3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2966 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/src/dashboard.tsx
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/src/handler.ts
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/src/index.ts
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-04 21:20:30.459581 jupyterlab_nvdashboard-0.9.0a3/style/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/style/base.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/style/expansion-card-variant-dark.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/style/expansion-card-variant-light.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/style/index.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/style/index.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/tsconfig.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2023-10-04 21:11:12.000000 jupyterlab_nvdashboard-0.9.0a3/tslint.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.829952 jupyterlab_nvdashboard-0.9.0a4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-12-04 16:31:01.829952 jupyterlab_nvdashboard-0.9.0a4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2991 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/install.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.825951 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/_version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.825951 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/cpu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16090 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/gpu.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.825951 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2724 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/package.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.825951 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6752 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/remoteEntry.3b54148a5b3606889173.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-12-04 16:31:00.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/style.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1339 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.825951 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1260 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-12-04 16:31:01.000000 jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2582 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/package.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-12-04 16:31:01.829952 jupyterlab_nvdashboard-0.9.0a4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2966 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.829952 jupyterlab_nvdashboard-0.9.0a4/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/src/dashboard.tsx
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/src/handler.ts
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/src/index.ts
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-04 16:31:01.829952 jupyterlab_nvdashboard-0.9.0a4/style/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/style/base.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/style/expansion-card-variant-dark.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/style/expansion-card-variant-light.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/style/index.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/style/index.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/tsconfig.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2023-12-04 16:21:30.000000 jupyterlab_nvdashboard-0.9.0a4/tslint.json
```

### Comparing `jupyterlab_nvdashboard-0.9.0a3/LICENSE` & `jupyterlab_nvdashboard-0.9.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/PKG-INFO` & `jupyterlab_nvdashboard-0.9.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nvdashboard
-Version: 0.9.0a3
+Version: 0.9.0a4
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nvdashboard-0.9.0a3/README.md` & `jupyterlab_nvdashboard-0.9.0a4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/__init__.py` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/cpu.py` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/cpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/apps/gpu.py` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/apps/gpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/package.json` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/remoteEntry.3b54148a5b3606889173.js` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/remoteEntry.3b54148a5b3606889173.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard/server.py` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard/server.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/PKG-INFO` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nvdashboard
-Version: 0.9.0a3
+Version: 0.9.0a4
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nvdashboard-0.9.0a3/jupyterlab_nvdashboard.egg-info/SOURCES.txt` & `jupyterlab_nvdashboard-0.9.0a4/jupyterlab_nvdashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/package.json` & `jupyterlab_nvdashboard-0.9.0a4/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/setup.py` & `jupyterlab_nvdashboard-0.9.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/src/dashboard.tsx` & `jupyterlab_nvdashboard-0.9.0a4/src/dashboard.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/src/handler.ts` & `jupyterlab_nvdashboard-0.9.0a4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/src/index.ts` & `jupyterlab_nvdashboard-0.9.0a4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/style/base.css` & `jupyterlab_nvdashboard-0.9.0a4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/tsconfig.json` & `jupyterlab_nvdashboard-0.9.0a4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.9.0a3/tslint.json` & `jupyterlab_nvdashboard-0.9.0a4/tslint.json`

 * *Files identical despite different names*

