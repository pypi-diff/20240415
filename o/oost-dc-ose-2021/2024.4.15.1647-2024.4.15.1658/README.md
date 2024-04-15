# Comparing `tmp/oost_dc_ose_2021-2024.4.15.1647.tar.gz` & `tmp/oost_dc_ose_2021-2024.4.15.1658.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oost_dc_ose_2021-2024.4.15.1647.tar", last modified: Mon Apr 15 14:47:04 2024, max compression
+gzip compressed data, was "oost_dc_ose_2021-2024.4.15.1658.tar", last modified: Mon Apr 15 14:58:53 2024, max compression
```

## Comparing `oost_dc_ose_2021-2024.4.15.1647.tar` & `oost_dc_ose_2021-2024.4.15.1658.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1071 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/LICENSE
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      275 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1616 2024-04-15 14:11:22.000000 oost_dc_ose_2021-2024.4.15.1647/README.md
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.661413 oost_dc_ose_2021-2024.4.15.1647/datachallenge/
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.661413 oost_dc_ose_2021-2024.4.15.1647/datachallenge/scripts/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      439 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/datachallenge/scripts/format_metrics.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      286 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/datachallenge/scripts/wrap_yaml.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.661413 oost_dc_ose_2021-2024.4.15.1647/docs/
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.661413 oost_dc_ose_2021-2024.4.15.1647/docs/tmp/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3354 2024-04-09 14:09:24.000000 oost_dc_ose_2021-2024.4.15.1647/docs/tmp/ocb_dc_ose_2021_data.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/__init__.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1357 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/cmems_get.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3224 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/interp_on_track.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     5301 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/lambdax.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2504 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/mu.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3674 2024-04-11 14:27:40.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/prepare_track.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/__init__.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2593 2024-04-15 14:14:35.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/input_data.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3264 2024-04-15 14:14:35.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/metrics.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      275 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      739 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/SOURCES.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/dependency_links.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      166 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/entry_points.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       22 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/requires.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       54 2024-04-15 14:47:04.000000 oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/top_level.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      644 2024-04-15 14:47:00.000000 oost_dc_ose_2021-2024.4.15.1647/pyproject.toml
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-15 14:47:04.665413 oost_dc_ose_2021-2024.4.15.1647/setup.cfg
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1071 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/LICENSE
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      275 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1616 2024-04-15 14:11:22.000000 oost_dc_ose_2021-2024.4.15.1658/README.md
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.610862 oost_dc_ose_2021-2024.4.15.1658/datachallenge/
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.610862 oost_dc_ose_2021-2024.4.15.1658/datachallenge/scripts/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      439 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/datachallenge/scripts/format_metrics.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      286 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/datachallenge/scripts/wrap_yaml.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.610862 oost_dc_ose_2021-2024.4.15.1658/docs/
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.610862 oost_dc_ose_2021-2024.4.15.1658/docs/tmp/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3354 2024-04-09 14:09:24.000000 oost_dc_ose_2021-2024.4.15.1658/docs/tmp/ocb_dc_ose_2021_data.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.610862 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/__init__.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1357 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/cmems_get.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3224 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/interp_on_track.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     5301 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/lambdax.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2504 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/mu.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3674 2024-04-11 14:27:40.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/prepare_track.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-10 13:13:46.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/__init__.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2617 2024-04-15 14:54:21.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/input_data.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3324 2024-04-15 14:54:21.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/metrics.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      275 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      739 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/SOURCES.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/dependency_links.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      166 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/entry_points.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       22 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/requires.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       54 2024-04-15 14:58:53.000000 oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/top_level.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      644 2024-04-15 14:47:00.000000 oost_dc_ose_2021-2024.4.15.1658/pyproject.toml
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-15 14:58:53.614862 oost_dc_ose_2021-2024.4.15.1658/setup.cfg
```

### Comparing `oost_dc_ose_2021-2024.4.15.1647/LICENSE` & `oost_dc_ose_2021-2024.4.15.1658/LICENSE`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/README.md` & `oost_dc_ose_2021-2024.4.15.1658/README.md`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/docs/tmp/ocb_dc_ose_2021_data.py` & `oost_dc_ose_2021-2024.4.15.1658/docs/tmp/ocb_dc_ose_2021_data.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/cmems_get.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/cmems_get.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/interp_on_track.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/interp_on_track.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/lambdax.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/lambdax.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/mu.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/mu.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/mods/prepare_track.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/mods/prepare_track.py`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/input_data.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/input_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aprl.appareil
 import aprl.utils
-import oost.mods.cmems_get as cmems_get
-import oost.mods.prepare_track as prepare_track
+import oost_dc_ose_2021.mods.cmems_get as cmems_get
+import oost_dc_ose_2021.mods.prepare_track as prepare_track
 
 cmems_get_cfg = aprl.utils.make_partial(cmems_get.cfg)
 dataset_id_cfg = cmems_get.cfg.dataset_id
 regex_cfg = cmems_get.cfg.regex
 _01_dl_track = cmems_get_cfg(
     dataset_id=dataset_id_cfg(sat="${....params.sat}"),
     regex=regex_cfg(
```

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021/pipelines/metrics.py` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021/pipelines/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import aprl.appareil
-import oost.mods.cmems_get as cmems_get
-import oost.mods.interp_on_track as interp_on_track
-import oost.mods.lambdax as lambdax
-import oost.mods.mu as mu
-import oost.mods.prepare_track as prepare_track
+import oost_dc_ose_2021.mods.cmems_get as cmems_get
+import oost_dc_ose_2021.mods.interp_on_track as interp_on_track
+import oost_dc_ose_2021.mods.lambdax as lambdax
+import oost_dc_ose_2021.mods.mu as mu
+import oost_dc_ose_2021.mods.prepare_track as prepare_track
 
 dataset_id_cfg = cmems_get.cfg.dataset_id
 regex_cfg = cmems_get.cfg.regex
 cmems_get_cfg = aprl.utils.make_partial(cmems_get.cfg)
 _01_dl_track = cmems_get_cfg(
     dataset_id=dataset_id_cfg(sat="${....params.sat}"),
     regex=regex_cfg(
```

### Comparing `oost_dc_ose_2021-2024.4.15.1647/oost_dc_ose_2021.egg-info/SOURCES.txt` & `oost_dc_ose_2021-2024.4.15.1658/oost_dc_ose_2021.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oost_dc_ose_2021-2024.4.15.1647/pyproject.toml` & `oost_dc_ose_2021-2024.4.15.1658/pyproject.toml`

 * *Files identical despite different names*

